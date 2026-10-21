# What happened to grocery price-comparison Comparables in Central and Eastern Europe?

Desk research for ticket #3 on the Grocery Basket Index map (#1). Researched 2026-10-21. Every figure carries the date it refers to. Romania's Monitorul Prețurilor has its own ticket and appears here only for contrast.

**Evidence tiers used below**

- **[T1]** causal academic study, peer-reviewed
- **[T2]** evaluation or official statistics from a regulator, central bank or ministry (including studies a regulator commissioned or promoted)
- **[T3]** usage statistics and consumer surveys
- **[T4]** media reports, anecdotes, and claims by interested parties (chains, ministers, organisers, developers)

## Answer

- **States built almost every Comparable in the region, each during a crisis, and each alongside price controls.** Examples: Greece in 2020 (Covid), Slovenia in 2022 and Hungary in 2023 (food inflation), Croatia in 2025 (the boycotts), Bulgaria in 2025 (the euro changeover). Each came with price caps, margin caps or "basket" schemes, so no study separates the Comparable's own effect from the controls. This research found no peer-reviewed causal study of any CEE grocery Comparable [T1 gap].
- **The ones that lasted had a legal mandate; usage did not decide it.**
  - Hungary's Árfigyelő has run since July 2023 and has had a statutory basis since 2025.
  - Greece's e-katanalotis ran from March 2020 to June 2026. The new PosoKanei portal replaced it.
  - Bulgaria's kolkostruva.bg has run since September 2025, and the euro-adoption rules require it until at least August 2027.
  - Slovenia's ministry basket survey has published nothing since December 2023.
- **Uptake was modest and jumped with price news.**
  - Bulgaria: more than 1 million visits in about 11 months, or "several thousand" a day, peaking at the euro changeover and at a fuel-price shock (August 2026) [T3].
  - Hungary: about 21,000 daily visitors after launch, a figure critics called "extremely low" (reported June 2024) [T4].
  - Greece: 500,000 unique weekly visitors and 300,000 app users (April 2023) [T3].
- **The best evidence of Social value is thin and comes mostly from state bodies.**
  - Hungary: a synthetic-control study promoted by the regulator credits Árfigyelő with 1.11 pp lower food inflation by February 2024, and HUF 19.4 bn saved by households over three winter months. It was not peer-reviewed, and its funding was not disclosed [T2].
  - Bulgaria: the ECB used the portal's micro-data to show that euro-changeover price changes were "only a few euro cents". That is the clearest case of a Comparable helping a cost-of-living debate tell the truth [T2].
- **Croatia has the most open model.** Since May 2025, the law requires large Chains to publish daily, store-level, machine-readable price lists and to allow automated collection, for example by API.
  - Within weeks, volunteers built an open-source crawler (AGPL, 29 Chains) and several free apps on that data.
  - From 17 November 2026 the duty widens to every consumer-facing seller with a website.
  - No evaluation of its effect on prices exists yet.
  - Its stated model, Israel's 2015 transparency rule, did lower prices and price dispersion [T1]. There, the effect came through media price surveys and discounters' advertising, not through comparison apps.
- **Chains complied once required to, but disputed the methods.**
  - Slovenia: the retail chamber asked for the survey to be halted, citing "irreparable damage" from errors [T4].
  - Bulgaria: chains said item-level daily data is "unlikely to provide useful information to consumers" [T4].
  - Croatia: Chains often published late or inconsistent files [T4].
  - Hungary: Lidl's "cheapest" advertising claims must now rest on Árfigyelő data. This is a commitment the competition authority accepted in November 2025 [T2].
- **Harms and truth problems were real, though documented mostly by anecdote rather than measurement.**
  - Gaming of basket surveys was suspected in Slovenia (bread at €0.19/kg). Inspections found no irregularities.
  - Croatian price files contain promotional prices not valid on the stated date, and products listed at stores that do not sell them.
  - Hungary's reporting threshold leaves out franchise Chains and small shops.
  - Hungary's regulator took civil and criminal steps against an unofficial app that reused its data (2023).
  - The academic risk that price transparency helps sellers coordinate (Danish concrete prices +15–20%, Chilean fuel margins +9%) [T1] has not been tested on any CEE grocery Comparable.
- **The only recurring cross-country Basket index found that includes Romania comes from a Greek retail-research institute, and it shows how fragile such comparisons are.** IELKA prices a 40–41-category Basket at Romanian Chains (only Carrefour, Auchan and Mega Image). In its comparison with Greece:
  - Romania was 5% more expensive (December 2024 data) and 20% more expensive (May 2026 data), including VAT. The releases do not explain the jump.
  - IELKA's funders and members are not disclosed on its site.
  - Every edition concludes that Greek supermarkets are cheaper [T4].
- **The 2025 Balkan boycotts changed policy, not prices.**
  - Tax data show one-day falls in Chain turnover of 29–56% [T2].
  - Croatia's central bank found no effect on one Chain's prices or on January food inflation [T2 via T4].
  - What lasted were Croatia's price caps and price-list duty, freezes in Bosnia and Herzegovina, North Macedonia's margin caps, and tighter Bulgarian rules. Romania's boycott had little uptake [T4].
- **What this means for the Grocery Basket Index.** State portals leave gaps a civic index can fill: price history, Baskets, readable comparisons and cross-country views. Three lessons carry over:
  - Design against gaming.
  - Publish the method before Chains dispute it.
  - Use the new open data in Bulgaria and Croatia (and perhaps Greece and Hungary) as a possible source for the cross-country Basket.

## Comparison table

