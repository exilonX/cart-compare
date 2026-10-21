# What does Monitorul Prețurilor do, who uses it, and why hasn't it closed the gap?

Research for ticket [#8](https://github.com/exilonX/cart-compare/issues/8) on map [#1](https://github.com/exilonX/cart-compare/issues/1). Desk research, 2026-10-21. Monitorul Prețurilor's public pages were read, not scraped. Romanian quotes are given with an English translation.

**Evidence tiers.** Each important claim carries a tag, ranked from strongest to weakest:

- **[A]** academic study. None was found (see Gaps).
- **[O]** official or regulator document: the Competition Council, Monitorul Oficial, the platform's own pages.
- **[Obs]** our own direct look at the official site or a public registry on 2026-10-21.
- **[U]** usage statistics: the regulator's own analytics, app-store figures.
- **[I]** independent technical analysis: civic-tech or developer analyses of the platform's data. These are not peer-reviewed. They rank above anecdotes and below official statistics.
- **[M]** media report or user anecdote.

## Answer

- **It is a state-owned lookup tool, not a comparator.** The Competition Council (Consiliul Concurenței) owns and runs Monitorul Prețurilor, with ANPC as institutional partner. It started as a voluntary pilot in November 2016, became a nationwide service for fuel in July 2019 and for food in October 2019, and cost 1.42 million lei before VAT from the state budget [O]. Its own description says the project "nu își propune să fie un comparator de prețuri" ("does not aim to be a price comparator") [O].
- **Legal basis: a "send prices on request" duty with a small fine.** Since October 2020, Law 21/1996 art. 4(6) obliges companies to send the Council their sale prices on request "for … price comparisons included in online platforms intended to inform consumers". Failing to do so carries a fine of 20,000–50,000 lei (art. 54²), roughly €4,000–10,000 [O]. An earlier 2017 version of the duty fell in 2020, when the Constitutional Court struck down the ordinance that introduced it [O]. In May 2024 the Council said "doar jumătate dintre vânzători" ("only half of the sellers") had sent the data it asked for [M, quoting the regulator].
- **All 8 Chains report, unevenly.** Lidl, Kaufland, Carrefour, Mega Image, Profi, Penny, Auchan and Selgros all have stores and prices on the platform in 2026 [I][M]. The official partners page is out of date: it still lists Cora and omits Auchan [Obs]. In 2020 the Council said chains upload "zilnic" ("daily"), except Selgros (every 2 days) [O]. No newer official statement on frequency was found.
- **The data is broad but not ready to compare.** An independent mirror counted 87,775 products and 4,135 stores in June 2026 [I]. But 69% of products are sold by only one chain, only 78 products are sold by all ten networks, and units and brand names are not standardised [I]. Documented quality failures include:
  - a €2 million fine on Mega Image (2022) for price data. A 3.69 lei/l sunflower-oil price shown in the app could not be found in stores [O];
  - Cora's prices not updated since May 2025 [M];
  - an app outage in June 2026, and prices showing "0.0" in August 2026 [M].
  The Council has not published any audit of overall accuracy.
- **Usage is small and falling after a 2022 peak.** In 2025 the website had 15,938 unique desktop users and 176,120 visits. The Android app averaged 1,358 daily active users and iOS 340 daily active devices [U, Council annual report]. These figures cover fuel and food together. Usage peaked in 2022, with 94,861 desktop users and 162,325 Android installs [U]. App ratings are 1.9/5 on iOS (last update April 2020) and 2.2/5 on Google Play (October 2026) [U].
- **The regulator itself calls the UX poor.** In May 2024 the Council's president said the app "este foarte complicat de utilizat" ("is very complicated to use") [M, quoting the regulator]. App reviews and press tests from 2016, 2021 and 2026 make the same point [M].
- **The data is not open data.** No dataset exists on data.gov.ro, and the Council has no publisher account there [Obs]. The site has no licence, no terms of reuse, no documented API, no bulk download and no price history. It is only a disclaimer plus an undocumented web service, and searches are meant to work only from inside Romania [O][Obs]. Even so, third parties already reuse the data:
  - a civic mirror ([gov2-ro](https://github.com/gov2-ro/monitorulpreturilor)) since April 2026 [I];
  - money.ro, for a basket ranking published on 10 October 2026 [M].
- **Verdict on the Overview's "clarity and trust, not data existence" claim: mostly right, but incomplete.**
  - *Confirmed:* the data exists and covers all 8 Chains; the UX is weak, and the regulator says so itself; specific price inconsistencies are documented.
  - *Missing from the claim:* four other gaps.
    1. **Reusability.** There is no licence, no history and no API.
    2. **Comparability.** No product matching exists across chains.
    3. **Mandate.** The Council explicitly declines to rank chains or run a "comparator", and keeps the platform from becoming an "advertising channel".
    4. **Reach.** Very few people use it.
  - *Suggested rewording:* "the data exists but is locked in an unaudited lookup tool. The gap is clarity, trust, comparability and reusability."

## 1. What it is: owner, legal basis, history

### Owner and set-up

- **Owner and operator.** The Competition Council manages the platform. The partner chains load the data themselves: "Consiliul Concurenței gestionează platforma, dar datele/informațiile sunt încărcate în aplicație, la nivel național, de către companiile partenere" ("the Council manages the platform, but the data is loaded into the application, nationally, by the partner companies") ([CC press release, Oct 2019](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/)) [O].
- **Developer and cost.** "Aplicația Monitorul prețurilor este dezvoltată de compania Maguay." The project cost 1,422,346 lei excluding VAT (€305,880), "finanțat integral de la bugetul de stat" ("fully funded from the state budget") ([CC, Oct 2019](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/)) [O]. The app-store publisher is "Consiliul Concurentei" ([App Store](https://apps.apple.com/ro/app/monitorul-preturilor/id1468449358), [Google Play](https://play.google.com/store/apps/details?id=ro.ingr.pmonand)) [Obs].
- **Partners.**
  - ANPC (the consumer-protection authority) is the institutional partner ([partners list on the site](https://monitorulpreturilor.info/partners.min.js)) [Obs].
  - The 2016 pilot was built with GS1 Romania as technical developer and Nielsen, which chose the product list. Chirițoiu said all parties "au aderat voluntar" ("joined voluntarily") ([CC press release, Nov 2016](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor/)) [O].

### What the platform says it is, and is not

- **Not a comparator.** "Trebuie subliniat faptul că proiectul nu își propune să fie un comparator de prețuri." ("It must be stressed that the project does not aim to be a price comparator.") ([Retail description page](https://monitorulpreturilor.info/Home/Retail/Descriere)) [O]
- **Not an advertising channel.** Information is shown "fără a transforma, însă, platforma într-un canal de publicitate" ("without, however, turning the platform into an advertising channel"). The page also notes that the authority "nu are competența de a interveni în formarea unor prețuri" ("has no power to intervene in price setting") ([mission page](https://monitorulpreturilor.info/Home/Monitor)) [O].
- **No liability for accuracy.** The disclaimer reads [O]:
  - "Prețurile afișate la punctul de vânzare pot diferi de cele afișate pe acest site, prețurile valabile fiind întotdeauna cele afișate la punctul de vânzare." ("Prices at the point of sale may differ from those on this site; the valid prices are always those at the point of sale.")
  - The Council and the participants "nu pot fi ținuți responsabili de nicio daună" ("cannot be held liable for any damage").
  - Till discounts may exist that the site does not show ([home page](https://monitorulpreturilor.info/)).

### Timeline

| Date | Event | Source |
|---|---|---|
| Nov 2016 | Pilot for Bucharest–Ilfov only. 128 products (64 categories × cheapest and best-selling). Voluntary participation by 7 chains: Mega Image, Lidl, Kaufland, Selgros, Carrefour, Penny, Profi. | [CC](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor/) [O] |
| Jun 2017 | OUG 39/2017 obliges modern-trade chains to send sale prices to the Council on request, with a fine of 20,000–50,000 lei. Before this, the Council could not force a retailer to join. | [ZF, 24 Jun 2017](https://www.zf.ro/companii/retelele-comertul-modern-obligate-transmita-preturile-vanzare-consiliului-concurentei-retailerii-vor-raspunde-solicitarilor-acestia-vor-sanctionati-amenzi-variaza-20-000-50-000-lei-16511381) [M] |
| 1 Jul 2019 | Fuel component launched. About 1.8 million searches in the first 3.5 months. | [CC, Oct 2019](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/) [O][U] |
| 15 Oct 2019 | Food component goes national: about 30,000 products, more than 1,700 stores. Chains: Carrefour, Kaufland, Penny, Selgros, Mega Image, Lidl, Cora, Auchan. Results only once 5 or more products are in the basket. | [CC, Oct 2019](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/) [O] |
| Apr 2020 | Single-product comparison added. Profi and Supeco listed. Data loaded "zilnic". | [CC, Apr 2020](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-aplicatia-monitorul-preturilor-a-fost-imbunatatita/) [O] |
| Jul 2020 | Constitutional Court Decision 239/2020 finds OUG 39/2017 and its approval law unconstitutional. | Recital of [OUG 170/2020](https://legislatie.just.ro/Public/DetaliiDocumentAfis/231241) [O] |
| 16 Oct 2020 | OUG 170/2020 re-enacts the duty as Law 21/1996 art. 4(6), with the fine in art. 54². | [legislatie.just.ro](https://legislatie.just.ro/Public/DetaliiDocumentAfis/231241) [O] |
| Jul 2022 | Mega Image fined 10.08 million lei for inaccurate price information, including a price shown in the app. | [CC, Jul 2022](https://www.consiliulconcurentei.ro/wp-content/uploads/2022/07/amenda-Mega-Image-iul-2022.pdf) [O] |
| May 2024 | Council president says the app is "foarte complicat de utilizat" and announces a simplified version for price-capped staples. Only half of sellers had sent data. | [Rador, 26 May 2024](https://www.rador.ro/2024/05/26/consiliul-concurentei-va-lansa-o-varianta-simplificata-a-aplicatiei-monitorul-preturilor/) [M] |
| 3 Jul 2024 | "Produse cu adaos plafonat" section added: 41 staples under the markup cap, on the web first, mobile "later". | [retail-fmcg.ro](https://www.retail-fmcg.ro/analize/consiliul-concurentei-monitorul-preturilor-actualizare.html), [Economedia](https://economedia.ro/consiliul-concurentei-introduce-in-platforma-online-monitorul-preturilor-o-sectiune-pentru-produsele-cu-preturi-plafonate.html) [M] |
| 6 Apr 2026 | The Council, warning against announced price rises, still points consumers to the app. | [retail-fmcg.ro](https://www.retail-fmcg.ro/retail/consiliul-concurentei-cresterile-de-pret-anuntate-public-pot-duce-la-sanctiuni-consumatorii-pot-utiliza-aplicatia-monitorul-preturilor.html) [M] |
| 17 Jun 2026 | Android app update, after users reported a multi-day outage. | [Google Play](https://play.google.com/store/apps/details?id=ro.ingr.pmonand&hl=ro) [U][M] |

### The legal text in force

OUG 170/2020, point 2, inserted into Law 21/1996 ([legislatie.just.ro](https://legislatie.just.ro/Public/DetaliiDocumentAfis/231241)) [O]:

> "(6) Întreprinderile transmit la cererea Consiliului Concurenței prețurile de vânzare a produselor comercializate de acestea, în vederea realizării de analize, studii de piață sau comparații de preț incluse în platformele online destinate informării consumatorilor. În acest scop, selectarea sectoarelor din economie incluse în platformele online se realizează de către Consiliul Concurenței, cu consultarea autorității de reglementare din sectorul respectiv."
>
> *"(6) Undertakings shall send the Competition Council, at its request, the sale prices of the products they sell, for analyses, market studies or price comparisons included in online platforms intended to inform consumers. To this end, the Competition Council selects the economic sectors included in the online platforms, after consulting the sector's regulator."*

> "Articolul 54² — Constituie contravenție și se sancționează cu amendă de la 20.000 lei la 50.000 lei neîndeplinirea obligației prevăzute la art. 4 alin. (6)."
>
> *"Failure to meet the obligation in art. 4(6) is a contravention punishable by a fine of 20,000 to 50,000 lei."*

What this means:

- **The duty is to send prices when asked.** It applies to all undertakings, not only chains, and to sectors the Council selects. It does not prescribe a format, a frequency, an accuracy standard, or publication as open data.
- **The fine is small next to chain turnover.** At the Council's own conversion (10.08 million lei ≈ €2 million), 50,000 lei is about €10,000.
- **Retailers read the cap the same way.** In 2022 Mega Image argued that "dacă sancțiunea s-ar fi aplicat pentru încărcarea de informații incorecte în platforma Monitorul Prețurilor, atunci amenda aplicabilă nu ar fi putut depăși suma de 50.000 lei" ("had the sanction been for loading incorrect information into the Monitorul Prețurilor platform, the fine could not have exceeded 50,000 lei") ([Observator, 28 Jul 2022](https://observatornews.ro/economic/mega-image-reactie-publica-dupa-amendarecord-de-2-milioane-de-euro-primita-pentru-informatiile-inexacte-legate-preturile-481358.html)) [M, quoting the retailer]. The €2 million fine was for inaccurate answers in a separate market inquiry, not for the platform data.

## 2. Which Chains report, and how often

| Chain | 2016 pilot [O] | Oct 2019 launch [O] | Official partners page, read 2026-10-21 [Obs] | Stores in the June 2026 independent mirror [I] | In money.ro basket, 9 Oct 2026 [M] |
|---|---|---|---|---|---|
| Lidl | yes | yes | yes | 396 | yes |
| Kaufland | yes | yes | yes | 198 | yes |
| Carrefour | yes | yes | yes (plus franchisee Artima) | 380 | yes (prices vary by format) |
| Mega Image | yes | yes | yes | 977 | yes |
| Profi | yes | listed from Apr 2020 | yes | 1,613 | yes |
| Penny | yes | yes | yes | 439 | yes |
| Auchan | no ("probleme tehnice", per [Ziare 2016](https://ziare.com/preturi/supermarketuri/avem-un-monitor-de-comparat-preturile-din-magazine-dar-nu-ne-ajuta-prea-mult-1444865)) | yes | **not listed** | 53 | yes |
| Selgros | yes | yes | yes | 23 | excluded (cash & carry) |

Sources for the table:

- Pilot: [CC 2016](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor/).
- Launch: [CC 2019](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/) and [CC Apr 2020](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-aplicatia-monitorul-preturilor-a-fost-imbunatatita/).
- Partners page: [partners.min.js](https://monitorulpreturilor.info/partners.min.js), which the [Participanți page](https://monitorulpreturilor.info/Home/Retail/Participanti) renders.
- Store counts: [gov2-ro data audit, 21 Jun 2026, corrected addendum](https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/data-audit-2026-06-21.md).
- Basket: [money.ro, 10 Oct 2026](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026).

Notes:

- **Non-target networks.**
  - Cora joined in 2019. Its stores were taken over by Carrefour, and money.ro reports "no updated prices since May 2025", yet Cora still appears on the partners page and in the data [M][Obs].
  - Supeco joined in April 2020 [O] and had 26 stores in the June 2026 data [I].
  - Metro is not a partner. money.ro says it had no prices on the platform on 9 October 2026 [M].
- **Ownership change.** The Council cleared Mega Image's takeover of Profi with conditions; its [2024 annual report](https://www.consiliulconcurentei.ro/wp-content/uploads/2025/04/Raport-anual-2024.pdf) calls it "cea mai mare tranzacție din piața de retail din România" ("the largest transaction in Romania's retail market") [O]. Two of the 8 Chains now share an owner.
- **Coverage looks uneven.** Auchan's 53 stores and Carrefour's 380 look like partial coverage of their store networks. We did not verify this against store counts from the chains themselves, so treat it as a lead, not a finding.
- **Frequency.**
  - 2016 pilot: prices updated "cam o dată pe săptămână" ("about once a week") ([Ziare, 29 Nov 2016](https://ziare.com/preturi/supermarketuri/avem-un-monitor-de-comparat-preturile-din-magazine-dar-nu-ne-ajuta-prea-mult-1444865)) [M].
  - April 2020: data loaded "zilnic", with the footnote "Cu excepția Selgros, care actualizează prețurile la 2 zile, și Carrefour, care a plafonat prețurile pentru 500 de produse alimentare de bază" ("except Selgros, which updates every 2 days, and Carrefour, which had frozen prices on 500 staples") ([CC, Apr 2020](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-aplicatia-monitorul-preturilor-a-fost-imbunatatita/)) [O].
  - The app shows a per-store "ultima actualizare" (last update) ([CC, Oct 2019](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/)) [O].
  - No official statement on frequency after 2020 was found.
- **Compliance.** For the 2024 capped-staples section, "doar jumătate dintre vânzători au trimis datele necesare" ("only half of the sellers have sent the necessary data") ([Rador, 26 May 2024](https://www.rador.ro/2024/05/26/consiliul-concurentei-va-lansa-o-varianta-simplificata-a-aplicatiei-monitorul-preturilor/)) [M, quoting the regulator]. No fine under art. 54² for not reporting was found.

## 3. Data-quality problems on record

### Regulator evidence [O]

The Council fined Mega Image 10.08 million lei in July 2022 ([CC, Jul 2022](https://www.consiliulconcurentei.ro/wp-content/uploads/2022/07/amenda-Mega-Image-iul-2022.pdf)):

> "Mega Image practica cel mai mic preț la raft dintre retailerii analizați, de 3,69 de lei/litru, preț afișat și în aplicația Monitorul Prețurilor. Produsul nu se regăsea, însă, în magazine la prețul indicat."
>
> *"Mega Image had the lowest shelf price of the retailers analysed, 3.69 lei/litre, a price also shown in the Monitorul Prețurilor app. The product, however, could not be found in stores at that price."*

Chirițoiu said the company "a indus în eroare … și consumatorii care folosesc Monitorul Prețurilor" ("misled … also the consumers who use Monitorul Prețurilor").

- **The mechanism Mega Image described.** "am comunicat Consiliului Concurenței atât prețuri pentru produse active, cât și pentru produse inactive" ("we sent the Council prices for both active and inactive products") ([Observator](https://observatornews.ro/economic/mega-image-reactie-publica-dupa-amendarecord-de-2-milioane-de-euro-primita-pentru-informatiile-inexacte-legate-preturile-481358.html)) [M]. Stale prices for delisted products are one route to "inconsistent prices".
- **Court outcome.** Press reports say the Bucharest Court of Appeal upheld the fine in December 2023. [Profit.ro](https://www.profit.ro/povesti-cu-profit/retail/mega-image-pierde-in-anularea-unei-amenzi-record-22445867) reports a final loss at the High Court (ÎCCJ). We could not open that article or confirm the date of the ruling [M, unverified].

### Structural problems in the data [I]

- **No product identity across chains.** Product names are free text. The weight appears only in the name, and the `unit` field mixes forms such as `Kg`/`K`/`kg`/`1kg` and `BUC`/`BUCATA`/`Buc.`. Brands come in variants, for example `DR OETKER` spelled 6 ways. Some items are miscategorised, for example Jacobs coffee filed under alcoholic drinks ([gov2-ro data notes](https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/data-notes.md)).
- **Little overlap between chains.** Of 75,710 priced products, 51,795 (69%) are sold by a single chain and only 78 by all ten networks. Selgros sizes are wholesale packs ([gov2-ro audit](https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/data-audit-2026-06-21.md)).
- **Automated matching is unreliable.** A separate developer probe found automated name matching correct in only 46 of 124 single-candidate cases (37%). It concluded that a human-approved link list is needed ([hbrnm/legendary-winner PR #22, 12 Oct 2026](https://github.com/hbrnm/legendary-winner/pull/22)).
- **Prices genuinely differ.** For context, the same audit found that about 81% of products sold by two or more chains differ by more than 5% between chains on base prices, so price comparison is worth doing. The audit also says the widest gaps likely mix promotion timing with "some data noise" ([gov2-ro audit](https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/data-audit-2026-06-21.md)).

### Staleness and outages [M]

- **Stale chain data.** Cora's prices have not been updated since May 2025 ([money.ro, Oct 2026](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)).
- **User reports on Google Play** ([Google Play, Romanian reviews](https://play.google.com/store/apps/details?id=ro.ingr.pmonand&hl=ro); reviews shown in English may be machine-translated):
  - 18 Jun 2026: "Aplicatie foarte folositoare. Dar, din păcate de doua zile nu mai functioneaza." ("Very useful app. But unfortunately it hasn't worked for two days.")
  - 15 Aug 2026: "nu are preturi, apare 0.0 la orice" ("no prices, it shows 0.0 for everything").
- **Press tests and guides.**
  - [Economedia's May 2026 guide](https://economedia.ro/ghid-cum-sa-identifici-cele-mai-mici-preturi-la-alimente-fara-sa-pierzi-ore-intregi-in-magazine.html) says "unele prețuri nu reflectă actualizările prețurilor de la raft" ("some prices do not reflect shelf-price updates"). It lists weak UX, incomplete data and inconsistencies between retailers. This appears to be the origin of the Overview's wording.
  - The [Ziare 2016 test](https://ziare.com/preturi/supermarketuri/avem-un-monitor-de-comparat-preturile-din-magazine-dar-nu-ne-ajuta-prea-mult-1444865) found weekly updates, no fresh produce, and some stores showing only basket totals.

### Shelf price is not always the till price [M]

On 29 May 2025 ANPC inspected 232 operators, including stores of Kaufland, Lidl, Carrefour, Auchan, Profi, Mega Image and Metro. It found 105 shelf-versus-till mismatches (no per-chain breakdown was published, except for Metro) and issued 260 fines totalling 2,015,000 lei ([Buletin de București, 30 May 2025, citing ANPC](https://buletin.de/bucuresti/105-diferente-de-pret-intre-raft-si-casa-de-marcat-identificate-de-protectia-consumatorului-la-mai-multe-hipermarketuri-din-bucuresti-au-fost-date-260-de-amenzi/)). Trust problems therefore start at the shelf, not only in the platform.

### What nobody has published

- An accuracy audit of platform prices against shelf prices.
- The number of error reports or corrections received through the app's complaint channel.

## 4. Usage figures

All figures below are [U] from the Council's annual reports: [2025 report, §6.1 and Annex 7](https://www.consiliulconcurentei.ro/raport/raport-anual-2025/) (approved April 2026) and the [2024 report](https://www.consiliulconcurentei.ro/wp-content/uploads/2025/04/Raport-anual-2024.pdf). **They combine the fuel and food components**, and the reports do not split them.

**Website (desktop)**

| Period | Unique users | New users | Returning | Visits ("accesări") |
|---|---|---|---|---|
| Jul–Dec 2019 | 46,657 | – | 14.6% | 92,396 |
| 2020 | 31,510 | 30,431 | 17.5% | 122,743 |
| 2021 | 23,822 | 23,057 | 28.7% | 123,277 |
| 2022 | 94,861 | 92,948 | 18.8% | 286,997 |
| 2023 | 24,392 | 21,213 | 25.6% | 181,960 |
| 2024 | 16,157 | 14,900 | 28.4% | 187,478 |
| 2025 | 15,938 | 14,858 | 25.3% | 176,120 |

**Android app**

| Period | Installs (incl. reinstalls) | Uninstalls | Active installs at 31 Dec | Sessions | Google Play rating |
|---|---|---|---|---|---|
| Jul–Dec 2019 | 68,438 | 28,412 | 36,160 | 240,141 | n.a. |
| 2020 | 58,050 | 27,411 | 26,769 | 522,956 | 3.3/5 |
| 2021 | 43,028 | 13,568 | 23,318 | 410,231 | 3.3/5 |
| 2022 | 162,325 | 110,221 | 73,316 | 1,863,893 | 2.7/5 |
| 2023 | 65,180 | 17,342 | 48,939 | 496,406 | 2.74/5 |
| 2024 | 26,128 | 16,102 | 35,722 | 149,011 | 2.65/5 |
| 2025 | 20,252 | 10,840 | 29,349 | 123,092 | 2.68/5 |

The Android table rows were read from a PDF table layout, so check the column order against the report before quoting them.

**Daily averages in 2025:**

- Android: 1,358 daily active users and 5,902 new users.
- iOS: 340 daily active devices, 2,810 first-time downloads and 190,728 sessions.

**Interpretation:**

- Usage peaked in 2022, which coincides with that year's fuel-price spike. That timing is our reading; the report gives no reason.
- In 2025, about 1,700 people opened the app on an average day across both stores. The website drew about 480 visits a day.
- **Food-only figures are older.** The food component had 19,145 visits in January–February 2020, 36,152 in March–April 2020 (the COVID lockdown) and 9,123 in 1–15 May 2020 ([CC, May 2020](https://www.consiliulconcurentei.ro/comunicate/monitorul-preturilor-alimentelor-numarul-accesarilor-a-crescut-cu-90-%E2%80%AC%E2%80%AC/)) [U]. Compare 1.8 million fuel searches in the first 3.5 months after the July 2019 launch [O][U]. The units differ (searches against visits), but the gap in scale is large.

**Who uses it** (2025 report; demographics cover about 35% of desktop users) [U]:

- 61% men, 39% women.
- Largest age groups: 35–44 and 45–54.
- Bucharest accounts for 32% of desktop users. Windows accounts for 91%, which suggests heavy use from office PCs.
- Romania accounts for 81% of desktop users. Austria accounts for 9%, with Vienna at 10% of users by city in both 2024 and 2025. The report does not explain this, so part of the desktop traffic may not be shoppers.

**Current app-store figures** [Obs/U, read 2026-10-21]:

- Google Play: 100K+ downloads, 2.2/5 from about 1.1K reviews, last updated 17 Jun 2026 ([Google Play](https://play.google.com/store/apps/details?id=ro.ingr.pmonand)).
- App Store: 1.9/5 from 169 ratings. The latest version is 1.4, released 20 Apr 2020 ([App Store](https://apps.apple.com/ro/app/monitorul-preturilor/id1468449358)).

**Secondary users** (evidence that the data is valued even if the interface is not):

- The Council itself used the platform in its 2022 market inquiry [O].
- money.ro published an 11-item basket for Bucharest, Cluj and Iași built from platform data, with a CSV download [M].
- A civic mirror (gov2-ro) and at least one developer project (hbrnm/legendary-winner) have probed the data [I].

## 5. Criticism

### From the regulator

> "deşi actualul Monitor conţine preţurile alimentelor furnizate de toate magazinele din ţară, aplicaţia este foarte complicat de utilizat"
>
> *"although the current Monitor contains food prices from all stores in the country, the application is very complicated to use"*

This is Bogdan Chirițoiu, president of the Council, reported by [Rador on 26 May 2024](https://www.rador.ro/2024/05/26/consiliul-concurentei-va-lansa-o-varianta-simplificata-a-aplicatiei-monitorul-preturilor/) [M, quoting the regulator]. The planned fix was a simplified version covering only capped staples. What shipped, in July 2024, was a section inside the same platform [M].

### From users [M]

- **"Useless … it doesn't display any prices"** ([App Store, 16 Oct 2019](https://apps.apple.com/ro/app/monitorul-preturilor/id1468449358)).
- **The 5-product minimum.** Several reviews from October 2019 objected to having to add at least five products before seeing any result. The Council removed the minimum in April 2020 [O].
- **2026 reviews on Google Play** ([Google Play](https://play.google.com/store/apps/details?id=ro.ingr.pmonand)):
  - Missing products and chains: "a lot of products are missing and they don't include prices at supermarkets like Kaufland or Auchan", 6 May 2026.
  - Outages and blank pages: "either one opens a blank page", 14 Jun 2026.

### From the press [M]

- **Ziare, 29 Nov 2016:** "La ce e bun Monitorul Prețurilor? Nu la mare lucru" ("What is Monitorul Prețurilor good for? Not much"). Problems found: voluntary participation, Bucharest only, weekly updates, no fresh produce, no brand filter, cheapest basket only rather than cheapest product ([Ziare](https://ziare.com/preturi/supermarketuri/avem-un-monitor-de-comparat-preturile-din-magazine-dar-nu-ne-ajuta-prea-mult-1444865)).
- **Ziarul Financiar, 22 Sep 2021:** the app "analizează oferta a doar 5% din magazinele din București" ("covers only 5% of Bucharest stores"). The Council replied that searches use a 5 km radius and show at most 50 stores, "număr convenit de autoritate cu dezvoltatorul aplicației" ("a number agreed by the authority with the app developer") ([ZF](https://www.zf.ro/companii/retail-agrobusiness/explicatia-consiliului-concurentei-la-faptul-ca-monitorul-preturilor-20270028)).
- **Economedia, May 2026:** weak UX, incomplete data, inconsistencies ([Economedia](https://economedia.ro/ghid-cum-sa-identifici-cele-mai-mici-preturi-la-alimente-fara-sa-pierzi-ore-intregi-in-magazine.html)).

### Design and maintenance signals [O][Obs]

- **Login wall for saved baskets.** Saving baskets requires an account, with a maximum of 20 baskets of 50 products each ([Retail description page](https://monitorulpreturilor.info/Home/Retail/Descriere)).
- **No price history.** The platform has no price-history or trend view.
- **No ranking of chains.** It does not rank chains, which follows from its stated non-comparator stance.
- **Old code and stale content.** On 2026-10-21 [Obs]:
  - The site loads libraries from 2015–2019 (jQuery, Kendo UI, Bootstrap 3.3.6, Firebase 6.2.4) and a Google Universal Analytics tag. Google retired that analytics product in 2023.
  - The page code still contains a June 2020 maintenance notice.
  - The partners page has not been updated for Cora's exit or Auchan's entry.
  - The server sends an intermediate TLS certificate that does not match the issuer of its own certificate. Strict clients fail with "unable to verify the first certificate"; most browsers recover.
  - None of this is visible to a typical user, but it signals light maintenance.

## 6. Open data and licence

- **Not on data.gov.ro** [Obs, 2026-10-21]:
  - Searches of the portal's CKAN API for "monitorul preturilor", "preturi", "prețuri", "consiliul concurentei" and "carburanti" returned no datasets.
  - None of the portal's 181 publisher organisations is the Competition Council or ANPC ([API query](https://data.gov.ro/api/3/action/package_search?q=monitorul%20preturilor)).
- **No licence or reuse terms** [Obs]:
  - The site's only legal text is the disclaimer on the [home page](https://monitorulpreturilor.info/). It covers liability and includes "nu sunt responsabili pentru utilizarea ilicită de către terți a informațiilor afișate pe site" ("[the Council and participants] are not responsible for unlawful use by third parties of the information on the site"). That sentence acknowledges third-party use but grants no permission.
  - There is no terms-of-use page, and `robots.txt` returns 404.
- **No documented API, bulk download or history.**
  - The web front end calls an undocumented service (`wsURL = '/pmonsvc/Retail'` in the [home page](https://monitorulpreturilor.info/) source) [Obs].
  - A developer probe describes the access route as "serviciul XML nedocumentat" ("the undocumented XML service"), with no key and no history ([PR #22](https://github.com/hbrnm/legendary-winner/pull/22)) [I].
  - The data shows only current prices. Anyone who wants history has to record it themselves, as gov2-ro does with roughly 29,760 calls per full sweep ([gov2-ro cadence notes](https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/pipeline-cadence.md)) [I].
- **Romania-only access.** The 2019 launch release says "căutările și consultarea aplicației pot fi efectuate doar pe teritoriul țării" ("searches can be run only from within the country") ([CC, Oct 2019](https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/)) [O]. A developer working from a hosted environment reported that the site "dă tot 403" ("still returns 403") ([PR #22](https://github.com/hbrnm/legendary-winner/pull/22)) [I]. This matters for any project that runs its collector from a cloud host outside Romania.
- **Reuse is happening anyway.**
  - gov2-ro ("Guvernul Paralel") has run an alternative interface with baskets, a basket cost trend and anomaly flags since 14 April 2026 ([repo](https://github.com/gov2-ro/monitorulpreturilor)) [I]. Its repo has no licence, and the advertised domain did not resolve on 2026-10-21 [Obs].
  - money.ro republished platform-derived prices as a CSV [M].
  - Neither states a legal basis for reuse.
- **Licence status is unknown.** Whether the Council, the retailers or nobody holds rights over this compilation, and whether open-data rules on public-sector information apply, is a question for the IT-lawyer consult. Data supplied by companies under art. 4(6) may raise commercial-confidentiality arguments, even though it is already published. Desk research could not settle this.

## 7. Verdict on the Overview's claim

| Part of the claim | Verdict | Strongest evidence |
|---|---|---|
| "has the data breadth" | **Supported, with caveats.** All 8 Chains are present, with about 76k priced products and about 4.1k stores, but coverage is uneven (Auchan, Carrefour), a dead banner (Cora) is still listed, and there is no product matching across chains. | [O] 2019–2020 releases; [I] June 2026 audit |
| "weak UX" | **Strongly supported.** | [M quoting O] the regulator's own words (2024); [U] ratings of 1.9–2.7/5; iOS app unchanged since 2020; 2026 outages |
| "inconsistent prices" | **Supported by documented cases; size of the problem unknown.** | [O] 2022 Mega Image fine; [O] platform disclaimer; [M] stale Cora prices, "0.0" prices |
| "the gap is clarity and trust, not data existence" | **Mostly right, but incomplete.** | See below |

The claim misses four things:

1. **Reusability.** The data exists but is not open: no licence, no API documentation, no history, Romania-only access. Clarity and trust cannot be built on it without legal certainty and our own history-keeping.
2. **Comparability.** The platform shows each chain's own product list. Building Comparable Baskets requires the product matching that neither the Council nor the chains provide, and that automated attempts get wrong most of the time [I].
3. **Mandate.** A competition authority that "does not aim to be a price comparator" and avoids becoming "an advertising channel" will not publish "Chain X is cheapest this week". The clarity gap is partly by design, not only through neglect [O].
4. **Reach.** Even its best year reached fewer than 100k desktop users. In 2025 it averaged about 1,700 daily app users [U]. Any civic index has a distribution problem the state tool never solved.

**Proposed wording for Overview v2:** "Monitorul Prețurilor proves that chain-reported prices for all 8 Chains exist. They sit in an unaudited, hard-to-use lookup tool with no Basket view, no history and no open licence. The gap is clarity, trust, comparability and reusability, not data existence."

## Other Romanian Comparables

State and regulator:

- **Monitorul Prețurilor, fuel component** (July 2019). Five of seven fuel networks quote identical standard-petrol prices to the cent, per the [gov2-ro audit](https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/data-audit-2026-06-21.md) [I]. Fuel-price transparency counts only as evidence about effects (map rule).
- **Competition Council market inquiries and monitoring.**
  - 2022 inquiry into shelf and purchase prices of staples [O].
  - Monitoring of capped-markup food prices, continuing in 2026. The Council recommended "un plan de tranziție pentru eliminarea graduală a plafonării" ("a transition plan for phasing out the cap") ([2025 annual report](https://www.consiliulconcurentei.ro/raport/raport-anual-2025/)) [O].
  - 2025 dawn raids on six chains (Auchan, Carrefour, Kaufland, Mega Image, Metro, Selgros) over unfair trading practices towards dairy suppliers. This is not price comparison but shows the institutional climate [O].
- **ANPC.** Institutional partner of the platform and enforcer of shelf-versus-till price accuracy (see §3) [M citing O].

Civic, media and developer projects:

- **gov2-ro / monitorulpreturilor.gov2.ro** (Apr 2026–). An alternative interface on platform data, with baskets per network and municipality, a basket cost trend, anomaly flags and price-quality checks. It is the closest local Comparable to this project, and a possible collaborator. Its repo has no licence, and the site did not resolve on 2026-10-21 ([repo](https://github.com/gov2-ro/monitorulpreturilor)) [I][Obs].
- **money.ro basket ranking** (10 Oct 2026). An 11-item staples basket in Bucharest, Cluj and Iași built from platform data. It publishes its method, a CSV, and an offer to print chains' replies. Results for Bucharest: Lidl 45.38 lei, Mega Image 61.38 lei (+35.3%). This is close to our MVP's "basket ranking" feature, already done by a newsroom ([money.ro](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)) [M].
- **hbrnm/legendary-winner.** A developer project probing platform data for a shelf-price feature (Oct 2026) ([PR #22](https://github.com/hbrnm/legendary-winner/pull/22)) [I].

Private apps and sites (not examined in depth; descriptions from the sites themselves or press) [M]:

- **RadarPrețuri** (radarpreturi.ro). A per-product comparator across retailers. Economedia notes it "may lag behind in-store price changes" and struggles with duplicate products ([Economedia](https://economedia.ro/ghid-cum-sa-identifici-cele-mai-mici-preturi-la-alimente-fara-sa-pierzi-ore-intregi-in-magazine.html); [Google Play](https://play.google.com/store/apps/details?id=com.radarpreturi)). Probably a Comparable.
- **PromoAzi** (Axiom Software SRL). "Colectăm automat ofertele din cataloagele retailerilor" ("we automatically collect offers from retailers' catalogues"), with 90-day price history and basket comparison marked "în curând" ("coming soon") ([promoazi.ro](https://promoazi.ro/)). Leaflet-based, so a **Demand signal** unless it adds Basket comparison.
- **zgârcit.ro.** A deal aggregator across 9 chains with a loyalty-card filter, funded by donations ([zgarcit.ro](https://zgarcit.ro/)). **Demand signal.**
- **Blix, Ofertelino, Listiq.** Leaflet and catalogue aggregators ([Economedia](https://economedia.ro/ghid-cum-sa-identifici-cele-mai-mici-preturi-la-alimente-fara-sa-pierzi-ore-intregi-in-magazine.html)). **Demand signals.**

## Gaps and uncertainties

- **No academic study found.** Our web-search allowance ran out before an exhaustive academic search; Google Scholar and university repositories were not queried. A follow-up should search for Romanian or international studies of Monitorul Prețurilor's effect on prices or competition.
- **No impact evaluation.** The Council's annual reports give only usage figures, not price outcomes. No evidence of Social value (price effects, shopper behaviour) was found either way.
- **Current reporting chains and frequency.** There is no official 2025–2026 statement. Store counts come from an independent mirror (gov2-ro) whose method we did not reproduce.
- **Food versus fuel usage** is not separated in the Council's statistics.
- **Accuracy rate.** There is no audit of platform prices against shelf prices. Documented errors are cases, not rates.
- **Loyalty price.** It is unclear whether chains report Loyalty prices or app-only prices. The disclaimer's mention of discounts "la casa de marcat" (at the till) suggests not, and money.ro says promotions active that day are included. To verify.
- **The 2024 "simplified app".** Only the in-platform section (July 2024) is confirmed. A standalone app was not found.
- **Mega Image appeal.** The date and text of the final ruling are unverified.
- **Vienna traffic.** About 10% of desktop users in 2024–2025 are unexplained.
- **Licence and reuse.** The legal position on reusing platform data, including bulk collection and the Romania-only restriction, is unresolved.

## Questions this raises

1. **Flip the data strategy?** The Overview uses Monitorul Prețurilor "only as a cross-check" and collects from retailer sites while logged in. Platform data is state-published and retailer-supplied, so the chains have already agreed to its publication, and it covers all 8 Chains. Should Overview v2 use it as the primary source for Shelf price, and collect from retailer sites only for Loyalty price and spot checks? This could shrink the terms-of-service risk the legal tickets are studying.
2. **Ask the Council for open data.** Should the project formally ask the Council to publish the data as open data, with a licence, documented API and history? Or ask for written reuse permission? This is a lighter alternative to campaigning for a Croatia-style legal duty, and a natural opener for the "Partnerships" item on the map.
3. **Collaborate with gov2-ro?** It already mirrors the data daily and builds baskets. Should we collaborate, reuse its work (it has no licence, so ask first), or build separately?
4. **What we add over money.ro.** A newsroom already publishes one-day, cheapest-product basket rankings from platform data. Our distinct value would be: published matching rules, Branded versus private-label Baskets, weekly history, a fake-discount flag, and cross-country comparison. Is that enough to justify the project?
5. **Questions for the IT lawyer.** Does reusing or bulk-collecting platform data infringe database rights (the Council's or the retailers')? Do open-data rules apply? Can we collect from outside Romania given the Romania-only restriction?
6. **Our own accuracy check.** If platform data feeds a citable index, how do we spot-check it against shelves (for example, monthly store visits) so the index does not inherit errors like the 2022 Mega Image case?

## Sources

Official and regulator:

1. Consiliul Concurenței, "Consiliul Concurenţei lansează Monitorul Preţurilor", press release, Nov 2016. https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor/
2. Consiliul Concurenței, "Consiliul Concurenței lansează Monitorul prețurilor produselor alimentare", press release, Oct 2019. https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-lanseaza-monitorul-preturilor-produselor-alimentare/
3. Consiliul Concurenței, "Aplicația Monitorul Prețurilor a fost îmbunătățită", press release, Apr 2020. https://www.consiliulconcurentei.ro/comunicate/consiliul-concurentei-aplicatia-monitorul-preturilor-a-fost-imbunatatita/
4. Consiliul Concurenței, "Monitorul Prețurilor Alimentelor: numărul accesărilor a crescut cu 90%", press release, May 2020. https://www.consiliulconcurentei.ro/comunicate/monitorul-preturilor-alimentelor-numarul-accesarilor-a-crescut-cu-90-%E2%80%AC%E2%80%AC/
5. Consiliul Concurenței, "Consiliul Concurenței a sancționat Mega Image cu 2 milioane euro", press release, Jul 2022. https://www.consiliulconcurentei.ro/wp-content/uploads/2022/07/amenda-Mega-Image-iul-2022.pdf
6. Consiliul Concurenței, Raport anual 2025 (§6.1, Annex 7), approved Apr 2026. https://www.consiliulconcurentei.ro/raport/raport-anual-2025/
7. Consiliul Concurenței, Raport anual 2024, approved Apr 2025. https://www.consiliulconcurentei.ro/wp-content/uploads/2025/04/Raport-anual-2024.pdf
8. OUG nr. 170/2020 (Monitorul Oficial nr. 952, 16 Oct 2020), amending Law 21/1996 art. 4(6) and adding art. 54². https://legislatie.just.ro/Public/DetaliiDocumentAfis/231241
9. Monitorul Prețurilor: home page and disclaimer. https://monitorulpreturilor.info/
10. Monitorul Prețurilor: mission page. https://monitorulpreturilor.info/Home/Monitor
11. Monitorul Prețurilor: Retail description page. https://monitorulpreturilor.info/Home/Retail/Descriere
12. Monitorul Prețurilor: Participants page and its partner data. https://monitorulpreturilor.info/Home/Retail/Participanti, https://monitorulpreturilor.info/partners.min.js
13. data.gov.ro CKAN API (search and organisation list), queried 2026-10-21. https://data.gov.ro/api/3/action/package_search?q=monitorul%20preturilor

Usage statistics:

14. Google Play listing "Monitorul Prețurilor" (ro.ingr.pmonand), read 2026-10-21. https://play.google.com/store/apps/details?id=ro.ingr.pmonand
15. App Store listing "Monitorul Preturilor", read 2026-10-21. https://apps.apple.com/ro/app/monitorul-preturilor/id1468449358

Independent technical analysis:

16. gov2-ro, monitorulpreturilor repository. https://github.com/gov2-ro/monitorulpreturilor
17. gov2-ro, data audit of 21 Jun 2026. https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/data-audit-2026-06-21.md
18. gov2-ro, data notes. https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/data-notes.md
19. gov2-ro, pipeline cadence notes. https://github.com/gov2-ro/monitorulpreturilor/blob/main/docs/pipeline-cadence.md
20. hbrnm/legendary-winner, PR #22 "probă pe datele Monitorului Prețurilor", 12 Oct 2026. https://github.com/hbrnm/legendary-winner/pull/22

Media:

21. Ziare.com, "La ce e bun Monitorul Preturilor? Nu la mare lucru", 29 Nov 2016. https://ziare.com/preturi/supermarketuri/avem-un-monitor-de-comparat-preturile-din-magazine-dar-nu-ne-ajuta-prea-mult-1444865
22. Ziarul Financiar, on the 2017 obligation for chains to send prices, 24 Jun 2017. https://www.zf.ro/companii/retelele-comertul-modern-obligate-transmita-preturile-vanzare-consiliului-concurentei-retailerii-vor-raspunde-solicitarilor-acestia-vor-sanctionati-amenzi-variaza-20-000-50-000-lei-16511381
23. Ziarul Financiar, on the 50-store limit, 22 Sep 2021. https://www.zf.ro/companii/retail-agrobusiness/explicatia-consiliului-concurentei-la-faptul-ca-monitorul-preturilor-20270028
24. Observator, Mega Image's public reaction to the fine, 28 Jul 2022. https://observatornews.ro/economic/mega-image-reactie-publica-dupa-amendarecord-de-2-milioane-de-euro-primita-pentru-informatiile-inexacte-legate-preturile-481358.html
25. Profit.ro, "Mega Image pierde în anularea unei amenzi record" (not opened: HTTP 403; cited from search snippet only). https://www.profit.ro/povesti-cu-profit/retail/mega-image-pierde-in-anularea-unei-amenzi-record-22445867
26. Rador, "Consiliul Concurenţei va lansa o variantă simplificată a aplicaţiei Monitorul Preţurilor", 26 May 2024. https://www.rador.ro/2024/05/26/consiliul-concurentei-va-lansa-o-varianta-simplificata-a-aplicatiei-monitorul-preturilor/
27. Retail-FMCG.ro, on the capped-markup section, 3 Jul 2024. https://www.retail-fmcg.ro/analize/consiliul-concurentei-monitorul-preturilor-actualizare.html
28. Economedia, on the capped-markup section, 3 Jul 2024. https://economedia.ro/consiliul-concurentei-introduce-in-platforma-online-monitorul-preturilor-o-sectiune-pentru-produsele-cu-preturi-plafonate.html
29. Buletin de București, on ANPC's shelf-versus-till inspections, 30 May 2025. https://buletin.de/bucuresti/105-diferente-de-pret-intre-raft-si-casa-de-marcat-identificate-de-protectia-consumatorului-la-mai-multe-hipermarketuri-din-bucuresti-au-fost-date-260-de-amenzi/
30. Retail-FMCG.ro, on the Council's warning about announced price rises, 6 Apr 2026. https://www.retail-fmcg.ro/retail/consiliul-concurentei-cresterile-de-pret-anuntate-public-pot-duce-la-sanctiuni-consumatorii-pot-utiliza-aplicatia-monitorul-preturilor.html
31. Economedia, guide to finding the lowest food prices, 27 May 2026 (updated 16 Jul 2026). https://economedia.ro/ghid-cum-sa-identifici-cele-mai-mici-preturi-la-alimente-fara-sa-pierzi-ore-intregi-in-magazine.html
32. money.ro, "Coșul cu 11 produse de bază în 7 supermarketuri", 10 Oct 2026. https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026

Private Comparables and Demand signals:

33. PromoAzi. https://promoazi.ro/
34. zgârcit.ro. https://zgarcit.ro/
35. RadarPrețuri on Google Play. https://play.google.com/store/apps/details?id=com.radarpreturi
