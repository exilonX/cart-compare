# What did long-running Western basket indices and price apps achieve?

Ticket [#4](https://github.com/exilonX/cart-compare/issues/4), part of map [#1](https://github.com/exilonX/cart-compare/issues/1). Desk research, written 2026-10-21. Every figure carries the date its source gives. Terms follow the project glossary (`CONTEXT.md`): Comparable, Demand signal, Social value, Basket, Chain, Shelf price, Loyalty price.

**Evidence tiers** used to label claims, strongest first:

- **[T1 causal]**: peer-reviewed or working-paper studies with a control group.
- **[T2 regulator]**: regulator or court findings and evaluations.
- **[T3 usage]**: usage, membership or reach statistics.
- **[T4 media]**: media reports and the initiatives' or chains' own statements.

## Answer

- **The long-lived Comparables are consumer-association indices funded by member subscriptions, not by the index.** OCU (Spain) has offered its supermarket comparison since 1988; Which? (UK) publishes yearly results back to 2014 and a monthly ranking now; DECO PROteste (Portugal) has published a weekly Basket since January 2022. Each sits inside an organisation with roughly 250,000–500,000 paying subscribers. CHOICE's quarterly Basket (Australia, since 2024) is the exception: a government grant of A$1.1m over three years pays for it. [T3 usage, T4 media]
- **Indie price apps keep dying or decaying.** mySupermarket (UK, 2006–2020, venture-funded) closed. Trolley.co.uk (UK, 2021–) nearly closed in 2022 over a £28,800 data-licence bill; MoneySavingExpert funding and sponsors rescued it. Frugl (AU, around 2020) had about 40,000 users by 2022, and its website returned a server error on 2026-10-21. Heisse Preise (AT, open source, 2023) has lost 9 of its store feeds since February 2024. Project Hammer (CA, 2024–) still collects data daily but documents no users. [T3 usage, T4 media]
- **Media impact is high when the cadence is fixed and the output is one number.** The Portuguese news agency Lusa runs the weekly DECO Basket figure, and RTP, Renascença and ECO republish it. Which?'s monthly "cheapest supermarket" result is syndicated across UK regional titles. OCU's annual study makes national news each autumn. [T4 media]
- **Chains mostly react by using wins in their marketing and by contesting losses through regulators, not by suing the index.** Aldi UK issues a press release every month it wins the Which? title. Sainsbury's won a 2024 advertising ruling against an Aldi advert that used a Which? award. Portugal's retail association (APED) disputed the food-safety and economic regulator ASAE's 2023 findings on margins. I found no legal action against any consumer-group Basket. [T2 regulator, T4 media]
- **Causal evidence that price comparisons lower grocery prices exists, but none of it isolates these Comparables.** In Israel, a law making supermarket prices public, combined with media price surveys, cut price levels and price dispersion ([Ater & Rigbi 2023](https://ideas.repec.org/a/aea/aejmic/v15y2023i1p1-29.html)). In Portugal, the 2023 food VAT cut reached consumers in full, and the authors credit monitoring "by the Portuguese Association for Consumer Protection and major newspapers" as part of the reason ([Bernardino et al. 2025](https://doi.org/10.1016/j.jpubeco.2025.105416)). [T1 causal]
- **The clearest policy wins came from campaigns that used the price data, not from the rankings themselves.** In the UK, a Which? campaign led to a 2023 regulator (CMA) review and to unit-pricing rules in force from 6 April 2026. The CMA found in 2024 that 92% of Loyalty prices were genuine savings. In Australia, the competition regulator (ACCC) recommended in 2025 that chains publish prices online and give comparison tools access through APIs; the government agreed in principle in May 2026. [T2 regulator]
- **Several Comparables have told a distorted story through their method.** Which?'s "cheapest supermarket" for 2014–2019 left out Aldi and Lidl because their prices were not online. CHOICE's Aldi gap fell from about 25% (March 2024) to about 6% (March 2025) mostly because the Basket changed. Winners have been declared on gaps of 4p to 10p. Portugal's raw before-and-after Basket said the VAT cut had faded, while the causal study found it passed through in full and persisted. [T1 causal, T2 regulator, T4 media]
- **Harms deserve full weight.** In concentrated markets, publishing prices can help firms coordinate. Danish concrete prices rose 15–20% after a regulator published them. One study found German fuel prices rose after the state fuel-price unit launched. Loyalty prices shut out under-18s and people without smartphones (CMA). [T1 causal, T2 regulator]
- **Demand signal: the money in this space comes from retailers.** Bonial (kaufDA and MeinProspekt) reaches 14.4 million unique users a month in Germany (2024) and is paid by about 1,500 retailers and brands. Kaufino and Tiendeo both run Romanian sites that carry leaflets from most of the 8 Chains. [T3 usage, T4 media]

## Comparison at a glance

| Comparable | Country | Type | Running since | Cadence and Basket | Reach (dated) | Funding | Status, Oct 2026 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Which? cheapest supermarket | UK | Consumer-group index | Yearly results back to 2014; Aldi and Lidl only from 2020 | Monthly; 65–93 items drawn from a core list of about 200, plus a 180-item "big shop"; shows prices with and without loyalty cards | Which? had 500,063 members (June 2025) | Charity; income £83.7m in 2024/25, mostly subscriptions | Active |
| Trolley.co.uk | UK | Indie app | June 2021 | Item-level comparison; 160,000 products | 400,000 shoppers a month (June 2022); "over 1 million" (undated, page © 2023) | Sponsors and donations; a year of funding from MoneySavingExpert | Active |
| mySupermarket | UK | Venture-funded app | Oct 2006 | Swaps items in a shopper's basket for cheaper ones | "Tens of millions" of users over its life (own claim) | £3m (2007) and $10m (2012) venture rounds | Closed 1 Mar 2020 |
| DECO PROteste weekly Basket | PT | Consumer-group index | Jan 2022 | Weekly; fixed 63 foods; prices from online supermarkets | About 250,000 subscribers (undated); Lusa syndicates it weekly | Subscriptions are over 95% of revenue | Active; €256.26 (week to 14 Oct 2026) |
| OCU supermarket study | ES | Consumer-group index | Comparison tool since 1988 | Annual; 244 products, 690 stores, 101,520 prices (2026). Also a monthly 100-product observatory (2024) | National media every year | Member fees; about €0.55m in public grants listed for 2025 | Active; 2026 edition out 25 Sep 2026 |
| CHOICE quarterly Basket | AU | Consumer-group index, government-funded | Q2 2024 | Quarterly; fieldworkers price 81–104 stores in 27 locations; 8–17 items | A ministerial press release each quarter | A$1.1m federal grant over three years | Active; grant term ends around Q1/Q2 2027 |
| Frugl | AU | Commercial app | Around 2020 | Item comparison; about 60,000 products; Coles, Woolworths, Aldi, IGA and others | About 40,000 users (Feb 2022) | Planned to sell retail analytics to businesses | Website returned HTTP 500 on 21 Oct 2026; status unknown |
| Project Hammer | CA | Open dataset run by one person | 28 Feb 2024 | Daily web scrape of 8 Chains, plus Sobeys from 9 Oct 2026; Toronto store-pickup prices | No documented users | Not stated | Active; new data added daily |
| Heisse Preise | AT, with some German stores | Open-source app | May 2023 | Daily scrape | 1,039 GitHub stars | Volunteer | Decaying; 9 store feeds stopped between Feb 2024 and Nov 2025 |
| Bonial (kaufDA, MeinProspekt) | DE, FR | Leaflet aggregator (Demand signal) | 2008 | Digital leaflets | 14.4m unique users a month (2024) | Retailers and brands pay per performance | Active |
| Kaufino | 20 country sites, Romania included | Leaflet aggregator (Demand signal) | Not stated | Digital leaflets | Not published | Advertising (AdMob, Google Ads) | Active |
| Tiendeo (ShopFully) | 39 countries, Romania included | Leaflet aggregator (Demand signal) | Not stated | Digital leaflets | Not published | Marketing services for retailers (implied) | Active |

None of the Comparables reviewed here compares Baskets across countries; all are national.

## Detailed findings

### United Kingdom: Which? cheapest supermarket

**What it is.** Which? tracks prices daily at Aldi, Asda, Lidl, Morrisons, Ocado, Sainsbury's, Tesco and Waitrose "using an independent price comparison website". It averages each item over the month and adds the averages up for each store. The ranking includes special offers and, since June 2024, Loyalty prices; it excludes multibuys, points, personalised discounts and Asda Rewards cashback ([Which?, 9 Jan 2026](https://www.which.co.uk/policy-and-insight/article/aldi-crowned-cheapest-supermarket-of-the-year-which-reveals-af16x4l9jkFu); [Which? yearly results page, updated 5 Oct 2026](https://www.which.co.uk/news/article/which-was-the-cheapest-supermarket-in-2022-aulOn6x0ygaE)). The list changes size every month: 65 items in June 2024, 68 in December 2025, 93 in September 2026. Which? warns that totals "can't be compared between months or years because the product selection changes" ([yearly results page](https://www.which.co.uk/news/article/which-was-the-cheapest-supermarket-in-2022-aulOn6x0ygaE)). So it is a ranking, not a price index over time. [T4 media]

**Lifespan and results.** The yearly winners were Asda (2014–2016), Morrisons (2017–2018), Sainsbury's (2019), Lidl (2020), and Aldi every year from 2021 to 2025. Aldi also won every month from January to September 2026 ([yearly results page](https://www.which.co.uk/news/article/which-was-the-cheapest-supermarket-in-2022-aulOn6x0ygaE)). In 2025 Aldi won 10 months and Lidl 2, and Aldi was on average 77p a month cheaper than Lidl. In December 2025 the gap was £123.60 against £123.70: 10p on a 68-item list ([Which?, 9 Jan 2026](https://www.which.co.uk/policy-and-insight/article/aldi-crowned-cheapest-supermarket-of-the-year-which-reveals-af16x4l9jkFu)). [T4 media]

**Shelf price and Loyalty price.** Which? first left out Loyalty prices, because not every shopper can join a scheme. In October 2023 it found Sainsbury's dearer than Waitrose for shoppers without a Nectar card on a 131-item list (£359.23 against £355.51) ([Which?, 6 Oct 2023](https://www.which.co.uk/policy-and-insight/article/sainsburys-now-more-expensive-than-waitrose-for-customers-without-loyalty-card-which-finds-abaYL0e2pG9c)). From June 2024 it has shown both prices: "From this month on we will be regularly including loyalty prices in our analysis" ([Which?, 4 Jul 2024](https://www.which.co.uk/policy-and-insight/article/aldi-was-the-cheapest-supermarket-in-june-beating-other-supermarkets-loyalty-prices-which-reveals-azGak9C70LXO)). On the 180-item list in December 2025, the card mattered a lot: Tesco cost £462.00 with Clubcard and £493.53 without; Sainsbury's cost £468.61 with Nectar and £501.89 without. Only prices available to all shoppers count towards the "cheapest supermarket" endorsement ([Which?, 9 Jan 2026](https://www.which.co.uk/policy-and-insight/article/aldi-crowned-cheapest-supermarket-of-the-year-which-reveals-af16x4l9jkFu)). [T4 media]

**Did it tell the truth?** For 2014–2019 the "cheapest supermarket" was always a mainstream chain because "Prior to 2020, we were unable to include Aldi and Lidl in our analysis" ([yearly results page](https://www.which.co.uk/news/article/which-was-the-cheapest-supermarket-in-2022-aulOn6x0ygaE)). Discounters have won every year since they were added, so the earlier headlines most likely named the wrong winner. The cause was a coverage gap: the discounters' prices were not online. Separately, single winners have been declared on gaps of pennies (see the advertising ruling below). [T4 media; the inference is mine]

**How chains reacted.** Aldi uses the title in its own publicity: "We're proud to have been recognised as the UK's cheapest supermarket for the tenth consecutive month" ([Aldi UK press release, 3 Sep 2026](https://www.aldipresscentre.co.uk/?p=19273)). [T4 media] In March 2024 the advertising regulator (ASA) upheld a Sainsbury's complaint about an Aldi "Britain's cheapest Christmas dinner" advert that carried a Which? endorsement roundel. Which? had named both Aldi and Lidl "budget-friendly", with only 4p between them. The ASA said: "While Aldi was technically the cheapest, this was by a negligible amount" ([Grocery Gazette, 20 Mar 2024](https://www.grocerygazette.co.uk/2024/03/20/aldi-ad-christmas-misleading)). [T2 regulator] Which? said it was "disappointed that a Which? endorsement logo and our research was used in an advert" that broke the rules ([County Press/PA](https://countypress.co.uk/news/national/uk-today/24198333.aldi-cheapest-supermarket-advert-branded-misleading)). [T4 media]

**Policy and public discourse.** The bigger effect came from Which?'s pricing campaigns:

- **Unit pricing.** After a Which? campaign, the CMA reviewed unit pricing at 11 supermarkets and 7 variety retailers in July 2023, found problems at all of them, and asked the government to change the law ([Which?, 20 Jul 2023](https://www.which.co.uk/news/article/regulator-clamps-down-on-supermarket-pricing-following-which-campaign-ave4V6M3AhS2)). [T2 regulator, reported by Which?]
- **The law change.** The government amended the Price Marking Order to standardise units, require legible unit prices, and require unit prices for Loyalty prices and some multibuys. Which?'s petition had over 113,000 signatures ([Which?, 11 Nov 2024](https://www.which.co.uk/news/article/new-laws-to-make-supermarket-pricing-clearer-thanks-to-which-amawr4p4KBti)). A 2025 amendment moved the start from October 2025 to 6 April 2026 and widened which products are covered ([Lewis Silkin, 22 May 2025](https://www.lewissilkin.com/insights/2025/05/22/price-marking-update-another-price-marking-amendment-order-made-102kbul)). [T2 regulator]
- **Loyalty pricing.** The CMA's review of about 50,000 products on loyalty promotions found that "the overwhelming majority (92%)" offered genuine savings, averaging 17–25%. It also found 61 of 429 Loyalty-priced products were cheaper at another chain, and that "shoppers who are under 18 or without a smartphone are restricted from accessing loyalty prices at some supermarkets" ([CMA, 27 Nov 2024](https://gov.uk/government/publications/review-of-loyalty-pricing-in-the-groceries-sector/executive-summary)). Which?'s annual report says the CMA's loyalty-pricing guidance was "in line with our asks" ([Which? Annual Report 2024/25](https://media.product.which.co.uk/prod/files/file/gm-1ece30e6-0c1d-4839-85ff-dc37544931ae-ar-2025-1.pdf)). [T2 regulator]

**Funding.** Which? is the trading name of a group wholly owned by the Consumers' Association, a charity. Total income was £83.7m in 2024/25. Trading income was flat at £81.5m, with subscription income falling. Membership was 500,063 in June 2025, down 4.1% on the year. Non-subscription revenue (affiliates, switching, partnerships) rose to £21m ([Which? Annual Report 2024/25](https://media.product.which.co.uk/prod/files/file/gm-1ece30e6-0c1d-4839-85ff-dc37544931ae-ar-2025-1.pdf)). The supermarket ranking is a small product inside this machine and is not funded on its own. [T3 usage]

### United Kingdom: Trolley.co.uk, and the death of mySupermarket

**mySupermarket** launched in October 2006 and took prices from retailer websites. It raised £3m from Greylock and Pitango (2007) and $10m from WPP and others (2012). It closed on 1 March 2020; the company said it was shifting "toward other business areas" ([Wikipedia summary of company statements](https://en.wikipedia.org/wiki/MySupermarket); [Grocery Gazette, 7 Jul 2022](https://www.grocerygazette.co.uk/2022/07/07/supermarket-comparison-site/)). It gave no fuller public reason. [T4 media]

**Trolley.co.uk** was "launched by four volunteers" in June 2021 ([Trolley sponsors page](https://www.trolley.co.uk/our-sponsors/)), who were former mySupermarket staff ([Grocery Gazette, 29 Jun 2022](https://www.grocerygazette.co.uk/?p=33843)).

- **Near-closure.** By June 2022 the service had been used more than 11 million times by over 400,000 shoppers a month. That month it said it might close because it could not pay a licence fee for "certain data", and crowdfunded for £28,800 ([Grocery Gazette, 29 Jun 2022](https://www.grocerygazette.co.uk/?p=33843)). [T3 usage, T4 media]
- **Rescue.** Its sponsors page credits MoneySavingExpert. Martin Lewis is quoted: "we wanted to help, and hope the year's funding MSE's provided, will give the volunteer Trolley team time to get things in shape to thrive in future".
- **Costs and reach.** The page lists maintenance costs for "over 2.4 million price comparisons across 160,000 products every month", plus annual licences for product images. It says "Sponsors and donations are the only reason Trolley.co.uk is completely free to use", and claims it helps "over 1 million" shoppers. The page footer reads © 2023 ([Trolley sponsors page](https://www.trolley.co.uk/our-sponsors/)). [T3 usage, self-reported]
- **Chains.** I found no public reaction from any Chain to Trolley. The threat it faced came from data licensing, not from retailers.

### Portugal: DECO PROteste weekly Basket

**What it is.** DECO PROteste publishes the cost of 63 essential foods (meat, fish, dairy, fruit and vegetables, frozen and pantry items) every week. Its 2022 method note reads: "O custo do cabaz é obtido através do cálculo do preço médio por produto em todos os supermercados online, presentes no simulador da organização" ("The Basket cost is obtained by calculating the average price per product across all online supermarkets in the organisation's simulator") ([DECO PROteste, 3 Oct 2022](https://www.deco.proteste.pt/corporate/comunicados-de-imprensa/deco-proteste-revela-que-55-em-63-produtos-do-cabaz-essencial-aumentaram-de-preco)). Unlike Which?, it is a fixed-Basket time series. In the week to 14 October 2026 it cost €256.26, which is €68.56 (36.53%) more than at the start of 2022 ([RTP/Lusa, Oct 2026](https://www.rtp.pt/noticias/economia/cabaz-alimentar-volta-a-subir-e-ultrapassa-256-euros-na-ultima-semana_n1771652)). It reports an average across chains, not a ranking of Chains. [T4 media]

**Media impact.** The figure is a weekly news item. Lusa distributes it, and RTP, Renascença, ECO, DN and regional papers run it every Wednesday or Thursday (examples: [RTP, Oct 2026](https://www.rtp.pt/noticias/economia/cabaz-alimentar-volta-a-subir-e-ultrapassa-256-euros-na-ultima-semana_n1771652); [ECO, 2 Jul 2026](https://eco.sapo.pt/2026/07/02/preco-do-cabaz-alimentar-volta-a-baixar-e-custa-agora-25363-euros/); [dnoticias, 7 Oct 2026](https://www.dnoticias.pt/2026/10/7/508079-cabaz-alimentar-volta-a-subir-para-25556-euros-na-ultima-semana/)). It is the most repeatable media presence of any Comparable reviewed here. [T4 media]

**Policy: the 2023 zero-VAT measure ("IVA Zero").** Portugal set VAT to zero on 46 basic foods from 18 April 2023. DECO launched a campaign called "Cabaz Controlado" ("controlled Basket"): subscribers got weekly SMS price updates on the covered foods and could report shops that had not passed on the cut. DECO said it would forward justified reports to the authorities.

- **First day.** On 18 April, its 41-product Basket fell €4.66 against an expected €8.25. Of the 39 products whose price fell, "em 36 a quebra foi inferior aos 6 por cento de IVA esperados" ("in 36 the drop was smaller than the expected 6% VAT") ([DECO PROteste, 27 Apr 2023](https://www.deco.proteste.pt/familia-consumo/orcamento-familiar/noticias/deco-proteste-quer-garantir-iva-zero-carteira-consumidores)). [T4 media]
- **November 2023.** Renascença reported the Basket at €140.07, €1.30 above its level on the eve of the measure. DECO commented: "Há sempre muita rapidez quando é para subir preços, mas para os descer a velocidade não é a mesma" ("Prices always go up fast, but they don't come down at the same speed") ([Renascença, 16 Nov 2023](https://rr.pt/noticia/amp/explicador-renascenca/2023/11/16/cabaz-alimentar-mais-caro-do-que-antes-do-iva-zero-que-produtos-subiram-mais/355570/)). [T4 media]
- **The causal study.** A study with a control group used daily online prices from Portugal's main retailers. It found "the VAT cut was fully transmitted to consumer prices": 99.8% on impact, persistent, and symmetric when the cut ended. It estimates the measure cut inflation by 0.68 percentage points. Among its explanations, it notes that the policy was "continuously monitored by the Portuguese Association for Consumer Protection and major newspapers" ([SUERF Policy Brief 963, 29 Aug 2024](https://suerf.org/publications/suerf-policy-notes-and-briefs/can-a-temporary-vat-cut-bring-down-inflation); published as [Bernardino, Gabriel, Quelhas & Silva-Pereira, *Journal of Public Economics* 248, 2025](https://doi.org/10.1016/j.jpubeco.2025.105416)). [T1 causal]
- **Reading the two together.** DECO's November reading compared the covered Basket with itself before and after. That mixes the VAT cut with general food inflation. The study compared covered foods with uncovered ones and found the cut was passed on in full. The scrutiny DECO and the press applied may have helped deliver that result, which is real Social value. But the before-and-after Basket, read alone, pointed to the wrong conclusion about whether the cut reached shoppers. [T1 causal against T4 media; the interpretation is mine]

**How chains reacted.** I found no APED (Portuguese retail association) statement aimed at the DECO Basket. When ASAE reported margins above 50% on onions in March 2023, APED disputed it: distribution "é um negócio de volume e não de margem" ("is a business of volume, not of margin"). It put average margins at 2–3% and complained it "não tem conhecimento nem foi convidado a dar os seus contributos" ("had no knowledge of it and was not invited to contribute") ([Postal, 9 Mar 2023](https://postal.pt/economia/supermercados-contestam-asae-e-garantem-nao-ter-aumentado-margens-de-lucro/)). [T4 media]

**Funding.** "contando com cerca de 250 mil subscritores … [as subscrições] representam mais de 95% do total da faturação" ("with around 250,000 subscribers … subscriptions are over 95% of total revenue"). DECO PROteste says it takes no Portuguese state money; any public money comes only from EU projects ([DECO PROteste, funding page, undated, © 2026](https://www.deco.proteste.pt/info/os-nossos-servicos/fontes-de-financiamento)). The DECO association's 2026 activity plan calls financial sustainability "absolutamente prioritária" ("an absolute priority"), citing weaknesses in membership funding ([DECO, Plano de Atividades 2026](https://deco.pt/bfd_download/plano-de-atividades-2026/)). [T3 usage, self-reported]

### Spain: OCU supermarket study

**What it is.** OCU (Organización de Consumidores y Usuarios) runs an annual store-by-store study.

- **2026 edition** (published 25 September 2026): 101,520 prices for 244 products in 80 categories, from 690 stores and the main online supermarkets. It produces indices for 189 cities, weighted by household spending. "El ahorro anual medio en 2026 es de 1.310 €" ("the average annual saving in 2026 is €1,310"), about 20% of an average spend of €6,602. The cheapest Chains were Supermercados Dani, Family Cash, Tifer, Alcampo and Supeco; the dearest were the El Corte Inglés group (Hipercor, El Corte Inglés, Supercor, Sánchez Romero). The OCU Basket rose 1.8%, the smallest rise in five years ([OCU, 25 Sep 2026](https://www.ocu.org/organizacion/prensa/notas-de-prensa/2026/supermercados250926)).
- **2025 edition:** 106,320 prices in 718 stores; average saving €1,132 ([OCU, 24 Sep 2025](https://www.ocu.org/organizacion/prensa/notas-de-prensa/2025/supermercados240925)).
- **Lifespan.** OCU says it has offered the comparison "desde 1.988" ("since 1988"). This makes it the longest-running Comparable found.
- **Monthly observatory.** OCU also runs a monthly observatory of 100 products at 8 Chains ([OCU, 6 Nov 2024](https://www.ocu.org/organizacion/prensa/notas-de-prensa/2024/observatorioprecios061124)). [T4 media]

**Policy and public discourse.** OCU uses its price data to lobby. In April 2024 it reported that supermarket prices rose 38% from December 2020 to December 2023, "frente a poco más del 6% que lo hicieron los salarios" ("against little more than 6% for wages"). The base was 55,000 online prices for 122 products at seven Chains; Lidl and Aldi were left out because they had no online shop. OCU concluded that "la rebaja del IVA ha tenido un impacto limitado" ("the VAT cut had a limited impact") and asked for the cut to be kept and extended to meat and fish ([OCU, 3 Apr 2024](https://www.ocu.org/organizacion/prensa/notas-de-prensa/2024/preciossuper030424)). Three truthfulness problems apply:

- the wage figure has no source on the page;
- leaving out the online-less discounters is the same coverage gap Which? had;
- "limited impact" is a reading of raw trends with no control group.

The wider debate was heated. In March 2023 Mercadona's chairman Juan Roig said "Hemos subido una burrada los precios, tienen razón" ("we have raised prices enormously, they're right"). He said costs rose 12% and the chain passed 10% on to shoppers, while Podemos politicians attacked the chain ([El Español, 14 Mar 2023](https://elespanol.com/invertia/empresas/distribucion/20230314/juan-roig-admite-burrada-precios-mercadona-desastre/748425308_0.html)). [T4 media]

**How chains reacted.** I found no published Chain rebuttal of an OCU study. See the gaps section.

**Funding.** "La principal fuente de financiación de OCU son las cuotas de sus socios suscriptores" ("OCU's main source of funding is its subscribing members' fees"). Its 2025 transparency page lists public grants of about €0.55m to OCU itself, mostly Ministry of Consumer Affairs programmes (largest: €290,124), plus EU project funds to its publishing arm ([OCU transparency page](https://www.ocu.org/info/quienes-somos/transparencia)). [T3 usage, self-reported]

### Australia: CHOICE quarterly Basket and Frugl

**CHOICE.** CHOICE has been a non-profit member organisation since 1959 ([CHOICE](https://www.choice.com.au/about-us)).

- **Funding.** On 25 January 2024, alongside the ACCC supermarket inquiry, the government announced "$1.1 million to respected consumer group CHOICE to provide price transparency and comparison reports on a quarterly basis for three years", starting in the second quarter of 2024 ([Treasurer's release, 25 Jan 2024](https://ministers.treasury.gov.au/ministers/jim-chalmers-2022/media-releases/government-launch-accc-inquiry-supermarket-prices)). [T2 regulator]
- **First report** (data from March 2024): undercover shoppers visited 81 stores; Aldi's Basket was "about 25 per cent cheaper" than Coles' and Woolworths' ([Assistant Minister's release, 20 Jun 2024](https://ministers.treasury.gov.au/ministers/andrew-leigh-2022/media-releases/supermarket-price-monitoring-help-australians-make)).
- **A year later** (March 2025 data, 104 stores): Aldi cost $55.35 against $58.92 at Woolworths. The release says the gap narrowed because the Basket now held more fresh produce ([release, 25 Jun 2025](https://ministers.treasury.gov.au/ministers/andrew-leigh-2025/media-releases/supermarket-smarts-helping-shoppers-find-best-deals)).
- **Latest** (24 September 2026): an 8-item base Basket. Aldi was cheapest at $40.10; IGA rose 11% to $50.42 ([CHOICE, 24 Sep 2026](https://www.choice.com.au/about-us/media/media-releases/2026/september/latest-choice-supermarket-basket-research-reveals-price-rises-across-all-retailers-surveyed)). [T4 media]
- **Lesson.** The Basket keeps changing: 14 items for March 2025, 15 for June 2025, and an 8-item base Basket plus a 9-item "spotlight" Basket in September 2026. So the headline "how much cheaper is Aldi" mostly reflects which items were chosen.

**Policy.** The ACCC's final supermarkets report (released 21 March 2025) made 20 recommendations. Secondary summaries agree that one was to require Aldi, Coles and Woolworths to publish prices online, and Coles and Woolworths to give third parties, including comparison tools, live prices through APIs. The ACCC said this "could materially benefit consumers and competition" and would help "third-party price comparator businesses to develop effective models" that had relied on screen scraping ([Information Age, 24 Mar 2025](https://ia.acs.org.au/article/2025/supermarkets-should-publish-live-prices--accc.html)). [T2 regulator, via secondary; the ACCC site blocked automated retrieval]

In May 2026 the government said it agreed "in principle to the recommendations of that inquiry". It listed "funding CHOICE to give shoppers more information on supermarket prices" among its measures. It ran a consultation (20 January to 17 February 2026) "on proposals to improve transparency about prices, price trends, promotions and loyalty programs" ([Government response to the Senate Select Committee, May 2026](https://treasury.gov.au/sites/default/files/2026-06/p2026-779298.pdf)). [T2 regulator]

Separately, on 14 May 2026 the Federal Court found Coles misled shoppers with "Down Down" discounts. Higher "was" prices had been held for about four weeks, where the judge said shoppers would expect around 12 weeks. The Woolworths case was still pending ([Mediaweek, 14 May 2026](https://mediaweek.com.au/legal/coles-misled-shoppers-down-down-pricing)). [T2 court] This bears directly on the project's "is this discount real?" feature.

**Frugl.** By February 2022, Frugl had about 40,000 users "with no significant marketing spend". It compared about 60,000 products and had added Aldi, IGA, Drakes and Foodland to Coles and Woolworths. Its CEO said "the app simply collates public information available online" and "Frugl is a data analytics business"; the plan was to sell retail analytics to businesses ([Retailbiz, 23 Feb 2022](https://www.retailbiz.com.au/?p=38636); [Inside Retail, 2 Feb 2022](https://insideretail.com.au/sectors/frugl-grocery-unveils-a-new-version-with-advanced-features-202202)). [T3 usage, T4 media] On 2026-10-21, frugl.com.au returned HTTP 500 with a PHP dependency error (my own check). I found no closure notice, so its status is unknown.

### Canada: Project Hammer

Project Hammer's own page says: "Project Hammer aims to drive more competition and reduce collusion in the Canadian grocery sector." Its plan is to compile historical prices "for academic analysis and legal action" ([jacobfilipp.com/hammer](https://jacobfilipp.com/hammer/); [projecthammer.org](https://projecthammer.org/)).

- **Data.** Scraped daily from what websites display, as store-pickup prices for North York, Toronto (Save-On-Foods from Calgary). It starts on 28 February 2024, with only a small Basket until July 2024. It covers Voila, T&T, Loblaws, No Frills, Metro, Galleria, Walmart and Save-On-Foods, plus Sobeys from 9 October 2026 ([methodology](https://www.projecthammer.org/methodology.html); [get the data](https://www.projecthammer.org/get-the-data.html)).
- **Known problems.** It lists Walmart prices sometimes appearing 100 times too high, dropped multibuy prices, and duplicates ([methodology](https://www.projecthammer.org/methodology.html)).
- **Terms.** "You can use this data for whatever purposes you want." No funding source and no users are documented. Its resource page names a paid database with "essentially the same information … for more retailers and for a longer timespan" ([related resources](https://www.projecthammer.org/youre-not-alone.html)). [T4 self-reported]
- **Effect so far.** In June 2026 the Competition Bureau announced a review of food supply-chain competition, covering algorithmic pricing and shrinkflation; the reporting does not mention Project Hammer ([BNN Bloomberg, 16 Jun 2026](https://www.bnnbloomberg.ca/business/politics/2026/06/16/competition-bureau-to-examine-food-supply-chain-competition/)). I found no evidence that the dataset has been used by an academic, journalist or regulator. Social value: none measurable yet.

### Germany (and Austria)

I found no German consumer-group grocery Basket comparable to Which?, OCU or DECO; see the gaps section, since this search was cut short. The German examples found:

- **Heisse Preise** (Austria, open source; MIT licence) "fetches data from big Austrian grocery chains daily" ([GitHub](https://github.com/badlogic/heissepreise)). The repository was created on 8 May 2023, last pushed 17 February 2026, and has 1,039 stars ([GitHub API](https://api.github.com/repos/badlogic/heissepreise)). Its live site now warns "Folgende Stores werden nicht mehr aktualisiert" ("the following stores are no longer updated"). The feeds stopped one by one: Rewe Deutschland first (15 February 2024); then Unimarkt, Bipa and MPreis during 2024; then Müller and Müller Deutschland (3 March 2025), Lidl (27 March 2025), DM and DM Deutschland (29 July 2025), Penny (14 October 2025) and Hofer (10 November 2025). The historical data stays online ([heisse-preise.io](https://heisse-preise.io/)). This is the clearest case of a volunteer scraper slowly breaking down. The site does not say whether the cause was blocking or site changes. [T4 self-reported]
- **State fuel-price transparency (Markttransparenzstelle für Kraftstoffe, MTS-K).** Germany requires fuel stations to report prices, which apps then show. Using 27 European countries as controls, one study found that "both gasoline and diesel prices have increased" after the unit was introduced. Its explanation: stations "are also able to compare prices at almost no cost" ([Dewenter, Heimeshoff & Lüth, *Applied Economics Letters* 24(5), 2017](https://doi.org/10.1080/13504851.2016.1184371)). [T1 causal; one study, fuel rather than groceries]
- **Verbraucherzentrale Hamburg's "Mogelpackungsliste"** (shrinkflation list) has run for about 20 years, built from consumer reports. It has led to court wins against Sanella (Landgericht Hamburg) and Milka (Landgericht Bremen, under appeal) ([vzhh.de](https://www.vzhh.de/themen/mogelpackungen)). It is a price-integrity watchdog rather than a Basket. [T2 court, as reported by vzhh]
- **Leaflet and cashback apps.** kaufDA and MeinProspekt (Bonial, below) and marktguru (operated by marktguru Deutschland GmbH; leaflets plus cashback; TV-advertised) ([marktguru.de](https://www.marktguru.de/)) are the dominant consumer tools. They are Demand signals, not Comparables.

### Demand signal: leaflet aggregators

- **Bonial** (Berlin, "Teil der Axel Springer SE", meaning part of Axel Springer). kaufDA was founded in 2008; Bonial bought MeinProspekt in 2014. "Wir begeistern jeden Monat mehr als 14 Millionen Unique User" ("we delight more than 14 million unique users every month"); the 2024 figure is 14.4 million. It sells "individuelle Marketinglösungen für 1.500 namenhafte Einzelhändler" ("tailored marketing for 1,500 well-known retailers") ([Bonial company page](https://www.bonial.com/de/unser-unternehmen)). Advertisers pay "nur für die erbrachte Leistung" ("only for performance delivered") ([bonial.com](https://www.bonial.com/)). It operates in Germany and France only. [T3 usage, self-reported]
- **Kaufino** is run by Business Animals s.r.o. (Prague); its app publisher is Adsalva s.r.o. It has a Romanian site covering Lidl, Kaufland, Penny, Profi, Carrefour, Mega Image, Selgros, Auchan and others, and links to 19 other country sites. "Scopul nostru este de a ajuta utilizatorii să economisească timp și bani" ("our goal is to help users save time and money"). It runs on advertising: AdMob banners in the app, Google Ads and Facebook Pixel on the site ([about](https://www.kaufino.com/ro/despre-noi); [terms](https://www.kaufino.com/ro/termeni-si-date); [home](https://www.kaufino.com/ro/)). It publishes no usage figures. [T4 self-reported]
- **Tiendeo** is part of ShopFully (Shopfully Marketing S.L.U., Barcelona) and present in 39 countries. Tiendeo.ro lists leaflets from Lidl, Kaufland, Carrefour, Mega Image, Profi, Penny and Selgros, and says it is "accesată zilnic de mii de utilizatori" ("used daily by thousands of users") ([tiendeo.ro](https://www.tiendeo.ro/); [tiendeo.com](https://www.tiendeo.com/)). [T4 self-reported]
- **What this signals.** Interest in hunting grocery deals is large and long-lasting: Bonial has run for 18 years. But these businesses are paid by retailers or advertisers to send shoppers to stores. Both Romanian-facing aggregators already carry most of the 8 Chains, so local demand for leaflet browsing is evident. Neither publishes Romanian traffic.

### Cross-cutting: Social value and harms

**Price outcomes.**

- [T1 causal] In Israel, mandatory price publication cut price levels and dispersion. "These chains referenced price-comparison surveys conducted by the media to induce credibility for ads" ([Ater & Rigbi, *AEJ: Microeconomics* 15(1), 2023](https://ideas.repec.org/a/aea/aejmic/v15y2023i1p1-29.html)). That is the same pattern as Aldi publicising its Which? wins: comparisons become ammunition for low-price Chains.
- [T1 causal] Portugal's VAT cut passed through in full, with consumer-group and press monitoring cited as one reason ([SUERF 2024](https://suerf.org/publications/suerf-policy-notes-and-briefs/can-a-temporary-vat-cut-bring-down-inflation)).
- No causal study isolates the effect of Which?, OCU, DECO or CHOICE on prices.

**Shopper behaviour.** No evaluation found measures switching caused by these rankings. Reach figures (Which? 500k members, DECO 250k subscribers, Trolley 400k monthly users in 2022) are exposure, not behaviour change. [T3 usage]

**Public discourse and policy.** This is the strongest documented value:

- UK unit-pricing law, in force 6 April 2026, and CMA loyalty guidance [T2];
- Australian government funding for CHOICE and in-principle agreement to the ACCC's price-publication and API recommendation [T2];
- a weekly cost-of-living number in Portuguese news since 2022 [T4];
- OCU's VAT lobbying [T4].

**Harms.**

1. **Coordination risk.** [T1 causal] Published prices can soften competition in concentrated markets. When Denmark's competition authority published firm-level concrete prices from 1993, "average prices of reported grades increased by 15–20 percent within one year", which the authors attribute to publication letting firms ease off competing ([Albæk, Møllgaard & Overgaard, *Journal of Industrial Economics* 45(4), 1997](https://doi.org/10.1111/1467-6451.00057)). In Perth's fully transparent fuel market, dominant firms used price leadership "to create focal points that coordinate market prices, soften price competition, and enhance retail margins" ([Byrne & de Roos, *AER* 109(2), 2019](https://ideas.repec.org/a/aea/aecrev/v109y2019i2p591-619.html)). The risk is highest for real-time, per-product, store-level data. It is lower for a weekly aggregated Basket, but not zero.
2. **Marketing capture and overclaiming.** [T2 regulator] Winners are named on gaps of 4p to 10p and then used in adverts. The ASA called the gap behind one such claim "negligible".
3. **Exclusion.** [T2 regulator] Loyalty prices exclude under-18s and people without smartphones (CMA 2024), so a Shelf-price-only index understates what some shoppers pay less, while a Loyalty-price-only index overstates what others can get.
4. **Distorted results from method.** [T4 media] Coverage gaps (discounters with no online prices, at Which? before 2020 and at OCU in 2024) and Basket churn (CHOICE) moved headline results more than prices did.
5. **Fragility.** [T3 usage] Indie tools fail on data licences (Trolley), maintenance (Heisse Preise) or investor priorities (mySupermarket). Users who came to rely on them lose them.

**Did cost-of-living comparisons tell the truth?** Partly.

- Fixed-Basket series (DECO) track price levels well.
- Before-and-after Basket readings misattributed a policy effect: the causal Portuguese study disagrees with DECO's November 2023 reading.
- OCU compared a 38% price rise with an unsourced 6% wage figure.
- Rankings were most reliable once all major Chains were covered and both Shelf price and Loyalty price were shown (Which? from June 2024).

## Gaps and uncertainties

- **Search budget.** The shared web-search budget ran out partway through, before a full sweep of Germany and Austria. A German consumer-group Basket, an Austrian price-transparency law, or Arbeiterkammer (Austrian chamber of labour) price monitoring may exist and was not checked. Several facts below came from fetching known primary pages directly rather than searching.
- **Which? data supplier.** Which? names only "an independent price comparison company". Whether Chains pay to use the "cheapest supermarket" logo (a licensing income stream) was not confirmed.
- **DECO.** Whether the weekly Basket includes promotions and Loyalty prices is not stated in the sources read. Which supermarkets feed it is also not named in recent releases.
- **Chain reactions to OCU and DECO.** I found no Chain responses aimed at these Baskets. Absence of evidence is not evidence of absence; Spanish and Portuguese trade press were not searched in depth.
- **Frugl and Trolley today.** Frugl's current status is unknown (website erroring, no closure notice found). Trolley's "over 1 million" figure is undated (page © 2023).
- **The API recommendation.** Its exact wording and number in the ACCC report come from secondary summaries; the ACCC website blocked automated retrieval. The government's specific decision on it is not public beyond "agreed in principle" and the January 2026 consultation.
- **Romanian demand.** Neither Kaufino nor Tiendeo publishes Romanian usage figures.
- **Causal attribution.** No study isolates the effect of any of these Comparables on prices or behaviour. The Portuguese mechanism (monitoring as salience) is the authors' interpretation, not a separately tested effect.
- **Spain's VAT cut.** I did not verify a causal evaluation of the Spanish food VAT cut to set against OCU's "limited impact" claim.

## Questions this raises

1. **Fixed or rotating Basket?** A fixed Basket (DECO) gives a truthful time series. A per-month matched list (Which?) gives a fairer ranking but cannot be compared over time. Should the index publish both, and label which is which?
2. **Chains without online prices.** How will the index cover Chains that do not publish full prices online? Which?'s 2014–2019 rankings, and OCU's 2024 inflation study, both left out the discounters for this reason. This links to the data-access and terms-of-service tickets.
3. **When to name a winner.** What gap should be required before calling a Chain "cheapest"? What rules should apply when Chains quote the index in adverts? Which? lets only Shelf prices count towards its endorsement. Romanian comparative-advertising rules have not yet been checked.
4. **Who hosts it?** Every long-lived Comparable is hosted by a funded institution. Is there a Romanian consumer association, university or foundation that could host the index, or a grant like CHOICE's A$1.1m over three years? What would three years of weekly runs cost?
5. **Open data versus coordination risk.** Should raw per-product price history be published as open data, as Project Hammer does? That may help researchers, but it is the form of transparency the coordination studies warn about. Publishing only aggregated weekly Baskets lowers the risk.
6. **Built-in evaluation.** Can the project record publication dates and keep price history so that an independent researcher could later measure Chain responses? That would give a T1 answer to "did it help?", which none of the Western Comparables have.
7. **Policy effects.** How should the index report policy effects (for example a VAT change or price caps) without the before-and-after misreading DECO's IVA Zero tracking produced? Should it compare covered with uncovered products?

## Sources

**United Kingdom**

- Which?, "Aldi crowned cheapest supermarket of the year", 9 Jan 2026. https://www.which.co.uk/policy-and-insight/article/aldi-crowned-cheapest-supermarket-of-the-year-which-reveals-af16x4l9jkFu
- Which?, yearly cheapest-supermarket results 2014–2026 (page updated 5 Oct 2026). https://www.which.co.uk/news/article/which-was-the-cheapest-supermarket-in-2022-aulOn6x0ygaE
- Which?, "Aldi was the cheapest supermarket in June, beating other supermarkets' loyalty prices", 4 Jul 2024. https://www.which.co.uk/policy-and-insight/article/aldi-was-the-cheapest-supermarket-in-june-beating-other-supermarkets-loyalty-prices-which-reveals-azGak9C70LXO
- Which?, "Sainsbury's now more expensive than Waitrose for customers without loyalty card", 6 Oct 2023. https://www.which.co.uk/policy-and-insight/article/sainsburys-now-more-expensive-than-waitrose-for-customers-without-loyalty-card-which-finds-abaYL0e2pG9c
- Which?, "Regulator clamps down on supermarket pricing following Which? campaign", 20 Jul 2023. https://www.which.co.uk/news/article/regulator-clamps-down-on-supermarket-pricing-following-which-campaign-ave4V6M3AhS2
- Which?, "New laws to make supermarket pricing clearer, thanks to Which?", 11 Nov 2024. https://www.which.co.uk/news/article/new-laws-to-make-supermarket-pricing-clearer-thanks-to-which-amawr4p4KBti
- Which?, Annual Report and Financial Statements 2024/25. https://media.product.which.co.uk/prod/files/file/gm-1ece30e6-0c1d-4839-85ff-dc37544931ae-ar-2025-1.pdf
- CMA, "Review of loyalty pricing in the groceries sector: executive summary", 27 Nov 2024. https://gov.uk/government/publications/review-of-loyalty-pricing-in-the-groceries-sector/executive-summary
- Lewis Silkin, "Price marking update: another Price Marking Amendment Order made", 22 May 2025. https://www.lewissilkin.com/insights/2025/05/22/price-marking-update-another-price-marking-amendment-order-made-102kbul
- Aldi UK press centre, August 2026 result, 3 Sep 2026. https://www.aldipresscentre.co.uk/?p=19273
- Grocery Gazette, "Aldi's 'cheapest Christmas dinner' ad ruled 'misleading' by watchdog", 20 Mar 2024. https://www.grocerygazette.co.uk/2024/03/20/aldi-ad-christmas-misleading
- County Press (PA), "Aldi cheapest supermarket advert branded misleading", Mar 2024. https://countypress.co.uk/news/national/uk-today/24198333.aldi-cheapest-supermarket-advert-branded-misleading
- Grocery Gazette, "Trolley.co.uk on the brink of closure due to licensing issues", 29 Jun 2022. https://www.grocerygazette.co.uk/?p=33843
- Grocery Gazette, "Supermarket price comparison sites decline as cost-of-living intensifies", 7 Jul 2022. https://www.grocerygazette.co.uk/2022/07/07/supermarket-comparison-site/
- Trolley.co.uk, "Our Sponsors" (© 2023). https://www.trolley.co.uk/our-sponsors/
- Wikipedia, "MySupermarket" (secondary; cites company statements). https://en.wikipedia.org/wiki/MySupermarket

**Portugal**

- DECO PROteste, "55 em 63 produtos do cabaz essencial aumentaram de preço", 3 Oct 2022. https://www.deco.proteste.pt/corporate/comunicados-de-imprensa/deco-proteste-revela-que-55-em-63-produtos-do-cabaz-essencial-aumentaram-de-preco
- DECO PROteste, "Quer garantir IVA zero na carteira dos consumidores", 27 Apr 2023. https://www.deco.proteste.pt/familia-consumo/orcamento-familiar/noticias/deco-proteste-quer-garantir-iva-zero-carteira-consumidores
- DECO PROteste, funding sources page (undated, © 2026). https://www.deco.proteste.pt/info/os-nossos-servicos/fontes-de-financiamento
- DECO, Plano de Atividades 2026. https://deco.pt/bfd_download/plano-de-atividades-2026/
- RTP/Lusa, "Cabaz alimentar volta a subir e ultrapassa 256 euros na última semana", Oct 2026. https://www.rtp.pt/noticias/economia/cabaz-alimentar-volta-a-subir-e-ultrapassa-256-euros-na-ultima-semana_n1771652
- ECO, "Preço do cabaz alimentar volta a baixar e custa agora 253,63 euros", 2 Jul 2026. https://eco.sapo.pt/2026/07/02/preco-do-cabaz-alimentar-volta-a-baixar-e-custa-agora-25363-euros/
- dnoticias, "Cabaz alimentar volta a subir para 255,56 euros", 7 Oct 2026. https://www.dnoticias.pt/2026/10/7/508079-cabaz-alimentar-volta-a-subir-para-25556-euros-na-ultima-semana/
- Renascença, "Cabaz alimentar mais caro do que antes do IVA zero", 16 Nov 2023. https://rr.pt/noticia/amp/explicador-renascenca/2023/11/16/cabaz-alimentar-mais-caro-do-que-antes-do-iva-zero-que-produtos-subiram-mais/355570/
- Postal, "Supermercados contestam ASAE e garantem não ter aumentado margens de lucro", 9 Mar 2023. https://postal.pt/economia/supermercados-contestam-asae-e-garantem-nao-ter-aumentado-margens-de-lucro/
- Bernardino, Gabriel, Quelhas & Silva-Pereira, "Can a temporary VAT cut bring down inflation?", SUERF Policy Brief 963, 29 Aug 2024. https://suerf.org/publications/suerf-policy-notes-and-briefs/can-a-temporary-vat-cut-bring-down-inflation
- Bernardino, Gabriel, Quelhas & Silva-Pereira, "The full, persistent, and symmetric pass-through of a temporary VAT cut", *Journal of Public Economics* 248 (2025) 105416. https://doi.org/10.1016/j.jpubeco.2025.105416

**Spain**

- OCU, "Estudio de supermercados 2026", 25 Sep 2026. https://www.ocu.org/organizacion/prensa/notas-de-prensa/2026/supermercados250926
- OCU, "Estudio de supermercados 2025", 24 Sep 2025. https://www.ocu.org/organizacion/prensa/notas-de-prensa/2025/supermercados240925
- OCU, price observatory, 6 Nov 2024. https://www.ocu.org/organizacion/prensa/notas-de-prensa/2024/observatorioprecios061124
- OCU, supermarket prices 2020–2023, 3 Apr 2024. https://www.ocu.org/organizacion/prensa/notas-de-prensa/2024/preciossuper030424
- OCU, transparency page. https://www.ocu.org/info/quienes-somos/transparencia
- El Español, "Juan Roig admite 'una burrada' de precios", 14 Mar 2023. https://elespanol.com/invertia/empresas/distribucion/20230314/juan-roig-admite-burrada-precios-mercadona-desastre/748425308_0.html

**Australia**

- Treasurer, "Government to launch ACCC inquiry into supermarket prices", 25 Jan 2024. https://ministers.treasury.gov.au/ministers/jim-chalmers-2022/media-releases/government-launch-accc-inquiry-supermarket-prices
- Assistant Minister Leigh, "Supermarket price monitoring to help Australians make informed choices", 20 Jun 2024. https://ministers.treasury.gov.au/ministers/andrew-leigh-2022/media-releases/supermarket-price-monitoring-help-australians-make
- Assistant Minister Leigh, "Supermarket smarts helping shoppers find best deals", 25 Jun 2025. https://ministers.treasury.gov.au/ministers/andrew-leigh-2025/media-releases/supermarket-smarts-helping-shoppers-find-best-deals
- Assistant Minister Leigh, "New report helps Australians get a fairer deal at the checkout", 25 Sep 2025. https://ministers.treasury.gov.au/ministers/andrew-leigh-2025/media-releases/new-report-helps-australians-get-fairer-deal-checkout
- CHOICE, "Latest CHOICE supermarket basket research reveals price rises across all retailers surveyed", 24 Sep 2026. https://www.choice.com.au/about-us/media/media-releases/2026/september/latest-choice-supermarket-basket-research-reveals-price-rises-across-all-retailers-surveyed
- CHOICE, About us. https://www.choice.com.au/about-us
- Information Age (ACS), "Supermarkets should publish live prices: ACCC", 24 Mar 2025. https://ia.acs.org.au/article/2025/supermarkets-should-publish-live-prices--accc.html
- ACCC, Supermarkets inquiry 2024–25 final report page (blocked automated fetch). https://www.accc.gov.au/inquiries-and-consultations/finalised-inquiries/supermarkets-inquiry-2024-25/final-report
- Australian Government response to the Senate Select Committee on Supermarket Prices, May 2026. https://treasury.gov.au/sites/default/files/2026-06/p2026-779298.pdf
- Mediaweek, "Coles misled shoppers with Down Down pricing", 14 May 2026. https://mediaweek.com.au/legal/coles-misled-shoppers-down-down-pricing
- Retailbiz, Frugl version 3 coverage, 23 Feb 2022. https://www.retailbiz.com.au/?p=38636
- Inside Retail, "Frugl Grocery unveils a new version with advanced features", 2 Feb 2022. https://insideretail.com.au/sectors/frugl-grocery-unveils-a-new-version-with-advanced-features-202202

**Canada**

- Project Hammer, original post. https://jacobfilipp.com/hammer/
- Project Hammer, site home. https://projecthammer.org/
- Project Hammer, methodology. https://www.projecthammer.org/methodology.html
- Project Hammer, get the data. https://www.projecthammer.org/get-the-data.html
- Project Hammer, related resources. https://www.projecthammer.org/youre-not-alone.html
- BNN Bloomberg, "Competition Bureau to examine food supply chain competition", 16 Jun 2026. https://www.bnnbloomberg.ca/business/politics/2026/06/16/competition-bureau-to-examine-food-supply-chain-competition/

**Germany and Austria**

- Heisse Preise, GitHub repository. https://github.com/badlogic/heissepreise
- Heisse Preise, repository metadata (GitHub API). https://api.github.com/repos/badlogic/heissepreise
- Heisse Preise, live site. https://heisse-preise.io/
- Dewenter, Heimeshoff & Lüth, "The impact of the market transparency unit for fuels on gasoline prices in Germany", *Applied Economics Letters* 24(5), 2017. https://doi.org/10.1080/13504851.2016.1184371
- Verbraucherzentrale Hamburg, Mogelpackungen. https://www.vzhh.de/themen/mogelpackungen
- marktguru. https://www.marktguru.de/

**Leaflet aggregators (Demand signal)**

- Bonial, company page. https://www.bonial.com/de/unser-unternehmen
- Bonial, home page. https://www.bonial.com/
- Kaufino Romania, home. https://www.kaufino.com/ro/
- Kaufino Romania, about. https://www.kaufino.com/ro/despre-noi
- Kaufino Romania, terms. https://www.kaufino.com/ro/termeni-si-date
- Tiendeo, global site. https://www.tiendeo.com/
- Tiendeo, Romanian site. https://www.tiendeo.ro/

**Academic studies on price transparency**

- Ater & Rigbi, "Price Transparency, Media, and Informative Advertising", *AEJ: Microeconomics* 15(1), 2023. https://ideas.repec.org/a/aea/aejmic/v15y2023i1p1-29.html (DOI 10.1257/mic.20200337)
- Albæk, Møllgaard & Overgaard, "Government-Assisted Oligopoly Coordination? A Concrete Case", *Journal of Industrial Economics* 45(4), 1997. https://doi.org/10.1111/1467-6451.00057
- Byrne & de Roos, "Learning to Coordinate: A Study in Retail Gasoline", *American Economic Review* 109(2), 2019. https://ideas.repec.org/a/aea/aecrev/v109y2019i2p591-619.html
