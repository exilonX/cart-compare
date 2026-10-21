# Can we lawfully get prices for the comparison countries?

Research for ticket [#18](https://github.com/exilonX/cart-compare/issues/18) on map [#1](https://github.com/exilonX/cart-compare/issues/1). Desk research done on 2026-10-21. Terms (Basket, Chain, Shelf price, Loyalty price, Reported price, Comparable) follow the glossary in `CONTEXT.md`. This note builds on [#3](https://github.com/exilonX/cart-compare/issues/3) (CEE Comparables), [#6](https://github.com/exilonX/cart-compare/issues/6) (cross-country truth) and [#9](https://github.com/exilonX/cart-compare/issues/9) (legal exposure of collection in Romania). It does not repeat their findings. The EU framework (database right, *Ryanair*, text and data mining, Open Data Directive) is set out in [#9](https://github.com/exilonX/cart-compare/blob/research/legal-collection/docs/research/legal-collection.md).

> **Not legal advice.** This is desk research by a volunteer project. It maps the reuse terms, legal bases and enforcement history we could find. It does not conclude that any practice is lawful or unlawful. A lawyer has to confirm the approach for each country before any data is used (see [Questions for a lawyer](#questions-for-a-lawyer)). The project's standing rule is to avoid any unlawful action, so where the law is unclear this note leans towards the cautious reading.

**How the sources were read.** Each portal page, terms document and statute was fetched once, by hand, on 2026-10-21. No price data files were downloaded or opened: the Bulgarian daily archives were looked at only as a listing. Terms published as PDFs (Árfigyelő, Lidl Plus) were read as documents. posokanei.gov.gr answered automated requests with HTTP 403. We did not try to get past it, so PosoKanei's own terms remain unread. EUR-Lex, njt.hu and data.egov.bg also refused or dropped automated requests. Where a fact comes only from a search-result summary, the text says so.

## Answer

- **Croatia is the cleanest source; Bulgaria is next.** Croatian law obliges supermarkets, hypermarkets, discounters and cash-and-carry Chains to publish price files and to "omogućiti uporabu softverskih alata i automatiziranih programa" ("allow the use of software tools and automated programs") that collect the data for comparison. Fines run from €3,000 to €30,000 ([NN 40/25 art. 12(10), art. 20](https://www.zakon.hr/z/842/Zakon-o-iznimnim-mjerama-kontrole-cijena-)). Bulgarian law obliges large retailers to publish daily price lists on their own sites "в машинночетим формат, позволяващ извличане на данни" ("in a machine-readable format allowing data extraction"), and the KZP to republish all of it ([Euro Act art. 55б](https://elhovo-rs.justice.bg/upload/136279/Закон%20за%20въвеждане%20на%20еврото%20в%20РБ.pdf)). Neither law grants an explicit licence to republish.
- **Bulgaria's open data has no licence, and the portal reserves all rights.** kolkostruva.bg's footer reads "© 2025 Комисия за защита на потребителите. Всички права запазени!" ("All rights reserved") ([kolkostruva.bg/opendata](https://kolkostruva.bg/opendata)). Under Bulgaria's Access to Public Information Act, reuse is provided "след отправяне на писмено искане" ("after a written request"), and data subject to third-party IP or trade secrets is excluded ([ЗДОИ arts. 41е, 41б](https://www.ciela.net/svobodna-zona-normativi/view/2134929408/zakon-za-dostap-do-obshtestvena-informatsiya)). The duty is also time-limited. The text we read ties it to the dual-pricing period, which that text ends on 8 August 2026. The KZP says the duty runs to at least August 2027, so a 2026 amendment we have not read must exist.
- **Hungary's data is public by statute, but the GVH has acted against a reuser.** Act L of 2025 and the GVH's July 2025 terms say the non-archived data "nyilvánosak" ("are public"). The terms protect the system's software and design, and limit trademarked content to information use. We found no clause on automated access or reuse of prices ([ÁFF XII.4, XIV](https://arfigyelo.gvh.hu/docs/arfigyelo_rendszer_AFF_latogato.pdf)). In 2023 the GVH took "polgári és büntetőjogi lépéseket" ("civil and criminal steps") against a look-alike app. The app had copied the data and parts of the visual identity, and the GVH said its prices were wrong ([Telex, 2023-08-05](https://telex.hu/belfold/2023/08/05/gvh-figyelmeztetes-kalozapplikacio-arfigyelo)). Only same-day data is public, and the archive is closed to the public. Building history would therefore mean collecting daily. **Ask the GVH in writing first.**
- **Greece has a favourable open-data law, but PosoKanei's own terms are unread.** Law 4727/2020 makes public-sector documents reusable "ελεύθερα … για εμπορικούς ή μη εμπορικούς σκοπούς" ("freely … for commercial or non-commercial purposes") without a request. Documents subject to third-party IP or commercial secrecy are excluded ([art. 61(1), art. 59(4)](https://dsanet.gr/Epikairothta/Nomothesia/N4727_184.htm)). PosoKanei gets direct feeds from six Chains and itself crawls the e-shops of four others ([Skai, 2026-06-17](https://www.skai.gr/news/greece/nea-platfmorma-kata-tis-akriveias-ti-einai-to-posokanei-pos-leitourgei)). No reuse terms, API or open-data release was found. **Ask the ministry in writing.**
- **No state source covers all three Chains.**
  - **Lidl** is covered in all four state-data countries (in Bulgaria by the turnover threshold, not yet seen in the files).
  - **Kaufland** is covered only in Croatia and, by the threshold, Bulgaria.
  - **Penny** is covered only in Hungary. It left Bulgaria in 2015 and does not appear in the Croatian or Greek Chain lists.
  - So a Lidl comparison works across the four state-data countries, with Germany needing another route. A Kaufland or Penny comparison does not.
- **Matching by barcode works in Croatia, Hungary and probably Greece, but not in Bulgaria.** Croatian price files must carry a "barkod" ([NN 75/2025 point III](https://narodne-novine.nn.hr/clanci/sluzbeni/2025_05_75_979.html)). Hungary's statutory product data includes "a termék vonalkódja" ("the product's barcode"), but we did not check whether the public site exposes it. PosoKanei can be searched by barcode. Bulgaria's statutory fields are store, name, brand, net quantity, price and category, with no barcode. Bulgarian items would have to be matched by brand and size.
- **Germany has no lawful bulk source.**
  - **No state data.** Germany has no state grocery price data. A Greens motion of June 2026 asking for a "Preistransparenzstelle" (price transparency office) is a proposal only ([hib 442/2026](https://www.bundestag.de/presse/hib/kurzmeldungen-1183088)).
  - **Lidl Plus.** The terms limit participation to consumers "zum privaten Gebrauch" ("for private use"). They also say different user groups are likely to get "unterschiedliche Rabattsätze für dieselben Produktkategorie" ("different discount rates for the same product category") ([Lidl Plus terms v2.3, May 2026](https://www.lidl.de/static/assets/20260518_Teilnahmebedingungen_Lidl_Plus_v2-3-2219220.pdf)). A logged-in Lidl Plus price is therefore not one Loyalty price, and collecting it would breach the terms.
  - **Penny app.** Its terms ban "ein Kopieren, ein Extrahieren" ("copying, extracting") of app content ([Penny app terms, May 2026](https://www.penny.de/nutzungsbedingungen-penny-app)).
- **German law is relatively tolerant of collecting public pages while logged out.** The BGH held that ignoring terms that ban automated retrieval is "regelmäßig nicht" ("as a rule not") enough to make screen scraping unfair. Circumventing a technical protection measure can be different ([BGH I ZR 224/12, Rn. 35, 37](https://urteile-gesetze.de/rechtsprechung/i-zr-224-12)). Kaufland shows its Card XTRA price to logged-out visitors on its offers pages. Lidl shows offers only. So Germany can supply offer and Loyalty prices from public pages. A full Basket would need volunteers' in-store or receipt prices (for example via the ODbL-licensed Open Prices project) or a data agreement with the Chains.
- **Suggested order.**
  - Build the international Basket first from Croatian Chain files and Bulgarian statutory files.
  - Send written reuse requests to the KZP, the GVH and the Greek Ministry of Development.
  - For Germany, use only logged-out offer pages and volunteer-recorded prices, and ask Lidl, Kaufland and Penny for data.
  - Never collect logged in.

## Per-country findings

Read date for every row: **2026-10-21**. A dash means not found.

| Country / source | Legal basis | Licence or reuse terms (quote) | Restrictions and enforcement | Identifiers for matching | Chains covered (Lidl / Kaufland / Penny) | Update cadence | Link |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **Bulgaria**: KZP portal kolkostruva.bg, daily open-data ZIPs | Euro Act art. 55б(4): the KZP "създава и поддържа публично достъпен интернет портал и публикува ежедневно индивидуалните продажни цени и всички данни" ("creates and maintains a publicly accessible portal and publishes daily the individual sale prices and all data") ([text to ДВ 115/2025](https://elhovo-rs.justice.bg/upload/136279/Закон%20за%20въвеждане%20на%20еврото%20в%20РБ.pdf)) | No licence. Footer: "© 2025 Комисия за защита на потребителите. Всички права запазени!" ([opendata](https://kolkostruva.bg/opendata)). Default regime: written reuse request under [ЗДОИ art. 41е(1)](https://www.ciela.net/svobodna-zona-normativi/view/2134929408/zakon-za-dostap-do-obshtestvena-informatsiya) | No action against reusers found. Duty tied to the dual-pricing period (8 Aug 2025 – 8 Aug 2026 in [art. 15(2)](https://elhovo-rs.justice.bg/upload/136279/Закон%20за%20въвеждане%20на%20еврото%20в%20РБ.pdf)); the KZP says at least to 9 Aug 2027 ([#3](https://github.com/exilonX/cart-compare/blob/research/cee-comparables/docs/research/cee-comparables.md)) | Statutory fields (art. 55б(5)): store, product name, brand, net quantity, retail price, category, discount data. **No barcode.** Actual file columns not checked | Lidl ✓ and Kaufland ✓ expected (both far above the BGN 10 m threshold; the two largest retailers in 2024 per a [Capital](https://www.capital.bg/biznes/kompanii/2025/12/09/4840601_klasaciiata_k100_nai-golemite_riteiluri_prez_2024_g/) search summary). Penny ✗ (left Bulgaria in 2015, [Capital](https://www.capital.bg/biznes/kompanii/2015/09/17/2612126_penny_osvobojdava_pazar_za_200_mln_lv/), search summary) | Daily; ZIPs listed for 07.10–20.10.2026 | [kolkostruva.bg/opendata](https://kolkostruva.bg/opendata) |
| **Bulgaria**: Chains' own price lists | Euro Act art. 55б(1): publish "ежедневно до 7.00 часа в машинночетим формат, позволяващ извличане на данни" ("daily by 7:00, in a machine-readable format allowing data extraction"), per store where prices differ (art. 55б(3)) | The statute contemplates extraction. Each Chain's site terms were not read | – | Same statutory fields as above | Same as above | Daily by 07:00 | [Euro Act](https://elhovo-rs.justice.bg/upload/136279/Закон%20за%20въвеждане%20на%20еврото%20в%20РБ.pdf) |
| **Croatia**: Chains' price files | [NN 40/25 art. 12](https://www.zakon.hr/z/842/Zakon-o-iznimnim-mjerama-kontrole-cijena-); decision [NN 75/2025](https://narodne-novine.nn.hr/clanci/sluzbeni/2025_05_75_979.html), replaced from 17 Nov 2026 by NN 101/26 ([RRiF](https://www.rrif.hr/odgada_se_primjena_odluka_o_isticanju_i_objavi_dod-2533-vijest/)) | Statutory permission to collect: the trader "dužan [je] omogućiti uporabu softverskih alata i automatiziranih programa" ("must allow the use of software tools and automated programs") "radi njihove usporedbe" ("for their comparison") (art. 12(10)). Also NN 75/2025 point V. No clause on republication | Duty enforced against traders (fines €3,000–30,000, art. 20). No action against reusers found | NN 75/2025: name, code, brand, net quantity, unit, retail price, unit price, **barcode**, category. NN 101/26 adds the anchor price and lists the barcode "if applicable" ([Fiskalopedija](https://fiskalopedija.hr/baza-znanja/objava-cjenika-na-web-stranici)) | Lidl ✓, Kaufland ✓ (both crawled by cijene-api). Penny ✗ (not among the 29 Chains crawled) | Daily by 08:00 (NN 75/2025); "at each change" under NN 101/26 | [NN 75/2025](https://narodne-novine.nn.hr/clanci/sluzbeni/2025_05_75_979.html) |
| **Croatia**: cijene-api / cijene.dev (third party) | Built on NN 75/2025 ([README](https://github.com/senko/cijene-api)) | Code: "licenciran pod AGPL-3 licencom" ("licensed under AGPL-3"). Processed product CSVs "dostupni su pod CC BY-NC-SA licencom" ("available under CC BY-NC-SA"). Hosted API: "komercijalnu (uz pretplatu) i nekomercijalnu (besplatnu) upotrebu" ("commercial (paid) and non-commercial (free) use") | AGPL obliges us to publish source if we run a modified version as a network service. NC limits the processed data to non-commercial use | Whatever the Chains publish (barcode included in raw files) | 29 Chains incl. Lidl, Kaufland | Daily | [GitHub](https://github.com/senko/cijene-api) |
| **Hungary**: GVH Árfigyelő | Act L of 2025, chapter V; GFM decree 11/2023 ([GVH FAQ, July 2025](https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf); [Act L of 2025](https://net.jogtar.hu/jogszabaly?docid=a2500050.tv)) | Visitor terms (in force 20 July 2025), accepted "ráutaló magatartással" ("by conduct", VI.1). Data: "az abban nyilvántartott, nem archivált adatok nyilvánosak" ("the non-archived data recorded in it are public", XII.4). The system and site are under copyright (XIV.1). Trademarked content may be used "kizárólag a Honlap céljával összhangban (tájékozódás, tájékoztatás)" ("only in line with the site's purpose (information)", XIV.2) ([ÁFF](https://arfigyelo.gvh.hu/docs/arfigyelo_rendszer_AFF_latogato.pdf)). No licence | 2023: civil and criminal steps against a look-alike app that used the data and visual identity without permission ([Telex](https://telex.hu/belfold/2023/08/05/gvh-figyelmeztetes-kalozapplikacio-arfigyelo)); outcome not found. The archive is open only to ministries, courts, the consumer authority and the KSH, and is deleted after 10 years (ÁFF XII.5) | Statutory product data includes the **barcode** ("a termék vonalkódja", ÁFF IV.18; Act L § 55 pt 7). Daily price, previous price and Loyalty price, per Chain and store. Whether the public site shows the barcode was not checked | Lidl ✓, Penny ✓ (both mandatory reporters). Kaufland ✗ (not on the list) ([FAQ](https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf)) | Daily; public only on the day it applies to | [arfigyelo.gvh.hu](https://arfigyelo.gvh.hu/) |
| **Greece**: PosoKanei (successor of e-katanalotis) | Supermarkets above €90 m turnover must report prices daily under a 2021 bill ([iefimerida, 2021-04-06](https://www.iefimerida.gr/oikonomia/e-katanalotes-platforma-me-sygkrisi-timon)); enacted law not verified. Reuse: [Law 4727/2020](https://dsanet.gr/Epikairothta/Nomothesia/N4727_184.htm) | PosoKanei terms unread (HTTP 403). Open-data law: reuse "δεν υπόκειται σε όρους, εκτός αν οι όροι αυτοί είναι αντικειμενικοί…" ("is not subject to conditions unless they are objective…", art. 66(1)) | No action against reusers found. PosoKanei itself crawls the e-shops of Sklavenitis, Chalkiadakis, My Market and Kritikos ([Skai](https://www.skai.gr/news/greece/nea-platfmorma-kata-tis-akriveias-ti-einai-to-posokanei-pos-leitourgei)) | Search "με το barcode" ("by barcode"); about 10,000 product codes; price history | Lidl ✓ (direct feed). Kaufland ✗, Penny ✗ (not among the 10 Chains) | Daily | [posokanei.gov.gr](https://posokanei.gov.gr/) (e-katanalotis.gov.gr redirects there) |
| **Germany** | None | – | See [Germany](#germany) | – | – | – | – |

### Notes by country

**Bulgaria.**
- The Euro Act gives two routes to the same data: the KZP portal (art. 55б(4)) and each Chain's own website files (art. 55б(1)). The second route is closer to Croatia's model, because the statute itself requires a format "allowing data extraction".
- The open-data page offers one ZIP per day "for all retail chains that submitted information". It shows no field list and no licence ([opendata](https://kolkostruva.bg/opendata)). The About page names the legal basis and the threshold, "с оборот за предходната финансова година над 10 000 000 лв." ("with turnover in the previous financial year above BGN 10,000,000") ([about](https://kolkostruva.bg/about)).
- ЗДОИ (last amended ДВ 55/2026, per the [Ciela text](https://www.ciela.net/svobodna-zona-normativi/view/2134929408/zakon-za-dostap-do-obshtestvena-informatsiya)) provides for:
  - reuse "за търговски или нетърговски цели" ("for commercial or non-commercial purposes") (art. 2а(1));
  - standard licences (art. 41а(5));
  - reuse "безусловно или при определени от тях условия" ("unconditionally or under conditions they set") (art. 41а(6)).
- Data whose reuse is excluded includes "обект на право на интелектуална собственост на трето лице" ("subject to a third party's IP right") (art. 41б(1)(3)) and trade or professional secrets (art. 41б(1)(8)). A Chain could invoke either, although the Chains publish the same data on their own sites by law.

**Croatia.**
- The Act's art. 12(10) is the only provision in the four countries that expressly permits automated collection.
- The new decision NN 101/26 extends publication to all retailers and service providers with a website. Fiskalopedija's summary (updated 2026-10-20) says the exact CSV/XML structure is not yet prescribed, and a draft of 15 October 2026 would change the timing ([Fiskalopedija](https://fiskalopedija.hr/baza-znanja/objava-cjenika-na-web-stranici)).
- NN 101/26 repeals the NN 75/2025 publication provision ([informator.hr](https://informator.hr/podzakonski-propisi/842580)). The Act's own duty to allow automated collection is unaffected.
- **Two ways to use the data:**
  - **Self-host the AGPL crawler against the Chains' files.** Our licence obligation is to publish our source, which an open-source project does anyway.
  - **Use cijene.dev's processed data.** It is CC BY-NC-SA, and the hosted API is free only for non-commercial use.

**Hungary.**
- **What the terms leave open.** The visitor terms bind by conduct. They say anyone may use the Service, and that the data are public. They contain no clause on bots, copying or reuse of prices ([ÁFF](https://arfigyelo.gvh.hu/docs/arfigyelo_rendszer_AFF_latogato.pdf)).
- **What the GVH objected to in 2023.** The app was "az Árfigyelőre megtévesztésig hasonlító" ("deceptively similar to Árfigyelő"). The GVH also opened a consumer-deception proceeding ([Telex](https://telex.hu/belfold/2023/08/05/gvh-figyelmeztetes-kalozapplikacio-arfigyelo)). A civic index that names its source, uses no GVH branding and shows Basket totals differs from that case. The GVH's choice of words, though ("illetéktelen, engedély nélküli felhasználása", "unauthorised, unlicensed use"), suggests it expects permission to be asked.
- **Database right.** Árfigyelő publishes only same-day data. A history would require daily collection, which is the "repeated and systematic" extraction pattern discussed in [#9](https://github.com/exilonX/cart-compare/blob/research/legal-collection/docs/research/legal-collection.md). It matters if the GVH holds a database right in the system.
- **The data are prices the Chains report to the state** (the Hungarian analogue of a Reported price). The law fines a Chain HUF 50,000 per product whose Shelf price is higher than its Árfigyelő price (ÁFF XIII.2).
- **Prices shown.** For its ranking, the site uses the price "a kereskedő üzleteinek 80%-ában alkalmazott" ("applied in 80% of the trader's stores"). It defines the Loyalty price as the lowest card price excluding coupons and quantity discounts ([FAQ](https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf); ÁFF XII.1).

**Greece.**
- e-katanalotis.gov.gr now redirects to `posokanei.gov.gr/?from=ekatanalotis` (checked 2026-10-21). PosoKanei refused our automated request, so its terms, any API and any open-data offer are unknown.
- Law 4727/2020 transposes Directive 2019/1024 ([ΦΕΚ Α' 184/2020 text](https://dsanet.gr/Epikairothta/Nomothesia/N4727_184.htm)). It makes documents available for reuse without any action by the requester (art. 61(1)). It excludes documents "για τα οποία τρίτοι διαθέτουν δικαιώματα πνευματικής ιδιοκτησίας" ("on which third parties hold intellectual property rights") (art. 59(4)(γ)) and those restricted for commercial secrecy (art. 59(4)(δ)). The Chains could invoke either for their price feeds. The four crawled Chains' prices were collected by the state itself.
- PosoKanei is the only state source that compares across countries, and it works "κυρίως σε επίπεδο κατηγορίας" ("mainly at category level") ([#3](https://github.com/exilonX/cart-compare/blob/research/cee-comparables/docs/research/cee-comparables.md)).

## Germany

**No state source.** Germany has no state grocery price portal. In June 2026 the Greens filed motion 21/6012: "Die Grünen fordern konkret, eine Preistransparenzstelle einzurichten" ("The Greens specifically call for setting up a price transparency office") ([hib 442/2026](https://www.bundestag.de/presse/hib/kurzmeldungen-1183088)). It is a proposal. The same search found mandatory retail price reporting in Austria (AMA) and a federal report in Switzerland, which are outside this ticket's scope.

**What each Chain shows, and on what terms**

| Chain | Prices visible logged out | Logged-in / app terms (quote) | Website terms |
| --- | --- | --- | --- |
| Lidl | Offers only. Lidl Germany publishes no permanent prices online, so money.ro used leaflets ([#6](https://github.com/exilonX/cart-compare/blob/research/comparison-truth/docs/research/comparison-truth.md)) | "Die Teilnahme darf lediglich zum privaten Gebrauch erfolgen. Eine kommerzielle Teilnahme als Unternehmer gemäß § 14 BGB ist ausgeschlossen" ("Participation is for private use only. Commercial participation as a business is excluded"). Discounts are personalised: "es ist wahrscheinlich, dass bestimmte Gruppen von Nutzern unterschiedliche Rabattsätze für dieselben Produktkategorie erhalten" ("it is likely that certain groups of users get different discount rates for the same product category"). Sharing an account is forbidden ([Lidl Plus v2.3, May 2026](https://www.lidl.de/static/assets/20260518_Teilnahmebedingungen_Lidl_Plus_v2-3-2219220.pdf)) | Not found. A search restricted to lidl.de returned only privacy notices, for example [Datenschutz](https://www.lidl.de/de/datenschutz/s21) |
| Kaufland | Store offers show a regular price and a separate "Mit Kaufland Card XTRA" price without login (offers valid 19–24 Oct 2026) ([Kaufland](https://filiale.kaufland.de/kaufland-xtra/loyalty-bereich.html)) | Kaufland Card XTRA participation terms not read | Not found |
| Penny | Offer pages exist ([penny.de](https://www.penny.de/angebote/top-angebote/)); not checked. The online shop closed on 1 Jan 2022 (search summary of [penny.de](https://www.penny.de/penny-onlineshop)) | "ausschließlich zu privaten Zwecken" ("exclusively for private purposes"); "ein Kopieren, ein Extrahieren und ein Bearbeiten von Inhalten der PENNY App" ("copying, extracting and editing content of the PENNY App") is not permitted; one account per person ([Penny app terms, May 2026](https://www.penny.de/nutzungsbedingungen-penny-app)) | Not found |

**German law on collection.** This adds German specifics to the EU framework in [#9](https://github.com/exilonX/cart-compare/blob/research/legal-collection/docs/research/legal-collection.md).
- **Contract.** Standard terms become part of a contract only if the user points to them, gives a reasonable chance to read them, "und wenn die andere Vertragspartei mit ihrer Geltung einverstanden ist" ("and if the other party agrees to them") ([§ 305(2) BGB](https://www.gesetze-im-internet.de/bgb/__305.html)). That makes binding a logged-out visitor harder. Registering for Lidl Plus or the Penny app is a clear acceptance.
- **Unfair competition.** In *Flugvermittlung im Internet* (Ryanair v Vtours, 2014), the BGH held that automated retrieval of freely accessible data is not unfair merely because terms forbid it: "Das bloße Sich-Hinwegsetzen über Vertragsbedingungen reicht … regelmäßig nicht aus" ("merely disregarding contract terms is … as a rule not enough") (Rn. 35). It added that "die Überwindung einer technischen Schutzvorrichtung" ("overcoming a technical protection device") can make it unfair (Rn. 37) ([I ZR 224/12](https://urteile-gesetze.de/rechtsprechung/i-zr-224-12)).
- **Database right.** A contract clause that stops a lawful user from using insubstantial parts of a database "ist insoweit unwirksam" ("is void to that extent"), where the use neither conflicts with normal exploitation nor unreasonably harms the maker ([§ 87e UrhG](https://www.gesetze-im-internet.de/urhg/__87e.html)).
- **Text and data mining.** For online works, a reservation "ist nur dann wirksam, wenn er in maschinenlesbarer Form erfolgt" ("is only effective if made in machine-readable form") ([§ 44b(3) UrhG](https://www.gesetze-im-internet.de/urhg/__44b.html)). This is stricter for rightholders than the Romanian wording discussed in #9.
- **Criminal law.** Data espionage requires access "unter Überwindung der Zugangssicherung" ("by overcoming access protection") to data "besonders gesichert" ("specially secured") ([§ 202a StGB](https://www.gesetze-im-internet.de/stgb/__202a.html)). Public offer pages are not secured. A login, a challenge page or app API protection would be different, and the project must not touch them.

**Lawful options for German prices**
1. **Logged-out public offer pages** of Lidl, Kaufland and Penny, collected slowly and identifiably, as in #9's option C. This gives offer and some Loyalty prices, not a full Basket.
2. **Volunteer-recorded prices.** [Open Prices](https://github.com/openfoodfacts/open-prices/blob/main/docs/guides/data.md) (Open Food Facts) publishes crowdsourced prices under the ODbL: "Make sure you comply with the OdBL licence, mentioning the source of your data". It offers daily dumps and an API. Each price carries a `product_code` (barcode) and a `proof_type` of `RECEIPT` or `PRICE_TAG`, and the dataset has about 333,000 rows ([Hugging Face](https://huggingface.co/datasets/openfoodfacts/open-prices)). German coverage of our Basket items was not checked. ODbL is share-alike for derived databases. Store house rules on photographing price tags are a lawyer question (also raised in #9).
3. **Ask the Chains** for a data feed or written permission. All three also operate in Romania, so one request could cover both countries.
4. **Not recommended: a logged-in Lidl Plus, Kaufland Card or Penny app account.** It breaches the private-use clauses, ties the collection to a named person, and, at Lidl, yields personalised prices that are not comparable.

## Questions for a lawyer

**Cross-cutting**
1. A Romanian project reuses foreign state data and publishes in Romania. Which law governs reuse in each case: the source country's open-data and database law, Romanian law, or both?
2. Do the KZP, the GVH and the Greek ministry hold a sui generis database right in their portals? Does each country's open-data law stop them using it against reuse? Directive 2019/1024 art. 1(6) is discussed in [#9](https://github.com/exilonX/cart-compare/blob/research/legal-collection/docs/research/legal-collection.md).
3. Could a Chain claim that its reported price feed is its own trade secret or IP, and so excluded from reuse? The same Chain publishes those prices to the public, and in Bulgaria and Croatia must publish them as files.
4. Is publishing weekly Basket totals and per-item prices for about 150 lines a "substantial part" of any of these databases? Does daily collection to build history count as "repeated and systematic" extraction?

**Bulgaria**
5. Does Euro Act art. 55б(1), with its "format allowing data extraction", amount to permission to extract and republish? Or does the KZP's "All rights reserved" notice require a written ЗДОИ art. 41е request first?
6. What is the current end date of the art. 55б duty after the 2026 amendments, and what happens to reuse rights in data already collected once it ends?

**Croatia**
7. Does NN 40/25 art. 12(10) ("radi njihove usporedbe", "for their comparison") cover publishing comparisons outside Croatia, including a cross-country Basket? Does it override any Chain website terms that restrict reuse?
8. Is a donation- or grant-funded civic index "non-commercial" for cijene.dev's CC BY-NC-SA data and its free API tier? If we self-host cijene-api, which AGPL obligations apply to our modifications?

**Hungary**
9. Do the GVH's visitor terms bind an automated client "by conduct"? Do they restrict anything beyond trademarked content and the site's software and design?
10. What were the legal grounds and outcome of the GVH's 2023 civil and criminal steps? Would a written request to the GVH (arfigyelo@gvh.hu) be the right route, and under which reuse law?

**Greece**
11. Do PosoKanei's terms (not readable to us) restrict reuse? Does Law 4727/2020 art. 61 make the Chains' direct feeds and the state-crawled prices reusable "without any action by the requester"?
12. Which enacted law and ministerial decision now oblige Greek Chains to report prices, and do they say anything about publication or reuse?

**Germany**
13. Under § 305(2) BGB and *Flugvermittlung*, may we collect Lidl's, Kaufland's and Penny's public offer pages logged out? Would a website terms clause (if one exists) change that?
14. What is a volunteer's personal exposure, and the project's, if the volunteer reports app-only or personalised prices from their own Lidl Plus or Penny account? Does a volunteer photographing shelf price tags in a German store breach house rules or any other law?
15. If volunteer prices go into Open Prices, what do the ODbL's share-alike terms require of our derived Basket dataset?

## Gaps and uncertainties

- **Search budget.** The shared web-search budget was tight, so several points below rest on a single source or a search-result summary.
- **Bulgaria.**
  - We did not open a daily data file, so we do not know whether the files carry a barcode or product code beyond the statutory fields.
  - The 2026 amendment that extends the art. 55б duty beyond 8 August 2026 was not read. The consolidated text we used runs to ДВ 115/2025.
  - Whether the KZP lists the dataset on data.egov.bg, and under what licence, is unknown: the portal returned 403.
  - The coverage of Lidl and Kaufland is inferred from the turnover threshold and press rankings. We did not see it in the files. Penny's 2015 exit comes from a search-result summary.
- **Croatia.**
  - The NN 101/26 text was not opened in Narodne novine. Its fields and timing come from Fiskalopedija and RRiF summaries, and the draft of 15 October 2026 may change them.
  - Lidl Croatia's and Kaufland Croatia's own website terms were not read.
- **Hungary.**
  - Hungary's public-data reuse act (Act LXIII of 2012, as we understand it) could not be read: njt.hu dropped the connection and the jogtar address returned 404.
  - We did not check whether the public site exposes barcodes.
  - The outcome of the 2023 case is unknown.
  - Section numbers of Act L of 2025 come from a single fetch of the Jogtár consolidated text and should be checked.
- **Greece.**
  - PosoKanei's terms, any API and any open-data release are unread (HTTP 403).
  - The legal basis for Chains' reporting is known only from a 2021 news report on the bill.
  - Law 4727/2020 was read in its 2020 text. Later amendments, for example by Law 5305/2026 to art. 67, were not checked.
- **Germany.**
  - No general website terms were found for lidl.de, kaufland.de or penny.de.
  - Kaufland Card XTRA participation terms were not read, and Penny's offer pages were not checked.
  - Commercial data vendors were not researched.
  - Open Prices' coverage of German Basket items is unknown.
- **EU texts.** EUR-Lex refused automated requests, so the Open Data Directive is cited through [#9](https://github.com/exilonX/cart-compare/blob/research/legal-collection/docs/research/legal-collection.md) and the national transpositions.
- **Reported price vs Shelf price.** All four state sources carry prices the Chains report. Hungary sanctions a Shelf price above the reported one, and #3 records accuracy warnings in Croatia. We did not test how far reported and Shelf prices diverge in any country.

## Sources

All read on 2026-10-21 unless a date is given.

**Bulgaria**
- KZP, kolkostruva.bg open data: https://kolkostruva.bg/opendata
- KZP, kolkostruva.bg About: https://kolkostruva.bg/about
- Euro Introduction Act (ЗВЕРБ), consolidated to ДВ 115/2025, arts. 15, 55б (court-hosted copy): https://elhovo-rs.justice.bg/upload/136279/Закон%20за%20въвеждане%20на%20еврото%20в%20РБ.pdf
- Access to Public Information Act (ЗДОИ), Ciela consolidated text (last amended ДВ 55/2026): https://www.ciela.net/svobodna-zona-normativi/view/2134929408/zakon-za-dostap-do-obshtestvena-informatsiya
- Capital, K100 retailers 2024 (2025-12-09, search summary only): https://www.capital.bg/biznes/kompanii/2025/12/09/4840601_klasaciiata_k100_nai-golemite_riteiluri_prez_2024_g/
- Capital, Penny exit (2015-09-17, search summary only): https://www.capital.bg/biznes/kompanii/2015/09/17/2612126_penny_osvobojdava_pazar_za_200_mln_lv/

**Croatia**
- Zakon o iznimnim mjerama kontrole cijena, NN 40/25 (zakon.hr consolidated, updated to NN 110/26): https://www.zakon.hr/z/842/Zakon-o-iznimnim-mjerama-kontrole-cijena-
- Odluka o objavi cjenika …, NN 75/2025: https://narodne-novine.nn.hr/clanci/sluzbeni/2025_05_75_979.html
- informator.hr, NN 75/2025 status: https://informator.hr/podzakonski-propisi/842580
- RRiF, NN 110/26 postponement (2026-09-30): https://www.rrif.hr/odgada_se_primjena_odluka_o_isticanju_i_objavi_dod-2533-vijest/
- Fiskalopedija, price-list publication (updated 2026-10-20): https://fiskalopedija.hr/baza-znanja/objava-cjenika-na-web-stranici
- senko/cijene-api README: https://github.com/senko/cijene-api

**Hungary**
- GVH, Árfigyelő FAQ (PDF created 2025-07-18): https://arfigyelo.gvh.hu/docs/arfigyelo_GYIK.pdf
- GVH, Árfigyelő visitor terms (in force 2025-07-20): https://arfigyelo.gvh.hu/docs/arfigyelo_rendszer_AFF_latogato.pdf
- GVH, Árfigyelő trader terms (in force 2025-07-20): https://arfigyelo.gvh.hu/docs/arfigyelo_rendszer_AFF_kereskedo.pdf
- Act L of 2025, chapter V (Jogtár): https://net.jogtar.hu/jogszabaly?docid=a2500050.tv
- Telex, unofficial app (2023-08-05): https://telex.hu/belfold/2023/08/05/gvh-figyelmeztetes-kalozapplikacio-arfigyelo

**Greece**
- Skai, PosoKanei Q&A (2026-06-17): https://www.skai.gr/news/greece/nea-platfmorma-kata-tis-akriveias-ti-einai-to-posokanei-pos-leitourgei
- iefimerida, e-katanalotis reporting duty bill (2021-04-06): https://www.iefimerida.gr/oikonomia/e-katanalotes-platforma-me-sygkrisi-timon
- Law 4727/2020, ΦΕΚ Α' 184/23.09.2020 (dsanet.gr copy): https://dsanet.gr/Epikairothta/Nomothesia/N4727_184.htm
- posokanei.gov.gr (HTTP 403 to automated request): https://posokanei.gov.gr/

**Germany**
- Bundestag, hib 442/2026 (2026-06-01): https://www.bundestag.de/presse/hib/kurzmeldungen-1183088
- Lidl Plus Teilnahmebedingungen v2.3 (May 2026): https://www.lidl.de/static/assets/20260518_Teilnahmebedingungen_Lidl_Plus_v2-3-2219220.pdf
- Penny app Nutzungsbedingungen (May 2026): https://www.penny.de/nutzungsbedingungen-penny-app
- Kaufland Card XTRA offers page: https://filiale.kaufland.de/kaufland-xtra/loyalty-bereich.html
- § 305 BGB: https://www.gesetze-im-internet.de/bgb/__305.html
- § 87e UrhG: https://www.gesetze-im-internet.de/urhg/__87e.html
- § 44b UrhG: https://www.gesetze-im-internet.de/urhg/__44b.html
- § 202a StGB: https://www.gesetze-im-internet.de/stgb/__202a.html
- BGH, I ZR 224/12, *Flugvermittlung im Internet* (2014-04-30): https://urteile-gesetze.de/rechtsprechung/i-zr-224-12
- Open Prices data guide: https://github.com/openfoodfacts/open-prices/blob/main/docs/guides/data.md
- Open Prices dataset (Hugging Face): https://huggingface.co/datasets/openfoodfacts/open-prices

**Earlier project research**
- #3, CEE Comparables: https://github.com/exilonX/cart-compare/blob/research/cee-comparables/docs/research/cee-comparables.md
- #6, cross-country truth: https://github.com/exilonX/cart-compare/blob/research/comparison-truth/docs/research/comparison-truth.md
- #9, legal exposure of collection: https://github.com/exilonX/cart-compare/blob/research/legal-collection/docs/research/legal-collection.md
