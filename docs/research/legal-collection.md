# What legal exposure does collecting Chain prices create for us?

Research for ticket [#9](https://github.com/exilonX/cart-compare/issues/9) on map [#1](https://github.com/exilonX/cart-compare/issues/1). Desk research done on 2026-10-21. Terms and conditions are quoted in Romanian, with an English translation.

> **Not legal advice.** This is desk research by a volunteer project. It maps what we would expose ourselves to. It does not conclude that any practice is lawful or unlawful. A Romanian IT lawyer has to confirm the approach before go/no-go (see [Questions for a Romanian IT lawyer](#questions-for-a-romanian-it-lawyer)). The project's standing rule is to avoid any unlawful action, so where the law is unclear this note leans towards the cautious reading.

**How the sources were read.** Each Chain's terms page and robots.txt were fetched once, by hand, on 2026-10-21. To check whether prices show without an account, we opened one public listing page per Chain. We did not collect, store or publish any prices. We did not try to get past any anti-bot page or access control. Profi's live site answered with a challenge page, so its terms come from a public web-archive copy. EU legal texts were read through the Publications Office's official content service ([Cellar](https://op.europa.eu/en/web/cellar)), because EUR-Lex and CURIA refused automated requests. The links below point to the EUR-Lex copies.

## Answer

- **The main exposure comes from contracts, with database law next.** Six of the 8 Chains publish website terms that limit use of their content to personal use and require written consent for anything else: Carrefour, Mega Image, Profi, Penny, Auchan and Selgros. Kaufland's loyalty terms limit use of its accounts to personal purposes. We found no website terms for Lidl. No Chain's terms use the words "robot", "bot" or "scraping". The strictest are **Carrefour**, **Mega Image** and **Selgros**: Carrefour bans putting site content into "any electronic information retrieval system"; Mega Image threatens criminal prosecution for any use beyond "consultation"; Selgros claims the site's data and databases and bans storing them on another server. **Lidl** and **Kaufland** publish no general website terms, only an imprint and the terms of their loyalty programmes ([per-Chain table](#per-chain-findings)).
- **robots.txt does not stand in the way.** No Chain's robots.txt disallows product or offer pages for generic crawlers. The disallowed paths are search, account, checkout and URLs with parameters. Auchan blocks a list of named "scraping bots" by name. Profi's live site served a "Just a moment…" challenge even for robots.txt. That challenge is an access-control measure, and the project must not try to get past it.
- **We need to log in far less than the Overview assumed.** Carrefour, Mega Image and Auchan show the Shelf price to logged-out visitors. Lidl, Kaufland and Penny show weekly offers to logged-out visitors, including the Loyalty price ("cu Lidl Plus", Kaufland Card, "preț cu PENNY card"). These three sites do not list a full priced assortment. Selgros's online shop is "dedicată exclusiv persoanelor juridice, pe baza unui contract încheiat în prealabil" ("only for legal entities, under a contract signed in advance"). Profi was not checked.
- **Logging in with a real account adds exposure and gives us nothing we need.** Creating an account means ticking "Sunt de acord" ("I agree"). That is clickwrap, a clear acceptance under [Civil Code art. 1.196](https://legislatie.just.ro/Public/DetaliiDocument/109884). Several account or loyalty terms limit use to personal purposes, for example Kaufland Card XTRA: "Utilizarea în scopuri comerciale este interzisă" ("commercial use is prohibited"). Collecting with a personal account would be a clear breach, and it would tie the activity to a named person. It also raises the "exceeds the limits of authorisation" question under criminal law (next bullet). **Recommendation: do not collect logged in. Never use a Selgros business account for collection.**
- **Criminal exposure is low for polite, logged-out collection of public pages. It is not zero, and it grows with logging in or getting around blocks.** [Criminal Code art. 360](https://legislatie.just.ro/Public/DetaliiDocument/109855) punishes access to a computer system "fără drept" (without right). The definition of "fără drept" in [Law 161/2003 art. 35(2)](https://legislatie.just.ro/Public/DetaliiDocument/43323) covers a person who "nu este autorizată, în temeiul legii sau al unui contract" (is not authorised under the law or a contract) or who "depășește limitele autorizării" (exceeds the limits of authorisation). The EU Directive on attacks against information systems says terms-of-service breaches alone "should not incur criminal liability" ([Directive 2013/40/EU, recital 17](https://eur-lex.europa.eu/eli/dir/2013/40/oj)). Getting around a challenge page or a geo-block could fall under the aggravated form, art. 360(3). Overloading a server could fall under art. 363.
- **The database right is the open legal question.** In *Ryanair v PR Aviation* the CJEU held that terms can restrict the use of a database that has neither copyright nor sui generis protection ([C-30/14, para. 45](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0030)). Where the right does exist, lawful users may extract insubstantial parts "for any purposes whatsoever", and contract clauses that say otherwise are void ([Directive 96/9/EC arts. 8(1), 15](https://eur-lex.europa.eu/eli/dir/1996/9/oj)). Whether a Chain's online catalogue is protected is unsettled. Investment in *creating* one's own prices does not count ([BHB, C-203/02](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62002CJ0203)), but investment in presenting an e-shop may count. A weekly Basket of about 150 items is a small part of each catalogue. Even so, "repeated and systematic" extraction of insubstantial parts is the line the law draws ([art. 7(5)](https://eur-lex.europa.eu/eli/dir/1996/9/oj); Romanian [Law 8/1996 art. 141(5)](https://legislatie.just.ro/Public/DetaliiDocument/7816)).
- **The text and data mining exceptions help little.** The general exception ([DSM Directive art. 4](https://eur-lex.europa.eu/eli/dir/2019/790/oj); [Law 8/1996 art. 36²](https://legislatie.just.ro/Public/DetaliiDocument/7816)) yields to an express reservation by the rightholder, and recital 18 counts website terms as one way to reserve. Unlike the research exception, it is not protected against contrary contract terms (art. 7(1)). The research exception (art. 3 / art. 36¹) is only for research organisations, which the project is not unless a university partners with it.
- **Monitorul Prețurilor is the most promising lawful source, but reuse rights are not settled.** The Chains load the data under a legal duty ([Law 21/1996 art. 4(6)](https://legislatie.just.ro/Public/DetaliiDocumentAfis/231241)). The site has no terms, no licence and no robots.txt, and calls its prices "publice şi actuale" ("public and current"). The open-data law ([Law 179/2022](https://legislatie.just.ro/Public/DetaliiDocument/256414), which replaced Law 109/2007) gives anyone the right to *request* reuse, and bars public bodies from using a database right to block reuse. It covers only data the body "created in its own activity", though, and that is debatable here. **The clean route is a written reuse request to the Competition Council.** Until then, collect only modestly, only from inside Romania, and never by getting around the Romania-only restriction.
- **Comparables abroad mostly rely on a legal duty, not on scraping.** Croatia's 2025 decision obliges retailers to publish price lists, and the [cijene-api](https://github.com/senko/cijene-api) project is built on it. Romania's own Monitorul Prețurilor rests on a reporting duty. Trolley.co.uk documents no legal basis. This supports the Overview's "ask the Chains, or campaign for a duty" path.

## Per-Chain findings

All fetched on **2026-10-21** unless marked otherwise. "Logged out" means a fresh visit with no account. The robots.txt column covers rules for `User-agent: *`.

| Chain | Terms clause on automated access, copying or reuse (quote → translation) | robots.txt stance on product / offer pages | Prices visible logged out? | Links |
| --- | --- | --- | --- | --- |
| **Lidl** | **No general website terms found.** The footer's "Informații" section lists payment, cookies, data protection and two imprint pages. The website imprint names LIDL DISCOUNT SRL as "operatorul tehnic al website-ului … responsabil pentru promovarea ofertelor din magazine" → "the technical operator of the website … responsible for promoting in-store offers". The Lidl Plus terms are published only as an image flipbook and were not read. | Allowed. Only `/q/search?id=*`, `/cc.js*`, `/cdn/assets/cwv/` and paths starting with a digit (`/1*` … `/9*`) are disallowed. Product pages live under `/p/…`. | **Yes, for weekly offers**, including the Lidl Plus price: the page data carries `"lidlPlusText":"cu Lidl Plus"`. Lidl.ro shows no full priced assortment and has no online grocery shop. | [imprint](https://www.lidl.ro/c/informatii-informatii-companie-pentru-website-ul-lidl/s10058424) · [Lidl Plus legal](https://www.lidl.ro/c/lidl-plus-informatii-legale/s10021655) · [robots](https://www.lidl.ro/robots.txt) |
| **Kaufland** | **No general website terms found.** The legal footer has only "Despre noi" (imprint), the privacy policy, the accessibility statement and the *Kaufland Card XTRA* terms. The card terms say: "Utilizarea va urmări strict scopuri personale. Utilizarea în scopuri comerciale este interzisă." → "Use shall be strictly for personal purposes. Commercial use is prohibited." They also say: "Prin înregistrare, utilizatorul recunoaște valabilitatea acestor condiții" → "By registering, the user acknowledges these terms as valid". | Allowed. Only `/etc.clientlibs/` is disallowed. | **Yes, for weekly offers**, including Kaufland Card prices: the page data has `loyaltyBasePrice` and `KcardPrice` fields. The site shows no full priced assortment. | [imprint](https://www.kaufland.ro/despre-noi.html) · [Card XTRA terms](https://www.kaufland.ro/regulament-privind-protectia-datelor/termeni-conditii-kaufland-card.html) · [robots](https://www.kaufland.ro/robots.txt) |
| **Carrefour** | The "Termene și condiții site și cont" PDF (last updated 26.07.2024), §1.2(iii): no reproducing or exploiting content "în niciun scop comercial" ("for any commercial purpose") without written consent. The ban covers "orice încercare de a încorpora orice informație disponibilă în Aplicație/Website în orice altă aplicație" → "any attempt to incorporate any information available in the App/Website into any other app", or into other electronic material. §14: content may not be "încorporată în orice sistem electronic sau mecanic de găsire a informațiilor, altfel decât în scopul folosirii personale" → "incorporated into any electronic or mechanical information retrieval system, other than for personal use". §1.2(iv) bans overloading servers. | Allowed. Disallowed: `/customer`, `/new_checkout`, `/wishlist`, `/mycarrefour`, `/catalogsearch`, `/catalog/product`, ajax and some parameters. `/produse/…` product pages are open. | **Yes**: the e-shop listing pages show the Shelf price. The *Act for Good* loyalty terms were not read. | [terms page](https://carrefour.ro/termene-si-conditii) · [PDF](https://accounts.eu1.gigya.com/accounts.store.downloadPublicConsentDocument?docID=69434470_575788182010_996fee49b1554b4883b9e1742617bd63.pdf) · [robots](https://carrefour.ro/robots.txt) |
| **Mega Image** | Art. 17: using any information on the Site "in alte scopuri decat cel consultativ, in special in scopuri publice, comerciale sau umoristice, poate face obiectul unor urmariri penale" → "for purposes other than consultation, in particular public, commercial or humorous purposes, may be subject to criminal prosecution". The same article requires written consent for any hyperlink to the site. Art. 13: no right "de a reproduce partial sau integral Continutul … fara acordul prealabil scris" → "to reproduce the Content in part or in whole … without prior written consent". | Allowed. The file opens with `# Allow bots`. Disallowed: `/login`, `/my-account`, `*/search/*`, `*/checkout*`, `*/registration/*`, `/en-ro/*`, `/en/`. | **Yes**: listing pages show the Shelf price logged out. Card Connect gives personalised offers in the account and a 1–3% discount on the basket total at the till, according to a banner on the site. | [terms](https://www.mega-image.ro/termeni-si-conditii) · [robots](https://www.mega-image.ro/robots.txt) |
| **Profi** | From the **archived copy of 2025-08-08**. Art. 3: the materials "nu pot fi copiate, reproduse, modificate, distribuite, replicate, stocate ori transmise … fără acordul prealabil și scris" → "may not be copied, reproduced, modified, distributed, replicated, stored or transmitted … without prior written consent". Use for commercial purposes "poate atrage răspunderea civilă și/sau penală" → "may give rise to civil and/or criminal liability". Links are allowed only to the home page. | **The live site was not readable.** On 2026-10-21 it answered HTTP 403 with a Cloudflare "Just a moment… Enable JavaScript and cookies" challenge, even for robots.txt. The archived copy of 2025-09-02 disallows only `/wp-admin/` and `?s=` search. | **Not checked.** The site challenges automated clients, and we did not try to get past it. | [terms (live)](https://www.profi.ro/termeni-si-conditii/) · [terms (archive)](https://web.archive.org/web/20250808041700/https://www.profi.ro/termeni-si-conditii/) · [robots (archive)](https://web.archive.org/web/20250902101726/https://www.profi.ro/robots.txt) |
| **Penny** | Art. 2: "Materialele publicate și conținutul www.penny.ro pot fi utilizate numai în scop personal, fiind interzisă comercializarea acestora" → "may be used only for personal purposes; selling them is prohibited". Reproducing the content requires prior written permission. Art. 8 says use of the site means acceptance (browsewrap). | **No rules at all.** The file holds a single `Sitemap:` line and is served as `text/html`. | **Yes, for weekly offers**, with both prices side by side: "preț fără PENNY card" / "preț cu PENNY card" ("price without / with the PENNY card"), plus "preț minim ultimele 30 de zile" ("lowest price in the last 30 days"). | [terms](https://www.penny.ro/termeni-conditii) · [robots](https://www.penny.ro/robots.txt) |
| **Auchan** | Art. 2: "Cumpărătorului nu îi este permisă copierea, distribuirea, publicarea … includerea oricărui Conținut în afara Site-ului … decât cu acordul scris expres" → "the Buyer may not copy, distribute, publish … include any Content outside the Site … without express written consent". "Cumpărător" (Buyer) is defined as someone who "își face un Cont în Site și efectuează o comandă" ("creates an Account and places an order"), so the clause targets account holders. | Allowed for `*`. Account, login, checkout, search (`/busca/`, `?query=`) and some parameters are disallowed. Under the comment "Blocheaza boti cunoscuți de scraping" ("blocks known scraping bots"), the whole site is disallowed for named bots such as HTTrack, WebCopier and MJ12bot. | **Yes**: the category page data carries `Price` and `ListPrice` logged out. | [terms](https://www.auchan.ro/termeni-si-conditii) · [robots](https://www.auchan.ro/robots.txt) |
| **Selgros** | II. Content is defined to include "datele sau informațiile accesibile prin intermediul său, inclusiv eventualele baze de date aferente" ("the data or information accessible through it, including any related databases"), and may be used "doar pentru folosința dvs. personală" ("only for your personal use"). Banned, and possibly "acte de contrafacere" (infringement): "reproducerea totală sau parțială sau stocarea Conținutului, precum si retransmiterea Conținutului către orice alt website, server" → "total or partial reproduction or storage of the Content, and retransmission to any other website, server". It also bans "prezentarea selectivă/trunchiată a revistelor de oferte" ("selective/truncated presentation of offer magazines"). Use of the site means acceptance. | Allowed. Drupal defaults plus `/search/` and login paths are disallowed. The sitemaps include a `products-index.xml`. | **No.** The www.selgros.ro assortment pages show no prices. shop.selgros.ro is "dedicată exclusiv persoanelor juridice, pe baza unui contract încheiat în prealabil" ("only for legal entities, under a contract signed in advance"). | [terms](https://www.selgros.ro/termeni-si-conditii-website) · [robots](https://www.selgros.ro/robots.txt) · [shop](https://shop.selgros.ro/) |

**What the table shows:**

- **Only three Chains publish full priced catalogues on the open web: Carrefour, Mega Image and Auchan.** Two of them have the strictest reuse clauses. For Lidl, Kaufland and Penny the web gives only offer prices, so a full Basket cannot come from their websites at all, logged in or not. Selgros's online prices sit behind a B2B contract.
- **How each Chain's terms bind** (see [Contract](#1-contract-browsewrap-clickwrap-and-the-effect-of-logging-in)):
  - **Browsewrap only:** Penny, Profi and Selgros say that using the site means accepting the terms.
  - **Clickwrap at account creation:** Mega Image ("Sunt de acord cu Termenii si Conditiile"), Auchan, Kaufland Card XTRA.
  - **Both:** Carrefour.
- **Ownership:** Mega Image and Profi now share an owner, after the Competition Council cleared Mega Image's takeover of Profi ([#8 findings](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md)). Their terms may converge.

## Legal framework

### 1. Contract: browsewrap, clickwrap and the effect of logging in

- **How a contract forms.** Under the Romanian Civil Code, "Orice act sau fapt al destinatarului constituie acceptare dacă indică în mod neîndoielnic acordul său" → "any act or conduct of the offeree is acceptance if it *unequivocally* indicates agreement". In contrast, "Tăcerea sau inacțiunea destinatarului nu valorează acceptare" → "silence or inaction is not acceptance", except where law, agreement, practice or usage says otherwise ([art. 1.196](https://legislatie.just.ro/Public/DetaliiDocument/109884)).
  - **Clickwrap** (ticking "Sunt de acord" when creating an account) plainly meets this test.
  - **Browsewrap** ("using the site means accepting") is uncertain. Merely loading public pages may not be conduct that "unequivocally" shows agreement. We found no Romanian ruling on this; the Overview's first pass relied on secondary commentary for the same point.
- **Standard terms.** Terms of use are standard clauses ([art. 1.202](https://legislatie.just.ro/Public/DetaliiDocument/109884)). [Art. 1.203](https://legislatie.just.ro/Public/DetaliiDocument/109884) requires express written acceptance only for "unusual" clauses: limitation of liability, unilateral termination, choice of law and jurisdiction, and similar. A personal-use-only clause is not on that list. So once a contract exists, the reuse limits can bind.
- **Ryanair defers to national law.** Where no EU database right exists, a site's terms may restrict use "without prejudice to the applicable national law" ([C-30/14, ruling](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0030)). In that case the visitor had to accept Ryanair's terms "by ticking a box" (para. 16), and the terms banned "the use of automated systems or software to extract data … for commercial purposes" (para. 16).
- **What logging in changes:**
  1. It turns probably-not-binding browsewrap into binding clickwrap.
  2. Account and loyalty terms add personal-use clauses. Kaufland Card XTRA bans commercial use, and Carrefour's buyer must act "în nume propriu și nu reprezintă nicio altă persoană" ("in their own name, not representing anyone else") (§1.2(i)).
  3. The Chain can identify the person behind every request.
  4. It invites account closure: Selgros may deactivate an account "fără preaviz" ("without notice"), and Kaufland may exclude abusive users.
  5. It raises the criminal-law "limits of authorisation" question in §4.
  6. For Selgros it would mean using a B2B account outside its contract.

### 2. EU database right and *Ryanair v PR Aviation* (C-30/14)

**What the Directive says** ([Directive 96/9/EC](https://eur-lex.europa.eu/eli/dir/1996/9/oj)):

- **Database** (art. 1(2)): "a collection of independent works, data or other materials arranged in a systematic or methodical way and individually accessible by electronic or other means." An online product catalogue with prices can meet this definition.
- **Sui generis right** (art. 7(1)): it protects a maker who made "a substantial investment in either the obtaining, verification or presentation of the contents". The maker can then prevent extraction or re-utilisation of "the whole or of a substantial part".
- **Repeated small extractions** (art. 7(5)): "The repeated and systematic extraction and/or re-utilization of insubstantial parts … implying acts which conflict with a normal exploitation of that database or which unreasonably prejudice the legitimate interests of the maker … shall not be permitted."
- **Lawful users** (art. 8(1)): the maker "may not prevent a lawful user … from extracting and/or re-utilizing insubstantial parts of its contents … for any purposes whatsoever."
- **Mandatory rules** (art. 15): "Any contractual provision contrary to Articles 6 (1) and 8 shall be null and void."

**How the CJEU has read it:**

- ***Ryanair v PR Aviation*** ([C-30/14, 15 January 2015](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0030)). The Court held that arts. 6(1), 8 and 15 "are not applicable to a database which is not protected either by copyright or by the sui generis right … so that it does not prevent the adoption of contractual clauses concerning the conditions of use of such a database" (para. 39). In the Court's words, lawful users are "third parties authorised by that person to use the database" (para. 40). The result is a paradox: **an unprotected price list can be locked down by contract more tightly than a protected one.**
- ***BHB v William Hill*** ([C-203/02, 9 November 2004](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62002CJ0203)). "Investment in … the obtaining" means "the resources used to seek out existing independent materials and collect them in the database. It does not cover the resources used for the creation of materials which make up the contents of a database." A Chain *creates* its own prices, so price-setting effort does not count. What may count is investment in presenting and verifying an e-shop catalogue.
- ***Innoweb v Wegener*** ([C-202/12, 19 December 2013](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62012CJ0202)). A dedicated meta search engine that mirrors a database site's search re-utilises "the whole or a substantial part" of it.
- ***CV-Online Latvia v Melons*** ([C-762/19, 3 June 2021](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62019CJ0762)). A specialised search engine that copies and indexes a freely accessible database extracts and re-utilises it. The maker can stop this only where it "adversely affect[s] its investment … namely that they constitute a risk to the possibility of redeeming that investment through the normal operation of the database".

**Romanian transposition.** Law 8/1996 arts. 140–143 ([legislatie.just.ro](https://legislatie.just.ro/Public/DetaliiDocument/7816)):

- **Art. 140(4)** defines the maker as the person who made "o investiție substanțială cantitativă și calitativă" ("a substantial quantitative *and* qualitative investment"). The Directive says "qualitatively and/or quantitatively", so the Romanian wording may be stricter.
- **Art. 141(1)** grants the exclusive right over the whole or a substantial part.
- **Art. 141(5)** copies the "repetată și sistematică" (repeated and systematic) limit.
- **Art. 142(1)** lets the lawful user take insubstantial parts "oricare ar fi scopul utilizării" ("whatever the purpose").
- **Art. 142(4)(b)** allows substantial extraction for "cercetare științifică" (scientific research), with the source indicated and "în măsura justificată de scopul necomercial urmărit" ("to the extent justified by the non-commercial purpose").
- **No express counterpart of art. 15** (nullity of contrary clauses) appears in arts. 140–143.
- **Art. 194 makes infringement a crime.** It punishes making available to the public "fără drept" (without right) products carrying "drepturi suigeneris ale fabricanților de baze de date", with 6 months to 3 years or a fine. This bears mainly on publishing (ticket #10), but it raises the stakes if a Chain's catalogue is protected.

**What this means for us:**

- **Is a Chain's catalogue protected?** This is a factual question for each Chain, with no ruling yet. The e-shops (Carrefour, Mega Image, Auchan) have the best case for a qualifying investment in presentation. Weekly offer pages (Lidl, Kaufland, Penny) are a weaker case.
- **If the catalogue is protected:** a Basket of about 150 lines from a catalogue of thousands is likely an insubstantial part. Art. 8 / art. 142 then protects us against the terms, but the art. 7(5) / art. 141(5) "repeated and systematic" limit applies to weekly collection.
- **If it is not protected:** under *Ryanair* the terms decide, subject to Romanian contract law (§1).

### 3. Text and data mining exceptions

**The EU rules** ([DSM Directive 2019/790](https://eur-lex.europa.eu/eli/dir/2019/790/oj)):

- **Definition** (art. 2(2)): TDM is "any automated analytical technique aimed at analysing text and data in digital form in order to generate information which includes but is not limited to patterns, trends and correlations". A weekly price index arguably fits.
- **Research exception** (art. 3): only for "research organisations and cultural heritage institutions". A research organisation (art. 2(1)) is an entity whose "primary goal … is to conduct scientific research" on a not-for-profit basis or under a public-interest mission.
- **General exception** (art. 4): covers reproductions and extractions "of lawfully accessible works and other subject matter", including the sui generis right. It applies only where use "has not been expressly reserved by their rightholders in an appropriate manner, such as machine-readable means in the case of content made publicly available online" (art. 4(3)).
- **Recital 18** says that for online content, an appropriate reservation uses "machine-readable means, including metadata and terms and conditions of a website or a service".
- **Contract override** (art. 7(1)): only clauses contrary to arts. 3, 5 and 6 are unenforceable. **Art. 4 can therefore be overridden by contract.**

**Romanian transposition.** Law 69/2022 added these articles to Law 8/1996, in force since 4 April 2022 (see the amendment notes in the [consolidated Law 8/1996](https://legislatie.just.ro/Public/DetaliiDocument/7816)):

- **Art. 36¹** (research). Its para. (2) expressly extends the exception to the database right in art. 141(1).
- **Art. 36²** (general) allows "reproducerile și extragerile din opere și din alte obiecte protejate accesibile în mod legal în scopul extragerii textului și a datelor" ("reproductions and extractions of lawfully accessible works and other protected subject matter for text and data mining"). It applies on condition that use was not reserved "în mod corespunzător, cum ar fi mijloace care pot fi citite automat" ("appropriately, such as by machine-readable means").
- **A possible gap:** unlike arts. 36¹, 36³ and 36⁴, art. 36² does not name the art. 141(1) database right.

**What this means for us:**

- **None of the 8 robots.txt files reserves TDM** or uses a TDM-specific protocol.
- **But the reuse bans in Carrefour's, Mega Image's and Selgros's terms may count as a reservation** under recital 18. Whether a natural-language clause counts as "machine-readable" is debated in commentary. We did not resolve it.
- **The exception covers copying for analysis, not publishing.** Publishing what was extracted is a separate act (ticket #10).
- **Copyright does not protect prices, which are facts.** Product photos and marketing texts can be protected, so we should not collect or republish them.

### 4. Criminal law: Criminal Code art. 360 and related offences

**What the Criminal Code says** ([Law 286/2009, consolidated](https://legislatie.just.ro/Public/DetaliiDocument/109855)):

- **Art. 360(1):** "Accesul, fără drept, la un sistem informatic se pedepsește cu închisoare de la 3 luni la 3 ani sau cu amendă." → "Access, without right, to a computer system is punished with imprisonment from 3 months to 3 years or a fine."
- **Art. 360(2):** if committed "în scopul obținerii de date informatice" ("to obtain computer data"), the penalty is 6 months to 5 years.
- **Art. 360(3):** "Dacă fapta … a fost săvârșită cu privire la un sistem informatic la care, prin intermediul unor proceduri, dispozitive sau programe specializate, accesul este restricționat sau interzis pentru anumite categorii de utilizatori, pedeapsa este închisoarea de la 2 la 7 ani." → "If the act concerns a computer system to which, by means of specialised procedures, devices or programs, access is restricted or prohibited for certain categories of users, the penalty is imprisonment from 2 to 7 years."
- **Art. 363** punishes seriously disrupting, "fără drept", the functioning of a computer system "prin introducerea, transmiterea … datelor informatice" ("by inputting, transmitting … computer data") with 2 to 7 years.
- **Art. 364:** "Transferul neautorizat de date dintr-un sistem informatic … se pedepsește cu închisoarea de la unu la 5 ani." → "Unauthorised transfer of data from a computer system … is punished with 1 to 5 years."
- **Art. 366:** the attempt is also punished.
- **Art. 181** defines "sistem informatic" (computer system) and "date informatice" (computer data) broadly. A retailer's web server qualifies.

**What "fără drept" means.** [Law 161/2003 art. 35(2)](https://legislatie.just.ro/Public/DetaliiDocument/43323) says: "În sensul prezentului titlu, acționează fără drept persoana care … a) nu este autorizată, în temeiul legii sau al unui contract; b) depășește limitele autorizării; c) nu are permisiunea …" → "For the purposes of this title, a person acts without right who a) is not authorised under the law or a contract; b) exceeds the limits of the authorisation; c) lacks permission …". The definition is written for that law's own title. Whether courts apply it to the Criminal Code articles is a question for the lawyer.

**The EU baseline** ([Directive 2013/40/EU](https://eur-lex.europa.eu/eli/dir/2013/40/oj)):

- Member States must criminalise illegal access "where committed by infringing a security measure" (art. 3). Romania's art. 360(1) goes further and does not require a security measure to be infringed.
- "Without right" means conduct "not authorised by the owner … or not permitted under national law" (art. 2(d)).
- Recital 17: "contractual obligations or agreements to restrict access to information systems by way of a user policy or terms of service … should not incur criminal liability where the access under such circumstances would be deemed unauthorised and thus would constitute the sole basis for criminal proceedings."

**Our reading, to be confirmed by the lawyer:**

| Scenario | Exposure under art. 360–364 |
| --- | --- |
| Logged-out requests to pages the Chain serves to anyone, low rate, robots.txt respected | **Low.** The access is the access the site offers the public. A terms breach alone should not make it criminal (recital 17). The "contract" limb of art. 35(2) is the residual risk. |
| Logged in with a personal or loyalty account, used for the project | **Higher.** This is arguably "depășește limitele autorizării" (exceeds the limits of authorisation) where the terms limit use to personal purposes. |
| Getting around a challenge page, CAPTCHA, IP block or geo-block | **Clearly to be avoided.** The block is a measure by which access "este restricționat sau interzis pentru anumite categorii de utilizatori" (art. 360(3), 2–7 years). This is off-limits for the project anyway. |
| Request volumes that slow or break a site | Art. 363 if the disruption is "grav" (serious). Throttling is a legal safeguard, not only good manners. |
| Copying public data | Art. 364 "transfer neautorizat" (unauthorised transfer). It is unclear whether copying publicly served data can be "unauthorised". This is a lawyer question. |

**Case law.** The legislative portal notes three referrals to the High Court of Cassation and Justice for a preliminary ruling (HP) on art. 360: HP 2/2021, HP 68/2021 and HP 53/2022. All three are marked "Decizie de respingere" (rejected), so they give no binding interpretation ([portal notes under art. 360](https://legislatie.just.ro/Public/DetaliiDocument/109855)).

### 5. Data Act

The Data Act ([Regulation (EU) 2023/2854](https://eur-lex.europa.eu/eli/reg/2023/2854/oj)) has applied since 12 September 2025. It governs data from connected products and related services. Its art. 43 switches off the database right only for data "obtained from or generated by a connected product or related service". **Retailers' web catalogues are outside its scope.** It neither helps nor hurts us.

### 6. Court cases on price scraping and comparison sites

- **EU:** the four CJEU judgments above (*Ryanair*, *BHB*, *Innoweb*, *CV-Online*) are the binding framework.
- **Romania:** we found no Romanian judgment on scraping retail prices, on browsewrap or clickwrap enforceability, or on art. 360 applied to public web pages. Our search budget ran out before we could check commentary systematically (see [Gaps](#gaps-and-uncertainties)).

### 7. What Comparables abroad rely on

- **Croatia.** Retailers must publish their price lists under the "Odluka o objavi cjenika i isticanju dodatne cijene kao mjeri izravne kontrole cijena u trgovini na malo", NN 75/2025 of 2 May 2025 (the decision on publishing price lists as a direct price-control measure in retail). Price apps build on that duty; [cijene-api](https://github.com/senko/cijene-api) says so in its README. *(Secondary: the decision is named in the project's README. We did not open it in Narodne novine, the official gazette.)*
- **Romania.** Monitorul Prețurilor rests on the reporting duty in [Law 21/1996 art. 4(6)](https://legislatie.just.ro/Public/DetaliiDocumentAfis/231241) (see below).
- **UK.** [Trolley.co.uk's About page](https://www.trolley.co.uk/about/) does not say how it obtains prices or on what legal basis. It mentions only that sponsorships "cover licensing fees".
- **Elsewhere.** The state-mandated reporting schemes in other CEE countries are covered in ticket #3 and were not re-verified here.

### 8. Check of the Overview's first-pass legal notes

| Overview claim | Verdict |
| --- | --- |
| "The main risk is contractual, not criminal" | **Supported.** We would add the database right as a second risk. For three Chains it is the main question. |
| *Ryanair* lets a site with no copyright or database right ban scraping through its terms | **Confirmed** against the judgment (para. 45 and ruling). The Pinsent Masons summary cited in the Overview is accurate. |
| Art. 360 "mainly targets bypassing security; public pages carry low risk" | **Partly.** Art. 360(1) does *not* require bypassing security; only the aggravated form in (3) does. "Fără drept" can be read through a contract (Law 161/2003 art. 35(2)). "Low risk for polite, logged-out access" remains our reading. |
| Clickwrap is enforceable; browsewrap depends on notice | **Consistent** with Civil Code art. 1.196 (acceptance needs conduct that "unequivocally" shows agreement). No Romanian case law was found. |
| Sources "collected live … logged in with a real user account" | **Should change.** Logging in is not needed for most prices, and it raises every kind of exposure. |
| "Respect robots.txt, throttle, never bypass CAPTCHAs" | **Supported.** Throttling also matters for art. 363. Profi's challenge page means Profi cannot be collected from its website at all. |

## Lawful alternatives

### A. Monitorul Prețurilor

The facts below come from the [#8 findings](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md), re-checked where marked.

- **The legal duty.** The Competition Council runs the platform. Since OUG 170/2020, [Law 21/1996 art. 4(6)](https://legislatie.just.ro/Public/DetaliiDocumentAfis/231241) says: "Întreprinderile transmit la cererea Consiliului Concurenței prețurile de vânzare a produselor comercializate de acestea, în vederea realizării de analize, studii de piață sau comparații de preț incluse în platformele online destinate informării consumatorilor." → "Undertakings send the Competition Council, on request, the sale prices of the products they sell, for analyses, market studies or price comparisons included in online platforms meant to inform consumers." *(re-checked)*
- **The site's legal text.** We re-checked the home page on 2026-10-21. It holds only a disclaimer, which says: "Preţurile afişate pe acest site sunt publice şi actuale" ("The prices shown on this site are public and current"). It also says the Council and participants "nu sunt responsabili pentru utilizarea ilicită de către terți a informațiilor afișate pe site" ("are not responsible for unlawful use by third parties of the information on the site"). That sentence acknowledges third-party use without granting permission. `robots.txt` returned **404**.
- **Not open data.** There is no licence, no documented API and no dataset on data.gov.ro. The front end calls an undocumented service, and searches are meant to work only from inside Romania. Third parties ([gov2-ro](https://github.com/gov2-ro/monitorulpreturilor), money.ro) already reuse the data without a stated legal basis ([#8](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md)).

**(1) Who, if anyone, holds rights in the data?**

- **Copyright: nobody.** Prices are facts. Product names and brand marks belong to manufacturers, and naming them descriptively is not an issue we found.
- **The Chains: probably no sui generis right in MP's dataset.** Per the Council, the Chains load the data themselves ([#8](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md)). Their effort is in *creating* prices, which does not count ([BHB](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62002CJ0203)). The Chains may still argue that their reported price feeds are commercial information supplied to an authority. That is the strongest argument for keeping the data out of open-data law (point 2).
- **The Council (the State): possibly a sui generis right.** It commissioned and paid for the platform: 1,422,346 lei, fully state-funded, developed by Maguay ([#8](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md)). That is investment in obtaining, verifying and presenting the data. The software itself is excluded from database protection ([Law 8/1996 art. 140(3)](https://legislatie.just.ro/Public/DetaliiDocument/7816)) and protected by copyright instead.
- **The Council cannot use that right to block reuse inside the open-data regime.** [Directive 2019/1024 art. 1(6)](https://eur-lex.europa.eu/eli/dir/2019/1024/oj) and [Law 179/2022 art. 1(7)](https://legislatie.just.ro/Public/DetaliiDocument/256414) say the database right "nu este exercitat de entitățile publice pentru a împiedica reutilizarea documentelor" → "is not exercised by public bodies to prevent re-use of documents". This holds only if the data fall within that law's scope.

**(2) Does Romanian open-data law give a right to reuse it?**

- **The current law is Law 179/2022, not Law 109/2007.** Law 179/2022 "privind datele deschise și reutilizarea informațiilor din sectorul public" ("on open data and the reuse of public-sector information") transposes Directive 2019/1024. It is the measure Romania notified to the Commission ([EU record MNE(2022)03782](https://eur-lex.europa.eu/legal-content/EN/NIM/?uri=CELEX:32019L1024)). Its art. 18(6) applies Law 109/2007 only to requests filed before it entered into force ([Law 179/2022](https://legislatie.just.ro/Public/DetaliiDocument/256414)).
- **What it gives:**
  - **A principle** that covered documents "sunt reutilizabile în scopuri comerciale sau necomerciale" ("are reusable for commercial or non-commercial purposes") (art. 3).
  - **A right to ask:** "Orice persoană fizică sau juridică poate adresa oricărei entități publice o solicitare de reutilizare" → "any natural or legal person may send any public body a reuse request" (art. 4(1)). The answer is due within 30 working days, extendable by 20 (art. 4(8)), with a licence or a standard licence (art. 4(4)–(5)).
- **Why it may not reach MP data:**
  - The law covers data "pe care acestea le-au creat în cadrul activității proprii" ("which [public bodies] created in their own activity") (art. 1(1)). The Chains load MP's prices.
  - It excludes "documentelor asupra cărora terții dețin drepturi de proprietate intelectuală" ("documents on which third parties hold intellectual property rights") (art. 1(2)(c)). It also excludes documents whose access is excluded on grounds of "secretul comercial" ("trade secrecy") (art. 1(2)(d)(iii)). The Chains could invoke either, although the platform itself calls the prices "publice" ("public").
  - It does not oblige the Council to build an API or a bulk download.
- **The High-Value Datasets rules do not cover it.** The [HVD Regulation (EU) 2023/138](https://eur-lex.europa.eu/eli/reg_impl/2023/138/oj) has six categories: geospatial, earth observation and environment, meteorological, statistics, companies, mobility. Its statistics category includes the *Harmonised Indices of Consumer Prices*, not retail prices per product. So no HVD duty applies to MP data. The HICP is open data and useful for context.
- **Free access to information.** [Law 544/2001](https://legislatie.just.ro/Public/DetaliiDocument/31413) gives a parallel route for asking about the platform: its contracts, data model and terms. Answers are due within 10 days, or 30 for complex requests.

**(3) Is systematic collection from the platform acceptable?**

- **Contract: no clause binds us.** There are no terms and no robots.txt, so there is also no machine-readable TDM reservation under [art. 36²(3)](https://legislatie.just.ro/Public/DetaliiDocument/7816).
- **Database right:** collecting the whole catalogue daily would be "extraction" of a substantial part if the Council holds a right (point 1). The Council's ability to object depends on Law 179/2022's scope. A Basket of about 150 items is likely insubstantial.
- **Criminal law: low risk if done gently.** Calling the same service the public front end calls, at a polite rate, is using what the site offers to the public. Getting around any limit is not. Heavy load engages art. 363.
- **The Romania-only restriction is the sensitive point.** It is a technical measure restricting access for a category of users, those outside Romania.
  - Running the collector from a Romanian connection, which is the intended audience, gets around nothing.
  - Hosting the collector abroad and routing through Romanian proxies or a VPN to look domestic would be getting around it. It could engage art. 360(3) (access "restricționat … pentru anumite categorii de utilizatori", i.e. restricted for certain categories of users), and the project rules forbid it.
  - In practice: **the collector must run from Romania, or not at all, until the Council says otherwise.** The restriction also signals that the operator means the service for domestic consumers, which is a further reason to ask first.
- **Third parties already reuse the data** (gov2-ro, money.ro). That shows tolerance so far, not permission.
- **Bottom line: send a reuse request under Law 179/2022 art. 4** describing the civic purpose, and ask for a licence or written confirmation. Until an answer arrives, if MP is used at all: collect a small Basket, at a low rate, from Romania, with an honest User-Agent and contact details.

### B. Ask the Chains for permission or a data feed

- **Every restrictive clause above comes with a consent route:** "fără acordul prealabil scris" / "acordul scris expres" ("without prior written consent" / "express written consent"). Written permission removes the contractual exposure entirely.
- **Precedent:** Ryanair's own terms carved out written licences "for the sole purpose of price comparison" ([C-30/14, para. 16](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0030)).
- **Starting point:** the Chains already report to MP under art. 4(6). As the Overview suggests, a joint request could go to the Chains that already report.

### C. Collect only what the Chains already publish to everyone, with safeguards

If the lawyer agrees, this lowers but does not remove the contractual exposure for Carrefour, Mega Image, Auchan, Selgros and Profi.

- Logged-out pages only.
- The Shelf price, plus the Loyalty price where the Chain itself shows it logged out (Lidl, Kaufland, Penny).
- Only the Basket lines.
- Weekly, throttled, respecting robots.txt, with an identifying User-Agent and a contact address.
- No images or product texts.
- Never anything behind a challenge page, a login or a geo-block.

### D. Manual collection

- **How:** volunteers record Shelf prices from public leaflets or in store.
- **Why it helps:** it avoids website terms and database extraction from websites.
- **Open points:**
  - Store house rules may restrict photography. This is a lawyer question.
  - Selgros's terms restrict republishing its offer magazines: a 60-day storage limit and no "selective" presentation.

### E. Official statistics, and campaigning

- **Official statistics:** INS/Eurostat HICP series (an HVD) are fully open and give context, not Basket prices.
- **Campaigning:** a Croatia-style duty to publish machine-readable price lists is the durable fix. This is already listed under "Not yet specified" on map #1.

## Questions for a Romanian IT lawyer

**Contract and accounts**

1. Do the website terms of Penny, Profi and Selgros bind a visitor who never registers? Romanian law requires conduct that "unequivocally" shows agreement ([Civil Code art. 1.196](https://legislatie.just.ro/Public/DetaliiDocument/109884)). Does Carrefour's dual mechanism (continued use plus a ticked box) change that for logged-out visitors?
2. Does a non-commercial civic index count as "scop comercial" (commercial purpose) under Carrefour §1.2(iii), Penny art. 2 and Profi art. 3? Is it "alte scopuri decât cel consultativ" (purposes other than consultation) under Mega Image art. 17? How far does Carrefour's "orice sistem electronic … de găsire a informațiilor" (any electronic … information retrieval system) reach?
3. Can a weekly index of about 150 items be "selective" presentation under Selgros's offer-magazine clause? Can its claim to "datele … inclusiv eventualele baze de date" (the data … including any databases) be enforced against a visitor?
4. If a volunteer uses their own loyalty or online account to read prices for the project, what is their personal exposure, and the project's? Consider Kaufland Card XTRA ("strict scopuri personale", strictly personal purposes) and Carrefour ("în nume propriu", in one's own name).
5. Is Mega Image's requirement of written consent for any hyperlink enforceable? This matters for linking to sources.

**Database right**

6. Is a Chain's online catalogue (Carrefour, Mega Image, Auchan) or its offer pages (Lidl, Kaufland, Penny) likely to qualify as a protected database? Consider *BHB* (creating prices does not count) and the stricter wording "cantitativă și calitativă" (quantitative and qualitative) in [Law 8/1996 art. 140(4)](https://legislatie.just.ro/Public/DetaliiDocument/7816).
7. Does weekly extraction of the same Basket lines amount to "repetată și sistematică" (repeated and systematic) extraction of insubstantial parts ([art. 141(5)](https://legislatie.just.ro/Public/DetaliiDocument/7816))?
8. Law 8/1996 seems to lack an express counterpart to Directive art. 15. Does Romanian law still void terms that restrict a lawful user's art. 142(1) rights? Is a logged-out visitor a "utilizator legitim" (lawful user)?
9. Could [Law 8/1996 art. 194](https://legislatie.just.ro/Public/DetaliiDocument/7816), the crime of making sui generis-protected content available "fără drept", apply to publishing Basket totals or item prices? (To be read together with ticket #10.)

**Text and data mining**

10. Does art. 36² cover the database right (art. 141(1)), given that it does not name it while art. 36¹ does? Do natural-language terms count as a reservation "în mod corespunzător" (appropriately)?
11. Could the project qualify as, or partner with, a "research organisation" to use art. 36¹ and art. 142(4)(b)?

**Criminal law**

12. Do courts read "fără drept" in Criminal Code art. 360 through [Law 161/2003 art. 35(2)](https://legislatie.just.ro/Public/DetaliiDocument/43323), including "depășește limitele autorizării" (exceeds the limits of authorisation) under a contract? How much weight do Romanian courts give to [Directive 2013/40/EU recital 17](https://eur-lex.europa.eu/eli/dir/2013/40/oj)?
13. Do robots.txt rules, rate limits, bot-challenge pages (such as Profi's) or geo-blocks count as "proceduri, dispozitive sau programe specializate" (specialised procedures, devices or programs) that restrict access under art. 360(3)? Is merely *ignoring* robots.txt relevant?
14. Can art. 364 ("transfer neautorizat de date", unauthorised transfer of data) apply to copying data that a site serves publicly?

**Monitorul Prețurilor**

15. Does the Competition Council (or the State) hold a sui generis right in Monitorul Prețurilor's database? Do the Chains hold any right in the prices they load?
16. Are MP's data "documents" within [Law 179/2022](https://legislatie.just.ro/Public/DetaliiDocument/256414), given art. 1(1) ("create în cadrul activității proprii", created in their own activity) and the exclusions for third-party rights and trade secrecy? If so, can the Council refuse a reuse request, or impose a licence that bars republication?
17. Is automated retrieval through the undocumented service the public front end uses lawful, at a polite rate and without a licence? Is the disclaimer's mention of "utilizarea ilicită de către terți" (unlawful use by third parties) relevant?
18. Does the Romania-only restriction make access from abroad "fără drept", or aggravated under art. 360(3)? Is a collector hosted outside Romania exposed even if it never gets around the restriction?
19. May MP-derived data be republished under an open licence?

**Process**

20. What should a written permission or data-feed request to a Chain contain to remove the contractual exposure? Should we notify the Chains before launch, even without asking for permission?

## Gaps and uncertainties

- **Our web search budget ran out midway.** Secondary commentary was not consulted systematically. That covers Romanian doctrine on browsewrap, Romanian case law on scraping, and commentary on whether terms count as a "machine-readable" TDM reservation. Foreign leads that are well known but **not verified here** include the German Federal Court of Justice (BGH) ruling of 2014 on screen scraping of Ryanair by a travel agent, and French case law on the database right in classified-ad sites (Leboncoin). A follow-up search should check them before the lawyer consult.
- **Not every set of terms was read:**
  - **Lidl Plus** terms are published as an image flipbook and were not read.
  - The **Penny Card** and **Carrefour Act for Good** terms were not read.
  - **Lidl** and **Kaufland** may publish website terms somewhere we did not find; we checked the footer and legal navigation only.
- **Profi** was read from web-archive copies of 2025-08-08 (terms) and 2025-09-02 (robots.txt). The live site may differ.
- **Logged-out price visibility** was checked on one listing page per Chain, not per item. We used static page data where possible. For Mega Image and Selgros we used one ordinary browser page view, without logging in and without dismissing the cookie banners.
- **Monitorul Prețurilor's Romania-only restriction** comes from #8 and was not re-tested from outside Romania.
- **The legislatie.just.ro consolidated texts** were read on 2026-10-21. We did not record the consolidation date shown on the portal.
- **EUR-Lex and CURIA refused automated requests** (an empty HTTP 202 and a JavaScript app). The texts were read from the Publications Office's Cellar service, which serves the same official documents.

## Sources

**Chains** (all fetched 2026-10-21 unless noted)

- Lidl: [website imprint](https://www.lidl.ro/c/informatii-informatii-companie-pentru-website-ul-lidl/s10058424) · [Lidl Plus legal info](https://www.lidl.ro/c/lidl-plus-informatii-legale/s10021655) · [robots.txt](https://www.lidl.ro/robots.txt) · [home page](https://www.lidl.ro/)
- Kaufland: [imprint (Despre noi)](https://www.kaufland.ro/despre-noi.html) · [Kaufland Card XTRA terms](https://www.kaufland.ro/regulament-privind-protectia-datelor/termeni-conditii-kaufland-card.html) · [robots.txt](https://www.kaufland.ro/robots.txt) · [weekly offers](https://www.kaufland.ro/oferte/prezentare-generala-oferte.html)
- Carrefour: [terms page](https://carrefour.ro/termene-si-conditii) · [site and account terms PDF, updated 26.07.2024](https://accounts.eu1.gigya.com/accounts.store.downloadPublicConsentDocument?docID=69434470_575788182010_996fee49b1554b4883b9e1742617bd63.pdf) · [robots.txt](https://carrefour.ro/robots.txt) · [grocery listing](https://carrefour.ro/bacanie-carrefour)
- Mega Image: [terms](https://www.mega-image.ro/termeni-si-conditii) · [robots.txt](https://www.mega-image.ro/robots.txt) · [listing](https://www.mega-image.ro/Fructe-si-legume-proaspete/c/001)
- Profi: [terms (live, not readable by our client)](https://www.profi.ro/termeni-si-conditii/) · [terms, archived 2025-08-08](https://web.archive.org/web/20250808041700/https://www.profi.ro/termeni-si-conditii/) · [robots.txt, archived 2025-09-02](https://web.archive.org/web/20250902101726/https://www.profi.ro/robots.txt)
- Penny: [terms](https://www.penny.ro/termeni-conditii) · [robots.txt](https://www.penny.ro/robots.txt) · [home page with offers](https://www.penny.ro/)
- Auchan: [terms](https://www.auchan.ro/termeni-si-conditii) · [robots.txt](https://www.auchan.ro/robots.txt) · [grocery listing](https://www.auchan.ro/bacanie/c)
- Selgros: [website terms](https://www.selgros.ro/termeni-si-conditii-website) · [robots.txt](https://www.selgros.ro/robots.txt) · [assortment](https://www.selgros.ro/exploreaza-sortimentul-selgros) · [online shop](https://shop.selgros.ro/)

**EU law and case law** (primary; retrieved via the Publications Office Cellar service)

- [Directive 96/9/EC on the legal protection of databases](https://eur-lex.europa.eu/eli/dir/1996/9/oj)
- [Directive (EU) 2019/790 (DSM), arts. 2–4, 7, recital 18](https://eur-lex.europa.eu/eli/dir/2019/790/oj)
- [Directive 2013/40/EU on attacks against information systems, arts. 2–3, recital 17](https://eur-lex.europa.eu/eli/dir/2013/40/oj)
- [Regulation (EU) 2023/2854 (Data Act), art. 43](https://eur-lex.europa.eu/eli/reg/2023/2854/oj)
- [Directive (EU) 2019/1024 (Open Data), art. 1](https://eur-lex.europa.eu/eli/dir/2019/1024/oj)
- [Implementing Regulation (EU) 2023/138 (High-Value Datasets)](https://eur-lex.europa.eu/eli/reg_impl/2023/138/oj)
- [Romanian transposition record for Directive 2019/1024 (Law 179/2022, MNE(2022)03782)](https://eur-lex.europa.eu/legal-content/EN/NIM/?uri=CELEX:32019L1024)
- [CJEU C-30/14 *Ryanair v PR Aviation*, 15 January 2015](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0030)
- [CJEU C-203/02 *British Horseracing Board v William Hill*, 9 November 2004](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62002CJ0203)
- [CJEU C-202/12 *Innoweb v Wegener*, 19 December 2013](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62012CJ0202)
- [CJEU C-762/19 *CV-Online Latvia v Melons*, 3 June 2021](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62019CJ0762)

**Romanian law** (primary; legislatie.just.ro, consolidated texts read 2026-10-21)

- [Criminal Code (Law 286/2009), arts. 181, 360, 363, 364, 366](https://legislatie.just.ro/Public/DetaliiDocument/109855)
- [Law 161/2003, art. 35](https://legislatie.just.ro/Public/DetaliiDocument/43323)
- [Law 8/1996 on copyright, arts. 36¹, 36², 140–143, 194](https://legislatie.just.ro/Public/DetaliiDocument/7816)
- [Civil Code (Law 287/2009), arts. 1.196, 1.202, 1.203](https://legislatie.just.ro/Public/DetaliiDocument/109884)
- [Law 179/2022 on open data and reuse of public-sector information](https://legislatie.just.ro/Public/DetaliiDocument/256414)
- [Law 544/2001 on free access to public-interest information](https://legislatie.just.ro/Public/DetaliiDocument/31413)
- [OUG 170/2020 (inserting Law 21/1996 art. 4(6))](https://legislatie.just.ro/Public/DetaliiDocumentAfis/231241)

**Monitorul Prețurilor and Comparables**

- [Monitorul Prețurilor home page and disclaimer](https://monitorulpreturilor.info/) (robots.txt: 404 on 2026-10-21)
- [Ticket #8 findings: Monitorul Prețurilor](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md) (project research; source of the platform facts marked as from #8)
- [gov2-ro/monitorulpreturilor](https://github.com/gov2-ro/monitorulpreturilor) (third-party reuse)
- [cijene-api README](https://github.com/senko/cijene-api) (secondary, for Croatia's NN 75/2025 decision)
- [Trolley.co.uk About page](https://www.trolley.co.uk/about/)
- [Project Overview, first-pass legal notes](https://github.com/exilonX/cart-compare/issues/1) (the starting brief verified above)
