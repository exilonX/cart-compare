# Grocery Basket Index — Project Overview v2

Nov 9, 2026 · Draft written by the agent from the decisions on the [map](https://github.com/exilonX/cart-compare/issues/1), at Ionel Merca's request · Supersedes the overview of Oct 20, 2026

**Status: conditional go.** No kill criterion is tripped by the evidence. Legal stays open until a Romanian IT lawyer answers the [brief](docs/legal/lawyer-brief.md). See [Go/no-go](#gono-go).

## Main goal

Show any person, at a glance, what a normal week of groceries costs at the Chains near them, which Chain is cheapest for it, and how long it takes to earn.

It answers three everyday questions:

- **Where do I shop cheapest this week?** Basket totals at named Bucharest stores, with Shelf price and Loyalty price side by side.
- **Is this discount real?** Each item's weekly price history is public, so a "was" price can be checked against what we recorded. We publish facts, not verdicts.
- **How long do I work for this?** The Basket in minutes of work at the average net hourly wage. The Pensioner Basket is shown in days of the average pension.

**Why now.**
- Food takes about a third of household consumption spending: 32.0% in Q2 2026, and 34.2% for pensioner households (INS).
- Romania gives food the largest weight of any EU country in its inflation basket: 27.4%, against an EU average of 16.3%.
- Romanian outlets already publish supermarket rankings without a stated method.
- No Romanian Comparable runs a regular, open, archived Basket index with Shelf and Loyalty prices side by side ([Romanian private Comparables](https://github.com/exilonX/cart-compare/issues/14)).

**Who it serves.**
- Shoppers directly: a free web page, no account, readable on a phone.
- The press, through a citable weekly publication.
- Pensioners mainly through the press and TV stories built on the Pensioner Basket ([Who do we serve first](https://github.com/exilonX/cart-compare/issues/12)).

## What changed from v1

| Topic | v1 (Oct 20) | v2 |
| --- | --- | --- |
| Price source | Retailer websites, logged in with a real account; Monitorul Prețurilor as a cross-check | Shelf labels, recorded by hand in store. No Monitorul Prețurilor, no websites, no accounts, no requests for permission or data |
| Chains | 8 | 4 priced weekly (Lidl, Kaufland, Penny, Mega Image); Carrefour, Auchan and Profi join as volunteer hours allow; Selgros out |
| Cities | Bucharest plus a second city | Bucharest only |
| Baskets | 6, including an International basket | One item list, three household Baskets (family, single person, pensioner), plus branded items shown separately; the International basket is dropped |
| Discount flag | "Flag for suspicious discounts" | Public price history only; no flag in the MVP |
| Country view | 2–3 countries, identical international brands | Cut from the MVP; a later option uses Croatia's legally open price files |
| Work time | Median net wage (INS) | INS mean net hourly earnings, labelled as a mean, with a note on the median; pension days for the Pensioner Basket |
| Food-share claim | "more than a third of household income" | "about a third of household consumption spending" |
| Framing | "cost of living" | Grocery Basket price and work time only, never "cost of living" |
| Audience | Families first, journalists second | One published index serving both |

## Basic MVP

**Scope**

- **Location:** Bucharest.
- **Chains priced every week:** Lidl, Kaufland, Penny and Mega Image, one named store each. Carrefour, Auchan and Profi join when volunteer hours allow ([Which Chains](https://github.com/exilonX/cart-compare/issues/29)).
- **Cadence:** one round of store visits a week, every store priced within the same 48 hours. Results are published on a fixed weekday and kept as history.

**Baskets**

One list of about 25–30 items, each defined by a written specification. Each Basket is a published set of quantities over that list ([How do we price a Basket](https://github.com/exilonX/cart-compare/issues/16)).

| Basket | Who it represents | Shown as |
| --- | --- | --- |
| Family weekly essentials | 2 adults + 2 children | Lei, Shelf and Loyalty; minutes of work |
| Single person | One person, tight budget | Lei, Shelf and Loyalty; minutes of work |
| Pensioner | Basic staples, low spend | Lei, Shelf and Loyalty; days of the average pension |
| Branded items (shown separately) | A few identical national-brand products | Lei per Chain; never used alone to name a cheapest Chain |

**Features**

1. **Basket ranking.** Shelf and Loyalty totals per Chain side by side, with the gap in lei and %. No Chain is named "cheapest" below a 2.5% lead; a tie is shown as "la egalitate".
2. **Price history** per item and per Basket.
3. **Work time:** minutes of work at INS mean net hourly earnings, and days of the average pension for the Pensioner Basket.
4. **Shareable weekly cards:** Chain names in plain text, no logos, no discount checks.
5. **Published method and data:** item specifications, quantities, stores, raw prices, code, changelog and a corrections log.

## Data and method

- **Source.** The price on the shelf label, noted by a person as any shopper sees it. The Loyalty price is read from the shelf label or the Chain's public leaflet, and only for offers open to all members. No accounts, cards or apps ([Do we build on Monitorul Prețurilor data, collect from Chain websites, or both?](https://github.com/exilonX/cart-compare/issues/15)).
- **Matching.**
  - Each item is a specification (category, pack-size band, quality tier); the price recorded is that of the cheapest product on the shelf meeting it, own brands included.
  - A product counts from its second weekly sighting onwards.
  - Fresh produce is priced per kg.
  - A Chain enters a ranking only if 80% or more of the items were found there.
- **Loyalty price rule.** Where no member offer applies, the Loyalty price equals the Shelf price. Coupons, points, multibuys and other Personalised offers are excluded.
- **Stores.** One named store per Chain, on days that vary and are not announced in advance. Once a month a second store per Chain is checked, and a gap beyond the tie threshold is published.
- **Versioning.** The item list stays fixed for at least 6 months. Changes are versioned, with one week priced on both lists.
- **Tie threshold.** 2.5% until 8 weeks of second-store checks give our own measurement error.

## Publishing

Decided in [What do we publish](https://github.com/exilonX/cart-compare/issues/11).

- **Licences.** Data under CC BY 4.0, stating that we claim no rights in the prices themselves. Code under MIT.
- **Same access for everyone.** Everything goes public at the same moment. No early, premium or private feeds to anyone, and no forecasts.
- **Claims policy, set by us alone.**
  - A citation must state the date, Basket, city, stores and price type, and link to the method.
  - No "cheapest in Romania" from a Bucharest Basket.
  - No badges or award logos.
  - When anyone overstates our results, we publish a note.
- **Corrections and replies.** A public corrections log; anyone can report an error. A Chain's reply is published next to the result when it writes. No notices are sent before publication.
- **Wording.** "Same price" for identical prices across Chains, never implying coordination.

## Legal approach

- **Collection.** Recording shelf prices in store involves no website terms, no database extraction and no computer system. The remaining collection question is house rules in stores.
- **Publication.** Exposure is civil and modest if every finding is dated, verifiable and backed by the published method ([publishing comparisons](https://github.com/exilonX/cart-compare/issues/10)). The discount check, the largest exposure, is out of the MVP ([discount check](https://github.com/exilonX/cart-compare/issues/22)).
- **Stop on notice.** Any activity a Chain or an authority objects to in writing is paused while the lawyer reviews the objection.
- **Before launch.** A Romanian IT lawyer answers [the brief](docs/legal/lawyer-brief.md). Under the kill criteria, Legal fails until then.

## Running and funding

Decided in [How is the index run and funded](https://github.com/exilonX/cart-compare/issues/25).

- **People and money.** One volunteer, 6 hours a week, store visits included. No legal entity and no income in the MVP. Running costs (a small server at about €6 a month, plus a domain) are paid by the maintainer.
- **No outreach.** The project sends nothing and asks no one: no grants, no partners, no permission requests. Others can reuse the data under CC BY without asking ([partners](https://github.com/exilonX/cart-compare/issues/26)).
- **Funding policy, binding if money ever comes in.**
  - No money, in cash or in kind, from Chains, suppliers, their foundations or grant programmes, or intermediaries passing on their money.
  - No advertising, affiliate links or paid data.
  - Every funder published; no single funder above a third of a year's income.

## Success signals and stop rules

**Success signals**

- The weekly index is published for 8 consecutive weeks without gaps.
- At least one media outlet cites the index.
- Visitors come back week after week.

**Stop rules** (from [What would make us say no?](https://github.com/exilonX/cart-compare/issues/2))

- **Data access and Sustainability, tested in the first 8 weeks.** If one person cannot price at least 4 Chains, with 80% of items found at each, within 6 hours a week, the index stops or is re-scoped.
- **Demand, at 6 months.** If no media outlet has cited the index **and** weekly returning visitors are below a threshold written down before launch, the index stops. The threshold and how returning visitors are counted are still open (see below).
- **Truthfulness, from the monthly second-store check.** If the Chain order does not hold across stores, the ranking is shown as a tie.

## Go/no-go

**Conditional go.** Read against the criteria set before the evidence was consulted, no Kill or Pivot criterion is tripped. The details are in [What would make us say no?](https://github.com/exilonX/cart-compare/issues/2) and its update.

| Criterion | Reading |
| --- | --- |
| Legal | Open: fails until the IT lawyer answers questions 1–6 of the brief |
| Data access | Not tripped by the evidence; met by design (4 Chains, own-brand specifications); proven only in the first 8 weeks |
| Social value too weak | Not tripped: causal evidence of value from Israel and Portugal |
| Social value harmful | Not tripped: weekly, aggregated, already-public prices give sellers nothing new |
| A Comparable already does the job | Not tripped: no Romanian Comparable has every Core property |
| Sustainability | Not tripped on paper; rests on 6 hours a week; tested in the first 8 weeks |
| Truthfulness | Not tripped; single channel, named stores and a tie threshold |
| Demand | Not tripped before building; tested at 6 months |

## Out of scope for the MVP

- Monitorul Prețurilor (the owner's ruling).
- Chain websites, accounts, cards and apps as price sources.
- Any request for permission or data, partners, outreach and grant applications.
- The discount check, the cross-country view and a second city.
- A native app, custom user Baskets and accounts, and live search across all products.

## Still open before launch

- [ ] The IT lawyer's answers ([Get a Romanian IT lawyer to confirm our collection and publication approach](https://github.com/exilonX/cart-compare/issues/23)).
- [ ] The item list: about 25–30 specifications and the quantities for each household Basket. ICCV's published decent-living Baskets are a reference to read.
- [ ] The four stores: one per Chain, close together, so a weekly round fits the hours.
- [ ] A trial round, timed, before the first published week.
- [ ] The returning-visitor threshold for the 6-month stop rule, and a privacy-respecting way to count returning visitors.
- [ ] A baseline for measuring our own Social value, collected before launch (see the map's "Not yet specified").
