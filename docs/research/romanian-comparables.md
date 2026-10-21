# What are Romanian private Comparables already doing, and what gap do they leave?

Research for ticket [#14](https://github.com/exilonX/cart-compare/issues/14) on map [#1](https://github.com/exilonX/cart-compare/issues/1). Desk research, 2026-10-21. This builds on [#8 Monitorul Prețurilor](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md), which first found gov2-ro, money.ro and RadarPrețuri, and on [#7 Romanian shoppers](https://github.com/exilonX/cart-compare/blob/research/romanian-shoppers/docs/research/romanian-shoppers.md). Findings from those files are not repeated here.

We read public pages, public GitHub repositories and their licences. We did not scrape or bulk-download any site. Terms follow `CONTEXT.md`: Comparable, Demand signal, Social value, Basket, Chain, Shelf price, Loyalty price, Reported price. Romanian quotes come with an English translation.

Every project here was built by people working on the same problem we are. Where we note a limitation, we mean it as a description of the current state, not as criticism.

**Evidence tiers**, strongest first. Each important claim carries one:

- **[A]** Academic study. None was found (see Gaps).
- **[O]** Official or regulator document.
- **[U]** Usage statistics: app-store ratings, traffic figures. Counters a project shows about itself are marked [U, self-reported].
- **[Obs]** Our own direct check of a public page, repository, licence or domain on 2026-10-21. This shows what is published, not whether it is true.
- **[S]** A project's own description of itself, on its site, in its repo or in its terms. We did not verify it independently.
- **[M]** Media report or anecdote.

## Answer

- **Ranking Baskets across Chains is already being done in Romania.**
  - [money.ro](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026) published a one-day ranking of 11 staples across 7 Chains in Bucharest on 10 Oct 2026, with a method note and a CSV [Obs].
  - [gov2-ro](https://github.com/gov2-ro/monitorulpreturilor) has computed 4 curated pantry Baskets per Chain since April 2026, nationally and for each municipality, with a cost trend [Obs].
  - RadarPrețuri says its shopping-list tool shows the cheapest store for a whole list [S].
  - So a Bucharest Basket ranking on its own would repeat existing work.
- **None of them is a regular, open, citable index today.**
  - money.ro's ranking covers a single day and is not announced as a series [Obs].
  - gov2-ro's public site was "dark for eight weeks" up to 4 Sep 2026, by its maintainer's own account. Its domain did not resolve on 21 Oct 2026, and the repository has no licence [Obs].
  - RadarPrețuri names neither its operator nor its matching method [Obs].
- **No Comparable found offers four of the Overview's features:**
  - Branded and private-label Baskets kept apart;
  - Shelf price and Loyalty price side by side;
  - a documented quality tier for private-label matching;
  - cost in minutes of work at the median wage, or a comparison with and without VAT.
- **Four features are partly done:**
  - *Published matching.* money.ro publishes exact product names, and gov2-ro publishes the product IDs in each Basket. Neither publishes written matching rules [Obs].
  - *History.* gov2-ro keeps a daily Basket cost trend and a "civic inflation" chart, but its site is offline [Obs]. PromoAzi offers 90 days of history per product [S].
  - *Suspicious discounts.* PromoAzi says its history lets users "vezi dacă reducerea e reală" ("see whether the discount is real"). It publishes no systematic flag [S].
  - *Cross-country.* money.ro priced a 7-item Lidl Basket in 6 countries on 8 Oct 2026 and expressed it as Baskets per average net salary. That was a one-off [Obs].
- **Both Basket rankings use Monitorul Prețurilor's Reported prices,** so they inherit its gaps (#8). Neither shows a Loyalty price.
  - gov2-ro's April 2026 notes say the platform carries no fresh dairy, meat or produce [S].
  - money.ro's October Basket includes milk, butter and cheese taken from the same platform [Obs].
  - This contradiction matters for the Family Basket and is unresolved.
- **The Demand signals are alive and growing in number.** Five deal or leaflet products were live on 21 Oct 2026:
  - two belong to international leaflet groups: Blix (Qpony, Poland) and Ofertelino, most likely Ofertolino (ShopFully/Offerista; `ofertelino.ro` does not resolve);
  - three are Romanian independents: PromoAzi (Axiom Software SRL, launched Oct 2025), zgârcit.ro (one person, funded by donations) and Listiq.
  - None publishes user numbers. All of them work from promotions or catalogues, not full Baskets [Obs][S].
- **We found little media pickup.**
  - The only third-party coverage found was Economedia's guide of May 2026, which is sponsored by Banca Transilvania. It describes RadarPrețuri, Blix, Ofertelino and Listiq [M].
  - We found no coverage of gov2-ro, of money.ro's ranking, of PromoAzi or of zgârcit.ro. Only three searches were run, so this is a weak negative.
- **A Comparable not on the ticket also exists.** The consumer NGO InfoCons publishes recurring "Cât ne costă alimentele de bază" ("what basic foods cost us") minimum-price studies across 9 Chains in Bucharest (Aug 2025 to Sep 2026), including a year-on-year comparison [Obs].
- **What only the Grocery Basket Index would add:** a weekly, openly licensed, archived Basket series, with:
  - published rules;
  - a Branded / private-label split;
  - the Shelf price and the Loyalty price side by side;
  - a wage-based cross-country view.
  The biggest overlap is with gov2-ro. money.ro is the closest newsroom doing similar work.

## 1. The projects compared

### Who runs it, whether it is alive, reach and media pickup

| Project | Type | Who runs it | Alive on 2026-10-21? | Audience and reach | Media pickup found |
|---|---|---|---|---|---|
| **gov2-ro / Guvernul Paralel**, [monitorulpreturilor.gov2.ro](https://github.com/gov2-ro/monitorulpreturilor) | Comparable (civic) | GitHub organisation "GOV2RO", described as "Guvernul Paralel" ("the Parallel Government"), created 2021, 23 public repos. The repo's main author is Alex Popescu (GitHub `pax`), with 153 of 172 commits. | **Data pipeline: yes.** Latest commit 19 Oct 2026, on branch `phase0-restore-publishing`. **Public site: no.** The domain does not resolve, and GitHub Pages returns 404 [Obs]. | GitHub: 1 star, 0 forks [Obs]. No traffic figures published. | None found |
| **money.ro Basket ranking** ([10 Oct 2026](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)) | Comparable (newsroom) | money.ro, published by OSAL LLC INTERNATIONAL SRL (CUI RO15807719). Launched 2008. Editor-in-chief Radu Burlacu. The article has no byline ([about page](https://www.money.ro/despre-noi)) [S]. | **Yes, as an outlet.** The ranking is a single-day piece. Related pieces: a compiled "Top 10" (16 Aug 2026) and a 6-country Lidl Basket (8 Oct 2026). No series is announced [Obs]. | No audience figures published [Obs]. | It is itself media. No re-reporting by others found. |
| **RadarPrețuri** ([radarpreturi.ro](https://radarpreturi.ro/despre)) | Comparable (private) | Not named. Guides are signed "fondatorul RadarPreturi" ("the RadarPreturi founder") [Obs]. | **Yes.** A guide was updated 19 Oct 2026, with data "până la 20.10.2026" ("up to 20 Oct 2026") [Obs]. It predates April 2026: gov2-ro's readme lists it as prior art ([readme](https://github.com/gov2-ro/monitorulpreturilor#reference--inspiration--previous-art)) [Obs]. | About 131,500 products in 35 categories: the sum of category counts on [/preturi](https://radarpreturi.ro/preturi), which may double-count [U, self-reported]. No user figures. | Economedia guide, 27 May 2026 (sponsored) [M] |
| **PromoAzi** ([promoazi.ro](https://promoazi.ro/)) | Demand signal; would become a Comparable once "Liste inteligente" (smart lists) ships | Axiom Software SRL, CUI 52759896. Part of an "Azi" family with FarmaAzi and CarburantAzi ([about](https://promoazi.ro/despre-noi)) [S]. | **Yes.** Launched October 2025 [S]. Shows "Date actualizate azi" ("data updated today"); latest blog post 17 Oct 2026 [Obs]. | About 19,746 active promotions and 50,000+ indexed offers [U, self-reported, 21 Oct 2026]. No user figures. | None found |
| **zgârcit.ro** ([zgarcit.ro](https://zgarcit.ro/)) | Demand signal | Vlad Solomon, a private individual in Bucharest, named as data controller in the [privacy policy](https://zgarcit.ro/confidentialitate) (updated 6 Apr 2026) [S]. | **Yes.** Shows offers valid to 27 October [Obs]. | 24,187 products listed [U, self-reported]. No user figures. | None found |
| **Blix** ([blix.ro](https://blix.ro/)) | Demand signal | Qpony.pl Sp. z o.o., Poznań, Poland, KRS 0000432201 ([terms](https://blix.ro/terms)) [S]. | **Yes.** iOS version 5.39.0, dated "13 Oct" with no year shown ([App Store RO](https://apps.apple.com/ro/app/id1583732676)) [U]. | iOS Romania: 4.9/5 from 12 ratings. The listing claims "peste un milion de utilizatori" ("over one million users"), apparently across all countries [U]. | Economedia guide [M] |
| **Ofertelino**, most likely **Ofertolino** ([ofertolino.ro](https://www.ofertolino.ro/)) | Demand signal | Its legal links point to Offerista and ShopFully. The imprint names Shopfully Romania SRL (J40/17109/2023, Bucharest) under "Offerista Group Romania" ([impressum](https://www.offerista.com/ro/impressum)). The App Store lists Prospecto Group JSC, with a provider in Sofia ([App Store RO](https://apps.apple.com/ro/app/id1262459120)) [S]. | **Yes.** The site shows "398 de oferte și 128 de cataloage" ("398 offers and 128 catalogues"). `ofertelino.ro` does not resolve [Obs]. | Website: 4.7 from 1,285 ratings. iOS Romania: 4.7 from 96 ratings [U]. | Economedia guide, which spells it both ways [M] |
| **Listiq** ([listiq.ro](https://listiq.ro/)) | Demand signal | Not named. Contact contact@listiq.ro. Terms updated March 2026 ([terms](https://listiq.ro/ro/terms)) [Obs]. | **Probably.** The site is up, with Google Play and App Store links [Obs]. | Its counters show only "0+" placeholders [Obs]. | Economedia guide [M] |

### Data source, method, openness

| Project | Data source | Method | Openness and licence |
|---|---|---|---|
| **gov2-ro** | Monitorul Prețurilor's undocumented XML service, so Reported prices. About 87K products and about 4,100 stores. Collected daily, with less frequent fetching for stores and products that rarely change. About 32.9M price rows on the maintainer's local copy on 7 Jul 2026 ([readme](https://github.com/gov2-ro/monitorulpreturilor), [activity log](https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/activity-log.md)) [Obs]. | **Baskets:** 4 curated Baskets defined in [`config/baskets.json`](https://github.com/gov2-ro/monitorulpreturilor/blob/main/config/baskets.json): Cămară (pantry, 11 items), Studentului (student, 8), de Copt (baking, 8), de Sărbători (holidays, 9). Each item lists 1–4 substitute product IDs plus a weekly quantity. The builder "picks the cheapest available at the network being scored", nationally and per municipality.<br>**Other features:** an anomaly list (the dearest Chain charging at least 1.5× the cheapest); price-quality flags (statistical outlier, day-over-day spike, `promo_too_deep` above 90%); a cost trend for each Basket; and "Inflația noastră vs. cea oficială" ("our inflation vs the official one"), which compares month-on-month rates with Eurostat HICP and INS, plus a nowcast [Obs]. | Public repo with **no licence**, so all rights are reserved by default [Obs]. The site, when online, served per-product CSVs and analytics CSVs; no licence was stated for them [Obs]. |
| **money.ro** | Monitorul Prețurilor, so Reported prices for 9 Oct 2026 [Obs]. | Per Chain, it takes "cel mai ieftin produs" ("the cheapest product") of each of 11 types, own brands included, so the items are not identical. Only products found in at least 30% of checked stores count. The price used is the most frequent one across up to 20 stores per Chain in different parts of Bucharest, or the middle value if no price repeats. Promotions active that day are included; Loyalty prices are not mentioned. Pack sizes are converted to standard quantities. Cluj-Napoca and Iași were recalculated with the same method; only their cheapest and dearest Chains are given [Obs]. | A per-Chain CSV with 84 rows ([csv](https://www.money.ro/date/cos-supermarketuri-bucuresti-2026-10-09.csv)). Columns: generic product, exact product name, pack size, Reported price, standardised price, promotion flag, stores with the product, stores checked, date. **No licence stated** [Obs]. Chains may reply at redactie@money.ro and the reply will be published in full; corrections are made visibly and dated [S]. |
| **RadarPrețuri** | "Surse publice online": merchant pages and catalogues, "feed-uri publice de prețuri" (public price feeds), and OpenStreetMap for locations ([despre](https://radarpreturi.ro/despre)) [S]. Covers four sectors: supermarkets, building materials, fuel, pharmacies. | Compares the same product across retailers, by unit price. Its guide says the list tool shows "which store is cheapest for the whole basket" and calls a Basket "o selecție fixă de produse echivalente" ("a fixed selection of equivalent products") ([guide](https://radarpreturi.ro/ghiduri/cosul-minim-de-cumparaturi)) [S]. No matching rules are published [Obs]. | No terms page and no licence found. Errors can be reported by email [Obs]. "Nu inventăm prețuri" ("we do not invent prices") [S]. |
| **PromoAzi** | "Colectăm automat ofertele din cataloagele retailerilor" ("we automatically collect offers from retailers' catalogues"). 9 Chains, including Metro and Selgros [S]. | Daily offers, 90-day history and price alerts. Some offers carry labels for card-only or app-only prices (for example "PENNY Card", "CONNECT"). Basket comparison ("Liste inteligente") is marked "În curând" ("coming soon"). Blog posts on trends and chain-versus-chain comparisons carry no byline and no method note ([example](https://promoazi.ro/blog/tendinte-preturi-septembrie-2026-ce-se-scumpeste-si-ce-se-ieftineste)) [Obs]. | The [terms](https://promoazi.ro/termeni-conditii) (10 Mar 2026) ban "instrumente automate (boți, scrapere)" ("automated tools, bots, scrapers") and reuse "în scop comercial … fără acordul nostru scris" ("for commercial purposes … without our written consent"). They state that prices and images belong to the retailers [S]. |
| **zgârcit.ro** | Not stated [Obs]. | Lists offers with old and new price, discount % and unit price. Filters for "Doar cu card de fidelitate" ("loyalty card only") and "Doar produse românești" ("Romanian products only"), plus a shopping list [Obs]. No ads; Google Analytics only with consent [S]. | No terms and no licence. Privacy policy only. Funded by donations through a personal Revolut link [Obs]. |
| **Blix** | Retailers' leaflets [S]. | Leaflet browsing, a shared shopping list, and a price comparison for favourite products, per its App Store description [S]. Economedia says it "nu compară direct toate prețurile" ("does not directly compare all prices") [M]. | Proprietary. The terms reserve all rights and ban bots that disrupt the app [S]. |
| **Ofertolino** | Retailers' catalogues, "more than 130 dealers" [S]. | Catalogues, favourites, alerts and a store map [S]. Economedia says it "nu colectează prețuri individuale din magazine" ("does not collect individual store prices") [M]. | Proprietary (Offerista terms) [Obs]. |
| **Listiq** | "Cataloage și oferte de la magazine terțe" ("catalogues and offers from third-party stores"), 16 Chains and DIY stores [S]. | Shopping list (1,000+ products), catalogues and a loyalty-card wallet. The site says users can compare prices between stores [S]. Economedia says it "nu compară automat prețuri între magazine" ("does not compare prices between stores automatically") [M]. | "© 2025 Listiq. Toate drepturile rezervate." ("All rights reserved") [Obs]. |

### Notes per project

**gov2-ro / Guvernul Paralel**

- **Purpose.** It describes itself as an "Interfață alternativă pentru monitorulpreturilor.info" ("an alternative interface for monitorulpreturilor.info"). It has the topics `civic-data`, `g0v` and `open-data` ([repo](https://github.com/gov2-ro/monitorulpreturilor)) [Obs]. The organisation runs other civic data projects: INS statistics, public-sector jobs, and a civic-tech directory ([gov2.ro](https://gov2.ro/)) [Obs].
- **Public site.**
  - The commit of 4 Sep 2026 says "the site had been dark for eight weeks and nothing regenerated it". It adds a daily build to a `gh-pages` branch, which was last built on 4 Sep 2026 ([commit 6d09bba](https://github.com/gov2-ro/monitorulpreturilor/commit/6d09bbac8144238a7a379f661ce0dbc58b3ec5ee)).
  - The script notes that GitHub Pages must be switched to that branch, and the custom domain re-added, by hand ([publish_site.sh](https://github.com/gov2-ro/monitorulpreturilor/blob/phase0-restore-publishing/scripts/publish_site.sh)).
  - On 21 Oct 2026 Pages still served `main:/docs` with no custom domain, and `monitorulpreturilor.gov2.ro` did not resolve [Obs].
  - The feature description below therefore comes from code and docs, not from the live site.
- **Data freshness, documented openly by the maintainer.**
  - On 4 Sep 2026, 79.69% of stores were "not yielding new data" ([commit 6d09bba](https://github.com/gov2-ro/monitorulpreturilor/commit/6d09bbac8144238a7a379f661ce0dbc58b3ec5ee)).
  - On 18 Oct 2026 a batch failure meant "the day wrote 0 prices". It was fixed the next day ([commit 0d7cfde](https://github.com/gov2-ro/monitorulpreturilor/commit/0d7cfdeb653fbef559ad509ec97808e83aaf4b0c)) [Obs].
  - It is essentially a one-maintainer project running a large, multi-day collection sweep across about 4,100 stores [Obs].
- **Fresh food.** The Basket file, last changed 18 Apr 2026, says: "The API only tracks shelf-stable goods (no fresh dairy / meat / produce), so these baskets reflect a PANTRY shop … labels and copy must be honest about that" ([baskets.json](https://github.com/gov2-ro/monitorulpreturilor/blob/main/config/baskets.json)) [S]. The product catalogue has since grown about 12-fold, to about 87K, per the [readme](https://github.com/gov2-ro/monitorulpreturilor). money.ro's October Basket draws milk, butter and cheese from the same platform [Obs]. The statement may be out of date. See Gaps.
- **Planned, not built.** The [UI plan](https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/ui-plan.md) lists:
  - a "Promo Analysis": "Are 'promo' prices actually cheaper than competitors' regular prices?";
  - a "Brand Landscape" that identifies private-label products;
  - a weekly HTML report "Shareable, SEO-friendly";
  - an open data API.
  Its roadmap also lists "Deduplicate products with different names but same item" [S].

**money.ro**

- **The October ranking (Bucharest, 9 Oct 2026 prices).** Lidl came out cheapest at 45.38 lei and Mega Image dearest at 61.38 lei (+35.3%), with Penny, Auchan, Kaufland, Carrefour and Profi in between. Excluded: Selgros (cash and carry), Supeco (one store), Cora (no updates since May 2025) and Metro (no prices) ([money.ro](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)) [Obs]. Figures beyond those in #8 are given in the table above.
- **The cross-country piece**, "Același coș de la Lidl, în 6 țări. Un român cumpără 131 de coșuri dintr-un salariu, un neamț 323" ("The same Lidl basket in 6 countries: a Romanian buys 131 baskets from one salary, a German 323"), 8 Oct 2026 ([money.ro](https://www.money.ro/stiri/acelasi-cos-de-la-lidl-in-6-tari-romania-germania-elvetia-oct-2026)) [Obs]:
  - **Countries:** Romania, Germany, Hungary, Bulgaria, Czechia and Switzerland. Austria, Italy, Slovakia and Poland were dropped because Lidl does not publish regular prices online there.
  - **Basket:** 7 core items, plus 3 items not available everywhere. The prices are "prețurile obișnuite, fără promoții" ("regular prices, without promotions"), taken from official price monitors (Romania, Hungary, Bulgaria) or from Lidl's own sites and catalogues. Lidl's own brands differ by country.
  - **Currency:** converted at BNR rates of 8 Oct 2026.
  - **Wage measure:** Baskets per average net monthly salary for a single person, from Eurostat 2025, or OECD for Switzerland. No minutes of work, no median wage, and VAT is not discussed.
  - **Result:** Romania is second cheapest on price (47.25 lei) and fourth of six on Baskets per salary.
  - No CSV is published.
- **The earlier "Top 10 supermarketuri" (16 Aug 2026)** compiles InfoCons studies (Sep 2025, Mar 2026), a LifeTips comparison (Nov 2025) and Monitorul Prețurilor. It gives totals for only some Chains and has no download ([money.ro](https://www.money.ro/topul-zilei/top-10-supermarketuri-dupa-preturi-romania-2026)) [Obs].
- **AI policy, dated 15 Oct 2026.** Reporters may use AI to check calculations, but "Nu publicăm citate, cifre sau afirmații produse de AI fără verificare în surse" ("we do not publish AI-produced quotes, figures or claims without checking them against sources") ([policy](https://www.money.ro/politica-ai)) [S].

**RadarPrețuri**

- **Classification.** A Comparable: it compares prices across Chains at product level and, by its own account, for a user's list.
- **Scale.** Its guide gives one category figure: "6.771 de produse urmărite" ("6,771 products tracked") in dairy and eggs, with data up to 20 Oct 2026 ([guide](https://radarpreturi.ro/ghiduri/cele-mai-ieftine-magazine)) [U, self-reported].
- **Rankings.** It deliberately does not name a cheapest Chain overall. Its guide says no Chain is cheapest in every category, and that a ranking for one Basket does not transfer to another [S].
- **Freshness.** Economedia notes "pot exista decalaje față de actualizările de prețuri din magazine" ("there may be lags behind price updates in stores") ([Economedia](https://economedia.ro/ghid-cum-sa-identifici-cele-mai-mici-preturi-la-alimente-fara-sa-pierzi-ore-intregi-in-magazine.html)) [M].
- **Not readable.** The Google Play page could not be read with our tools, so its install figures and developer name are missing. See Gaps.

**PromoAzi.** It is the closest Demand signal to a Comparable. It has three features in the Overview's territory: per-product history, alerts, and the claim to show whether a discount is real. Its basket feature is announced but not live. Its terms rule out reusing its data without written consent [S].

**zgârcit.ro, Blix, Ofertolino, Listiq.** All four are built around promotions or leaflets, and none totals a Basket.

- **zgârcit.ro** is the only one with a loyalty-card filter. It is a one-person, donation-funded project with no ads [Obs][S].
- **Blix and Ofertolino** belong to international leaflet-advertising groups. ShopFully also publishes the shopper surveys cited in #7, a conflict of interest that #7 already notes.

### Other Comparables surfaced (not on the ticket)

- **InfoCons (consumer NGO).** Recurring "Studiu InfoCons … Cât ne costă alimentele de bază" ("InfoCons study … what basic foods cost us") studies. Editions found: Aug 2025, Sep 2025, Mar 2026, Sep 2026, plus a Sep 2025 vs Sep 2026 comparison.
  - It reports minimum prices for 5 staples at one store of each of 9 Chains in Bucharest Sector 4 (including La doi pași and Selgros), VAT included.
  - Results come as top lists per product, not Basket totals, and the collection method is not stated.
  - "© Toate drepturile rezervate InfoCons" ("all rights reserved") ([Sep 2026](https://infocons.ro/studiu-infocons-protectia-consumatorilor-cat-ne-costa-alimentele-de-baza-in-luna-septembrie-2026/), [YoY comparison](https://infocons.ro/studiu-comparativ-infocons-protectia-consumatorilor-cat-ne-costa-alimentele-de-baza-septembrie-2025-vs-septembrie-2026/)) [Obs].
  - money.ro's August ranking relies on these studies.
- **Media Basket pieces.** Search results show more one-off media comparisons: a Christmas Basket ([Wall-Street.ro, 2025](https://www.wall-street.ro/articol/retail/cosul-de-craciun.html)) and a Lidl Romania vs Hungary piece ([Economica.net](https://www.economica.net/lidl-romania-vs-ungaria-unde-este-mai-ieftin-sa-faci-cumparaturi_538890.html/amp)). Neither was opened, so treat them as leads [M].
- **Developer projects on Monitorul Prețurilor data.** [hbrnm/legendary-winner](https://github.com/hbrnm/legendary-winner/pull/22) (see #8), and a Home Assistant fuel-price integration under the MIT licence ([mocanu-alexandru/ha-fuel-prices-ro](https://github.com/mocanu-alexandru/ha-fuel-prices-ro)) [Obs].

## 2. Feature gap: the Overview's planned features against existing work

"Nobody" means no Romanian Comparable or Demand signal found in this pass does it. It does not mean nobody does it anywhere.

| Overview feature | Who already does it in Romania (2026-10-21) | Verdict |
|---|---|---|
| **Basket ranking per Chain, gap in lei and %** | money.ro: 11 items, 7 Chains, one day, Bucharest totals; Cluj and Iași ranks only [Obs]. gov2-ro: 4 pantry Baskets, daily, national and per municipality, but the site is offline [Obs]. RadarPrețuri: user lists [S]. InfoCons: minimum prices per item, no totals [Obs]. | **Would duplicate** if offered alone. What stays distinct is a regular, archived series. |
| **Shelf price and Loyalty price side by side** | Nobody. money.ro and gov2-ro use Reported prices with promotions mixed in. PromoAzi labels some card-only offers; zgârcit.ro filters loyalty-card deals. Neither totals a Basket [Obs]. | **Nobody** |
| **Published item list and matching rules** | money.ro: item list, a method paragraph, and a CSV with exact product names [Obs]. gov2-ro: product IDs per item with a "cheapest substitute" rule, in an unlicensed repo [Obs]. RadarPrețuri: "produse echivalente" ("equivalent products"), with no rules [S]. Nobody documents a private-label quality tier. | **Partly done.** Written rules and a quality tier: nobody. |
| **Branded Basket vs private-label Basket** | Nobody. money.ro and gov2-ro both take the cheapest product, so brands and own labels are mixed. gov2-ro exports a "private_labels.csv" list of candidates and plans a "Brand Landscape" view [Obs][S]. | **Nobody** |
| **Weekly history per Basket and per product** | gov2-ro: daily Basket cost trend since April 2026, plus "civic inflation" against HICP; offline [Obs]. PromoAzi: 90-day history per product [S]. InfoCons: year-on-year snapshots [Obs]. | **Partly done.** A public, citable, archived Basket series that is online today: nobody. |
| **Flag for suspicious discounts** | PromoAzi: history so users can "vezi dacă reducerea e reală" ("see whether the discount is real"); no systematic or published flag found [S][Obs]. gov2-ro: flags data errors (promotion deeper than 90%, spikes), not fake discounts. Its "Promo Analysis" is only planned [Obs][S]. | **Partly overlaps PromoAzi** at product level. A published, rule-based flag: nobody. |
| **Region view (a second Romanian city)** | money.ro: Cluj-Napoca and Iași, ranks only [Obs]. gov2-ro: Basket cost per municipality on a map; offline [Obs]. | **Would duplicate** gov2-ro if it comes back online. |
| **Country view, same Basket elsewhere** | money.ro: Lidl in 6 countries, one-off, 8 Oct 2026, own brands that differ by country [Obs]. IELKA covers Romania with three Chains (see #3). | **Partly done** as one-offs. A recurring view of identical international brands: nobody. |
| **With and without VAT** | Nobody found. money.ro does not discuss VAT; InfoCons states its prices include VAT [Obs]. | **Nobody** |
| **Cost in minutes of work at the median net wage** | Nobody. money.ro expresses cost as Baskets per *average* net monthly salary (Eurostat 2025) [Obs]. | **Nobody**, though money.ro's measure is close in spirit |
| **Shareable weekly cards** | Not assessed; none seen on the pages read. | Unknown |

## 3. Collaboration potential (facts only)

- **gov2-ro.**
  - Practically a one-person project, by commit count: Alex Popescu (`pax`, blog [pax.mioritics.ro](https://pax.mioritics.ro)). It sits inside a civic organisation that publishes several open-government tools [Obs].
  - It already holds Monitorul Prețurilor price history from April 2026 [Obs].
  - Its roadmap includes product de-duplication and cross-referencing with Open Food Facts, which is matching work [S].
  - The repo has no licence, so reusing its code or data needs the author's permission [Obs].
  - Its readme credits radarpreturi.ro as prior art [Obs].
- **money.ro.**
  - It publishes Basket rankings and a cross-country Basket, both with a method note, and a CSV for the domestic one [Obs].
  - It invites Chains to reply (redactie@money.ro) and keeps a corrections page ([/corectii](https://www.money.ro/corectii)) [S].
  - Its AI policy requires source checks for figures [S].
- **InfoCons.** Runs recurring minimum-price studies at 9 Chains [Obs]. #7 notes it appears often on TV.
- **RadarPrețuri.** The operator is unnamed. It accepts error reports by email, and its guides cite sources and observation dates [S].
- **PromoAzi.** Run by a registered company. Its terms forbid scraping and commercial reuse without written consent, so any data use would need an agreement [S].
- **zgârcit.ro.** Run by one person (Vlad Solomon), funded by donations, no ads [S].
- **Blix, Ofertolino.** Commercial leaflet platforms owned by Qpony (Poland) and the ShopFully/Offerista group [S].
- **Listiq.** Operator not named; contact@listiq.ro [Obs].

## Gaps and uncertainties

- **No academic study** of any Romanian private Comparable was found [A: none]. The search budget was limited, and Google Scholar was not queried.
- **No usage figures for any project.**
  - Google Play pages could not be read with our fetch tool, so install bands for RadarPrețuri, Blix, Listiq and PromoAzi are missing.
  - iOS listings give rating counts only, with version dates that show no year.
  - Self-reported counters (offers, products) are not audience figures.
  - No traffic estimates (Ahrefs or similar) were collected for these sites.
- **Media pickup is a weak negative.** Only three web searches were run, on a US-indexed engine that under-covers Romanian outlets. "None found" does not mean "none exists".
- **We have not seen gov2-ro's site.** It was offline on 21 Oct 2026, so its features are inferred from code, configuration and commit messages. Whether the published pages showed CSV downloads, and under what terms, was not seen.
- **Fresh food on Monitorul Prețurilor.** gov2-ro (Apr 2026) says the platform has no fresh dairy, meat or produce. money.ro (Oct 2026) priced milk, butter and cheese from it. Either the catalogue changed, or "fresh" means different things in the two sources. This was not resolved.
- **RadarPrețuri's operator, launch date and app figures** are unknown. Its only data-source statement is generic ("surse publice online", public online sources).
- **PromoAzi's "is the discount real" claim** was not tested on a product page. We do not know whether it computes anything beyond showing history.
- **Blix's "over one million users"** is not broken down by country. Its Romanian iOS listing has 12 ratings.
- **Listiq's operator** is not named on its site or in its terms.
- **The Economedia guide** that most of the Demand signals' media pickup rests on is labelled "Articol susținut de Banca Transilvania" ("article supported by Banca Transilvania").
- **Social value.** No evidence was found, either way, about price outcomes, shopper behaviour or policy effects of any of these projects.
- **InfoCons' collection method** (in store or online) is not stated on the September 2026 page. Its exact collection date (15 Sep 2026) comes from a search snippet of the comparison page.

## Questions this raises

1. **Reframe the MVP pitch.** A Basket ranking per Chain is no longer new in Romania. Should Overview v2 lead with what nobody does instead? That means the weekly archived series, the Branded / private-label split, the Shelf price and the Loyalty price side by side, published rules with a quality tier, and the wage-based cross-country view.
2. **gov2-ro: collaborate or build separately?** It already mirrors Monitorul Prețurilor daily, with history since April 2026, and computes Baskets per municipality. Options:
   - ask for a licence and reuse its history;
   - agree to share matching rules;
   - build separately.
   Which one avoids two civic mirrors of the same state data? This ties to #8 question 3.
3. **money.ro as a distribution partner?** It already publishes Basket rankings, a cross-country Basket and a CSV, and it invites Chains to respond. Would it run a weekly series on our data? Would its method choices (most frequent price across 20 stores, cheapest product, promotions included) clash with ours?
4. **Check the fresh-food coverage of Monitorul Prețurilor.** Does it carry fresh dairy, meat and produce by product and per kg? The answer decides whether the Family Basket (about 30 items, fresh produce per kg) can rest on Reported prices or needs retailer-site collection.
5. **The suspicious-discount flag: what makes ours different?** PromoAzi already shows product history to judge discounts. Romanian rules on showing a prior reference price were not checked here. Should a separate ticket set out the legal reference-price rule, and design a Basket-level, rule-based flag?
6. **Minutes of work, or Baskets per salary?** money.ro uses average net salary; the Overview plans median net wage. Does #3's cross-country work, or a wage ticket, need to confirm median availability before the Overview commits to it?
7. **Bring in InfoCons?** It is a recurring NGO Comparable at 9 Chains, and #7 lists it as a possible partner. Should its studies be read in full: method, frequency, any data download?
8. **Correct an earlier finding.** #7 concluded that the press teaches readers to build a Basket index by hand "because no tool does it". gov2-ro, RadarPrețuri's list tool and money.ro now make that only partly true. Should #7's reading be amended on the map?

## Sources

Projects' own pages and repositories (read 2026-10-21):

1. gov2-ro, monitorulpreturilor repository and readme. https://github.com/gov2-ro/monitorulpreturilor
2. gov2-ro, Basket definitions, `config/baskets.json` (last changed 18 Apr 2026). https://github.com/gov2-ro/monitorulpreturilor/blob/main/config/baskets.json
3. gov2-ro, activity log. https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/activity-log.md
4. gov2-ro, backlog. https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/backlog.md
5. gov2-ro, UI plan. https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/ui-plan.md
6. gov2-ro, commit 6d09bba "restore publishing…", 4 Sep 2026. https://github.com/gov2-ro/monitorulpreturilor/commit/6d09bbac8144238a7a379f661ce0dbc58b3ec5ee
7. gov2-ro, commit 0d7cfde "split batches on 5xx…", 19 Oct 2026. https://github.com/gov2-ro/monitorulpreturilor/commit/0d7cfdeb653fbef559ad509ec97808e83aaf4b0c
8. gov2-ro, `scripts/publish_site.sh` (branch phase0-restore-publishing). https://github.com/gov2-ro/monitorulpreturilor/blob/phase0-restore-publishing/scripts/publish_site.sh
9. GOV2RO organisation and gov2.ro home page. https://github.com/gov2-ro, https://gov2.ro/
10. money.ro, "Coșul cu 11 produse de bază în 7 supermarketuri", 10 Oct 2026. https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026
11. money.ro, CSV for the 9 Oct 2026 Basket. https://www.money.ro/date/cos-supermarketuri-bucuresti-2026-10-09.csv
12. money.ro, "Același coș de la Lidl, în 6 țări…", 8 Oct 2026. https://www.money.ro/stiri/acelasi-cos-de-la-lidl-in-6-tari-romania-germania-elvetia-oct-2026
13. money.ro, "Top 10 supermarketuri după prețuri în România", 16 Aug 2026. https://www.money.ro/topul-zilei/top-10-supermarketuri-dupa-preturi-romania-2026
14. money.ro, about page, contact page and AI policy (15 Oct 2026). https://www.money.ro/despre-noi, https://www.money.ro/contact, https://www.money.ro/politica-ai
15. RadarPrețuri, about page and llms.txt. https://radarpreturi.ro/despre, https://radarpreturi.ro/llms.txt
16. RadarPrețuri, price categories. https://radarpreturi.ro/preturi
17. RadarPrețuri, guides "Cele mai ieftine magazine" and "Coșul minim de cumpărături" (published 22 Jun 2026, updated 19 Oct 2026). https://radarpreturi.ro/ghiduri/cele-mai-ieftine-magazine, https://radarpreturi.ro/ghiduri/cosul-minim-de-cumparaturi
18. PromoAzi, home page, about page, terms (10 Mar 2026) and blog. https://promoazi.ro/, https://promoazi.ro/despre-noi, https://promoazi.ro/termeni-conditii, https://promoazi.ro/blog
19. zgârcit.ro, home page and privacy policy (6 Apr 2026). https://zgarcit.ro/, https://zgarcit.ro/confidentialitate
20. Blix, home page and terms. https://blix.ro/, https://blix.ro/terms
21. Ofertolino, home page; Offerista imprint. https://www.ofertolino.ro/, https://www.offerista.com/ro/impressum
22. Listiq, home page and terms (March 2026). https://listiq.ro/, https://listiq.ro/ro/terms
23. InfoCons, minimum-price study for September 2026 (16 Sep 2026), and the Sep 2025 vs Sep 2026 comparison. https://infocons.ro/studiu-infocons-protectia-consumatorilor-cat-ne-costa-alimentele-de-baza-in-luna-septembrie-2026/, https://infocons.ro/studiu-comparativ-infocons-protectia-consumatorilor-cat-ne-costa-alimentele-de-baza-septembrie-2025-vs-septembrie-2026/

Usage statistics:

24. App Store Romania, "Blix – cataloage și oferte". https://apps.apple.com/ro/app/id1583732676
25. App Store Romania, "Ofertolino.ro". https://apps.apple.com/ro/app/id1262459120

Media:

26. Economedia (Elisabeta Minovici), price-hunting guide, 27 May 2026, updated 16 Jul 2026; sponsored by Banca Transilvania. https://economedia.ro/ghid-cum-sa-identifici-cele-mai-mici-preturi-la-alimente-fara-sa-pierzi-ore-intregi-in-magazine.html
27. Wall-Street.ro, Christmas Basket 2025 (search result only, not opened). https://www.wall-street.ro/articol/retail/cosul-de-craciun.html
28. Economica.net, Lidl Romania vs Hungary (search result only, not opened). https://www.economica.net/lidl-romania-vs-ungaria-unde-este-mai-ieftin-sa-faci-cumparaturi_538890.html/amp

Other repositories:

29. hbrnm/legendary-winner, PR #22. https://github.com/hbrnm/legendary-winner/pull/22
30. mocanu-alexandru/ha-fuel-prices-ro (MIT). https://github.com/mocanu-alexandru/ha-fuel-prices-ro

Earlier research on this map:

31. #8, Monitorul Prețurilor. https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md
32. #7, Romanian shoppers. https://github.com/exilonX/cart-compare/blob/research/romanian-shoppers/docs/research/romanian-shoppers.md
33. #3, CEE Comparables (IELKA). https://github.com/exilonX/cart-compare/blob/research/cee-comparables/docs/research/cee-comparables.md