| Country | Comparable | Run by | Lifespan (status 2026-10-21) | How data arrives | Funding | Uptake (dated) | Strongest Social value evidence |
|---|---|---|---|---|---|---|---|
| Hungary | [Árfigyelő](https://arfigyelo.gvh.hu/) | GVH (competition authority) with the government | 1 Jul 2023 – running; statutory since 2025 | Mandatory daily feed from Chains with >HUF 100 bn revenue; Shelf price, previous price and Loyalty price | State; cost not published | 25 m page downloads in week 1 (Jul 2023); ~21k daily visitors after launch (reported Jun 2024) | Synthetic control: −1.11 pp food inflation by Feb 2024 [T2] |
| Greece | [e-katanalotis](https://www.mindev.gov.gr/wp-content/uploads/2020/03/2020-3-5-E-KATANALOTIS-1.pdf) → PosoKanei | Ministry of Development; from 2026 also the Market Control and Consumer Protection Authority | e-katanalotis 5 Mar 2020 – Jun 2026; PosoKanei 17 Jun 2026 – running | Chain feeds; PosoKanei: 6 Chains direct, 4 crawled from their e-shops | e-katanalotis built for ≤ €30,000 (2020) | 500k weekly unique visitors, 300k app users (Apr 2023) | Surveys: 17–18% visited another store for "household basket" items [T3]; no price evaluation |
| Croatia | No state front end; open price lists plus apps ([cijene.dev](https://cijene.dev/), [usporedicijene.info](https://usporedicijene.info/), MojeCijene and others) | Government (rules); independent developers (apps) | Duty since 15 May 2025; widened from 17 Nov 2026 | Mandatory store-level CSV/XML, daily by 08:00, automated collection allowed | Chains bear compliance cost; apps are self-funded or free | One app: >30k weekly active users (Jun 2025, developer claim) | None yet |
| Bulgaria | foodprice.bg (2023) → [kolkostruva.bg](https://kolkostruva.bg/) | Caretaker government (2023); Consumer Protection Commission, KZP (2025–) | kolkostruva 30 Sep 2025 – required until at least 9 Aug 2027 | Mandatory daily feed, 101 product types; daily open-data ZIPs | KZP budget; foodprice.bg cost 30,000 leva | >1 m visits since launch, several thousand a day (Aug 2026) | ECB: changeover price changes "minimal" [T2] |
| Slovenia | [Primerjaj-cene.si](https://primerjaj-cene.si/) basket surveys | Ministry of Agriculture, Forestry and Food | 13 Sep 2022 – last results 22 Dec 2023 (dormant) | In-store surveys every 14 days at 6 Chains; daily tracking of 17k products at 4 e-shops | Ministry | Not published | Basket reported at successive lows (ministry's own count) [T2]; gaming suspected [T4] |
| Greece (cross-country) | [IELKA European Basket comparison](https://ielka.gr/anakoinosi-24-09-2026/) | IELKA, a non-profit retail research institute | Says it has run for 12 years; editions seen Feb 2025, Jun 2026, Sep 2026 | Comparison platforms, price observatories and price collection at Chains; 40–41 categories, >6,000 prices, 8 comparison countries | Not disclosed | Picked up by the press, including Romanian outlets (Feb 2025, per the map coordinator) | None; Romania's gap moved from +5% to +20% across editions [T4] |
| Poland | None found (see Gaps) | – | – | – | – | – | – |
| Slovakia | Asked to buy Hungary's Árfigyelő (Mar 2024) | Ministry of Finance | Outcome not found | – | – | – | – |

## Detailed findings

### Hungary: GVH Árfigyelő

**Who runs it, and on what legal basis.** Árfigyelő is run by the Gazdasági Versenyhivatal (GVH, the competition authority). The GVH's own FAQ (July 2025) describes it this way: "Az Árfigyelő rendszer Magyarország Kormánya és a Gazdasági Versenyhivatal által kifejlesztett ingyenes online adatbázis" ("The Árfigyelő system is a free online database developed by the Government of Hungary and the GVH") ([GVH FAQ PDF](https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf)). The rules first appeared in a May 2023 government decree ([Telex, 2023-05-08](https://telex.hu/gazdasag/2023/05/08/online-arfigyelo-adatszolgaltatas-kiskereskedelem-inflacio-gazdasagi-versenyhivatal)). Chapter V of Act L of 2025 now governs the system. That Act turned emergency decrees into statute, so Árfigyelő has a legal basis that no longer depends on the state of danger ([GVH FAQ](https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf)). Hungary's state of danger ended on 14 May 2026 ([Economx, 2026-05-14](https://www.economx.hu/belfold/2026/05/14/hivatalos-megszunt-az-orosz-ukran-haboru-miatt-elrendelt-veszelyhelyzet/)).

**Who must report.** Any retailer whose net revenue in the previous year exceeded HUF 100 bn must report. From 1 June 2025 that means Aldi, Auchan, Lidl, Penny, SPAR and Tesco, plus the drugstores Müller, dm and Rossmann. Smaller retailers may join voluntarily ([GVH FAQ](https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf)).

**What it shows.**
- The "daily price, previous price and loyalty price, by retailer and by store." This is a state precedent for showing a Loyalty price beside the Shelf price.
- The price used to rank products is the one applied in 80% of a Chain's stores, so some stores may be cheaper.
- Daily data is public only on the day it applies to: "A napi áradatok mindig csak azon a napon érhetők el nyilvánosan, amelyre vonatkoznak" ("daily price data are publicly available only on the day they refer to"). It is archived the next day ([GVH FAQ](https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf)). The public therefore cannot use Árfigyelő to check whether a discount is real.

**Scope over time.**
- July 2023: 60+ product groups, about 1,200 stores, six Chains ([GVH, 2023-07-08](https://gvh.hu/en/press_room/press_releases/press-releases-2023/the-price-monitoring-system-has-been-up-and-running-for-a-week-more-improvements-coming-soon)).
- February 2025: 78 categories and more than 2,000 products, with about 20 more categories planned ([Economx, 2025-02-25](https://www.economx.hu/gazdasag/2025/02/25/arfigyelo-gvh-uj-termekek-eljarasok-804936/)).

**Uptake.**
- The GVH reported 25 million page downloads in the first week (8 July 2023) [T3] ([GVH](https://gvh.hu/en/press_room/press_releases/press-releases-2023/the-price-monitoring-system-has-been-up-and-running-for-a-week-more-improvements-coming-soon)).
- By June 2024, HVG called the 21,000 daily visitors after launch "rendkívül alacsony" ("extremely low"). It said Google search interest was "lassan a nullához konvergál" ("slowly converging to zero"), and that a promised official phone app had not appeared [T4] ([HVG, 2024-06-28](https://hvg.hu/gazdasag/20240628_GVH:-Nemzetkozi-erdeklodes-van-az-Arfigyelo-irant)).
- No later official usage figures were found.

**Funding.** It is state-funded. The GVH runs the system, while "a fejlesztéseket, az informatikai és a jogszabályi hátteret a kormányzat és szervezetei biztosítják" ("the government and its bodies provide the development, IT and legal background") ([VG, 2024-03-05](https://www.vg.hu/vilaggazdasag-magyar-gazdasag/2024/03/hivatalosan-is-lepett-a-szlovak-kormany-lemasolnak-az-arfigyelot)). No cost figure was found.

**Measured Social value.**
- **GVH before-and-after claim [T2, confounded].** In November 2023 the GVH said food inflation had "fallen by almost a third" since launch, and that average prices fell 5.5% in 50 of 62 categories ([GVH, 2023-11-10](https://gvh.hu/en/press_room/press_releases/press-releases-2023/gvh-the-price-monitoring-database-in-hand-with-government-measures-has-helped-to-achieve-single-digit-inflation)). Food inflation was already falling from 44.8% (December 2022), and the release credits "government measures" alongside the database, so the claim does not isolate Árfigyelő.
- **Makronóm Institute synthetic-control study [T2, quasi-causal, not peer-reviewed].** The study estimates that Árfigyelő lowered food inflation by 1.11 pp by February 2024 and by an average of 1.45 pp in December 2023 – February 2024. That equals HUF 19.4 bn of household savings over those three months. It found significant effects in 14 of 21 subcategories, the largest on low-fat milk (12.19 pp) and eggs (12.16 pp) ([GVH press release, 2024-09-04](https://www.gvh.hu/en/press_room/press_releases/press-releases-2024/hungarian-families-saved-nearly-huf-20-billion-in-three-months-thanks-to-the-online-price-monitor)). The release does not say who funded the study or describe the donor pool, and the full paper was not reviewed here.
- **GVH margin claim [T2, primary not found].** The GVH has also said that, because of Árfigyelő, participating retailers' gross margin on dairy fell by about 10 pp ([Economx, 2025-11-13](https://www.economx.hu/magyar-gazdasag/2025/11/13/gvh-versenyhivatal-eljaras-lidl-arak-819279/)).
- **Independent caution [T1].** A peer-reviewed study of Hungarian pork prices (Fertő and Podruzsik, *Agribusiness*; summarised 17 September 2026) covers the regime of "online price monitoring and a margin cap". It warns that its "estimates should be interpreted as comparisons between observed regulatory regimes" and do not identify the effect of any one measure ([ELTE KRTK, 2026-09-17](https://krtk.elte.hu/en/2026/09/price-caps-do-not-stop-price-transmission-they-change-where-it-happens-by-imre-ferto-and-szilard-podruzsik/)).

**How Chains and the state reacted.**
- **Coverage criticism [T4].** Telex noted that the threshold covers only the large Chains, "amelyek között egyébként is éles a verseny" ("among which competition is already sharp"). Franchise Chains (CBA, Coop, Reál) and small shops stay out of view ([Telex G7, 2023-05-10](https://telex.hu/g7/kozelet/2023/05/10/a-kormany-arfigyelo-rendszere-ott-elezne-az-arversenyt-ahol-mar-nem-lehet)).
- **The data became the referee for advertising [T2].** In November 2025 the GVH closed a case against Lidl's "az alacsony árak bajnoka" ("champion of low prices") slogan after Lidl made commitments, without finding an infringement. Lidl must:
  - base claims to be cheapest on Árfigyelő data;
  - make a monthly average-basket claim only if it is at least 2.5% cheaper than the second-cheapest Chain ([Economx, 2025-11-13](https://www.economx.hu/magyar-gazdasag/2025/11/13/gvh-versenyhivatal-eljaras-lidl-arak-819279/)).
- **Hostility to re-users [T4].** In August 2023 an unofficial free app that copied Árfigyelő appeared in the app stores. The GVH called it "az online Árfigyelő rendszer illetéktelen, engedély nélküli felhasználása" ("an unauthorised, unlicensed use of the online Árfigyelő system"). It said it took "a szükséges polgári és büntetőjogi lépéseket" ("the necessary civil and criminal steps") against the app's makers and asked for the app's removal ([Telex, 2023-08-05](https://telex.hu/belfold/2023/08/05/gvh-figyelmeztetes-kalozapplikacio-arfigyelo)). The GVH also said the app showed inaccurate prices.
- **Copying abroad.** Slovakia's Ministry of Finance formally asked the GVH about buying the system in March 2024 ([VG, 2024-03-05](https://www.vg.hu/vilaggazdasag-magyar-gazdasag/2024/03/hivatalosan-is-lepett-a-szlovak-kormany-lemasolnak-az-arfigyelot)). No outcome was found.

**Political context.** Árfigyelő came alongside heavier controls.
- The "árrésstop" margin cap on food and drugstore products started in March 2025. In April 2026 the outgoing government removed its 31 May 2026 expiry date, so the cap stays in force indefinitely ("határozatlan ideig hatályban vannak"). The new finance minister said it would be phased out on a planned schedule ([444, 2026-04-18](https://444.hu/2026/04/18/orbanek-hagyjak-hogy-magyar-peterek-dontsenek-az-arres-es-kamatstopokrol)).
- On 2 October 2026, Prime Minister Péter Magyar said the government should consider phasing the cap out, because it is "increasingly damaging farmers and small shops" ([Daily News Hungary, 2026-10-02](https://dailynewshungary.com/pm-magyar-hungary-food-margin-cap-stop/)).
- No statement on Árfigyelő's own future was found.

### Greece: e-katanalotis, the "household basket", and PosoKanei

**e-katanalotis (2020–2026).**
- **Launch.** It launched on 5 March 2020 under the Ministry of Development and Investment, together with the Central Markets Organisation (OKAA). The contractor was Warply.
- **Cost and scope [T2].** Minister Adonis Georgiadis said that "σε λιγότερο από 4 μήνες και ελάχιστα χρήματα, όχι περισσότερα των 30.000 ευρώ, η εφαρμογή e-katanalotis είναι πλέον προσβάσιμη" ("in less than 4 months and with very little money, no more than €30,000, the e-katanalotis app is now available"). It tracked the 1,000 products the statistics office ELSTAT records.
- **How Chains took part.** The ministry presented participation as voluntary: "συμμετέχουν καθολικά και αυτοβούλως οι εταιρείες" ("companies take part universally and of their own will") ([Ministry press release, 2020-03-05](https://www.mindev.gov.gr/wp-content/uploads/2020/03/2020-3-5-E-KATANALOTIS-1.pdf)).
- **Uptake [T3].** In April 2023 it had "500.000 μοναδικοί επισκέπτες την εβδομάδα" ("500,000 unique visitors a week"), 300,000 app users, and 150,000 users who had built their own Baskets ([Parapolitika, 2023-04-12](https://www.parapolitika.gr/oikonomia/article/1265932/e-katanalotis-stin-platforma-ta-timologia-ilektrikis-energeias-kai-fusikou-aeriou-olon-ton-parohon/)). The article does not name its source for these figures.

**The "household basket" (from November 2022).** Retailers offered a set of staple products, and the scheme was promoted through e-katanalotis. The evidence comes from surveys by IELKA, a retail research institute [T3]:
- **November 2022 (1,000 consumers, first 10 days).** 39% bought basket products at least once, and 18% visited a supermarket other than their usual one to find them. Buyers spent 12% less a week (€81.65 against €93.35), but IELKA said this is not evidence of cause, because the scheme mainly drew lower-income shoppers ([iefimerida, 2022-11-14](https://www.iefimerida.gr/ellada/ereyna-ielka-proionta-kalathi-toy-noikokyrioy)).
- **January 2023.** 17% had visited a different supermarket because of the basket, though the release's summary says "1 in 7". 85% said it "δεν επαρκεί για την αντιμετώπιση της ακρίβειας" ("is not enough to tackle high prices"), and 84% would prefer a VAT cut on food ([IELKA via oenet.gr, 2023-02-07](https://www.oenet.gr/τελευταία-νέα/τρόφιμα/item/99673-ielka-anakoinosi-tipou-gia-to-kalathi-tou-noikokiriou)).

**PosoKanei (from 17 June 2026).** PosoKanei replaced e-katanalotis ([iefimerida, 2026-06-17](https://www.iefimerida.gr/english/greece-launches-ai-price-comparison-app-put-supermarket-costs-under-public-scrutiny)).
- **Where data comes from [T2].** Per the ministry FAQ as reported by Skai:
  - six Chains send data directly (Galaxias, SYNKA, Masoutis, AB Vassilopoulos, Market In, Lidl);
  - four are crawled from their e-shops by product code (Sklavenitis, Chalkiadakis, My Market, Kritikos);
  - prices update daily, about 10,000 product codes are covered, and price history is shown ([Skai, 2026-06-17](https://www.skai.gr/news/greece/nea-platfmorma-kata-tis-akriveias-ti-einai-to-posokanei-pos-leitourgei)).
  So a state Comparable collects prices from some Chains' websites automatically.
- **Cross-country comparison.** PosoKanei shows prices from Italy, France, Belgium, Romania, Bulgaria, Cyprus and Spain. In the FAQ's words, "Η σύγκριση γίνεται κυρίως σε επίπεδο κατηγορίας προϊόντων και όχι βάσει πλήρους αντιστοίχισης" ("the comparison is made mainly at product-category level, not by full matching") ([Skai](https://www.skai.gr/news/greece/nea-platfmorma-kata-tis-akriveias-ti-einai-to-posokanei-pos-leitourgei)).
- **Launch-day details [T4].** Coverage reported 7,973 products. Private-label goods are not compared automatically. The authority's head, Despina Tsaggari, said: «Όπου βρίσκουμε διαφορές θα αναφέρονται στον υπουργό και τον πρωθυπουργό» ("wherever we find differences they will be reported to the minister and the prime minister") ([newmoney, 2026-06-17](https://www.newmoney.gr/roh/palmos-oikonomias/oikonomia/theodorikakos-sto-mikroskopio-ke-i-diafores-timon-elladas-evropis-meso-tou-posokanei/)).
- **Funding.** A €4.6 m package funds AI for the new Market Control and Consumer Protection Authority ([iefimerida](https://www.iefimerida.gr/english/greece-launches-ai-price-comparison-app-put-supermarket-costs-under-public-scrutiny)).

**Context.**
- Greece also caps supermarkets' gross margins. In June 2026 the minister cited a €3 m fine on a multinational for breaching the cap on 48 product codes, and said "Δεν θέλουμε να έχει μόνιμο χαρακτήρα" ("we do not want it to be permanent") [T4] ([Powergame, 2026-06-05](https://www.powergame.gr/ikonomia/1365220/theodorikakos-pote-xekina-i-nea-efarmogi-posokanei/)).
- The consumer federation INKA called a nationwide day of spending nothing on 19 February 2025 ([To Vima](https://www.tovima.com/society/greek-consumer-group-calls-for-market-boycott-over-price-hikes/)).

**Social value.** No evaluation of the effect of e-katanalotis or PosoKanei on prices was found. The survey evidence shows some store switching (17–18%) and low perceived usefulness compared with tax cuts.

### Greece, cross-country: IELKA's European Basket comparison (includes Romania)

**Who runs it.** IELKA (Ινστιτούτο Έρευνας Λιανεμπορίου Καταναλωτικών Αγαθών, the Research Institute for Consumer Goods Retail) runs the comparison.
- It describes itself as "Ν.Π.Ι.Δ. μη κερδοσκοπικού χαρακτήρα με κοινωφελή ερευνητικό σκοπό" ("a non-profit private-law entity with a public-benefit research purpose").
- It says it "Δεν εκπροσωπεί ούτε αντιπροσωπεύει τα μέλη ενώπιον οποιασδήποτε αρχής" ("does not represent its members before any authority") and works with "επιστημονικής και ακαδημαϊκής ουδετερότητας" ("scientific and academic neutrality") ([IELKA, about](https://ielka.gr/%cf%84%ce%b1%cf%85%cf%84%cf%8c%cf%84%ce%b7%cf%84%ce%b1-%cf%80%cf%81%ce%b1%ce%ba%cf%84%ce%b9%ce%ba%ce%ad%cf%82/)).
- The page does not name its members or funders.
- IELKA also runs the "household basket" surveys cited above and a monthly supermarket price index ([IELKA press releases](https://ielka.gr/category/%ce%b1%ce%bd%ce%b1%ce%ba%ce%bf%ce%b9%ce%bd%cf%8e%cf%83%ce%b5%ce%b9%cf%82/page/4/)).

**How often, and how it works.** IELKA calls it an "Επαναλαμβανόμενη έρευνα" ("recurring survey") and says the result has held "διαχρονική την τελευταία 12ετία" ("consistently over the last 12 years") ([IELKA, 2025-02-24](https://ielka.gr/sygkrisi-timwn-12-2024/)). The press archive shows editions on 24 February 2025 (December 2024 data), 23 June 2026 (May 2026 data) and 24 September 2026 (August 2026 data). The last two are 93 days apart, which suggests a roughly quarterly series in 2026 ([IELKA press archive](https://ielka.gr/category/%ce%b1%ce%bd%ce%b1%ce%ba%ce%bf%ce%b9%ce%bd%cf%8e%cf%83%ce%b5%ce%b9%cf%82/page/4/)).
- **Basket and prices.** 40–41 product categories and more than 6,000 final prices, both branded and private-label.
- **Sources.** Price-comparison platforms and price observatories in each country, plus price collection at Chains.
- **Reporting.** Results are shown with and without VAT.
- **Romania sample.** Only Carrefour, Auchan and Mega Image, so none of the discounters (Lidl, Kaufland, Penny, Profi) that the Grocery Basket Index plans to cover.
- **Bulgaria sample** (added from 2026). Kaufland, Lidl, Supermag and eBag.
- **Stated limits.** Excise duties (for example on coffee) are left out, and only supermarket Chains are covered ([IELKA, 2025-02-24](https://ielka.gr/sygkrisi-timwn-12-2024/); [IELKA, 2026-09-24](https://ielka.gr/anakoinosi-24-09-2026/)).
- **Not published.** The matching rule for products, the treatment of promotions and Loyalty prices, and the exchange rates (except the UK's 1.20 EUR/GBP).

**Results for Romania [T4: one interested party, method not fully published].**

| Edition (data month) | Romania vs Greece, incl. VAT | excl. VAT | Bulgaria vs Greece, incl. VAT | excl. VAT |
|---|---|---|---|---|
| 24 Feb 2025 (Dec 2024) | +5% | +10% | not covered | not covered |
| 23 Jun 2026 (May 2026) | +20% | +26% | +17% | +13% |
| 24 Sep 2026 (Aug 2026) | +16% | +22% | +15% | +11% |

Sources: [Feb 2025](https://ielka.gr/sygkrisi-timwn-12-2024/), [Jun 2026](https://ielka.gr/anakoinosi-23-06-2026/), [Sep 2026](https://ielka.gr/anakoinosi-24-09-2026/).

Every edition is headlined that the Greek Basket "συνεχίζουν να είναι χαμηλότερες" ("continues to be cheaper") than in every comparison country. The September 2026 release also uses the comparison to argue that Greece's food VAT is the second-highest burden of the 10 countries examined ([IELKA, 2026-09-24](https://ielka.gr/anakoinosi-24-09-2026/)).

**How it was received.** According to a lead from the map coordinator, the Romanian business outlet Economedia reported the February 2025 edition. That article could not be retrieved in this pass. No independent check of the method was found.

**Why it matters here.**
- It is the closest existing match to the brief's cross-country Basket, and it already puts Romania in the comparison.
- Its Romanian sample leaves out every discounter.
- Romania's gap moved by 15 points in 17 months, and the releases give no explanation. Romanian food inflation (above 7% year on year in April 2026, per the project brief's [Economedia source](https://economedia.ro/?p=350054)) may account for part of it.
- It comes from a body whose funders are not disclosed and whose conclusions consistently favour the domestic retail sector.

It is a cautionary example on whether a cost-of-living comparison tells the truth. That makes the brief's published item lists and matching rules more important.

### Croatia: the 2025 duty to publish price lists, and the apps built on it

**Trigger.** The consumer group "Halo, inspektore" started boycotts on 24 January 2025 ([Wikipedia summary](https://en.wikipedia.org/wiki/2025_Southeast_Europe_retail_boycotts)).
- **Effect on that day [T2].** Tax-administration data show that full-day retail receipts fell from 3,697,571 (worth €60.57 m, on Friday 17 January) to 2,081,506 (€28.60 m, on 24 January), roughly −44% in number and −53% in value. On 31 January the fall against 17 January was −32% and −44% ([tportal reporting Porezna uprava data, 2025-02-01](https://www.tportal.hr/vijesti/clanak/crni-petak-za-trgovce-porezna-uprava-objavile-nove-podatke-o-bojkotu-20250201); see also [Porezna uprava, partial-day figures](https://porezna-uprava.gov.hr/Stranice/Vijest.aspx?NewsID=3859&List=Vijesti)).
- **Effect on prices [T2 via T4].** Croatia's central bank (HNB) had been tracking about 11,000 items in Konzum's online store since December 2024. It found that how often prices changed did not shift after the boycott, and that January food inflation was "gotovo identičn[a]" ("almost identical") before and after it. It added that a wider assessment was hard because most Chains did not publish price data ([biznis.rs citing Jutarnji list, 2025-02-28](https://biznis.rs/vesti/region/analiza-hrvatske-narodne-banke-bojkot-trgovina-bio-je-promasaj/)). The organisers disputed this, claiming €108 m less spending over three weeks [T4] (same source).
- **Price caps.** The government widened its price caps from 30 to 70 products in February 2025 ([ESM Magazine, 2025-04-01](https://www.esmmagazine.com/features/what-happens-when-shoppers-boycott-their-supermarkets-285543); [informator.hr](https://informator.hr/vijesti/krece-treci-bojkot-trgovina-na-snazi-odluka-o-ogranicenoj-cijeni-70-proizvoda)).

**The law** is the Zakon o iznimnim mjerama kontrole cijena (Act on Exceptional Measures of Price Control), NN 40/25, in force since 8 March 2025 ([zakon.hr](https://www.zakon.hr/z/842/Zakon-o-iznimnim-mjerama-kontrole-cijena-)). Article 12:
- Price lists must be published on the trader's website in a digital form suitable for automatic processing, as `.xml` or `.csv`.
- "Trgovac je dužan ažurirati objavljene cijene u cjenicima … u realnom vremenu" ("the trader must update the published prices in real time").
- Traders must allow software tools or automated programs to collect the data, for example through an API.
- The duty applies to supermarkets, hypermarkets, discount stores and cash-and-carry outlets that have a website.

Other provisions:
- Fines for a company run from €3,000 to €30,000 (Art. 20).
- Market inspectors of the State Inspectorate supervise compliance (Art. 18).
- There is no sunset date: the measure lasts "dok se ne otklone razlozi za njezino propisivanje" ("until the reasons for imposing it are removed") (Art. 16) ([zakon.hr](https://www.zakon.hr/z/842/Zakon-o-iznimnim-mjerama-kontrole-cijena-)).

**The implementing decision** is NN 75/2025, adopted 2 May 2025 and in force 15 May 2025 ([Narodne novine](https://narodne-novine.nn.hr/clanci/sluzbeni/2025_05_75_979.html)). It requires:
- files for each store plus one chain-level file, with name, code, brand, quantity, unit, retail price, unit price, barcode and category;
- promotional, clearance and seasonal prices;
- daily updates "najkasnije do 8:00 sati ujutro" ("by 8:00 a.m. at the latest");
- 30 days of retention.

The decision text does not list a Loyalty price field. The government described the measure as the "Israeli model" ([ESM Magazine, 2025-05-06](https://www.esmmagazine.com/retail/croatian-retailers-to-publish-daily-price-lists-287803)).

**Widening in 2026.**
- New decisions in NN 101/26 (adopted 10 September 2026) replace NN 75/25. They extend price-list publication to all retailers and registered service providers with a website, and the "anchor price" to all products ([TEB, 2026-09-22](https://www.teb.hr/novosti/2026/od-1102026-obveza-isticanja-dodatne-sidrene-cijene-i-objave-cjenika-proizvoda-i-usluga/); [informator.hr](https://informator.hr/podzakonski-propisi/842580)).
- NN 110/26 postponed the start from 1 October to 17 November 2026. The ministry's stated aim: "osigurati jasna i provediva pravila" ("to ensure clear and enforceable rules") ([RRiF, 2026-09-30](https://www.rrif.hr/odgada_se_primjena_odluka_o_isticanju_i_objavi_dod-2533-vijest/)).
- An adviser noted "Zakonski tekst je štur i za sada ne postoje dodatna službena tumačenja" ("the legal text is sparse and there are no official interpretations yet") ([Forvis Mazars](https://www.forvismazars.com/hr/en/insights/news/accounting-news/nova-pravila-za-trgovce-i-pruzatelje-usluga)).

**Apps built on the data.** No state-run consumer front end was found; independent developers filled the gap.
- **cijene.dev / cijene-api** (Senko Rašić, Dobar Kod):
  - The first version took four days. It is aimed at developers and researchers, offers free daily archives, and its API is free for non-commercial use ([Lider, 2025-05-23](https://en.lider.media/?p=22751)).
  - The repository has been AGPL-3.0 since 20 May 2025 and was last updated on 10 October 2026. It crawls 29 Chains, from Konzum, Lidl, Plodine, Spar, Kaufland and dm down to regional stores ([GitHub senko/cijene-api](https://github.com/senko/cijene-api)).
  - Data quality [T4]: Chains often publish late, so updates land around 10:00 instead of 08:00. Studenac publishes only some stores. Product names and units are inconsistent, and file structures keep changing ([Lider](https://en.lider.media/?p=22751)).
- **usporedicijene.info:**
  - One developer, Ivo Ugrina, reported more than 30,000 active users in seven days (June 2025) [T4, developer claim] ([Index.hr, 2025-06-05](https://www.index.hr/shopping/clanak/popularna-stranica-za-pracenje-cijena-sad-i-kao-aplikacija/2677687.aspx)).
  - In October 2026 the site lists 27 retailers and 225,453 unique products ([usporedicijene.info](https://usporedicijene.info/)).
  - Its own accuracy warnings: some Chains list promotional prices that do not apply on the stated date, some list products at stores that do not sell them, and dm publishes one uniform price without store addresses. The State Inspectorate confirmed that one unnamed Chain broke the display rules (same source).
- **MojeCijene.net** (Nenad Bakić) also launched in 2025 ([Index.hr](https://www.index.hr/shopping/clanak/popularna-stranica-za-pracenje-cijena-sad-i-kao-aplikacija/2677687.aspx)).

**Funding.** Chains pay to comply. Developers pay for the apps or run them free; cijene.dev offers paid tiers and is open to commercial partnerships ([Lider](https://en.lider.media/?p=22751); [cijene.dev](https://cijene.dev/)).

**Social value.** As of October 2026, no evaluation of the duty's effect on prices, price dispersion or shopper behaviour was found. The nearest causal evidence is from Israel, the model Croatia names: see the box below.

### Bulgaria: from foodprice.bg to kolkostruva.bg before the euro

**foodprice.bg (March 2023)** was launched by the caretaker government [T4] ([Sofia Globe, 2023-03-24](https://sofiaglobe.com/?p=111889)):
- It covered 30 basic foods, using data from the Customs Agency and the revenue agency.
- Chains with more than BGN 30 m turnover could join voluntarily, and promotional prices were barred.
- It compared 11 products with seven European cities, including Bucharest.
- It cost 30,000 leva.
- Reporters questioned its effect, since participation was voluntary and Chains had not submitted data.

What happened to it later was not found.

**Boycott (13 February 2025).** The finance minister said large Chains' turnover fell 28.8% against the previous day, according to data from their fiscal devices [T2] ([BNR, 2025-02-15](https://bnrnews.bg/en/post/126360/the-turnover-of-retail-chains-dropped-by-almost-29-on-the-day-of-the-boycott)). The trade association said a competition-authority probe found no evidence of price manipulation [T4] ([ESM Magazine](https://www.esmmagazine.com/features/what-happens-when-shoppers-boycott-their-supermarkets-285543)).

**kolkostruva.bg ("How much does it cost").**
- **Who and when.** The Consumer Protection Commission (KZP) launched it on 30 September 2025 under the Euro Adoption Act, Art. 55b ([kolkostruva.bg](https://kolkostruva.bg/); [Sofia Globe, 2025-09-30](https://sofiaglobe.com/?p=124932)).
- **Threshold.** At launch it covered retailers with more than BGN 10 m turnover. The prime minister said 256 retailers met that threshold. By August 2026 KZP gave the threshold as €25 m ([Economic.bg, 2026-08-27](https://www.economic.bg/bg/a/view/kolko-bylgari-proveriha-kolkostruva)).
- **Launch problems [T4].** Only 2 of 35 Chains with access had submitted data. The site was Bulgarian-only, needed several steps to reach a price, and had confusing charts ([Sofia Globe](https://sofiaglobe.com/?p=124932)).
- **Chains' view [T4].** Large volumes of item-level daily data are "unlikely to provide useful information to consumers", and the rules ignore multi-buy, end-of-day and near-expiry discounts (same source).
- **Uptake [T3, KZP figures].** KZP reports "над един милион пъти" ("more than one million") visits since launch and "няколко хиляди" ("several thousand") a day. Peaks came in early January 2026 (euro introduction) and early March 2026 (a fuel-price spike). All obligated traders now report ([Economic.bg, 2026-08-27](https://www.economic.bg/bg/a/view/kolko-bylgari-proveriha-kolkostruva)).
- **Supervisory use.** KZP uses the data to flag unusual price movements for inspection (same source).
- **How long it lasts.** The legal duty runs until at least 9 August 2027 (same source).
- **Open data.** The site publishes a daily ZIP archive of all reporting Chains. On 21 October 2026 the archives for 7–20 October were listed, with no licence stated ([kolkostruva.bg open data](https://kolkostruva.bg/opendata)).

**Measured Social value: the clearest truth-telling case [T2].** On 9 April 2026 an ECB blog analysed micro-data from the "Price monitoring portal maintained by Bulgaria's Consumer Protection Commission", covering about 1.4 million products ([ECB Blog](https://www.ecb.europa.eu/press/blog/date/2026/html/ecb.blog20260409~cc951a0d29.en.html)). It found that:
- "price changes during the euro changeover were minimal and typically amounted to only a few euro cents";
- there was "no evidence of systematic upward price adjustments";
- some earlier increases in services added about 0.1 pp to 2025 inflation.

HICP inflation fell from 3.5% (December 2025) to 2.3% (January 2026) (same source).

**Enforcement context [T4, headline only].** A trade outlet reported that KZP will fine €10,000–50,000 per product with an unjustified price increase (14 October 2026). The page could not be opened ([banker.bg](https://banker.bg/2026/10/14/kzp-globi-ot-10-000-do-50-000-evro/)).

### Slovenia: the ministry's basket survey (Primerjaj-cene.si)

**Who and how.** The Ministry of Agriculture, Forestry and Food ran the surveys. The first, on 13 September 2022, was done through the Naša super hrana portal.
- In-store surveys every 14 days at six Chains: Eurospin, Lidl, Hofer, Mercator, Spar and Tuš.
- A basic Basket of 15 food groups and an extended one of 28, priced at regular (non-promotional) prices.
- Daily online tracking of more than 17,000 products at four e-shops ([gov.si, 2023-11-24](https://www.gov.si/novice/2023-11-24-povprecni-vrednosti-najcenejse-osnovne-in-razsirjene-kosarice-trgovcev-dosegli-najnizjo-vrednost/)).
- The site was built by April 8 d.o.o. ([primerjaj-cene.si](https://primerjaj-cene.si/)).

**Results claimed [T2, ministry's own count].**
- The ministry's own surveys reported the basic Basket at successive lows: the 10th survey (January 2023) was headlined "lowest price to date" ([gov.si EN, 2023-01-20](https://www.gov.si/en/news/2023-01-20-10th-survey-of-the-basic-food-basket-shows-lowest-price-to-date/)), and by the 15th (March 2023) it was at "the lowest value since the start of monitoring" ([Eurofound record SI-2022-36](https://static.eurofound.europa.eu/covid19db/cases/SI-2022-36_2838.html)). Eurofound lists no evaluation of the measure.
- In November 2023 the basic Basket ranged from €16.37 at Hofer to €38.50 at Eurospin ([gov.si](https://www.gov.si/novice/2023-11-24-povprecni-vrednosti-najcenejse-osnovne-in-razsirjene-kosarice-trgovcev-dosegli-najnizjo-vrednost/)). Eurospin had been the cheapest Chain in the first round (€47.38) ([Slovenia Times](https://sloveniatimes.com/35282/census-shows-eurospin-and-slovenia-have-cheapest-staple-foods)). A Chain can swing from cheapest to dearest under the same method.

**Chains' reaction [T4].** On 20 September 2022 the Trade Chamber (TZS) asked the ministry to halt the project. It cited "primerjava med seboj neprimerljivih izdelkov, napačni so popisi cen in slikovne oznake" ("comparison of incomparable products, wrong price records and picture labels"), "nepopravljive škode" ("irreparable damage") to Chains, and VAT differences across countries ([24ur, 2022-09-21](https://www.24ur.com/novice/slovenija/tzs-pozvala-k-zacasni-ustavitvi-primerjanja-cen-osnovnih-zivil.html)). In December 2023 TZS called the Baskets "dodatno administrativno, finančno in organizacijsko breme" ("an additional administrative, financial and organisational burden") ([RTV SLO, 2023-12-27](https://www.rtvslo.si/n/692957)).

**Gaming and truth problems.**
- In September 2023 the ministry referred to the market inspectorate "prakse, ki lahko vodijo k zavajajočemu oglaševanju najcenejših košaric" ("practices that can lead to misleading advertising of the cheapest baskets") ([gov.si, 2023-09-18](https://www.gov.si/novice/2023-09-18-popis-osnovne-in-razsirjene-kosarice-osnovnih-skupin-zivil-skupaj-s-trznim-inspektoratom)).
- In December 2023 the former food-supply-chain ombudsman suspected that Chains cut prices only for the survey, noting "Potrošniki niso zaznali znižanja maloprodajnih cen" ("consumers did not notice lower retail prices"). The survey had recorded bread at €0.19/kg.
- The ministry replied that two unannounced inspections found no irregularities, and the competition agency denied any cartel ([RTV SLO](https://www.rtvslo.si/n/692957); [N1 Slovenija, 2023-12-27](https://n1info.si/novice/slovenija/ministrstvo-zavraca-ocitke-glede-spremljanja-cen-kosarice-zivil/)).
- Whatever the cause, a "cheapest Basket" built from the cheapest item in each category rewards a Chain for pricing one product very low.

**How long it lasted.** The ministry said in December 2023 that it would continue in 2024 ([RTV SLO](https://www.rtvslo.si/n/692957)). Checked on 21 October 2026, the site's latest results were still dated 22 December 2023 ([primerjaj-cene.si](https://primerjaj-cene.si/)), so it looks dormant.

**Boycotts.** There were only small boycotts. Croatians crossed the border to shop in Slovenia during their own boycott ([Wikipedia summary](https://en.wikipedia.org/wiki/2025_Southeast_Europe_retail_boycotts)).

### Poland

This research found no state-run grocery Comparable in Poland. The search budget ran out before Polish primary sources could be checked, so treat Poland as an open gap, not a finding of absence (see Gaps).

### Others found along the way

- **Slovakia.** Besides the March 2024 enquiry about buying Árfigyelő ([VG](https://www.vg.hu/vilaggazdasag-magyar-gazdasag/2024/03/hivatalosan-is-lepett-a-szlovak-kormany-lemasolnak-az-arfigyelot)), a boycott was called on 6 February 2025 ([Wikipedia summary](https://en.wikipedia.org/wiki/2025_Southeast_Europe_retail_boycotts)).
- **Montenegro.** A "limitirane cijene" scheme has fixed the prices of 73 products since March 2024. It is a price cap, not a Comparable ([RFE/RL, 2025-01-30](https://www.slobodnaevropa.org/a/bojkot-trgovina-crna-gora-limitirane-cijene/33297015.html)). The tax administration reported that the five largest Chains' revenue fell 56.14% on 31 January 2025, against the same period a week earlier [T2 via T4] ([N1 BiH, 2025-02-13](https://n1info.ba/english/news/cost-of-living-crisis-consumers-in-western-balkans-boycott-supermarkets/)).
- **North Macedonia.** The Public Revenue Office reported −46.59% at the eight largest Chains on 31 January 2025, then +11.2% the next day [T2 via T4] ([N1 BiH](https://n1info.ba/english/news/cost-of-living-crisis-consumers-in-western-balkans-boycott-supermarkets/)). Margins were then capped at 5%, 10% or 15% until 30 April 2025 [T4] ([ESM Magazine](https://www.esmmagazine.com/features/what-happens-when-shoppers-boycott-their-supermarkets-285543)).
- **Bosnia and Herzegovina.** Federation tax data show turnover falling from €53.8 m (6 February) to €24.4 m (8 February 2025). A three-month freeze on 65 products followed [T4] ([ESM Magazine](https://www.esmmagazine.com/features/what-happens-when-shoppers-boycott-their-supermarkets-285543)).
- **Serbia.** The tax administration reported a turnover drop of "roughly one-third" on 31 January 2025, while the organisers said 37%. The competition commission had opened proceedings against four Chains in October 2024 [T4] ([N1 BiH](https://n1info.ba/english/news/cost-of-living-crisis-consumers-in-western-balkans-boycott-supermarkets/); [ESM Magazine](https://www.esmmagazine.com/features/what-happens-when-shoppers-boycott-their-supermarkets-285543)).
- **Romania (for contrast only).** The 10–16 February 2025 boycott, led by Călin Georgescu, saw little uptake. The association of large retail networks reported no disruption across more than 4,500 stores, and Carrefour cut prices on about 1,500 products until 31 March [T4] ([ESM Magazine](https://www.esmmagazine.com/features/what-happens-when-shoppers-boycott-their-supermarkets-285543)). Monitorul Prețurilor is covered by its own ticket.

### Box: what causal studies elsewhere say about price-transparency mandates

- **Israel, 2015 supermarket price-publication rule (the model Croatia names) [T1].** Using a difference-in-differences design, the authors find that "price levels and price dispersion declined significantly after the regulation", and that Chains began setting identical prices in all stores. Low-priced Chains "referenced price-comparison surveys conducted by the media" in their ads (Ater and Rigbi, *AEJ: Microeconomics* 15(1), 2023) ([AEA](https://www.aeaweb.org/doi/10.1257/mic.20200337)). The 2018 working paper puts the fall at "4% to 5% after the regulation, primarily in premium chains". It adds that "price comparison platforms that became available after the regulation failed to gain traction" ([Falk Institute DP 18.04](https://falk.huji.ac.il/sites/default/files/falkheb/files/paper_18-04a.pdf)). For this project, the channel that worked was media price surveys that discounters could cite. That is close to what the Grocery Basket Index plans to be.
- **Denmark, 1993: the authority published ready-mixed concrete prices [T1].** "Average prices of reported grades increased by 15–20 percent within one year". The authors attribute this to softer competition (Albæk, Møllgaard and Overgaard, *Journal of Industrial Economics*, 1997) ([IDEAS/RePEc](https://ideas.repec.org/a/bla/jindec/v45y1997i4p429-443.html)).
- **Chile: online fuel-price disclosure [T1].** Margins rose about 9% on average, least in high-search, higher-income areas, so the effect was regressive (Luco, *AEJ: Microeconomics* 11(2), 2019) ([AEA](https://aeaweb.org/doi/10.1257/mic.20170110)).

These are concentrated or homogeneous markets, so they do not transfer directly to grocery Baskets. They are the reason harms deserve full weight: the same transparency can cut prices when it reaches shoppers and the media, or raise them when it mostly reaches rival sellers.

## Gaps and uncertainties

- **Search budget.** The shared web-search budget ran out partway through. Some later checks were done only by fetching known pages, so the next three items are open.
- **Poland** was not researched against primary sources. A follow-up is needed covering any state portal, consumer-group basket indices, private basket surveys, and Demand signals such as leaflet aggregators.
- **Slovenia after December 2023.** It is unconfirmed whether the surveys stopped formally or only stopped being published.
- **Greece.** The end date of the "household basket" scheme is not established. PosoKanei's cost, developer and uptake since June 2026 were not found, and posokanei.gov.gr refused automated access.
- **Hungary.**
  - The full Makronóm paper, its funder and its donor pool were not reviewed.
  - The GVH's claim of a ~10 pp dairy-margin reduction was seen only in a news report.
  - No official usage figures after July 2023 were found, and the cost of running Árfigyelő is unknown.
- **Croatia.**
  - The HNB boycott analysis is known only through press reports.
  - App usage rests on one developer's claim.
  - No study of the price-list duty's effect exists yet.
  - The final scope of the 17 November 2026 rules (fields, Loyalty price, service providers) should be checked against the NN 101/26 and NN 110/26 texts.
- **Bulgaria.**
  - The reporting threshold differs between sources (BGN 10 m on the portal, €25 m per KZP in August 2026), possibly because of the August 2026 amendments.
  - The enforcement figures (fines per product) come from a headline only.
  - foodprice.bg's fate is unknown.
- **Western Balkans.** Several boycott figures reach this note only through secondary sources (N1, ESM Magazine), and baselines differ by country (previous day against the same day a week earlier), so they cannot be compared directly.
- **Harms.** No study tests whether any CEE grocery Comparable made it easier for sellers to coordinate prices, and no CEE study measures distributional effects (who benefits).
- **IELKA.**
  - The Economedia article on the February 2025 edition was not retrieved.
  - IELKA's members, funders and full method (product matching, promotions, Loyalty prices, exchange rates) are not published on the pages read.
  - The VAT rates IELKA states for Romania in September 2026 (11% and 5%) were not checked against Romanian law.
  - Editions before 2025 were not reviewed.
- **Truth-telling.** Apart from the ECB's Bulgarian analysis, no source checks whether these Comparables' cost-of-living comparisons were accurate. Greece's cross-country comparison works at category level, a method that can mislead.

## Questions this raises

1. **Basket method against gaming.** Should the index rank Chains on the cheapest item per category, which Slovenia's €0.19 bread shows can be gamed, or on fixed matched products or category medians? Should it flag prices below a plausibility floor?
2. **Cadence and harms.** Does publishing weekly Basket totals rather than daily item-level prices lower the risk of helping Chains coordinate, while keeping the value for shoppers and the media?
3. **Open-data advocacy.** Should the project propose that Romania copy Croatia's statutory model: daily machine-readable store-level price lists, plus an explicit right to collect them automatically? That would largely settle the terms-of-service risk in the project brief.
4. **Cross-country data source.** Could the international Basket use state open data instead of scraping? Candidates are Bulgaria's daily ZIPs, Croatia's price lists or the AGPL cijene-api, Hungary's same-day Árfigyelő and Greece's PosoKanei. Which reuse terms and licences apply? Hungary's action against an app that copied Árfigyelő says check before reusing.
5. **Chains citing the index.** Under the GVH's Lidl commitments, a Chain may claim to be cheapest only with at least a 2.5% gap and on the regulator's data. Should the index publish its own rule for Chains that cite it in advertising?
6. **Loyalty price precedent.** Hungary requires a Loyalty price beside the Shelf price. Could that support asking Romanian Chains or authorities for Loyalty price data?
7. **Evaluation design.** No CEE Comparable planned an evaluation, so their Social value cannot be shown. Should the index set up its counterfactual and evaluation design (for example a synthetic control on Basket prices) before launch?
8. **Media as the mechanism.** If the Israeli result holds, value comes from journalists and discounters citing comparisons, not from shoppers opening an app. Does that make the brief's "cited by media" success signal more important than app features?
9. **The existing Romania-in-Europe comparison.** IELKA already tells the press that Romania's Basket costs 16–20% more than Greece's (2026), based on three Romanian Chains and no discounters. Should the international Basket be designed so it can confirm or correct such claims, matching identical products, comparing with and without VAT, and covering discounters? Should the project contact IELKA about its method?
10. **Scope notes for the map.**
   - Poland needs its own follow-up.
   - The Monitorul Prețurilor ticket should compare Romania with the Croatian and Bulgarian statutory open-data models.
   - A possible new ticket: "Reuse terms of state price data in BG/HR/HU/GR".

## Sources

**Hungary**
- GVH, Árfigyelő FAQ (July 2025): https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf
- GVH, first-week press release (2023-07-08): https://gvh.hu/en/press_room/press_releases/press-releases-2023/the-price-monitoring-system-has-been-up-and-running-for-a-week-more-improvements-coming-soon
- GVH, single-digit inflation release (2023-11-10): https://gvh.hu/en/press_room/press_releases/press-releases-2023/gvh-the-price-monitoring-database-in-hand-with-government-measures-has-helped-to-achieve-single-digit-inflation
- GVH, Makronóm study release (2024-09-04): https://www.gvh.hu/en/press_room/press_releases/press-releases-2024/hungarian-families-saved-nearly-huf-20-billion-in-three-months-thanks-to-the-online-price-monitor
- Telex, rules published (2023-05-08): https://telex.hu/gazdasag/2023/05/08/online-arfigyelo-adatszolgaltatas-kiskereskedelem-inflacio-gazdasagi-versenyhivatal
- Telex G7, coverage criticism (2023-05-10): https://telex.hu/g7/kozelet/2023/05/10/a-kormany-arfigyelo-rendszere-ott-elezne-az-arversenyt-ahol-mar-nem-lehet
- Telex, unofficial app (2023-08-05): https://telex.hu/belfold/2023/08/05/gvh-figyelmeztetes-kalozapplikacio-arfigyelo
- HVG, usage (2024-06-28): https://hvg.hu/gazdasag/20240628_GVH:-Nemzetkozi-erdeklodes-van-az-Arfigyelo-irant
- VG, Slovak enquiry (2024-03-05): https://www.vg.hu/vilaggazdasag-magyar-gazdasag/2024/03/hivatalosan-is-lepett-a-szlovak-kormany-lemasolnak-az-arfigyelot
- Economx, expansion (2025-02-25): https://www.economx.hu/gazdasag/2025/02/25/arfigyelo-gvh-uj-termekek-eljarasok-804936/
- Economx, Lidl commitments (2025-11-13): https://www.economx.hu/magyar-gazdasag/2025/11/13/gvh-versenyhivatal-eljaras-lidl-arak-819279/
- Economx, end of state of danger (2026-05-14): https://www.economx.hu/belfold/2026/05/14/hivatalos-megszunt-az-orosz-ukran-haboru-miatt-elrendelt-veszelyhelyzet/
- 444, margin cap made open-ended (2026-04-18): https://444.hu/2026/04/18/orbanek-hagyjak-hogy-magyar-peterek-dontsenek-az-arres-es-kamatstopokrol
- Daily News Hungary, PM Magyar on the margin cap (2026-10-02): https://dailynewshungary.com/pm-magyar-hungary-food-margin-cap-stop/
- ELTE KRTK, Fertő and Podruzsik (2026-09-17): https://krtk.elte.hu/en/2026/09/price-caps-do-not-stop-price-transmission-they-change-where-it-happens-by-imre-ferto-and-szilard-podruzsik/

**Greece**
- Ministry of Development, e-katanalotis launch (2020-03-05): https://www.mindev.gov.gr/wp-content/uploads/2020/03/2020-3-5-E-KATANALOTIS-1.pdf
- Parapolitika, usage (2023-04-12): https://www.parapolitika.gr/oikonomia/article/1265932/e-katanalotis-stin-platforma-ta-timologia-ilektrikis-energeias-kai-fusikou-aeriou-olon-ton-parohon/
- iefimerida, IELKA survey (2022-11-14): https://www.iefimerida.gr/ellada/ereyna-ielka-proionta-kalathi-toy-noikokyrioy
- IELKA via oenet.gr (2023-02-07): https://www.oenet.gr/τελευταία-νέα/τρόφιμα/item/99673-ielka-anakoinosi-tipou-gia-to-kalathi-tou-noikokiriou
- iefimerida, PosoKanei launch (2026-06-17): https://www.iefimerida.gr/english/greece-launches-ai-price-comparison-app-put-supermarket-costs-under-public-scrutiny
- Skai, PosoKanei FAQ (2026-06-17): https://www.skai.gr/news/greece/nea-platfmorma-kata-tis-akriveias-ti-einai-to-posokanei-pos-leitourgei
- newmoney, PosoKanei launch (2026-06-17): https://www.newmoney.gr/roh/palmos-oikonomias/oikonomia/theodorikakos-sto-mikroskopio-ke-i-diafores-timon-elladas-evropis-meso-tou-posokanei/
- Powergame, minister interview (2026-06-05): https://www.powergame.gr/ikonomia/1365220/theodorikakos-pote-xekina-i-nea-efarmogi-posokanei/
- To Vima, INKA boycott call: https://www.tovima.com/society/greek-consumer-group-calls-for-market-boycott-over-price-hikes/
- IELKA, about: https://ielka.gr/%cf%84%ce%b1%cf%85%cf%84%cf%8c%cf%84%ce%b7%cf%84%ce%b1-%cf%80%cf%81%ce%b1%ce%ba%cf%84%ce%b9%ce%ba%ce%ad%cf%82/
- IELKA, press archive: https://ielka.gr/category/%ce%b1%ce%bd%ce%b1%ce%ba%ce%bf%ce%b9%ce%bd%cf%8e%cf%83%ce%b5%ce%b9%cf%82/page/4/
- IELKA, European comparison, December 2024 data (2025-02-24): https://ielka.gr/sygkrisi-timwn-12-2024/
- IELKA, European comparison, May 2026 data (2026-06-23): https://ielka.gr/anakoinosi-23-06-2026/
- IELKA, European comparison, August 2026 data (2026-09-24): https://ielka.gr/anakoinosi-24-09-2026/

**Croatia**
- Zakon o iznimnim mjerama kontrole cijena, NN 40/25: https://www.zakon.hr/z/842/Zakon-o-iznimnim-mjerama-kontrole-cijena-
- Decision NN 75/2025: https://narodne-novine.nn.hr/clanci/sluzbeni/2025_05_75_979.html
- informator.hr, decision status: https://informator.hr/podzakonski-propisi/842580
- TEB, NN 101/26 (2026-09-22): https://www.teb.hr/novosti/2026/od-1102026-obveza-isticanja-dodatne-sidrene-cijene-i-objave-cjenika-proizvoda-i-usluga/
- RRiF, postponement NN 110/26 (2026-09-30): https://www.rrif.hr/odgada_se_primjena_odluka_o_isticanju_i_objavi_dod-2533-vijest/
- Forvis Mazars, new rules: https://www.forvismazars.com/hr/en/insights/news/accounting-news/nova-pravila-za-trgovce-i-pruzatelje-usluga
- ESM Magazine, "Israeli model" (2025-05-06): https://www.esmmagazine.com/retail/croatian-retailers-to-publish-daily-price-lists-287803
- GitHub senko/cijene-api: https://github.com/senko/cijene-api
- cijene.dev: https://cijene.dev/
- Lider, cijene.dev (2025-05-23): https://en.lider.media/?p=22751
- Index.hr, usporedicijene app (2025-06-05): https://www.index.hr/shopping/clanak/popularna-stranica-za-pracenje-cijena-sad-i-kao-aplikacija/2677687.aspx
- usporedicijene.info: https://usporedicijene.info/
- tportal, Porezna uprava boycott data (2025-02-01): https://www.tportal.hr/vijesti/clanak/crni-petak-za-trgovce-porezna-uprava-objavile-nove-podatke-o-bojkotu-20250201
- Porezna uprava, boycott figures (2025-02-07): https://porezna-uprava.gov.hr/Stranice/Vijest.aspx?NewsID=3859&List=Vijesti
- biznis.rs, HNB analysis (2025-02-28): https://biznis.rs/vesti/region/analiza-hrvatske-narodne-banke-bojkot-trgovina-bio-je-promasaj/
- informator.hr, 70-product cap: https://informator.hr/vijesti/krece-treci-bojkot-trgovina-na-snazi-odluka-o-ogranicenoj-cijeni-70-proizvoda

**Bulgaria**
- kolkostruva.bg: https://kolkostruva.bg/ and open data: https://kolkostruva.bg/opendata
- Sofia Globe, foodprice.bg (2023-03-24): https://sofiaglobe.com/?p=111889
- Sofia Globe, kolkostruva launch (2025-09-30): https://sofiaglobe.com/?p=124932
- Economic.bg, usage (2026-08-27): https://www.economic.bg/bg/a/view/kolko-bylgari-proveriha-kolkostruva
- ECB Blog, euro adoption and prices (2026-04-09): https://www.ecb.europa.eu/press/blog/date/2026/html/ecb.blog20260409~cc951a0d29.en.html
- BNR, boycott turnover (2025-02-15): https://bnrnews.bg/en/post/126360/the-turnover-of-retail-chains-dropped-by-almost-29-on-the-day-of-the-boycott
- banker.bg, fines headline (2026-10-14): https://banker.bg/2026/10/14/kzp-globi-ot-10-000-do-50-000-evro/

**Slovenia**
- primerjaj-cene.si: https://primerjaj-cene.si/
- gov.si, November 2023 survey: https://www.gov.si/novice/2023-11-24-povprecni-vrednosti-najcenejse-osnovne-in-razsirjene-kosarice-trgovcev-dosegli-najnizjo-vrednost/
- gov.si EN, 10th survey (2023-01-20): https://www.gov.si/en/news/2023-01-20-10th-survey-of-the-basic-food-basket-shows-lowest-price-to-date/
- Eurofound COVID-19 EU PolicyWatch record SI-2022-36: https://static.eurofound.europa.eu/covid19db/cases/SI-2022-36_2838.html
- gov.si, inspectorate referral (2023-09-18): https://www.gov.si/novice/2023-09-18-popis-osnovne-in-razsirjene-kosarice-osnovnih-skupin-zivil-skupaj-s-trznim-inspektoratom
- Slovenia Times, first census: https://sloveniatimes.com/35282/census-shows-eurospin-and-slovenia-have-cheapest-staple-foods
- 24ur, TZS demands halt (2022-09-21): https://www.24ur.com/novice/slovenija/tzs-pozvala-k-zacasni-ustavitvi-primerjanja-cen-osnovnih-zivil.html
- RTV SLO (2023-12-27): https://www.rtvslo.si/n/692957
- N1 Slovenija (2023-12-27): https://n1info.si/novice/slovenija/ministrstvo-zavraca-ocitke-glede-spremljanja-cen-kosarice-zivil/

**Regional boycotts and others**
- Wikipedia, 2025 Southeast Europe retail boycotts: https://en.wikipedia.org/wiki/2025_Southeast_Europe_retail_boycotts
- N1 BiH (2025-02-13): https://n1info.ba/english/news/cost-of-living-crisis-consumers-in-western-balkans-boycott-supermarkets/
- ESM Magazine (2025-04-01): https://www.esmmagazine.com/features/what-happens-when-shoppers-boycott-their-supermarkets-285543
- RFE/RL Montenegro (2025-01-30): https://www.slobodnaevropa.org/a/bojkot-trgovina-crna-gora-limitirane-cijene/33297015.html

**Academic**
- Ater and Rigbi (2023), AEJ: Micro 15(1): https://www.aeaweb.org/doi/10.1257/mic.20200337
- Ater and Rigbi, Falk Institute DP 18.04 (2018): https://falk.huji.ac.il/sites/default/files/falkheb/files/paper_18-04a.pdf
- Albæk, Møllgaard and Overgaard (1997), JIE 45(4): https://ideas.repec.org/a/bla/jindec/v45y1997i4p429-443.html
- Luco (2019), AEJ: Micro 11(2): https://aeaweb.org/doi/10.1257/mic.20170110
