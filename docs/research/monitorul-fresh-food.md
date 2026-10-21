# Does Monitorul Prețurilor cover fresh food, and for which Chains?

Research for ticket [#27](https://github.com/exilonX/cart-compare/issues/27) on map [#1](https://github.com/exilonX/cart-compare/issues/1). Desk research, 2026-10-21. This builds on [#8 Monitorul Prețurilor](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md) and [#14 Romanian Comparables](https://github.com/exilonX/cart-compare/blob/research/romanian-comparables/docs/research/romanian-comparables.md), where the contradiction was found. Findings from those files are not repeated.

**Method.** The platform was not queried and its API was not called. Evidence comes from:

- the Competition Council's own releases;
- two public platform pages, read by hand;
- gov2-ro's public GitHub repository, including its `gh-pages` site build of 4 Sep 2026 and its committed CI database (prices from 13–25 Apr 2026);
- money.ro's 10 Oct 2026 method note and CSV.

Every observation of a file is dated 2026-10-21 unless stated otherwise.

**Evidence tags** (same scheme as #8): **[O]** official or regulator document; **[I]** independent technical analysis or data (gov2-ro); **[M]** media; **[Obs]** our own reading of a public file or page on 2026-10-21.

## Answer

- **Yes, the platform carries fresh food, and has done since at least April 2026.** gov2-ro's own published category trend shows priced products in dairy (LACTATE), fruit (FRUCTE), vegetables (LEGUME), eggs (OUA), fish (PESTE) and cold cuts (MEZELURI) on most days from 26 Apr to early September 2026, with up to 168 dairy, 234 fruit, 358 vegetable and 25 egg products a day ([trends.html](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/trends.html)) [I][Obs]. The platform's own category tree has branches for fresh meat, fresh vegetables, fresh fish, fresh bread, milk and eggs ([category list saved by gov2-ro, 14 Apr 2026](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/reference/GetProductCategoriesNetwork.xml)) [I].
- **Coverage is strong for dairy and bread across all 8 Chains, thinner for produce, and weakest for eggs and raw meat.**
  - *Dairy:* milk, butter, cheese and yoghurt have Reported prices at all 8 Chains. Branded dairy is among the most widely reported products on the platform. For example, Albalact butter 200 g is reported by 10 networks in 98% of stores ([analytics.html](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/analytics.html)) [I].
  - *Bread:* 7 Chains, including unpackaged loaves ([money.ro CSV](https://www.money.ro/date/cos-supermarketuri-bucuresti-2026-10-09.csv)) [M].
  - *Packed fruit:* 7 Chains [I].
  - *Fruit and vegetables sold by weight:* evidence for only 3 Chains (Lidl, Penny, Carrefour) [I].
  - *Eggs:* the category is priced, but which Chains report it is not visible in any public file.
  - *Raw meat:* no solid evidence for any Chain. What appears is mostly cooked meat sold by the kilo (see table).
- **Fresh produce is sometimes priced per kg, but the data cannot tell you which items are.** Loose items appear under names such as "Nectarine Vrac" or "Ananas/Kg", or under bare names such as "Rosii", next to fixed packs such as "Ceapa Galbena 5 Kg" [I]. The `unit` field cannot separate them: in April 2026, Carrefour sent "K" and Profi "Kg" as the unit for most rows, including jars and packets ([CI database](https://github.com/gov2-ro/monitorulpreturilor/blob/8ed0d5a893226ad1a52d22b107b0f83ec6ce4f09/data/prices_ci.db)) [I][Obs].
- **Updates are nightly loads, not a fresh-food schedule.** The only official statement is still the 2020 "daily" upload (see #8). On the platform, prices carry a load stamp of 20:00 or 04:00 for every Chain and every category [I][Obs]. gov2-ro found that this stamp "increments daily even when prices don't change" ([activity log, 28 Apr 2026](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/activity-log.md)) [I]. So no public source shows how quickly a change to a fresh price reaches the platform.
- **The Competition Council describes the scope as all food, and its capped-staples section names fresh items.**
  - In May 2024 its president said "Avem toate magazinele din ţară, cu toate produsele alimentare" ("we have all the shops in the country, with all food products") ([Economica.net, 25 May 2024](https://www.economica.net/consiliul-concurentei-va-lansa-o-varianta-simplificata-a-monitorului-preturilor-care-va-contine-doar-produsele-de-baza-ale-caror-preturi-au-fost-plafonate_749405.html/amp)) [M quoting O].
  - Its July 2024 section for products with a capped markup lists 41 staples. They include milk, eggs, chicken and pork cuts, tomatoes, potatoes and apples, shown "aşa cum sunt ele încărcate de fiecare retailer" ("as each retailer uploads them") ([Agerpres, 3 Jul 2024](https://agerpres.ro/economic/2024/07/03/consiliul-concurentei-a-actualizat-monitorul-preturilor-cu-o-sectiune-dedicata-produselor-cu-preturi--1322317)) [M quoting O].
  - No public document defines which categories each retailer must report.
- **Verdict: the family weekly Basket can rest on Reported prices only in part.**
  - *Can rest on Reported prices:* dairy, bread and pantry items, for all 8 Chains.
  - *Needs a second source:* fresh meat, eggs, and loose fruit and vegetables priced per kg. Retailer sites or store checks could fill this, or at least a verification pass before launch. The Overview's rule "fresh produce priced per kg" cannot be met from Reported prices alone.

## Coverage by category and Chain

What the cells mean:

- **Yes:** at least one Reported price was found in a public file.
- **Not seen:** not found in the files read. This is *not* proof that the Chain does not report the category.
- **?:** the evidence is ambiguous.

Dates are those of the underlying data.

Source keys:

- **MR:** [money.ro CSV](https://www.money.ro/date/cos-supermarketuri-bucuresti-2026-10-09.csv), Bucharest, 9 Oct 2026.
- **GP:** gov2-ro per-product CSVs, 26 Apr–2 Sep 2026, for these products:
  - [Napolact milk](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/data/products/1026990.csv)
  - [Albalact butter](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/data/products/1023867.csv)
  - [Olympus telemea](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/data/products/1043376.csv)
  - [Covalact yoghurt](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/data/products/1032584.csv)
  - [Almette sour cream](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/data/products/1021379.csv)
  - [packed oranges 1 kg](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/data/products/1013392.csv)
  - [packed strawberries 250 g](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/data/products/1010344.csv)
- **GA:** gov2-ro [analytics.html](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/analytics.html), snapshot to 2 Sep 2026.
- **GV:** gov2-ro [price variability analysis](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/price_variability_analysis.md), 6 May 2026.
- **GC:** gov2-ro [CI database](https://github.com/gov2-ro/monitorulpreturilor/blob/8ed0d5a893226ad1a52d22b107b0f83ec6ce4f09/data/prices_ci.db), prices from 13–25 Apr 2026.

| Category | Lidl | Kaufland | Carrefour | Mega Image | Profi | Penny | Auchan | Selgros |
|---|---|---|---|---|---|---|---|---|
| Milk | Yes, fresh "Lapte proaspat 1.5% Pilos" (MR) | Yes (MR, GP) | Yes, UHT (MR, GP) | Yes, UHT, in 7 of 20 stores (MR, GP) | Yes, fresh "Lapte proaspat 1.5%" (MR, GP) | Yes (MR, GP) | Yes (MR, GP) | Yes, until 12 May 2026 (GP) |
| Butter | Yes (MR, GP) | Yes (MR, GP) | Yes (MR, GP) | Yes (MR, GP) | Yes (MR, GP) | Yes (MR, GP) | Yes (MR, GP) | Yes, until 12 May 2026 (GP) |
| Cheese (cașcaval, telemea) | Yes (MR) | Yes, including loose cașcaval at 28.90 lei/kg (MR, GP) | Yes (MR, GP) | Yes (MR, GP) | Yes (MR, GP) | Yes (MR) | Yes (MR, GP) | Yes, until 25 Jun 2026 (GP) |
| Yoghurt, sour cream | Yes (GP) | Yes (GP) | Yes (GP) | Yes (GP) | Yes (GP) | Yes (GP) | Yes (GP) | Yes, until May–Jun 2026 (GP) |
| Bread | Yes (MR) | Yes, unsliced loaf (MR) | Yes (MR) | Yes (MR) | Yes, unpackaged (MR) | Yes, unpackaged (MR) | Yes, loaf (MR) | Not seen |
| Eggs | ? | ? | ? | ? | ? | ? | ? | ? |
| Packed fresh fruit | Yes, strawberries and oranges (GP) | Yes, strawberries, until 6 Aug 2026 (GP) | Yes, both (GP) | Yes, strawberries and avocado (GP, GA) | Yes, both (GP) | Yes, both (GP) | Yes, both (GP) | Not seen |
| Fruit and vegetables sold by weight | Yes: "Rosii", "Mere Rosii", "Pere", "Ardei Gras Verde", "Ananas/Kg" (GA) | Not seen | Yes: bell peppers 19.99–21.49 lei, potatoes 2.29 lei, at per-kg price levels (GV) | Not seen | Not seen | Yes: "Pastarnac,Vrac", "Nectarine Vrac", "Lamai Vrac" (GA) | Not seen | Not seen |
| Raw meat | ? "Piept Curcan Dez. Feliat", 22.99–27.79 lei; form unclear (GA) | Not seen | Not seen | Not seen | Cooked only: rotisserie chicken and sausages "/Kg", e.g. 24.90 lei (GC) | Not seen | Not seen | Not seen |

Notes on the table:

- **Eggs.** The OUA category carried up to 25 priced products a day between 26 Apr and 31 Aug 2026 ([trends.html](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/trends.html)). One egg product, "Oua 10+2buc Cod 0/Mi", appears at two unnamed networks (GA) [I]. money.ro's Basket has no eggs, and its method note does not say why ([money.ro](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)) [M].
- **Dairy and produce work differently.**
  - *Dairy* shares product IDs across Chains. At least 22 of the 200 most widely stocked products are dairy, such as Zuzu milk 1.5% (9 networks, 87.9% of stores) and Hochland telemea 350 g (10 networks, 97.8%).
  - *Produce, meat and eggs* appear nowhere in that top-200 list (GA) [I][Obs]. Fresh items are mostly chain-specific product IDs with free-text names. A Basket needs manual matching for them, which #8 already found unreliable when done automatically.
- **Store-level gaps in fresh items.** In money.ro's CSV, several fresh items were found in only some of the stores checked [M]:
  - Mega Image milk and cheese: 7 of 20 stores.
  - Profi bread: 8 of 20.
  - Carrefour butter and cheese: 11 of 20.

  Across all 7 Chains, the four fresh items were found in 82% of checked stores on average, with 6 of 28 entries below 60%. The seven pantry items were found in 89%, with 3 of 49 below 60% (our calculation from the CSV) [Obs]. The difference is modest.
- **Selgros.** Its series in gov2-ro's files stop in May–June 2026, as do Supeco's. This may reflect which stores gov2-ro polled and when, rather than these networks ceasing to report. We could not tell which [I][Obs].

## Per-kg pricing

- **The platform has per-kg items.**
  - Kaufland's loose cașcaval appears as "vrac / la kg" at 28.90 lei. money.ro converted it to 7.23 lei for 250 g ([CSV](https://www.money.ro/date/cos-supermarketuri-bucuresti-2026-10-09.csv)) [M].
  - Lidl, Penny and Carrefour report loose produce (table above) [I].
  - Profi reports cooked meat with "/Kg" in the product name (GC) [I][Obs].
- **Packs and loose items sit side by side.** Examples are "Portocale Amb 1kg" (packed oranges), "Cartofi Albi Spalati Punga 5kg" (a 5 kg bag of potatoes) and "Ceapa Galbena 5 Kg" (a 5 kg bag of onions) (GA) [I].
- **The unit field is not a guide.** In gov2-ro's April 2026 database [Obs]:
  - 36,010 of 39,668 Carrefour price rows carry the unit "K"; the rest carry "L". The "K" rows include "Jacobs Kronung Solubila 200g" at 59.25 lei.
  - 90,442 of 99,334 Profi rows carry "Kg"; most of the rest carry "Litru". The "Kg" rows include "Heinz Ketchup De Rosii 570g" at 1.99 lei.
  - Mega Image uses "BUCATI" (pieces), Kaufland "BUC" and Penny "BUCATA" for almost everything.

  Per-kg items have to be identified from the product name and a plausibility check on the price. Neither is reliable on its own.
- **Produce comparisons across Chains are noisy.** gov2-ro's list of the largest cross-chain spreads includes:
  - "Ceapa Galbena 5 Kg" at 5 networks, with per-network averages from 11.73 to 350.59 lei;
  - "Cartofi Rosii Spalati Punga 3kg" (a 3 kg bag of potatoes), with a tenfold spread.

  Gaps that large point to mixed units or bad rows, not real price differences (GA) [I][Obs].
- **Prices also vary by store format.** gov2-ro found Carrefour peppers at 19.99 lei in hypermarkets and 21.49 lei in smaller formats. Potatoes and sweet potatoes showed similar steps (GV) [I]. A per-kg Basket item therefore needs a rule for which store format to use.

## Update frequency

- **Official.** The latest statement is still the Council's April 2020 "zilnic" (daily), except Selgros every 2 days (see #8). It applies to all products. No fresh-food schedule has been published.
- **How data arrives.** In May 2024 the Council's president said retailers "trebuie să se conecteze la sistemul nostru ca să ne livreze datele" ("must connect to our system to deliver the data"), and that "nu avem date de la toţi retailerii" ("we don't have data from all retailers") ([Economica.net](https://www.economica.net/consiliul-concurentei-va-lansa-o-varianta-simplificata-a-monitorului-preturilor-care-va-contine-doar-produsele-de-baza-ale-caror-preturi-au-fost-plafonate_749405.html/amp)) [M quoting O].
- **What the data shows.**
  - In gov2-ro's April 2026 database, every Chain's prices are stamped either 20:00 or 04:00 (GC) [Obs].
  - Its freshness table for 4 Aug–2 Sep 2026 shows one stamp a day, almost always 20:00 (GA) [Obs].
  - gov2-ro notes the stamp moves forward daily even when the price is unchanged ([activity log, 28 Apr 2026](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/activity-log.md)) [I].

  The stamp marks a nightly load. It does not mark when a fresh price last changed.
- **Promotions.** money.ro says its Reported prices "includ promoțiile active în acea zi" ("include promotions active that day") ([money.ro](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)) [M]. Short fresh-food promotions may therefore show up, but no one has measured the delay.

## What the Competition Council says about scope

- **2019 launch.** The launch release describes about 30,000 products in over 1,700 stores. Its how-to tells users to search for "iaurt" (yoghurt) or pick a product from a category, "de exemplu, categoria «Lactate»" ("for example, the Dairy category"). The screenshot shows the categories FRUCTE, CARNE, LACTATE, MEZELURI, PESTE/FRUCTE DE MARE and PANIFICATIE. The release states no exclusion of fresh food and says nothing about per-kg prices ([CC, Oct 2019](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/)) [O].
- **May 2024.** "Avem toate magazinele din ţară, cu toate produsele alimentare, deci e gigantic" ("we have all the shops in the country, with all food products, so it is gigantic"), said as the reason for a simplified view of capped staples ([Economica.net](https://www.economica.net/consiliul-concurentei-va-lansa-o-varianta-simplificata-a-monitorului-preturilor-care-va-contine-doar-produsele-de-baza-ale-caror-preturi-au-fost-plafonate_749405.html/amp)) [M quoting O].
- **July 2024: the "Produse cu adaos plafonat" menu (products with a capped markup).** It lists 41 products ([Agerpres](https://agerpres.ro/economic/2024/07/03/consiliul-concurentei-a-actualizat-monitorul-preturilor-cu-o-sectiune-dedicata-produselor-cu-preturi--1322317)) [M quoting O]:
  - bread and milk;
  - telemea, yoghurt, sour cream and butter;
  - eggs;
  - whole chicken, chicken legs, thighs and wings;
  - several pork cuts and minced meat;
  - tomatoes, onions, cucumbers, beans, carrots, peppers, potatoes and garlic;
  - apples, plums, melons, grapes and pears.

  The markup cap behind this list (OUG 67/2023) was extended to 31 Dec 2026 when the law approving OUG 22/2026 was promulgated ([Antena 3, 24 Jun 2026](https://www.antena3.ro/actualitate/social/nicusor-dan-a-promulgat-legea-prin-care-se-prelungeste-pana-la-31-decembrie-plafonarea-adaosului-comercial-la-alimentele-de-baza-793320.html)) [M]. Kaufland still labels such items "OUG …", for example "OUG VDR LAPTE 1.5% 1L" in the 9 Oct 2026 CSV ([money.ro CSV](https://www.money.ro/date/cos-supermarketuri-bucuresti-2026-10-09.csv)) [M].
- **The capped list cannot be read from outside the platform.**
  - The platform's API has a separate set of 40 "OUG" categories that mirrors this list ([saved by gov2-ro](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/reference/GetProductCategoriesNetworkOUG.xml)) [I].
  - gov2-ro found that these categories "return 0 products" through the catalogue call it uses ([backlog](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/backlog.md)) [I].
- **No published definition of what each retailer must report.** The law leaves the choice of sectors to the Council (see #8). No request template, data specification or methodology for retailers was found in public. The platform's description page covers Basket mechanics only ([Descriere, read 2026-10-21](https://monitorulpreturilor.info/Home/Retail/Descriere)) [O][Obs].

## How the contradiction resolves

Both sources were accurate about what they saw. They saw different snapshots.

1. **gov2-ro's statement is from 18 April 2026.** It was written into `config/baskets.json` in [commit 9eb285d](https://github.com/gov2-ro/monitorulpreturilor/commit/9eb285d) on 18 Apr 2026 [I]. On that date gov2-ro's pipeline indexed only 6,932 products, all in 7 top-level categories ([activity log, 18 Apr 2026](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/activity-log.md)) [I]. We confirmed this in its committed database (GC) [Obs]:

   | Category | Products |
   |---|---|
   | Bakery (PANIFICATIE) | 3,487 |
   | Sweets (COFETARIE) | 1,406 |
   | Staples (ALIMENTE DE BAZA) | 1,010 |
   | Alcohol | 573 |
   | Coffee and tea | 376 |
   | Meat (CARNE), mostly cooked or marinated items sold by the kilo, priced mainly at Profi | 77 |
   | Baby food | 3 |

   No products were in dairy, fruit, vegetables or eggs. Its category explorer that day recorded that "136 categories have no prices … meat, dairy, fresh produce categories are empty" [I].
2. **About ten days later, gov2-ro's catalogue grew roughly twelvefold.**
   - Its logs give "6,932 → 87,617 items (April 28 reference run)" ([activity log, 12 May 2026 entry](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/activity-log.md)) [I].
   - Its category trend shows dairy, fruit, vegetables, eggs, fish and cold cuts priced from 26 Apr 2026 20:00 onwards ([trends.html](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/trends.html)) [I][Obs].
   - The logs do not say whether the platform or the pipeline changed. The Council's 2019 release already showed yoghurt results under a "Lactate" category, so the April gap most likely sat in gov2-ro's first catalogue fetch, not in the platform.
3. **The note was not revised after the catalogue grew.**
   - The `baskets.json` comment still reads "The API only tracks shelf-stable goods (no fresh dairy / meat / produce)" on `main` [Obs].
   - gov2-ro's methodology page, built 3–4 Sep 2026, still lists "Produse proaspete lipsesc … Carne, ouă, lactate, legume, fructe nu sunt acoperite" ("fresh products are missing … meat, eggs, dairy, vegetables, fruit are not covered") ([metodologie.html](https://github.com/gov2-ro/monitorulpreturilor/blob/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/metodologie.html)) [Obs].
   - Meanwhile gov2-ro's own May 2026 analysis discusses fresh produce priced per kg at Carrefour (GV) [I].

   This looks like an unrevised known-gaps note in an actively maintained civic project, not an error in the data.
4. **money.ro's October Basket matches the current data.** All 7 Chains it ranked have Reported prices for milk, butter, bread and cheese on 9 Oct 2026 ([CSV](https://www.money.ro/date/cos-supermarketuri-bucuresti-2026-10-09.csv)) [M].
5. **gov2-ro's caution still holds in one sense.** Fresh items rarely share product IDs across Chains, so a cross-chain Basket of produce, meat and eggs cannot be built by simply joining on product IDs. The 2016 pilot also had no fresh produce (see #8), which may explain why the "no fresh food" idea persists.

## Gaps and uncertainties

- **No direct look at the platform's catalogue.** By design, we did not call the API or search the platform, and searches only work from inside Romania. Per-Chain category counts are therefore not known. gov2-ro's full database (about 87K products) is on its own server and is not published. Only samples are public: 119 product CSVs, analytics tabs and category trends.
- **"Not seen" is weak evidence.** The table's gaps for Kaufland, Mega Image, Profi and Auchan produce, for raw meat, and for Selgros bread may only mean that no public file happened to include such items.
- **Eggs and raw meat by Chain** are unresolved. The category totals show eggs exist on the platform, but not who reports them.
- **Per-kg status of loose items** cannot be confirmed from the data. Names such as "Rosii" carry no unit, and the unit field is unreliable.
- **gov2-ro's sampling shapes the series.** Which stores it polled affects what appears. From 23 Jun 2026, for Penny, Lidl, Kaufland and Supeco, it queried a few "sentinel" stores and copied their prices to other stores of the same network ([activity log](https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/activity-log.md)) [I]. Selgros and Supeco series end in May–June. Its category labels come from the category it queried and include misfiles, such as Orbit gum under BRANZETURI (cheeses) (GA).
- **The cause of the late-April jump** in gov2-ro's catalogue is undocumented. "Most likely pipeline-side" is our inference.
- **Freshness of fresh prices.** No source measures how fast a change to a fresh price reaches the platform, or how often fresh Reported prices differ from the Shelf price. Fresh items vary by store and store format (GV), which raises the risk that the Reported price differs from the Shelf price.
- **Council documents.** No request template, data specification or written scope for retailers was found. The capped-markup section was seen only through press reports of the Council's release. The Council's own page for it was not opened.
- **Loyalty prices** were out of scope here and remain open from #8.
- **Time window.** gov2-ro's public snapshot ends on 2 Sep 2026. money.ro's CSV (9 Oct 2026) covers dairy and bread but no produce, meat or eggs.
- **Search budget.** 3 web searches were used. The platform's TLS chain still fails strict clients, so the description page was read with a plain HTTPS client on 2026-10-21.

## Sources

Official and regulator:

1. Consiliul Concurenței, "Consiliul Concurenței lansează Monitorul prețurilor produselor alimentare", press release, Oct 2019. https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/
2. Consiliul Concurenței, "Aplicația Monitorul Prețurilor a fost îmbunătățită", press release, Apr 2020. https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-aplicatia-monitorul-preturilor-a-fost-imbunatatita/
3. Monitorul Prețurilor, Retail description page, read 2026-10-21. https://monitorulpreturilor.info/Home/Retail/Descriere

Independent technical analysis and data (gov2-ro, read 2026-10-21):

4. Platform category tree saved from `GetProductCategoriesNetwork`, 14 Apr 2026. https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/reference/GetProductCategoriesNetwork.xml
5. Platform OUG (capped-staples) categories saved from `GetProductCategoriesNetworkOUG`. https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/reference/GetProductCategoriesNetworkOUG.xml
6. `config/baskets.json`, last changed 18 Apr 2026 (commit 9eb285d). https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/config/baskets.json
7. Activity log: entries of 18 Apr, 28 Apr, 2 May, 6 May, 12 May and 23 Jun 2026. https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/activity-log.md
8. Backlog: OUG categories return 0 products. https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/backlog.md
9. Price variability analysis, 6 May 2026. https://github.com/gov2-ro/monitorulpreturilor/blob/832fd7610e17d7a0bdca24bac6f1940e53758db4/docs/price_variability_analysis.md
10. CI database `data/prices_ci.db` (commit 8ed0d5a, 1 May 2026; prices 13–25 Apr 2026), queried read-only. https://github.com/gov2-ro/monitorulpreturilor/blob/8ed0d5a893226ad1a52d22b107b0f83ec6ce4f09/data/prices_ci.db
11. Site build of 4 Sep 2026 (`gh-pages`, commit bb86dfd): `trends.html` (category trend), `analytics.html` (popular products, per-network spread, cross-network spread, price freshness), `metodologie.html` (known gaps). https://github.com/gov2-ro/monitorulpreturilor/tree/bb86dfd4b40177bcb9b45b605de60eefa9fd931f
12. Per-product CSVs on the same build: 1026990, 1023867, 1043376, 1032584, 1021379, 1013392, 1010344, 1024121, 1020198. https://github.com/gov2-ro/monitorulpreturilor/tree/bb86dfd4b40177bcb9b45b605de60eefa9fd931f/data/products

Media:

13. money.ro, "Coșul cu 11 produse de bază în 7 supermarketuri", 10 Oct 2026 (method note). https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026
14. money.ro, CSV for the 9 Oct 2026 Basket. https://www.money.ro/date/cos-supermarketuri-bucuresti-2026-10-09.csv
15. Economica.net, on a simplified Monitor for capped staples, 25 May 2024 (quotes the Council's president). https://www.economica.net/consiliul-concurentei-va-lansa-o-varianta-simplificata-a-monitorului-preturilor-care-va-contine-doar-produsele-de-baza-ale-caror-preturi-au-fost-plafonate_749405.html/amp
16. Agerpres, "Consiliul Concurenţei a actualizat Monitorul Preţurilor cu o secţiune dedicată produselor cu preţuri plafonate", 3 Jul 2024 (reports the Council's release). https://agerpres.ro/economic/2024/07/03/consiliul-concurentei-a-actualizat-monitorul-preturilor-cu-o-sectiune-dedicata-produselor-cu-preturi--1322317
17. Antena 3, on the law approving OUG 22/2026 and extending the markup cap to 31 Dec 2026, 24 Jun 2026. https://www.antena3.ro/actualitate/social/nicusor-dan-a-promulgat-legea-prin-care-se-prelungeste-pana-la-31-decembrie-plafonarea-adaosului-comercial-la-alimentele-de-baza-793320.html
