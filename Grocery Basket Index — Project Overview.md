# Grocery Basket Index — Project Overview

Oct 20, 2026 · @Ionel Merca

## Main goal

Show any person, in one glance, what a normal week of groceries costs where they live, which store is cheapest for it, and how that compares to other regions and countries.

The product answers three everyday questions:

- **Where do I shop cheapest this week?** Ready-made baskets priced across the major Romanian chains.
- **Is this discount real?** Price history per product exposes promotions that follow a price hike.
- **How expensive is life here, really?** The same basket priced in other Romanian cities and other countries, shown both in money and in minutes of work at the local median wage.

Why now: food prices in Romania rose over 7% year on year in April 2026, and food takes more than a third of household income ([Economedia](https://economedia.ro/?p=350054)). The official Monitorul Prețurilor has the data breadth but weak UX and inconsistent prices, so the gap is clarity and trust, not data existence.

Who it serves first: families and individuals doing a weekly shop on a budget; second, journalists and NGOs who need a citable, regularly updated cost-of-living index.

## Basic MVP

The MVP is a weekly-updated basket index for Bucharest across 6–8 chains, plus one cross-country comparison built from identical international brands.

**Scope**

- Location: Bucharest first; one more Romanian city (e.g. Cluj or Iași) to test regional differences.
- Chains: Lidl, Kaufland, Carrefour, Mega Image, Profi, Penny, Auchan, Selgros.
- Countries for comparison: 2–3 at launch (e.g. Bulgaria, Hungary, Germany).
- Update cadence: one price snapshot per week, kept as history.

**Baskets**

| Basket | Who it represents | Items |
| --- | --- | --- |
| Family weekly essentials | 2 adults + 2 children | \~30 |
| Single person / student | One person, tight budget | \~20 |
| Pensioner | Basic staples, low spend | \~20 |
| Branded basket | Same national brands everywhere | \~20 |
| Private-label basket | Cheapest store-brand equivalents | \~20 |
| International basket | Identical global brands (Coca-Cola, Nutella, Barilla) | \~15 |

**Features**

1. Basket ranking: total price per chain, cheapest first, with the gap in lei and %, shown both at shelf price and at loyalty/app price.
2. Price history: weekly trend per basket and per product; flag for suspicious discounts.
3. Region and country view: same basket priced elsewhere, with and without VAT, in EUR and in minutes of work at the median net wage (INS for Romania).
4. Shareable cards: one image per weekly result, ready for social media and press.

**Data and matching**

- Sources: collected live from retailer websites on every run, logged in with a real user account; Monitorul Prețurilor used only as a cross-check.
- Matching rule: branded items by exact product and size; private label by category, size and a documented quality tier; fresh produce priced per kg.
- Every basket publishes its item list and matching rules, so users can verify them.

**Out of scope for the MVP**

- Live per-product search across all 30,000 SKUs.
- Custom user baskets and accounts.
- Store-level pricing and online delivery costs.

**Success signals**

- Weekly index published for 8 consecutive weeks without gaps.
- At least one media outlet cites the index.
- Returning visitors week over week.

**Open questions**

- [ ] Index shows both prices: public shelf price and logged-in loyalty/app price. To check per chain: which offers need an account or loyalty card?
- [ ] Wage figure: median net wage from INS for Romania and its regions; for each comparison country, the same figure from its national statistics office (NSI Bulgaria, KSH Hungary, Destatis Germany). To check: whether each publishes a median net wage, else use the closest equivalent?
- [ ] Retailer ToS limits on collecting prices from their sites.

**Price collection: legal notes (first pass, not legal advice)**

The main risk is contractual, not criminal: a retailer's terms can ban automated price collection, and logging in with a real account makes those terms binding on us.

- **EU case law.** In Ryanair v PR Aviation (C-30/14, 2015), the CJEU held that a site whose data has no copyright or database-right protection can still ban screen scraping through its terms ([Pinsent Masons](https://www.pinsentmasons.com/out-law/news/website-operators-can-prohibit-screen-scraping-of-unprotected-data-via-terms-and-conditions-says-eu-court-in-ryanair-case)). Where a database right does apply, the Directive's lawful-user exceptions limit what terms can forbid.
- **Romania.** Criminal exposure (Cod penal Art. 360, access without right) mainly targets bypassing security; public pages carry low risk. Clickwrap terms, the kind accepted when creating an account, are treated as enforceable, while browsewrap depends on notice ([ungovr summary](https://law.ungovr.org/ai/ro), secondary source).
- **Practical barriers.** Most Romanian sites run a WAF and about a fifth use anti-bot tools ([Zyte, 2026](https://www.zyte.com/sowa/2026/geo/country/eu-ro)). Logged-in collection can get the account banned.

Implications for the design:

- Prefer public, logged-out pages where they show the same price; use the account only for prices visible only after login.
- Respect robots.txt, throttle requests, never bypass CAPTCHAs or anti-bot checks.
- Collect only prices and product data, never personal data.
- Publish aggregated basket totals and trends, not a mirror of each retailer's catalogue.

Still to do:

- [ ] Read the website terms of each of the 8 chains for clauses on bots, automated extraction or commercial reuse.
- [ ] Ask a Romanian IT lawyer to confirm the approach before launch.
- [ ] Consider asking chains for a data feed or permission, starting with those that already report to Monitorul Prețurilor.
