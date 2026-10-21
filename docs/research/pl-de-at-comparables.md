# What grocery price Comparables exist in Poland, Germany and Austria?

Desk research for ticket [#20](https://github.com/exilonX/cart-compare/issues/20) on the Grocery Basket Index map ([#1](https://github.com/exilonX/cart-compare/issues/1)). Researched 2026-10-21. Every figure carries the date it refers to. Terms follow the project glossary (`CONTEXT.md`): Comparable, Demand signal, Social value, Basket, Chain, Shelf price, Loyalty price.

This note extends three earlier notes and does not repeat them: CEE Comparables (ticket #3, which left Poland open), Western Comparables (ticket #4, which covered Heisse Preise's decline, German leaflet apps, Verbraucherzentrale Hamburg's shrinkflation list and one MTS-K study), and transparency effects (ticket #5, which covered the academic MTS-K studies).

**Evidence tiers used below** (same scheme as the CEE note)

- **[T1]** causal academic study
- **[T2]** evaluation, decision or official statistics from a regulator, ministry, statistics office or parliament
- **[T3]** usage statistics and consumer surveys
- **[T4]** media reports, and claims or price surveys by interested parties (Chains, trade associations, consumer groups, developers, politicians)

## Answer

- **No state in the three countries runs a Comparable that compares Chains.**
  - Poland and Germany have no state grocery price portal.
  - Austria's statistics office launched a food "Preisradar" on 19 January 2026. It shows about 100 foods as indices, average prices and price bands built from Chains' scanner data, with no price for any named Chain [T2].
  - Austria's 2023 plan for a state price calculator was dropped in September 2023. The government chose instead to require Chains to give private comparison sites an API. The competition authority (BWB) designed that duty. No law enacting it was found, and in September 2025 the opposition was still asking for one [T2].
- **The state's main role was to police Chains' price claims, not to publish prices.**
  - Poland's UOKiK said in 2018 that consumers have a right to compare prices. It fined Biedronka's owner PLN 115 m in 2020 over checkout prices above Shelf prices. It has since acted repeatedly on misleading discounts and on Chains' "cheapest basket" claims (2022–2026) [T2].
  - Germany has debated a state food price observatory since at least 2024, pushed by the federal consumer group (vzbv), foodwatch and the Greens. The retail association calls it bureaucracy. The agriculture minister said in January 2026 he "cannot and will not intervene in the market" [T4].
- **Volunteers built Austria's Comparables within days, and they decayed within about two years.**
  - Heisse Preise's code repository was created on 8 May 2023, the day of the government's food summit. By September 2023 the BWB had surveyed five volunteer comparison sites. All five named legal uncertainty about crawling Chains' web shops as an obstacle [T2].
  - The BWB concluded that such sites would strengthen competition, because Chains already crawl each other's prices [T2].
  - By November 2025 Heisse Preise had stopped updating 11 store feeds, per its own site (see also the Western note).
- **The consumer-group Baskets that last measure price levels; none of them ranks Chains.**
  - Austria's Chamber of Labour (AK Wien) has two recurring surveys:
    - a Vienna Basket of the 40 cheapest products, which found supermarkets 11% dearer than discounters (September 2026);
    - an Austria-versus-Germany comparison of identical branded foods, run every year since 2021. Its net gap grew from 8.8% (2022) to 23.2% (2025), and it feeds the EU debate on "territorial supply constraints" [T4].
  - No recurring Chain-ranking Basket was found in Germany. Instead it has:
    - one-off market checks (Verbraucherzentrale NRW, May 2023);
    - a Stiftung Warentest test of 16 saving apps, which rated none "good" (April 2023);
    - foodwatch's Preisradar, which began scraping three Chains' own-brand prices daily in May 2024, without Lidl because Lidl publishes no full online prices; its page does not show whether it is still updated [T4].
- **Poland's Comparables are private or media-run, and the method decides the winner.**
  - ASM SFA prices 40 identical branded products at 13 Chains every month. In July 2026, Auchan was cheapest at PLN 264.66 and Aldi dearest at PLN 344.62. On average, discounters were the dearest format, because a brand-only Basket leaves out their private labels [T4].
  - The tabloid Fakt's 25–26-item Basket put Lidl below Biedronka in every month it reported for January–June 2024, and Lidl quoted its Fakt wins in its leaflets [T4].
  - Industry analysts said the 2024–2025 "basket war" of Chain-run comparisons left shoppers believing "nobody" [T4].
- **The German fuel price monitor (MTS-K) was evaluated first-hand by the economics ministry, not by the Bundeskartellamt** (Bundestag Drucksache 19/3693, 3 August 2018).
  - **Uptake** [T3]. About a quarter of drivers used price apps "constantly to occasionally", which the report equates to "several million" people.
  - **Behaviour** [T3]. About a quarter said they now fill up at other times of day, and about 15% at other stations.
  - **Cost** [T2]. Reporting costs fuel companies about €1.5 m a year, half the estimate, and the Bundeskartellamt spends about 6.5 full-time staff on the monitor.
  - **Side effect** [T2]. The oil industry also uses the published prices for its own pricing.
  - **Conclusion** [T2]. It was "too early" to judge the effect on competition. The report recommended continuing the monitor and evaluating it again after five years. No second evaluation was found.
- **Measured Social value is thin.**
  - No causal study of any Polish, German or Austrian grocery Comparable was found.
  - AK's check of Austria's July 2026 food VAT cut found it fully passed on at all seven Chains checked [T4].
  - The BWB's estimate of "up to 4%" lower prices from better comparison rests on the Israeli study, not on Austrian data [T2 citing T1].
  - The finding repeated in all three countries is cent-identical own-brand prices across Chains (Heisse Preise 2023, VZ NRW 2023, foodwatch Germany 2025, foodwatch Austria 2026) [T4]. No authority has found collusion: the BWB found no price-fixing in November 2023 [T2].
- **Harms and truth problems centre on matching and on cross-country gaps.**
  - Austria's retail association documented comparison-site errors: branded goods matched against discount own brands, promotional prices against regular prices, wrong pack sizes. The BWB agreed these occur "in individual cases" [T2].
  - Estimates of Austria's price gap with Germany range widely by method [T2, T4]:
    - 10–15% net, from one retailer's calculation reported by the BWB;
    - 15–20%, from the consumer association VKI;
    - 21–26%, from AK;
    - up to 60% on some products, per the Austrian retail association.
  - Poland's ministry, with UOKiK, dismissed a 7-product Poland–Germany comparison: it gave "no basis" for conclusions, and its method was unknown (April 2025) [T2].
- **What this means for the Grocery Basket Index.**
  - Germany, a launch comparison country, offers no state price data at Chain level.
  - Scraping cannot reach discounters' full ranges there.
  - AK's method (identical brands, online shops, gross and net of VAT, promotions in, Loyalty prices out) is a ready template for the international Basket. So is the warning that brand-only Baskets misrank discounters.

## Comparison table

| Country | Comparable | Type | Run by | Lifespan (status 2026-10-21) | Method | Uptake (dated) | Funding | Strongest Social value evidence |
|---|---|---|---|---|---|---|---|---|
| Austria | [Statistik Austria Preisradar](https://www.statistik.at/preisradar/) | State index tool, no Chain prices | Statistik Austria, after a government decision in September 2025 | 19 Jan 2026 – running; updated 16 Oct 2026 | Weekly scanner data from "the largest" Chains since 2022; ~100 foods; producer, wholesale and retail levels; group-level comparison with DE, CH and the euro area | Not published | State; cost not published | None; foodwatch calls it "incomplete, confusing" (Jun 2026) [T4] |
| Austria | [Heisse Preise](https://heisse-preise.io/) and four similar sites (Preismonitor.at, Preisrunter.at, Supermarkt.at, Teuerungsportal.at) | Indie apps | Individuals, unpaid | Heisse Preise: 8 May 2023 – decaying (11 feeds stopped by Nov 2025) | Daily crawling of Chains' web shops; Heisse Preise covered 10 AT, 2 DE, 1 SI retailers, history from 2017 (Sept 2023) | Not published | Volunteers; "simple server" costs | Exposed cent-identical own-brand prices [T4]; shaped BWB's API proposal [T2] |
| Austria | [AK Preismonitor](https://wien.arbeiterkammer.at/preismonitor) (Vienna) | Consumer-body Basket | Arbeiterkammer Wien (statutory chamber of labour) | At least Jun 2024 (earliest edition seen in listings) – running; latest Sept 2026 | 40 cheapest products plus some cleaning products, 7 Chains, 3 Vienna branches each; brand Basket of 31 items online | Wire and regional press pick-up (Oct 2026) [T4] | Chamber budget | VAT cut fully passed on (Jul 2026) [T4] |
| Austria | AK Austria–Germany branded comparison | Consumer-body cross-country Basket | Arbeiterkammer Wien | Yearly since 2021 | ~70 identical branded foods at Billa and Interspar (AT) vs Rewe and Globus (DE) online; gross and net of VAT; promotions in, Loyalty prices out | Cited in the EU Semester country report (2019, per AK) | Chamber budget | Fed the EU "territorial supply constraints" debate [T4] |
| Germany | MTS-K fuel price monitor (fuel, not groceries) | State data feed to licensed apps | Bundeskartellamt | Regular operation since 1 Dec 2013 – running | Stations report each price change in real time; data passed to licensed consumer information services | ~¼ of drivers use apps regularly; "several million" users (survey late 2016) | ~6.5 FTE at the Bundeskartellamt; industry €1.5 m/yr | Ministry evaluation 2018 [T2]; causal studies in the transparency note [T1] |
| Germany | [foodwatch Preisradar](https://www.foodwatch.org/de/informieren/foodwatch-preisradar) | Consumer-group price tracker | foodwatch (NGO) | Tracking since May 2024; published 14 Jan 2025; current update status not shown | Daily scrape of entry-level own brands at Rewe (Cologne store), Edeka (one store) and Aldi Nord online; Lidl excluded | Not published | Not stated on the pages read | Documented lockstep own-brand prices [T4] |
| Germany | Verbraucherzentrale NRW market check | One-off consumer-centre Basket | Verbraucherzentrale NRW | Single check, 9 May 2023 | 19 staples, 20 branches of Edeka, Rewe, Aldi and Lidl in 5 cities | Press release | Consumer centre | Spreads above 100% for 17 of 19 foods [T4] |
| Poland | ASM SFA Koszyk Zakupowy, plus app (Jul 2025) | Private Basket index | ASM Group, a sales and merchandising agency selling data to FMCG firms and Chains | At least Mar 2023 – running (monthly) | 40 identical branded products and sizes, 13 Chains, stores and e-commerce | App uptake not published | Commercial | None; Polomarket disputed its method (Mar 2023) [T4] |
| Poland | Koszyk Faktu | Media Basket | *Fakt* daily | Running in 2024; start not found | 25–26 items at randomly chosen stores of Lidl, Biedronka, Dino, Lewiatan (Aldi once) | Lidl cites it in leaflets (Apr 2024) | Newspaper | None [T4] |
| Poland | UCE Research / WSB Merito "Indeks cen w sklepach detalicznych" | Private price index (no Chain ranking) | UCE Research and WSB Merito University | Monthly; latest Jul 2026 data | 100 products, 17 categories, >103,000 prices, >47,300 stores, 64 Chains; regular and promotional prices | Wide press pick-up (PAP, Forsal, money.pl) | Not disclosed | None |
| Poland | No state Comparable found | – | UOKiK polices claims | – | – | – | – | UOKiK decisions on price claims [T2] |

## Detailed findings

### Poland

#### The state: enforcement, not a portal

No Polish state grocery price portal, draft law or ministry plan for one was found. The searches covered UOKiK's site, the Sejm interpellation database and the Polish trade press. Two ministry answers to MPs in 2025 discuss food prices without mentioning one ([Ministry of Finance, 20 June 2025, interpellation 9699](https://api.sejm.gov.pl/sejm/term10/interpellations/attachment/ATTDHWHNG/i09699-o1.pdf); [Ministry of Development and Technology, 16 April 2025, interpellation 8798](https://api.sejm.gov.pl/sejm/term10/interpellations/attachment/ATTDFUF8P/i08798-o1.pdf)). A Polish trade outlet asked in May 2025 whether Poland would follow Croatia's and North Macedonia's daily price-list duties. No follow-up was found ([Wiadomości Handlowe, 6 May 2025](https://www.wiadomoscihandlowe.pl/prawo-i-polityka/kolejny-kraj-wprowadza-obowiazek-codziennego-publikowania-w-internecie-cen-ze-sklepow-stacjonarnych-wkrotce-pora-na-polske-2525456), headline only).

UOKiK (Urząd Ochrony Konkurencji i Konsumentów, the competition and consumer authority) acted on how Chains present and compare prices:

- **The right to compare prices (2018) [T2 via T4].** Customers complained that "Sprzedawcy nie pozwalają fotografować cen produktów i skanować kodów kreskowych" ("sellers do not allow photographing prices and scanning barcodes"). UOKiK asked 25 Chains for explanations, saying "konsument ma prawo porównywać ceny, zabranianie mu tego można uznać za nieuczciwą praktykę rynkową" ("the consumer has the right to compare prices; forbidding this may be considered an unfair market practice") ([Wiadomości Handlowe, 22 February 2018](https://www.wiadomoscihandlowe.pl/prawo-i-polityka/prawo-i-zmiany-legislacyjne/uokik-wystapil-do-25-sieci-handlowych-o-wyjasnienia-ws-zakazu-porownywania-cen-2420019)). The outcome is behind a paywall.
- **Shelf price integrity (2020) [T2].** UOKiK fined Jeronimo Martins Polska (Biedronka) PLN 115 m because checkout prices were higher than Shelf prices, and because "średnio aż 14 proc. towarów nie miało informacji o cenie" ("on average as many as 14% of goods had no price information"). The practice ran since at least 2016. The decision was open to appeal ([UOKiK, 10 August 2020](https://archiwum.uokik.gov.pl/aktualnosci.php?news_id=16663)).
- **A Chain's own price-match comparison (2022) [T2].** Biedronka's "Tarcza Antyinflacyjna" promised to refund the difference if 150 products were found cheaper elsewhere. UOKiK brought three charges, alleging the following:
  - the rules were hard to find;
  - shoppers had to buy at both Biedronka and the rival in the same week and mail the proofs;
  - only the most popular Chains counted as rivals;
  - the "refund" was an e-code valid for 7 days at Biedronka only ([UOKiK, 16 August 2022](https://archiwum.uokik.gov.pl/aktualnosci.php?news_id=18793)).
  No final decision was found.
- **"Cheapest basket" advertising (2024) [T2].** UOKiK opened preliminary investigations into the following campaigns ([UOKiK, 18 November 2024](https://uokik.gov.pl/en/biedronkas-promotional-campaigns-with-charges-of-the-president-of-uokik)):
  - Lidl's "Price Reviews in Lidl" campaign;
  - Biedronka's "I'm going to Biedronka to Get the Cheapest Full-of-Shopping Cart" campaign;
  - Eurocash franchise campaigns ("Low Prices Have No Owner").
  No outcomes were found.
- **Discount presentation (2025–2026) [T2].**
  - In September 2025 UOKiK charged Biedronka over "false discounts", where reductions were calculated from the regular price instead of the lowest price of the previous 30 days. Seven further investigations into stores were pending, including Aldi, Dino, Lidl and Żabka ([UOKiK, 9 September 2025](https://uokik.gov.pl/en/biedronkas-promotional-prices-under-investigation-by-the-president-of-uokik)).
  - In December 2025 it fined Biedronka nearly PLN 105 m over voucher promotions.
  - In April 2026 Biedronka and Lidl changed how discounts appear on checkout screens and receipts after UOKiK intervened ([UOKiK tag page, entries for 4 December 2025 and 2 April 2026](https://uokik.gov.pl/en/tag/biedronka); [UOKiK, 2 April 2026](https://uokik.gov.pl/en/discounts-or-puzzles-the-president-of-uokik-intervenes)).

**Reaction to a cross-country comparison [T2].** Two MPs cited prices of 7 products at international Chains in Poland and Germany. The ministry's answer, prepared with UOKiK, said the following ([Ministry of Development and Technology, 16 April 2025](https://api.sejm.gov.pl/sejm/term10/interpellations/attachment/ATTDFUF8P/i08798-o1.pdf)):

- **Method.** "porównania oparte na siedmiu obserwacjach, nie dają podstaw do wniosków" ("comparisons based on seven observations give no basis for conclusions"). The method was unknown: store selection, dates, promotions, and product positioning in each country.
- **Relevance.** Prices abroad matter little to Polish consumers, who cannot shop there without significant extra cost.
- **Legality.** Price differences across countries within one Chain do not break consumer law.
- **Price regulation.** It is unjustified in a market with "intensywnej konkurencji" ("intense competition").

This is the clearest statement found of how a state may receive a cross-country Basket that includes Germany.

#### Private and media Baskets

- **ASM SFA "Koszyk Zakupowy" [T4].**
  - **What it measures.** The same 40 popular products, "identyczne produkty tych samych marek i gramatur w 13 sieciach" ("identical products of the same brands and sizes in 13 chains"), across cash and carry, hypermarkets, supermarkets and discounters, in stores and online.
  - **July 2026.** The Basket cost from PLN 264.66 (Auchan) to PLN 344.62 (Aldi), 30.2% more. The average was PLN 317.29, against PLN 319.58 a year earlier. By format: cash and carry PLN 307.30, hypermarkets PLN 310.18, supermarkets PLN 315.02, discounters PLN 331.11 ([direct.money.pl, 13 August 2026](https://direct.money.pl/artykuly/porady/prawie-80-zl-roznicy-za-ten-sam-koszyk-w-tej-sieci-zakupy-kosztowaly-najmniej)).
  - **June 2026.** Auchan cut its Basket 9.10% month on month, and the average stood 2.91% above a year earlier ([Wiadomości Handlowe, 16 July 2026](https://www.wiadomoscihandlowe.pl/raporty-i-analizy-rynkowe/biedronka-i-lidl-podnosza-ceny-auchan-nokautuje-rywali-w-czerwcowym-koszyku-2536565)).
  - **Why discounters come out dearest.** A Basket of identical national brands leaves out the private labels that make up much of discounters' ranges. This is the same problem the project brief addresses with separate branded and private-label Baskets.
  - **Who runs it.** ASM Group says it supplies data and analysis to FMCG producers and Chains.
  - **App.** It launched a free "Koszyk Zakupowy" app with prices collected weekly at 13 Chains, and plans a user database "that FMCG companies and retail chains could also use" ([bank.pl, 18 July 2025](https://bank.pl/?p=522031)). No usage figures were published.
  - **Criticism.** In March 2023 the Chain Polomarket called the survey unreliable, with "brak transparentności" ("lack of transparency"). ASM replied "Nasze analizy są rzetelne, a metodologia wiarygodna" ("our analyses are reliable and our methodology credible") ([Wiadomości Handlowe, 17 March 2023](https://www.wiadomoscihandlowe.pl/handel-i-dystrybucja/hipermarkety-i-supermarkety/asm-odpowiada-na-zarzuty-sieci-polomarket-dotyczace-badania-i-raportu-koszyk-zakupowy-firma-nasze-analizy-sa-rzetelne-a-metodologia-wiarygodna-2448483)). The full method is behind paywalls.
- **Koszyk Faktu [T4].**
  - **Method.** The tabloid *Fakt* prices 25–26 everyday products in "wybranych losowo marketach" ("randomly selected stores") of Lidl, Biedronka, Dino and Lewiatan. It calls the Basket "forma dziennikarska" ("a journalistic format") that is not an inflation measure.
  - **Results.** In its January–June 2024 table, Lidl was cheaper than Biedronka every month, for example PLN 142.91 against PLN 144.20 in January.
  - **Method changes.** The article notes the item list changed: premium brands were swapped for cheaper ones ([Bankier, 13 June 2024](https://www.bankier.pl/wiadomosc/Mierzymy-inflacje-Koszykiem-Faktu-8765048.html)).
- **How Chains used them [T4].**
  - **Lidl.** After the March 2024 ASM Basket put Biedronka first and Lidl third, Lidl's spokesperson replied: "W tym roku już sześć razy koszyk zakupowy Lidla był najtańszy w opracowaniach 'Faktu'" ("this year Lidl's basket has already been the cheapest six times in Fakt's studies"). Lidl's leaflet carried the same claim ([Wiadomości Handlowe, 18 April 2024](https://www.wiadomoscihandlowe.pl/handel-i-dystrybucja/lidl-nie-rezygnuje-z-wyscigu-o-miano-najtanszej-sieci-handlowej-jak-siec-komentuje-wyniki-koszyka-asm-2508264)).
  - **Biedronka.** It published its own comparison of 20 identical products bought at Auchan, Dino and Lidl, which found itself cheapest ([Wiadomości Handlowe, 3 August 2023](https://www.wiadomoscihandlowe.pl/handel-i-dystrybucja/biedronka-zrobila-wlasne-porownanie-koszykow-sprawdzili-ceny-w-auchan-dino-i-lidlu-wynik-2486874)).
- **The "basket war" and trust [T4].** In March 2025 PAP reported analysts' views on the round of Chain-run basket comparisons ([eska.pl/PAP, 25 March 2025](https://www.eska.pl/wiadomosci/koniec-wojny-na-koszyki-eksperci-kwestionuja-wiarygodnosc-cenowych-porownan-sieci-handlowych-aa-Dack-cmr8-bU2Q.html)):
  - Piotr Biela of Grupa Blix said "klienci nie wierzą już nikomu" ("customers no longer believe anyone"), and that "wystarczy obrać odpowiednie zasady" ("it is enough to choose the right rules") to get a desired result.
  - Baskets of a dozen to several dozen products "nie daje rzetelnego obrazu" ("do not give a reliable picture").
  - He proposed comparing regular prices across the full shared range, private labels included, weighted by sales, with promotions compared separately.
  - ABR SESTA's own comparison had Biedronka cheaper than Lidl in 10 of 14 months (January 2024 – February 2025).
- **UCE Research and WSB Merito index [T4].**
  - **Method.** A monthly index of 100 frequently bought products in 17 categories, covering more than 103,000 prices from more than 47,300 stores of 64 Chains, including regular and promotional prices.
  - **July 2026.** It reported store prices up 1.9% year on year and food up 1.2%, against official CPI of 3% ([direct.money.pl, 11 August 2026](https://direct.money.pl/artykuly/porady/ceny-w-sklepach-wyhamowaly-do-1,9-proc-eksperci-ostrzegaja-przed-kolejnymi-miesiacami)).
  - **Limits.** It does not rank Chains, and its data source is not stated in the articles read.
- **Demand signals.** Leaflet apps such as Blix and Gazetkowo cover Biedronka, Lidl, Dino and others, with list and price-comparison features ([Blix, App Store](https://apps.apple.com/app/id1012288672); [Gazetkowo, App Store](https://apps.apple.com/pl/app/gazetkowo-gazetki-sklepowe/id1439014330)). No usage figures were found.

#### Social value in Poland

- **Price outcomes.** No evaluation found.
- **Shopper behaviour.** No data found.
- **Public discourse.** The monthly ASM and UCE releases are a steady press item [T4]. The Chain-run "basket war" reportedly eroded trust in all Basket claims [T4].
- **Policy.** UOKiK's interventions targeted how Chains present comparisons and discounts [T2], not the independent Baskets.
- **Truthfulness.**
  - ASM's brand-only Basket and Fakt's mixed Basket give opposite answers on whether discounters are cheap.
  - The state rejected a selective cross-border comparison as unscientific [T2].

### Germany

#### MTS-K: the first-hand evaluation (fuel)

The evaluation the ticket asks for is the federal government's report under § 47l of the Competition Act, written by the Federal Ministry for Economic Affairs and Energy (BMWi), not by the Bundeskartellamt. The ministry drew on the Bundeskartellamt's four annual MTS-K reports. It transmitted the report on 1 July 2018, and it was printed as Bundestag Drucksache 19/3693 on 3 August 2018 ([Drucksache 19/3693](https://dserver.bundestag.de/btd/19/036/1903693.pdf)). Page numbers below refer to that PDF.

- **Why it was created (pp. 2–3) [T2].** The Bundeskartellamt's 2011 fuel sector inquiry found five integrated oil companies forming a dominant oligopoly. It found no illegal agreements. Instead, it found that "die hohe Transparenz auf den Kraftstoffmärkten" ("the high transparency in fuel markets") let the companies observe prices everywhere and react quickly without agreements. The legislator's answer was transparency for consumers: real-time station prices passed to licensed apps. The plan to collect volume and wholesale data was dropped.
- **Data-feed licences (p. 9) [T2].** The legislator expected about 30 applications for licences to receive the data. More than 350 arrived (over 200 in 2013). About half were approved, and about 50 services were active. Applications that suggested the data might be passed to oil companies were refused.
- **Uptake (pp. 11–12) [T3].** A market research institute surveyed 1,001 people who pay for their own fuel, in late 2016:
  - About three-quarters had heard of fuel price apps and websites.
  - About a third had used one.
  - About a quarter used them "ständig bis gelegentlich" ("constantly to occasionally"). The report equates this to "mehreren Millionen" ("several million") consumers. Single providers reported unique users a month "bis in Richtung des Millionenbereichs" ("approaching the million range").
  - Younger people tried the apps more but used them less often than older people.
  - Almost 40% felt they had more reliable price information than three years earlier.
  - About two-thirds rated the information useful.
- **Behaviour (p. 18) [T3, self-reported].**
  - Almost three-quarters said they pay more attention to price than before.
  - About half would switch time or station for up to 5 ct/l; over three-quarters would do so for up to 10 ct/l.
  - About a quarter said they now generally fill up at other times of day, and about 15% at other stations.
- **Prices (pp. 1, 18, 21) [T2, citing T1].**
  - Prices "scheinen … im Wesentlichen der Entwicklung des Rohölpreises zu folgen" ("seem essentially to follow the crude oil price"), and holiday price hikes were no longer observed.
  - Daily price cycles had become more pronounced. The average gap between a station's daily high and low was about 10 ct/l, with about another 10 ct/l between stations in a city.
  - Two studies using largely the same data and methods reached opposite conclusions on the price level: Dewenter et al. 2017 found higher prices; Buchholz and Tode 2016 found no effect.
  - The report says capturing the savings "erfordert von den Verbrauchern erhöhte Aufmerksamkeit" ("requires heightened attention from consumers").
- **The industry uses the data (p. 13) [T2].**
  - "Die Daten werden aber immer für die eigene Preisgestaltung eingesetzt" ("the data are always used for companies' own pricing").
  - One chain with several hundred stations matched a cheaper nearby rival's price for drivers who showed a screenshot from a well-known app.
  - Software vendors sell competitor-price tools to small stations.
  - The ministry judged this hard to prevent without harming consumer information, and the Bundeskartellamt was "watching very closely".
- **Costs (pp. 8, 24–25) [T2].** The Bundeskartellamt uses about 6.5 full-time equivalents. Ex-ante estimates were €7.1 m one-off and €2.8 m a year for industry (by the Statistics Office), and €2.2 m one-off and €0.9 m a year for the Bundeskartellamt. The Statistics Office later re-measured the industry's running cost at about €1.5 m a year.
- **Conclusion (pp. 1–2) [T2].**
  - The monitor "hat die Transparenz für die Verbraucher erheblich erhöht" ("has considerably increased transparency for consumers").
  - But "Insgesamt ist es zu früh, um abschließende Aussagen zu den wettbewerblichen Auswirkungen treffen zu können" ("overall it is too early to make final statements on the competitive effects"), partly because volume data are missing.
  - It recommended continuing in the same form, re-evaluating after five more years, discussing powers to collect volume and wholesale data, and no price regulation.
- **Follow-up.** No second evaluation (due around 2023) was found. The academic evidence since then, including Montag et al. (prices fell 1–3%), Kahl and Wein (2026) and the 2026 noon rule, is summarised in the transparency note.

#### Groceries: demands for a state observatory, no portal

- **vzbv (federal consumer organisation) [T4].**
  - In August 2024 it published a feasibility study by Agrarmarkt Informations-Gesellschaft (AMI). The study found a price observatory along the food chain feasible, because much of the data already exists.
  - vzbv proposed housing the observatory at the federal agriculture and food agency (BLE). It would start with fresh staples and report to the Bundestag every year.
  - Its board member Ramona Pop said "Die Lebensmittelpreise gleichen einer Blackbox" ("food prices are like a black box") ([vzbv, 29 August 2024](https://www.vzbv.de/pressemitteilungen/hohe-lebensmittelpreise-politik-muss-fuer-transparenz-sorgen); [feasibility study PDF](https://www.vzbv.de/sites/default/files/2024-09/2024-08-29_Machbarkeitsstudie_Preisbeobachtungsstelle.pdf)).
  - It repeated the demand in January 2025 ([vzbv, 16 January 2025](https://www.vzbv.de/pressemitteilungen/gruene-woche-vzbv-fordert-mehr-verbraucherschutz-im-supermarkt)).
- **foodwatch Preisradar [T4].**
  - **Method.** Since May 2024 foodwatch has scanned the online shops of Rewe (one Cologne store), Edeka (one store) and Aldi Nord every day, for entry-level own brands and one branded comparator per category. Prices are per pack, promotions included.
  - **Lidl.** It is left out because "Lidl verfügt über keine umfassend online verfügbaren Preisdaten" ("Lidl has no comprehensively available online price data").
  - **Scope.** It says it "ist kein Einkaufsratgeber" ("is not a shopping guide") ([foodwatch Preisradar page](https://www.foodwatch.org/de/informieren/foodwatch-preisradar)).
  - **Findings at launch (14 January 2025).** The three Chains' own-brand yogurt cost €0.89 in June 2024, rose 6 cents together in July, and reached €0.99 by January 2025. Coffee moved from €4.29 to €4.79 at all three in July 2024.
  - **Demand.** foodwatch asked the next government to end "dem Preisgeheimnis der Handelsketten" ("the Chains' price secrecy") through a price observatory ([foodwatch, 14 January 2025](https://www.foodwatch.org/de/preisradar-fuer-mehr-transparenz-bei-aldi-rewe-co)).
  - **Response.** No Chain or regulator response to the Preisradar's findings was found.
- **Verbraucherzentrale NRW market check, 9 May 2023 [T4].**
  - **Method.** 19 staples in 20 branches of Edeka, Rewe, Aldi and Lidl in Düsseldorf, Cologne, Bonn, Münster and Essen, with current promotions included.
  - **Spread.** The dearest Basket cost €71.58 and a comparable one €34.78. Spreads exceeded 100% for 17 of 19 foods.
  - **Own brands.** These were often identical "auf den Cent genau" ("to the cent").
  - **Discounters.** They were not cheapest for every item ([VZ NRW factsheet, 31 May 2023](https://verbraucherzentrale.nrw/node/84747)).
  - **Lifespan.** It was a one-off; no repeat was found.
- **Stiftung Warentest on saving apps, April 2023 [T4, independent test].**
  - **Scope.** It tested 16 grocery saving apps, including marktguru, kaufDA and Smhaggle, and "Ein gutes Testurteil erreichte keine Anwendung" ("no app achieved a 'good' rating").
  - **Savings.** On a €55.59 family Basket, the best app saved €5.89 and the worst under €2.
  - **Accuracy.** Testers found about three of four promised offers in store and needed about three shops to collect them ([Tagesspiegel/AFP, 25 April 2023](https://www.tagesspiegel.de/wirtschaft/stiftung-warenttest-spar-apps-fur-lebensmittel-bringen-wenig-ersparnis-9717146.html)).
  - **Relevance.** This is the only independent quality test of German grocery Demand-signal apps found.
- **The Greens' proposal [T2 for the motion, T4 for reactions].**
  - In December 2025 the Green parliamentary leader Katharina Dröge proposed a mandatory price comparison app. Large supermarkets would report prices and changes in real time, and smaller ones could join voluntarily ([Tagesspiegel, 30 December 2025](https://www.tagesspiegel.de/wirtschaft/preise-experte-preisvergleichs-app-fur-lebensmittel-nicht-sinnvoll-15090280.html)).
  - The motion (Drucksache 21/6012) asks for "eine Preistransparenzstelle …, die vor plötzlichen Preissprüngen warnt" ("a price transparency office that warns of sudden price jumps"), a price comparison app, a duty for large supermarkets to report prices, and a cap on markups ([hib 442/2026, 1 June 2026](https://www.bundestag.de/presse/hib/kurzmeldungen-1183088)).
  - Its fate in committee was not found.
- **Reactions [T4].**
  - **Retail professor.** Markus Szajna (DHBW Karlsruhe) called the app "technisch überkomplex, ökonomisch ineffizient, bürokratisch belastend" ("technically overcomplex, economically inefficient, bureaucratically burdensome"). He argued it would add little to legally required unit prices and that its costs would reach shoppers ([Tagesspiegel](https://www.tagesspiegel.de/wirtschaft/preise-experte-preisvergleichs-app-fur-lebensmittel-nicht-sinnvoll-15090280.html)).
  - **Retail association (HDE), on foodwatch's observatory demand.** Deputy chief executive Stephan Tromp said it would contribute "zur weiteren Bürokratisierung des Wirtschaftslebens" ("to further bureaucratisation of economic life"). He added that Destatis statistics already make prices transparent and that retail margins are "zwischen einem und drei Prozent" ("between one and three percent") ([Lebensmittel Praxis, 14 March 2025](https://lebensmittelpraxis.de/handel-aktuell/43575-aufruf-an-kuenftige-bundesregierung-foodwatch-draengt-auf-massnahmen-gegen-hohe-lebensmittelpreise.html)).
  - **Agriculture minister.** In January 2026 Alois Rainer (CSU) rejected the SPD's idea of a legally required cheap staples basket ("Deutschlandkorb"): "Ich kann und will nicht in den Markt eingreifen" ("I cannot and will not intervene in the market") ([top agrar, 14 January 2026](https://www.topagrar.com/management-und-politik/news/rainer-lehnt-vorstoss-zu-gunstigem-grundnahrungsmittelkorb-ab-20022223.html)).
  - **Government.** No federal decision to create an observatory or portal was found.
- **Private apps.** Bonial (kaufDA, MeinProspekt) and marktguru dominate as Demand signals; see the Western note. Heisse Preise stopped updating its German feeds: Rewe Germany (15 February 2024), Müller Germany (3 March 2025) and DM Germany (29 July 2025) ([heisse-preise.io](https://heisse-preise.io/)). No German indie grocery Basket comparator with documented uptake was found.

#### Social value in Germany

- **Fuel (MTS-K) [T2, T3, T1].** Wide uptake and self-reported switching are documented. The ministry left price effects open in 2018. Later causal work finds small price falls (see the transparency note).
- **Groceries.**
  - No Comparable with measurable effects exists.
  - Consumer groups' work shaped the debate: the observatory demand, and evidence of lockstep own-brand pricing [T4]. It has not changed policy so far.
  - The Stiftung Warentest result is a caution about the accuracy of deal apps [T4].

### Austria

#### From a promised state calculator to an index without Chain prices

- **May 2023 [T2].** After sharp food inflation, ministers held a "Lebensmittelgipfel" (food summit) on 8 May 2023. On 10 May the government decided to strengthen competition law. Economy minister Martin Kocher held a round table on 12 May on "ob und wie eine Lebensmittelpreise-Transparenzdatenbank eingerichtet werden soll" ("whether and how a food price transparency database should be set up") ([BWB focus paper, September 2023, p. 5](https://www.bwb.gv.at/fileadmin/user_upload/Fokuspapier_Preisvergleichsplattformen_Sept_2023_barrierefrei_14.09.2023.pdf)). Kocher had announced a state tool for 16 staple foods ([Trending Topics, 18 September 2023](https://www.trendingtopics.eu/online-preisvergleiche-warum-derart-heftig-um-supermarktpreise-gekaempft-wird/)).
- **Volunteers moved first [T4].** Developers launched sites before the state tool existed: "Programmierer überholen Regierung mit Lebensmittel-Vergleichsportalen" ("programmers overtake government with food comparison portals") ([Der Standard, 2023](https://www.derstandard.at/story/3000000176002)).
  - **Heisse Preise.** Mario Zechner's repository was created on 8 May 2023 (GitHub data in the Western note). By his own account the first prototype took "wenigen Stunden" ("a few hours") ([BWB focus paper, p. 9](https://www.bwb.gv.at/fileadmin/user_upload/Fokuspapier_Preisvergleichsplattformen_Sept_2023_barrierefrei_14.09.2023.pdf)). By September 2023 it covered ten Austrian, two German and one Slovenian retailer, with price history from 2017 (p. 7). It credits historical data to the outlet Dossier and to @h43z ([heisse-preise.io](https://heisse-preise.io/)).
  - **The pattern Zechner reported.** He compared 40 own-brand product pairs at the two largest Chains: "Die Preise stimmten auf den Cent genau überein" ("the prices matched to the cent"). Changes followed within one to two days. He suspected tacit collusion ([Trending Topics, 18 September 2023](https://www.trendingtopics.eu/online-preisvergleiche-warum-derart-heftig-um-supermarktpreise-gekaempft-wird/)) [T4, developer claim].
- **BWB focus paper on comparison platforms, September 2023 [T2].** The BWB surveyed five platform operators: Heisse-Preise.io, Preismonitor.at, Preisrunter.at, Supermarkt.at and Teuerungsportal.at. They "werden … zur Zeit nur von Einzelpersonen betrieben" ("are currently run only by individuals") and are free to use (p. 7). Findings:
  - **Legal uncertainty (p. 8).** All operators named the unclear legality of web crawling. One Chain's terms required written consent for "jede Nutzung von Inhalten … insbesondere die Speicherung in Datenbanken" ("any use of content … in particular storage in databases").
  - **Data gaps (pp. 9–10).**
    - Products are hard to match across shops.
    - Some Chains list only promotional items online, and online ranges differ from store ranges.
    - Chains can block a crawler's IP address.
  - **Chains' error claims (p. 14).** The retail association (Handelsverband) sent spreadsheets of errors on two platforms. Branded goods were matched with discount own brands, promotional prices with regular prices, and wrong pack sizes compared. The BWB said all three errors "in Einzelfällen vorkommen" ("occur in individual cases").
  - **Assessment (pp. 15–16).** Price patterns across thousands of products suggest Chains "bereits jetzt vermehrt die Preise der Konkurrenz online crawlen" ("already increasingly crawl competitors' prices online") and set their own prices by algorithm. Information is therefore already asymmetric in sellers' favour. More consumer-side transparency "den Wettbewerb intensiviert" ("intensifies competition"), provided new rules do not ease automated exchange between Chains.
  - **Recommendation (pp. 18–20).** Chains with online shops, and perhaps all above a size threshold, should be required to provide a free, standardised API to a "qualifizierten Öffentlichkeit" ("qualified public"): comparison platforms, the BWB, consumer organisations and researchers. Other retailers "als Wettbewerber … explizit ausgeschlossen" ("explicitly excluded as competitors"). Required fields: EAN, name, manufacturer, brand, price, quantity, origin, offer flag, organic flag and category. Terms of service banning reuse would not apply. Platforms financed by Chains would raise independence concerns.
- **The state dropped its own tool [T4].** In September 2023 Kocher said he saw no need for an "amtliches Angebot" ("official offering") given the number of private calculators. He planned the API duty instead, with a bill "in den nächsten Wochen" ("in the coming weeks") and parliament by the end of 2023 ([ORF, 15 September 2023](https://orf.at/stories/3331293/)). The BWB's interim head cited the Israeli finding of 4–5% lower prices (same source). The grocery trade group in the Chamber of Commerce opposed a "Preis-Meldepflicht" ("price reporting duty") and warned of a "Preisspirale nach unten" ("downward price spiral") ([Trending Topics](https://www.trendingtopics.eu/online-preisvergleiche-warum-derart-heftig-um-supermarktpreise-gekaempft-wird/)).
- **BWB sector inquiry final report, 3 November 2023 [T2 via T4].** As reported by APA ([vol.at, 3 November 2023](https://www.vol.at/bericht-der-bundeswettbewerbsbehorde-zu-lebensmittelpreisen/8386885)):
  - Spar, Rewe (Billa, Penny), Hofer and Lidl held 91% of the market, against 76% for the top four in Germany.
  - Retail margins did not rise "systematisch" ("systematically").
  - Suppliers reported many unfair practices.
  - The BWB found no price-fixing.
  - A retailer's calculation put net prices 10–15% above Germany's. The BWB said it would raise this "Österreich-Aufschlag" ("Austria surcharge") with the European Commission.
- **The API law did not appear [T2, T4].** No bill was found.
  - In August 2025 the BWB's head, Natalie Harsdorf, still called for "einen klaren rechtlichen Rahmen" ("a clear legal framework") for comparison platforms. She said transparency measures could lower prices by "bis zu 4 Prozent" ("up to 4%"), citing only "international studies" ([vol.at/APA, 25 August 2025](https://www.vol.at/bwb-chefin-senkung-der-lebensmittelpreise-durch-mehr-transparenz/9626363)).
  - The Handelsverband's Rainer Will said price calculators or a price commission "würden lediglich den bestehenden Bürokratiedschungel noch verdichten" ("would only thicken the existing bureaucratic jungle"). He blamed manufacturers' territorial supply constraints instead (same source).
  - On 24 September 2025 the opposition Greens tabled a motion asking the government to give the BWB "die erforderlichen Kompetenzen und Ressourcen zur Erstellung einer Preisvergleichsplattform" ("the powers and resources needed to build a price comparison platform"). It noted that the cabinet's measures of 3 September 2025 ranged from "Erhöhung der Preistransparenz" ("more price transparency") to more inspections ([Entschließungsantrag 479/A(E) XXVIII. GP](https://www.parlament.gv.at/dokument/XXVIII/A/479/fname_1715283.pdf)).
- **Statistik Austria Preisradar, 19 January 2026 [T2].**
  - **Launch.** The finance ministry presented it as a response to the government's September measures. Minister Markus Marterbauer called it "ein wichtiger Schritt zu mehr Transparenz" ("an important step towards more transparency") ([BMF, 19 January 2026](https://bmf.gv.at/presse/pressemeldungen/2026/jaenner-2026/inflation-preisradar.html)).
  - **What it covers.** "Gut 100" ("a good 100") foods, at producer, wholesale and retail level, with product-group comparisons against Germany, Switzerland and the euro area ([ORF, 19 January 2026](https://orf.at/stories/3417575/)).
  - **Data and display.** Data come from weekly scanner data that "die größten Handelsketten" ("the largest Chains") have supplied since 2022, with checkout discounts included. Results appear as indices, average prices and price bands, not per Chain. The page was last updated on 16 October 2026 ([Statistik Austria Preisradar](https://www.statistik.at/preisradar/)).
  - **What it is not.** It is a cost-of-living tool, not a Comparable in the glossary sense: a shopper cannot use it to choose a Chain.
- **VAT cut and foodwatch Austria, 2026 [T4].**
  - From 1 July 2026, VAT on selected basic foods fell from 10% to 4.9%, at an estimated cost of about €400 m.
  - foodwatch Austria called the Preisradar "unvollständig, unübersichtlich, wenig benutzer:innenfreundlich" ("incomplete, confusing, not user-friendly"). It said Austria has "keine unabhängige Preisbeobachtungsstelle" ("no independent price observatory"). It reported that many BILLA and SPAR own-brand staples were priced identically "auf den Cent genau" ("to the cent") ([foodwatch Austria, 29 June 2026](https://www.foodwatch.org/at/eigenmarken-grundnahrungsmittel)).
  - At launch foodwatch had noted that half the foods named for the VAT cut were missing from the database ([ORF](https://orf.at/stories/3417575/)).

#### Consumer-body Baskets: the Chamber of Labour (AK)

- **AK Preismonitor, Vienna [T4].**
  - **Method.** AK records the cheapest available product, by unit price, for each of 40 foods and some cleaning products, in three Vienna branches each of Billa, Billa Plus, Spar, Interspar, Hofer, Lidl and Penny. A separate 31-item brand Basket is priced in the Billa and Interspar online shops.
  - **September 2026.** The cheapest-products Basket cost about €74, down 9% from "fast 82 Euro" ("almost €82"), a record, in September 2025. Brands rose 5.3%. Supermarkets were 11% dearer than discounters on average. Chains are named but not ranked ([AK Wien Preismonitor](https://wien.arbeiterkammer.at/preismonitor); [AK press release, 13 October 2026](https://wien.arbeiterkammer.at/service/presse/Preisalarm-Billige-Lebensmittel-so-teuer-wie-noch-nie-.html)).
  - **March 2026.** The Basket was 49% above its autumn 2021 level, according to AK's March 2026 edition as summarised in search results. That page was not opened, so this figure is unverified.
- **VAT pass-through check, July 2026 [T4].**
  - **Method.** AK computed target prices from Shelf prices collected 6–13 May 2026, excluding promotions. It compared them with prices from 6–14 July 2026: 576 prices, 78–95 products per Chain, seven Chains. Three Chains were checked online and four in three branches each.
  - **Result.** "alle geprüften Handelsketten geben die niedrigere Mehrwertsteuer komplett weiter" ("all Chains checked pass on the lower VAT in full"), and many cut prices further ([AK Wien, 23 July 2026](https://wien.arbeiterkammer.at/grundnahrungsmittel)).
  - **Limit.** It is a before-and-after reading with no control group. The Western note shows how such readings can mislead in either direction.
- **Austria–Germany identical-brand comparison [T4].**
  - **Method in 2024.** In May 2024 AK priced 70 identical branded foods at Billa and Interspar (Austria) and Rewe and Globus (Germany), online. Promotions were included; loyalty-card prices and volume discounts were not.
  - **2024 results.** 61 of 70 products were dearer in Austria. The Basket was about 24% dearer gross of VAT and about 21% net ([Salzburg24/APA, 1 June 2024](https://www.salzburg24.at/news/oesterreich/heimische-lebensmittelpreise-online-deutlich-ueber-deutschen-art-276890)).
  - **2021–2025 series.** AK's own net gap was 13.5% (2021), 8.8% (2022), 14.9% (2023), 20.6% (2024) and 23.2% (2025) ([AK factsheet, January 2026](https://wien.arbeiterkammer.at/interessenvertretung/eu/europa/eu-semester/Factsheet_Oesterreichaufschlag_DE_2026.pdf)).
  - **May 2026 edition.** Search summaries of AK's May 2026 study ([PDF](https://wien.arbeiterkammer.at/beratung/konsumentenschutz/einkaufundrecht/Online-Supermaerkte_Oe_und_D_202605.pdf), which returned an error when fetched) give 69 products, +25.5% gross and +21.6% net. These figures are unverified.
- **Policy reach [T4, AK's own account].**
  - AK says the European Commission's 2019 Semester country report cited its price surveys.
  - Austria's chamber of labour (BAK), the BWB and the grocery trade body raised the issue with the Commission in June 2024.
  - Parliament called on the government to act in November 2025.
  - Austria joined Belgium, Greece, Croatia, Luxembourg, the Netherlands, Slovenia and Czechia in an initiative against territorial supply constraints ([AK factsheet](https://wien.arbeiterkammer.at/interessenvertretung/eu/europa/eu-semester/Factsheet_Oesterreichaufschlag_DE_2026.pdf)).
  - The same factsheet cites VKI, the consumer association, for a 15–20% gap (November 2024).
  - Of the Comparables in this note, this one has the clearest line from a recurring Basket to policy, though the policy target is manufacturers' cross-border pricing, not Chains.

#### Social value in Austria

- **Price outcomes.** No causal evidence. The BWB's "up to 4%" figure is borrowed from Israel [T2 citing T1]. AK found the VAT cut passed through in full [T4].
- **Shopper behaviour.** No usage data was found for any Austrian Comparable or for the Preisradar.
- **Public discourse and policy.**
  - Volunteer sites changed the government's plan within four months, from a state calculator to an API duty, and drew a detailed BWB proposal [T2].
  - AK's cross-border Basket fed an EU initiative [T4].
  - The state's eventual output was an index without Chain prices [T2].
- **Harms.**
  - Chains documented matching errors on volunteer sites [T2].
  - Volunteer sites decayed: Heisse Preise stopped updating Hofer, Lidl and Penny in 2025, a loss for users who relied on them.
  - The BWB flagged the coordination risk if rules eased automated exchange between Chains, and proposed excluding competitors from the API [T2].
- **Truthfulness.** The Austria–Germany gap is real on identical brands, but its size depends on method, from 10–15% to 21–26% [T2, T4]. Retailers and AK attribute it to manufacturers, not to Chains.

### What the three countries add to the earlier findings

1. **States chose different levels of transparency.**
   - Hungary, Croatia and Bulgaria publish Chain-level prices (CEE note).
   - Austria publishes only indices, although its competition authority designed a Chain-level API duty.
   - Germany publishes Chain-level fuel prices but nothing for groceries.
   - Poland publishes nothing and polices claims instead.
2. **Cent-identical own-brand prices are the most repeated finding** of volunteers and consumer groups, in Austria (2023, 2026) and Germany (2023, 2025). The BWB attributes price alignment to algorithmic monitoring that is not itself illegal (focus paper, p. 16, note 4). No authority has found an agreement.
3. **The method decides the "cheapest Chain".**
   - In Poland a brand-only Basket ranks discounters dearest (ASM), while a mixed Basket ranks Lidl cheapest (Fakt).
   - This matches Slovenia's cheapest-to-dearest swing (CEE note) and Which?'s pre-2020 rankings without discounters (Western note).
4. **Discounters are hard to compare from outside.** Lidl publishes no full online prices in Germany (foodwatch), and in Austria some Chains list only promotional items online (BWB p. 10, Chains not named). Heisse Preise's Lidl, Penny and Hofer feeds stopped in 2025. Any scrape-based Comparable risks undercovering discounters.
5. **Cross-country comparisons are contested by whoever they embarrass.** UOKiK dismissed a selective Poland–Germany comparison. Austria's estimates of its gap with Germany span a factor of two. Chains and AK alike blame manufacturers for the gap.

## Gaps and uncertainties

- **Search budget.** The shared web-search budget was used sparingly. Several facts come from fetching known primary documents directly. Paywalls (Wiadomości Handlowe) hid most Polish methodology.
- **Poland.**
  - ASM SFA's full method is not published on pages read: store count, cities, treatment of promotions and Loyalty prices, start year. Its own site failed on a certificate error.
  - The data source of the UCE Research and WSB Merito index is not stated.
  - The outcomes of UOKiK's 2018 enquiry, the 2022 "Tarcza" charges and the 2024 preliminary investigations (Lidl "Price Reviews", Biedronka "cheapest full basket") were not found.
  - Polish consumer federations (Federacja Konsumentów, SKP) appear to run no Basket; one search found none.
  - dlahandlu.pl's "Koszyk cenowy" (2021; 50 products, 14 Chains, 6 cities per search snippets) was not opened, so its status is unknown.
  - No usage figures were found for Blix, Gazetkowo or the ASM app.
- **Germany.**
  - No second MTS-K evaluation was found. A May 2026 government answer (Drucksache 21/6169) reportedly mentions evaluation duties but was not opened.
  - The Bundesrat's 2018 statement on the evaluation was seen only in a search listing.
  - The fate of the Greens' motion 21/6012 and of an NRW state hearing on a price observatory (10 April 2025, seen only in a search listing) is unknown.
  - Whether the 2025 federal coalition agreement mentions a price observatory was not checked.
  - Stiftung Warentest's original report was read only through AFP coverage.
  - No Chain or Bundeskartellamt response to foodwatch's lockstep-pricing evidence was found.
- **Austria.**
  - No document was found stating why the 2023 API bill was never tabled.
  - The current status of Preismonitor.at, Preisrunter.at, Supermarkt.at and Teuerungsportal.at was not checked.
  - Heisse Preise publishes no reason for its stopped feeds (blocking, site changes or upkeep).
  - The Preisradar's cost, usage and list of reporting Chains are not published.
  - AK's May 2026 Austria–Germany figures and its March 2026 "+49% since 2021" figure come from search summaries; the AK PDF returned an error.
  - The BWB final report was read through APA coverage, not the report itself (its URL redirected).
  - The VKI comparison (November 2024) is known only through AK's citation.
- **Causal evidence.** None exists for any grocery Comparable in the three countries. The BWB's and politicians' price-effect figures borrow from Israel.

## Questions this raises

1. **Pricing discounters in Germany.** Lidl publishes no full online prices in Germany or Austria. How will the international Basket price Lidl and Aldi in Germany: in-store collection, Aldi Süd's online range, or leaving them out with a published caveat? This belongs with the data-collection tickets.
2. **Adopting AK's cross-country method.** Should the Romania–Germany comparison copy AK's design? That means identical branded items in named online shops on both sides, gross and net of VAT, promotions included and Loyalty prices excluded, and a yearly series. How should the index answer UOKiK's objection that prices abroad matter little to local shoppers? The brief's "minutes of work" framing may be the answer.
3. **Never crowning a "cheapest Chain" from a brand-only Basket.** ASM's results show such a Basket ranks discounters dearest. Should rankings require the private-label Basket alongside, or a combined rule?
4. **Wording for identical prices.** Should the index report cent-identical prices across Chains as a neutral fact, and how, given that no authority has found collusion and that Chains will read it?
5. **A claims policy before Chains cite the index.** Lidl Poland advertised its Fakt wins (2024). UOKiK has acted on "cheapest basket" claims, and Hungary requires a 2.5% gap. Should the index publish rules for Chains that cite it?
6. **Which access model to advocate in Romania.** The options are the BWB's "qualified public" API, which excludes competitors to limit coordination risk, and Croatia's fully open price lists (CEE note).
7. **A Romanian counterpart to AK or foodwatch.** Every lasting consumer Basket here sits in a funded statutory or member body. Who could play that role in Romania, as host or partner?
8. **Monitoring a tax change.** AK computed target prices from pre-change Shelf prices with promotions excluded. Should the index have this ready for any Romanian food VAT change, with a comparison group of uncovered products, which AK lacked?
9. **Evaluating the index itself.** The MTS-K evaluation combined a 1,001-person user survey, industry consultation and re-measured costs. Should the project plan a light version of this for its own Social value?
10. **Scope notes for the map.**
    - Poland has no state price data to reuse, so the "reuse terms of state price data" idea from the CEE note does not apply to it.
    - Austria's Preisradar cannot supply Chain-level prices.
    - Germany's only state price feed covers fuel.

## Sources

**Poland**

- UOKiK via Wiadomości Handlowe, request to 25 Chains on bans on photographing prices, 22 Feb 2018. https://www.wiadomoscihandlowe.pl/prawo-i-polityka/prawo-i-zmiany-legislacyjne/uokik-wystapil-do-25-sieci-handlowych-o-wyjasnienia-ws-zakazu-porownywania-cen-2420019
- UOKiK, "Prezes UOKiK nałożył 115 mln zł kary na Biedronkę", 10 Aug 2020. https://archiwum.uokik.gov.pl/aktualnosci.php?news_id=16663
- UOKiK, "Tarcza Biedronki Antyinflacyjna z zarzutami Prezesa UOKiK", 16 Aug 2022. https://archiwum.uokik.gov.pl/aktualnosci.php?news_id=18793
- UOKiK, "Biedronka's promotional campaigns with charges of the President of UOKiK", 18 Nov 2024. https://uokik.gov.pl/en/biedronkas-promotional-campaigns-with-charges-of-the-president-of-uokik
- UOKiK, "Biedronka's Promotional Prices Under Investigation", 9 Sep 2025. https://uokik.gov.pl/en/biedronkas-promotional-prices-under-investigation-by-the-president-of-uokik
- UOKiK, Biedronka tag page (entries 2023–2026). https://uokik.gov.pl/en/tag/biedronka
- UOKiK, "Discounts or puzzles? The President of UOKiK intervenes", 2 Apr 2026. https://uokik.gov.pl/en/discounts-or-puzzles-the-president-of-uokik-intervenes
- Ministry of Development and Technology, answer to interpellation 8798 (prepared with UOKiK), 16 Apr 2025. https://api.sejm.gov.pl/sejm/term10/interpellations/attachment/ATTDFUF8P/i08798-o1.pdf
- Ministry of Finance, answer to interpellation 9699, 20 Jun 2025. https://api.sejm.gov.pl/sejm/term10/interpellations/attachment/ATTDHWHNG/i09699-o1.pdf
- Wiadomości Handlowe, "Kolejny kraj wprowadza obowiązek codziennego publikowania w internecie cen…", 6 May 2025 (headline only). https://www.wiadomoscihandlowe.pl/prawo-i-polityka/kolejny-kraj-wprowadza-obowiazek-codziennego-publikowania-w-internecie-cen-ze-sklepow-stacjonarnych-wkrotce-pora-na-polske-2525456
- direct.money.pl, ASM SFA July 2026 Basket, 13 Aug 2026. https://direct.money.pl/artykuly/porady/prawie-80-zl-roznicy-za-ten-sam-koszyk-w-tej-sieci-zakupy-kosztowaly-najmniej
- Wiadomości Handlowe, ASM SFA June 2026 Basket, 16 Jul 2026. https://www.wiadomoscihandlowe.pl/raporty-i-analizy-rynkowe/biedronka-i-lidl-podnosza-ceny-auchan-nokautuje-rywali-w-czerwcowym-koszyku-2536565
- Wiadomości Handlowe, ASM replies to Polomarket, 17 Mar 2023. https://www.wiadomoscihandlowe.pl/handel-i-dystrybucja/hipermarkety-i-supermarkety/asm-odpowiada-na-zarzuty-sieci-polomarket-dotyczace-badania-i-raportu-koszyk-zakupowy-firma-nasze-analizy-sa-rzetelne-a-metodologia-wiarygodna-2448483
- Wiadomości Handlowe, Lidl comments on the ASM Basket, 18 Apr 2024. https://www.wiadomoscihandlowe.pl/handel-i-dystrybucja/lidl-nie-rezygnuje-z-wyscigu-o-miano-najtanszej-sieci-handlowej-jak-siec-komentuje-wyniki-koszyka-asm-2508264
- Wiadomości Handlowe, Biedronka's own Basket comparison, 3 Aug 2023. https://www.wiadomoscihandlowe.pl/handel-i-dystrybucja/biedronka-zrobila-wlasne-porownanie-koszykow-sprawdzili-ceny-w-auchan-dino-i-lidlu-wynik-2486874
- bank.pl, "Aplikacja Koszyk Zakupowy pokaże, w którym sklepie są najniższe ceny", 18 Jul 2025. https://bank.pl/?p=522031
- Bankier, "Mierzymy inflację Koszykiem Faktu", 13 Jun 2024. https://www.bankier.pl/wiadomosc/Mierzymy-inflacje-Koszykiem-Faktu-8765048.html
- eska.pl (PAP), "Koniec 'Wojny na Koszyki'? Eksperci kwestionują wiarygodność…", 25 Mar 2025. https://www.eska.pl/wiadomosci/koniec-wojny-na-koszyki-eksperci-kwestionuja-wiarygodnosc-cenowych-porownan-sieci-handlowych-aa-Dack-cmr8-bU2Q.html
- direct.money.pl, UCE Research and WSB Merito index, July 2026 reading, 11 Aug 2026. https://direct.money.pl/artykuly/porady/ceny-w-sklepach-wyhamowaly-do-1,9-proc-eksperci-ostrzegaja-przed-kolejnymi-miesiacami
- Forsal (PAP), UCE Research and WSB Merito index, June 2026 reading, 10 Jul 2026. https://forsal.pl/gospodarka/inflacja/artykuly/11274086,ceny-w-sklepach-czerwiec-2026-podwyzki-wyhamowaly.html
- Blix, App Store listing. https://apps.apple.com/app/id1012288672
- Gazetkowo, App Store listing. https://apps.apple.com/pl/app/gazetkowo-gazetki-sklepowe/id1439014330

**Germany**

- Bundesregierung (BMWi), "Bericht über die Ergebnisse der Arbeit der Markttransparenzstelle für Kraftstoffe und die hieraus gewonnenen Erfahrungen", Bundestag Drucksache 19/3693, 3 Aug 2018. https://dserver.bundestag.de/btd/19/036/1903693.pdf
- vzbv, "Hohe Lebensmittelpreise: Politik muss für Transparenz sorgen", 29 Aug 2024. https://www.vzbv.de/pressemitteilungen/hohe-lebensmittelpreise-politik-muss-fuer-transparenz-sorgen
- AMI for vzbv, feasibility study on a price observatory, Aug 2024. https://www.vzbv.de/sites/default/files/2024-09/2024-08-29_Machbarkeitsstudie_Preisbeobachtungsstelle.pdf
- vzbv, Grüne Woche press release, 16 Jan 2025. https://www.vzbv.de/pressemitteilungen/gruene-woche-vzbv-fordert-mehr-verbraucherschutz-im-supermarkt
- foodwatch, "Preisradar für mehr Transparenz bei Aldi, Rewe & Co.", 14 Jan 2025. https://www.foodwatch.org/de/preisradar-fuer-mehr-transparenz-bei-aldi-rewe-co
- foodwatch, Preisradar tool page. https://www.foodwatch.org/de/informieren/foodwatch-preisradar
- Verbraucherzentrale NRW, "Marktcheck zu Lebensmittelpreisen" factsheet, 31 May 2023. https://verbraucherzentrale.nrw/node/84747
- Tagesspiegel (AFP), Stiftung Warentest test of 16 saving apps, 25 Apr 2023. https://www.tagesspiegel.de/wirtschaft/stiftung-warenttest-spar-apps-fur-lebensmittel-bringen-wenig-ersparnis-9717146.html
- Tagesspiegel, "Experte: Preisvergleichs-App für Lebensmittel nicht sinnvoll", 30 Dec 2025. https://www.tagesspiegel.de/wirtschaft/preise-experte-preisvergleichs-app-fur-lebensmittel-nicht-sinnvoll-15090280.html
- Deutscher Bundestag, hib 442/2026, "Grüne fordern Initiativen gegen hohe Lebensmittelpreise" (Drucksache 21/6012), 1 Jun 2026. https://www.bundestag.de/presse/hib/kurzmeldungen-1183088
- Lebensmittel Praxis, HDE response to foodwatch, 14 Mar 2025. https://lebensmittelpraxis.de/handel-aktuell/43575-aufruf-an-kuenftige-bundesregierung-foodwatch-draengt-auf-massnahmen-gegen-hohe-lebensmittelpreise.html
- top agrar, "Rainer lehnt Vorstoß zu günstigem Grundnahrungsmittelkorb ab", 14 Jan 2026. https://www.topagrar.com/management-und-politik/news/rainer-lehnt-vorstoss-zu-gunstigem-grundnahrungsmittelkorb-ab-20022223.html
- Heisse Preise, live site (stopped feeds). https://heisse-preise.io/

**Austria**

- Bundeswettbewerbsbehörde, "Preisvergleichsplattformen im Lebensmittelsektor. Fokuspapier zur Branchenuntersuchung Lebensmittel", Sep 2023. https://www.bwb.gv.at/fileadmin/user_upload/Fokuspapier_Preisvergleichsplattformen_Sept_2023_barrierefrei_14.09.2023.pdf
- ORF, "Kocher: Lebensmittelpreise müssen gemeldet werden", 15 Sep 2023. https://orf.at/stories/3331293/
- Trending Topics, "Online-Preisvergleiche: Warum derart heftig um Supermarktpreise gekämpft wird", 18 Sep 2023. https://www.trendingtopics.eu/online-preisvergleiche-warum-derart-heftig-um-supermarktpreise-gekaempft-wird/
- Der Standard, "Programmierer überholen Regierung mit Lebensmittel-Vergleichsportalen", 2023. https://www.derstandard.at/story/3000000176002
- vol.at (APA), "Bericht der Bundeswettbewerbsbehörde zu Lebensmittelpreisen", 3 Nov 2023. https://www.vol.at/bericht-der-bundeswettbewerbsbehorde-zu-lebensmittelpreisen/8386885
- vol.at (APA), "BWB-Chefin: Senkung der Lebensmittelpreise durch mehr Transparenz", 25 Aug 2025. https://www.vol.at/bwb-chefin-senkung-der-lebensmittelpreise-durch-mehr-transparenz/9626363
- Nationalrat, Entschließungsantrag 479/A(E) XXVIII. GP (Greens), 24 Sep 2025. https://www.parlament.gv.at/dokument/XXVIII/A/479/fname_1715283.pdf
- BMF, Preisradar press release, 19 Jan 2026. https://bmf.gv.at/presse/pressemeldungen/2026/jaenner-2026/inflation-preisradar.html
- ORF, Preisradar launch, 19 Jan 2026. https://orf.at/stories/3417575/
- Statistik Austria, Preisradar (updated 16 Oct 2026). https://www.statistik.at/preisradar/
- foodwatch Austria, "Senkung der Mehrwertsteuer: foodwatch schaut Supermärkten bei Eigenmarken auf die Finger", 29 Jun 2026. https://www.foodwatch.org/at/eigenmarken-grundnahrungsmittel
- AK Wien, Preismonitor (September 2026 survey). https://wien.arbeiterkammer.at/preismonitor
- AK Wien, press release "AK Preismonitor: Billig-Lebensmittel günstiger, Marken teurer!", 13 Oct 2026. https://wien.arbeiterkammer.at/service/presse/Preisalarm-Billige-Lebensmittel-so-teuer-wie-noch-nie-.html
- AK Wien, VAT cut check, 23 Jul 2026. https://wien.arbeiterkammer.at/grundnahrungsmittel
- AK Wien, factsheet "Österreich-Aufschlag abschaffen", Jan 2026. https://wien.arbeiterkammer.at/interessenvertretung/eu/europa/eu-semester/Factsheet_Oesterreichaufschlag_DE_2026.pdf
- AK Wien, "Markenlebensmittel in österreichischen und deutschen Online-Supermärkten", May 2026 (PDF returned an error when fetched). https://wien.arbeiterkammer.at/beratung/konsumentenschutz/einkaufundrecht/Online-Supermaerkte_Oe_und_D_202605.pdf
- Salzburg24 (APA), AK Austria–Germany comparison, 1 Jun 2024. https://www.salzburg24.at/news/oesterreich/heimische-lebensmittelpreise-online-deutlich-ueber-deutschen-art-276890
- vienna.at, "Wiener AK-Preistest: Diese Lebensmittel sind billiger", 13 Oct 2026. https://www.vienna.at/wiener-ak-preistest-diese-lebensmittel-sind-billiger/10539959

**Earlier notes in this repository**

- CEE Comparables (ticket #3): `docs/research/cee-comparables.md` on branch `research/cee-comparables`
- Western Comparables (ticket #4): `docs/research/western-comparables.md` on branch `research/western-comparables`
- Transparency effects (ticket #5): `docs/research/transparency-effects.md` on branch `research/transparency-effects`
