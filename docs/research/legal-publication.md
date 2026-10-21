# What legal exposure does publishing comparisons and discount flags create?

Research for ticket [#10](https://github.com/exilonX/cart-compare/issues/10) on map [#1](https://github.com/exilonX/cart-compare/issues/1). Related tickets: [#9](https://github.com/exilonX/cart-compare/issues/9) (legality of *collecting* prices), [#11](https://github.com/exilonX/cart-compare/issues/11) (open data or code only), [#8](https://github.com/exilonX/cart-compare/issues/8) (Monitorul Prețurilor), [#6](https://github.com/exilonX/cart-compare/issues/6) (truthful cost-of-living comparisons). Desk research, 2026-10-21.

> **Not legal advice.** This is desk research by contributors to an open-source civic project. It was written from public primary sources (EUR-Lex and the EU Publications Office, CURIA, HUDOC, legislatie.just.ro, the Competition Council and Monitorul Prețurilor sites). Points that rest on secondary commentary are marked *(secondary)*. A Romanian IT and media lawyer must confirm the conclusions before launch. The questions to put to them are listed near the end.

**What is being published.** The [project overview](https://github.com/exilonX/cart-compare/issues/1) plans four features: a Basket ranking per Chain at Shelf price and at Loyalty price; weekly price history per product with a discount flag; a region and country view; and shareable social-media cards. This note assumes the project stays non-commercial (no ads, no affiliate links, no money from any Chain) and publishes only the Basket items (roughly 125 items per Chain), not a catalogue mirror. Section 10 covers the scenario raised after #8, where Shelf prices would come from the state-run Monitorul Prețurilor platform instead of our own collection. Section 11 covers Chains quoting the index in their own advertising.

## Answer

- **The exposure is civil, not criminal, and it is modest if we publish dated, verifiable facts with a published method.** The consolidated Romanian Criminal Code contains no offence of insult or calumny ([Criminal Code](https://legislatie.just.ro/Public/DetaliiDocument/109855)). The realistic risk is a civil claim by a Chain for harm to its reputation ([Civil Code art. 72, 253, 257, 1357](https://legislatie.just.ro/Public/DetaliiDocument/175630)). Good-faith exercise of free expression, within the European Convention on Human Rights, is not a breach (art. 75).
- **The discount flag is our largest exposure.** It implies that a Chain broke HG 947/2000 art. 4^1, an administrative offence fined at 5,000–30,000 lei and enforced by ANPC ([HG 947/2000](https://legislatie.just.ro/Public/DetaliiDocumentAfis/255257)). A flag is defensible only as a narrow, mechanical, evidenced check, such as "the prior price shown is higher than the lowest price we recorded in the previous 30 days". It should never say "fake", "fals" or "înșelătorie".
- **Romania's rule differs from the bare EU rule in ways that matter for groceries.** It has a 10-day window for perishable goods, special rules for new products and progressive reductions, and it measures the prior price per sales area ([HG 947/2000 art. 4^1](https://legislatie.just.ro/Public/DetaliiDocumentAfis/255257)). Weekly snapshots cannot reliably test perishable goods.
- **Loyalty prices are only partly covered by the 30-day rule.** The rule does not cover standing loyalty-programme discounts or personalised vouchers. It does cover member-only reductions announced to the public when many or most customers are members, and then the reference is the lowest publicly available price ([Commission guidance, s. 2.3](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52021XC1229%2806%29)). The Romanian text is silent on this, so Loyalty price flags are a lawyer question.
- **Unfair-competition and comparative-advertising law probably do not reach a non-commercial civic publisher.** Law 11/1991 targets enterprises denigrating competitors ([Law 11/1991 art. 2](https://legislatie.just.ro/Public/DetaliiDocument/1440)), and Law 158/2008 targets advertising that promotes sales ([Law 158/2008 art. 3](https://legislatie.just.ro/Public/DetaliiDocumentAfis/150055)). This changes if we take money from a Chain or monetise. If a Chain quotes our ranking in its own advertising, the law puts liability on that Chain, not on us ([Law 158/2008 art. 17](https://legislatie.just.ro/Public/DetaliiDocumentAfis/150055)). A published claims policy with a tie threshold keeps noise-level wins from being advertised as "cheapest" (section 11).
- **Chain names in plain text are lawful referential use; logos are not worth the risk.** Naming a Chain to identify it is referential use ([EUTMR art. 14(1)(c)](https://eur-lex.europa.eu/eli/reg/2017/1001/oj/eng); Law 84/1998 art. 45(1)(c), *(secondary consolidated copy)*). A civic project is probably not using marks "in the course of trade" at all. Logos add copyright and confusion risk for no informational gain, so cards should carry names only.
- **Open data is low risk at Basket scale.** Prices are facts, outside copyright ([Law 8/1996 art. 9(f)](https://legislatie.just.ro/Public/DetaliiDocument/7816)). The database right protects only substantial parts, and extraction is unlawful only where it harms the maker's investment ([C-762/19](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62019CJ0762)). The residual risks are contractual (account terms behind Loyalty prices) and a long, item-level history. This supports publishing Basket-level data and the item lists first.
- **Competition law is a design constraint, not a blocker.** The Commission lists price-comparison data as an efficiency gain ([Horizontal Guidelines, para. 425](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52023XC0721%2801%29)), and the Competition Council runs a price platform itself ([consiliulconcurentei.ro](https://www.consiliulconcurentei.ro/)). Our rules: only prices already public, no non-public feeds from Chains, nothing forward-looking, the same access for everyone.
- **Building on Monitorul Prețurilor data moves the risk rather than removing it.** Chain account terms drop out of the picture, and Law 179/2022 bars public bodies from using their database right to block reuse ([Law 179/2022 art. 1(7)](https://legislatie.just.ro/Public/DetaliiDocument/256414)). But the platform has no licence, its prices "may differ" from the shelf, and it shows a current price rather than the Chain's reduction announcement, so it cannot ground a discount flag on its own. We remain liable for what we publish, and the Chain is answerable to the Council for what it reported, as the 2022 fine on Mega Image shows ([Competition Council](https://www.consiliulconcurentei.ro/wp-content/uploads/2022/07/amenda-Mega-Image-iul-2022.pdf)).
- **Comparables survive by attributing, dating and qualifying every finding.** Which? and money.ro both do this, and money.ro also offers a right of reply ([Which?](https://www.which.co.uk/news/article/cheapest-supermarket-of-the-month-ag3nQ4J0v6ht), [money.ro](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)). Where companies took critics to court, the European Court of Human Rights sided with the critics. In Hertel the speech was in the public interest; in Steel and Morris the procedure was unfair. In both, the Court stressed good faith and accuracy ([Hertel](https://hudoc.echr.coe.int/eng?i=001-59366), [Steel and Morris](https://hudoc.echr.coe.int/eng?i=002-4006)).

## 1. Naming and ranking Chains

**Rule.**

- The Constitution makes freedom of expression "inviolabile" (art. 30(1)). It may not prejudice a person's dignity, honour or reputation (art. 30(6)), and civil liability for information made public lies with the publisher or author (art. 30(8)) ([Constitution](https://legislatie.just.ro/Public/DetaliiDocument/47355)).
- The Civil Code protects freedom of expression, which can be restricted only within the limits of art. 75 (art. 70). It forbids harm to honour and reputation outside those limits (art. 72(2)). Under art. 75, an interference allowed by law or by human-rights treaties is not a breach, and neither is the good-faith exercise of constitutional rights consistent with those treaties ([Civil Code](https://legislatie.just.ro/Public/DetaliiDocument/175630)).
- These protections apply by analogy to legal persons (art. 257), so a Chain can sue over its reputation.
- **Remedies.** Where the harm comes from free expression, a court may order only that the breach stop and be declared unlawful. It cannot ban a statement in advance (art. 253(2)). It may also order the judgment published and damages paid (art. 253(3)–(4)).
- **General tort.** Liability follows a wrongful act committed with fault (art. 1357(1)), and the author "răspunde pentru cea mai uşoară culpă" ("is liable for the slightest fault", art. 1357(2)). This makes data quality a legal issue, not just a product issue.
- **Criminal law.** The consolidated Criminal Code on legislatie.just.ro contains no offence of insult or calumny ([Criminal Code](https://legislatie.just.ro/Public/DetaliiDocument/109855)).
- **Convention standards** (reached through Civil Code art. 75). Large companies "inevitably and knowingly" lay themselves open to close scrutiny, and the limits of acceptable criticism are wider for them. Small campaign groups get Article 10 protection, provided they act in good faith to give accurate and reliable information. Statements of fact are judged more strictly than value judgments ([Steel and Morris v. the United Kingdom, Information Note 72](https://hudoc.echr.coe.int/eng?i=002-4006)).

**How it applies to us.** A ranking combines statements of fact ("this Basket totalled 412.30 lei at Chain A on 14 October") with a method-dependent conclusion ("cheapest"). True, dated and attributable facts with a published method are the best defence. The realistic failure modes are factual errors: a wrong product match, wrong pack size, a stale price, a regional price presented as national, or a Loyalty price mixed with a Shelf price. Given the "slightest fault" standard, each of these is a liability point.

**Risk level: Low**, provided the method is published and errors are corrected quickly.

**How Comparables handle it.**

- **Which?** attributes and dates every finding: "Aldi was the cheapest supermarket in September, according to the latest Which? analysis". It includes only loyalty prices that apply to all scheme members, excludes personalised discounts and multibuys, and warns that own-brand items "won't be identical across supermarkets". It keeps its product list confidential so supermarkets cannot game it ([Which?, 5 Oct 2026](https://www.which.co.uk/news/article/cheapest-supermarket-of-the-month-ag3nQ4J0v6ht)).
- **money.ro** builds its ranking from Monitorul Prețurilor and states:
  - "Comparația și calculele aparțin Money.ro, nu Consiliului Concurenței" ("the comparison and calculations are Money.ro's, not the Competition Council's");
  - that it compared the cheapest product of each type, not identical products;
  - that prices "pot diferi de cele afișate în magazin" ("may differ from those shown in store");
  - that the result reflects one day.

  It links a CSV, invites retailers to send a reply that it will publish in full, and promises visible, dated corrections ([money.ro, 10 Oct 2026](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)).
- **The state platform** itself says its prices are "pur informativ" ("purely informative"), that prices at the point of sale may differ and always prevail, and it disclaims liability ([Monitorul Prețurilor](https://monitorulpreturilor.info/)).
- **An analogy from advertising law.** When retailers compare Baskets in their own ads, the Court of Justice requires a representative selection, disclosure of differences that matter to shoppers, and verifiable items ([C-159/09 Lidl v Vierzon](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62009CJ0159)). Differences in store format must be stated in the ad itself ([C-562/15 Carrefour Hypermarchés](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62015CJ0562)). These rules bind advertisers, not us, but they are a good quality bar.

**Safe phrasing and design implications.**

- **Scope every claim.** Write "On 14 Oct 2026 the Family Basket (30 items, Bucharest, prices on Chain websites) cost X lei at Chain A and Y lei at Chain B", not "Chain A is Romania's cheapest supermarket".
- **Rank Shelf prices and Loyalty prices separately**, and label each.
- **Link every ranking** to the Basket item list, the matching rules and the substitution rule for missing items. Publishing the list (unlike Which?) supports verifiability, at the cost of letting Chains target those items.
- **Run a corrections channel.** Give Chains a contact address and a public corrections log, and add a dated correction note to any changed figure.
- **Keep evidence.** Store timestamped raw captures behind every published price.
- **Keep region and country comparisons factual.** Do not claim that a product differs in composition between countries without test evidence. "Dual quality" marketing is itself regulated as a misleading practice for traders ([Directive 2019/2161, inserting UCPD art. 6(2)(c)](https://eur-lex.europa.eu/eli/dir/2019/2161/oj/eng)).

## 2. Flagging a discount as not real

### 2.1 What the law requires of the Chain

**EU rule.** Directive 98/6/EC art. 6a, inserted by the Omnibus Directive 2019/2161:

- **(1)** "Any announcement of a price reduction shall indicate the prior price applied by the trader for a determined period of time prior to the application of the price reduction."
- **(2)** The prior price is "the lowest price applied by the trader during a period of time not shorter than 30 days".
- **(3)–(5)** Member States may set different rules for perishable goods, products on the market for less than 30 days, and progressively increased reductions.

([Directive 98/6/EC, consolidated](https://eur-lex.europa.eu/eli/dir/1998/6/2022-05-28/eng); text reproduced in the [Commission guidance](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52021XC1229%2806%29), s. 1.)

**The Commission's guidance** (not binding) says:

- The rule covers "20 % off", crossed-out "was/now" prices, and claims such as "sales" or "Black Friday offers" that create the impression of a reduction.
- It does not cover price changes made without a reduction announcement, general "best/lowest prices" claims, or tied offers such as "buy one, get two" (s. 1.1).
- The prior price must include any earlier promotional price in the 30-day window, and any percentage must be calculated from that prior price (s. 2.1).
- The prior price is set per sales channel or point of sale, for example online versus a physical shop (s. 2.1).
- The rule binds the seller, not intermediaries "that merely aggregate and display information about the prices provided by other sellers (price comparison platforms)" (s. 1.2).
- Misleading price advantages outside art. 6a remain subject to the Unfair Commercial Practices Directive (s. 3).

**The Court of Justice applied the rule to groceries in Verbraucherzentrale Baden-Württemberg v Aldi Süd** (C-330/23, 26 September 2024). The case was brought by a German consumer association over a brochure advertising bananas at EUR 1.29 with EUR 1.69 struck through, when EUR 1.29 had been the price in a week within the previous 30 days. The Court ruled that a reduction announced "in the form of a percentage, or in the form of a promotional statement intended to highlight the advantageous nature of the announced price, must be determined on the basis of the 'prior price'" ([C-330/23](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62023CJ0330)).

**Romanian transposition: HG 947/2000 art. 4^1**, added by HG 686/2022 (Monitorul Oficial no. 520 of 26 May 2022, in force 28 May 2022) ([HG 947/2000, consolidated](https://legislatie.just.ro/Public/DetaliiDocumentAfis/255257)):

- **(1)** Every reduction announcement states the prior price "aplicat de vânzător în aceeași suprafață de vânzare" ("applied by the seller in the same sales area"). The Chain proves the prior price with its own documents at ANPC's request.
- **(2)** The prior price is the lowest price in that sales area in the 30 days before the reduction.
- **(3)** For "produselor susceptibile de a se deteriora sau a se perima rapid" ("goods liable to deteriorate or expire rapidly"), the window is **10 days**.
- **(4)** For products on sale for less than 30 days, the window is the period they have been on sale.
- **(5)** For reductions increased step by step in one campaign, the prior price is the price before the first reduction.
- **Sanction.** Breach of art. 4^1 is a contravention fined at 5,000–30,000 lei (art. 12(2)), established by ANPC inspectors (art. 13).
- **Overlap with misleading practices.** The other Omnibus changes were transposed into Law 363/2007 on unfair commercial practices and other acts by OUG 58/2022 ([DLA Piper](https://www.dlapiper.com/en-us/insights/publications/2022/05/change-of-an-era-geo-58-2022), *secondary*). A Romanian practitioner notes that failing to relate the discount to the 30-day lowest price can also be treated as a misleading commercial practice, and that ANPC tends to follow the Commission's guidance ([Lynx Legal](https://lynx.legal/?p=6225), *secondary*).
- **Scope question for the lawyer.** HG 947/2000 regulates prices of products "existente în suprafețele de vânzare" (art. 1). It defines "suprafață de vânzare" in physical terms: the area for customer access, display, payment and staff circulation (art. 2(e)). The Commission says art. 6a applies to online shops too. How the Romanian text reaches online prices, the main source for this project, is a lawyer question.

### 2.2 Does the 30-day rule apply to Loyalty prices?

**Partly.** Per the Commission's guidance, s. 2.3:

- **Not covered:** "customer loyalty programmes, such as discount cards or vouchers, which entitle the consumer to a price discount … during extended continuous periods", and genuinely personalised reductions such as a voucher after a purchase or a birthday discount.
- **Covered:** reductions that are "in reality offered/announced to consumers in general", for example "This weekend 20 % off on everything for loyalty members only", "where the code/the loyalty programme is accessible/used by many or the majority of customers". The prior price must then be "their lowest publicly available price in the last 30 days" ([Commission guidance](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52021XC1229%2806%29)).

HG 947/2000 does not mention loyalty schemes ([HG 947/2000](https://legislatie.just.ro/Public/DetaliiDocumentAfis/255257)). Which? similarly includes only loyalty prices that apply to all members of a scheme ([Which?](https://www.which.co.uk/news/article/cheapest-supermarket-of-the-month-ag3nQ4J0v6ht)).

**Implication.** A Loyalty price is not in itself an announced reduction. Flag it only if the Chain announces a member-only reduction (a crossed-out price or a percentage), the programme is widely used, and the test runs against the Shelf price history, which is the lowest publicly available price. Until a lawyer confirms ANPC's position, show Loyalty price history without flags.

### 2.3 Our exposure

- **We are not the addressee of art. 6a.** The Commission expressly excludes price-comparison intermediaries (s. 1.2).
- **The risk is the statement itself.** A flag tells the public that a named Chain displayed an unlawful prior price. If the flag is wrong, it is a false statement of fact damaging a legal person's reputation, actionable under Civil Code art. 72, 253, 257 and 1357 ([Civil Code](https://legislatie.just.ro/Public/DetaliiDocument/175630)). The Chain could also claim lost sales.
- **Unfair-competition law (Law 11/1991)** is discussed in section 3. It probably does not apply to us.

**Risk level: Medium.** This is the highest exposure in the project, and it can be brought down to Low–Medium with the design below.

### 2.4 Designing a defensible flag

This subsection is our own analysis of how to apply the rule to weekly data; it is not drawn from a source.

- **A one-sided test.** We sample prices once a week. The lowest price we observed in a window is therefore always greater than or equal to the true lowest price in that window. If the prior price the Chain shows is *higher* than our observed lowest price (same product, same channel, same region), it cannot be the true lowest price, so the test cannot produce a false positive from sampling alone. The converse does not hold: if the shown prior price is equal to or below our minimum, we cannot conclude that the Chain complied, so we stay silent.
- **A second check.** Test whether a displayed percentage ("-30%") is consistent with the prior price we observed ([C-330/23](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62023CJ0330)).
- **Sources of false positives, all of which must be excluded:**

| Situation | Why it can mislead | Design response |
|---|---|---|
| Perishable goods | 10-day window (HG 947/2000 art. 4^1(3)); a weekly sample has only 1–2 points in it | Do not flag fresh or perishable items at weekly cadence |
| Product on sale for less than 30 days | Window shortens (art. 4^1(4)) | Flag only once we have seen the product for at least 30 days |
| Step-by-step campaign | Prior price is the pre-campaign price (art. 4^1(5)) | Exclude our own observations taken inside the same campaign |
| Multibuy or conditional offers | Outside art. 6a (Commission guidance s. 1.1) | Never flag them |
| Loyalty-only offers | Covered only when announced to the public and widely used (s. 2.3) | Do not flag until a lawyer confirms |
| Different channel or store | Prior price is set per sales area or channel (art. 4^1(1); guidance s. 2.1) | Compare only like with like: same website, region and store type |
| Matching or pack-size error | A false fact | Exact product and size match; a human review before publishing |
| Raised price without an announcement | Not covered by art. 6a | Show it as history only, never as a flag |

- **Evidence.** Keep the raw capture (time, URL, HTML or screenshot) of the promotion and of every observation in the window, and show the observations under the flag.
- **Wording.** Rename the "suspicious discount" flag to a neutral "Prior-price check" ("Verificare preț anterior"). Example:
  - EN: "On 14 Oct, [Chain] showed this product reduced from 12.99 lei. The lowest price we recorded on [Chain]'s website in the 30 days before was 10.49 lei (7 Oct). HG 947/2000 art. 4^1 requires the prior price shown to be the lowest price of the last 30 days. Our records: [link]. Corrections: [address]."
  - RO: "Pe 14 oct., [Lanț] a afișat produsul redus de la 12,99 lei. Cel mai mic preț înregistrat de noi pe site-ul [Lanț] în cele 30 de zile anterioare a fost 10,49 lei (7 oct.). HG 947/2000 art. 4^1 prevede că prețul anterior afișat este cel mai scăzut preț din ultimele 30 de zile. Înregistrările noastre: [link]. Corecturi: [adresă]."
  - Avoid: "fake", "fals", "înșelătorie", "păcăleală", "suspect", "ilegal", "a încălcat legea". Let ANPC, not us, decide whether there was a breach. Shoppers can complain to ANPC ([anpc.ro](https://anpc.ro/)).
- **Notice and reply.** Consider sending each flag to the Chain's contact point a few days before it goes public, and publishing the reply next to it, as money.ro does for rankings ([money.ro](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)). Whether this is legally advisable is a lawyer question.
- **No flags on shareable cards.** A card travels without its evidence and caveats. Keep flags on product pages, where the observations sit beside them.

**How Comparables handle it.** In Germany a consumer association took the Chain to court over a grocery discount instead of labelling it publicly, which produced C-330/23 ([C-330/23](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62023CJ0330)). Which?'s monthly analysis ranks Baskets and does not flag individual discounts ([Which?](https://www.which.co.uk/news/article/cheapest-supermarket-of-the-month-ag3nQ4J0v6ht)). We found no Comparable that publishes per-product "fake discount" labels against named Romanian Chains.

## 3. Unfair competition (Law 11/1991)

**Rule.**

- Enterprises must act according to honest practices (art. 1(2)), and the law applies to enterprises and natural persons who commit unfair-competition practices (art. 1(3)) ([Law 11/1991](https://legislatie.just.ro/Public/DetaliiDocument/1440)).
- **Prohibited practices of "the enterprise"** (art. 2(1)):
  - (a) denigrating "unei întreprinderi concurente" ("a competing enterprise") by another enterprise communicating "informații care nu corespund realității" ("information that does not correspond to reality");
  - (c) discrediting a competing enterprise by other means;
  - (d) any other commercial practice contrary to honest practices that harms competitors.
- **"Practici comerciale"** means an enterprise's conduct "în legătură directă cu producerea, furnizarea, promovarea și comercializarea unui produs" ("directly connected with producing, supplying, promoting or selling a product", art. 1^1(b)).
- **Enforcement.**
  - The Competition Council enforces the law (art. 2^1(1)).
  - Fines are 50,000–500,000 lei for legal persons where the public interest is affected (art. 4(1)).
  - Anyone with a legitimate interest may sue, including for an urgent interim injunction (art. 7(1), 7(3)).
  - Using a firm name, emblem or packaging "de natură să producă confuzie" ("liable to cause confusion") with another trader's is a criminal offence (art. 5(a)).

**How it applies to us.** The law is built around an enterprise acting against a competitor. A civic project that sells nothing is not a competitor of grocery Chains, and its publications are not commercial practices connected with selling a product, so we are probably outside it. The contrast with Switzerland is instructive. Swiss unfair-competition law required "no competitive relationship", and a household-appliance makers' association used it against a scientist's statements about microwave ovens. The European Court of Human Rights found a violation of Article 10 because he had "participated in a debate affecting the general interest" ([Hertel v. Switzerland](https://hudoc.echr.coe.int/eng?i=001-59366); [case summary](https://hudoc.echr.coe.int/eng?i=002-6815)). Romania's text is narrower than the Swiss one.

**Risk level: Low** while non-commercial. **Medium** if the project takes money or data deals from a Chain or its competitors, earns affiliate revenue from retailers, or is run by someone working in grocery retail or supply. Each of these makes it arguable that our publications are an enterprise's commercial practice.

**Design implications.**

- Adopt a funding policy: no money, sponsorship or data deals from any Chain, grocery supplier or retail-adjacent business, and publish the project's funding sources.
- Keep cards visually distinct from any Chain's communications (see section 5), to stay clear of art. 5(a).

## 4. Comparative advertising (Law 158/2008, Directive 2006/114/EC)

**Rule.**

- "Publicitate" is any presentation of a commercial, industrial, craft or professional activity "în scopul promovării vânzării de bunuri ori servicii" ("to promote the sale of goods or services", art. 3(a)). Comparative advertising is advertising that identifies a competitor or its goods (art. 3(c)) ([Law 158/2008, republished](https://legislatie.just.ro/Public/DetaliiDocumentAfis/150055)).
- Comparative advertising is lawful only if it meets all of the conditions in art. 6, including that it is not misleading, compares objectively, does not denigrate, and creates no confusion.
- The Ministry of Finance and ANPC enforce it (art. 7). The law transposes [Directive 2006/114/EC](https://eur-lex.europa.eu/eli/dir/2006/114/oj/eng).

**How it applies to us.** We do not promote the sale of our own goods or services, so our rankings are not advertising, and the law should not apply to a non-advertiser publisher.

It matters in two other ways:

- **If a Chain cites our results in its own advertising** ("cheapest according to the Grocery Basket Index"), that advertising is comparative advertising and the Chain must meet art. 6. The case law asks for a representative selection, verifiable items and disclosed format differences ([C-159/09](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62009CJ0159), [C-562/15](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62015CJ0562)). Trademark law separately lets owners stop use of their mark in unlawful comparative advertising ([Law 84/1998 art. 39(3)(f)](https://www.euroavocatura.ro/legislatie/1785/Legea_nr__84_1998__Republicata_si_actualizata_2020,_privind_marcile_si_indicatiile_geografice), *secondary consolidated copy*; [EUTMR art. 9(3)(f)](https://eur-lex.europa.eu/eli/reg/2017/1001/oj/eng)).
- **The criteria are a good quality bar for our own method**: representative Baskets, interchangeable products, verifiable items, disclosed format and region differences.
- **Joint liability.** Law 148/2000 art. 18, as amended by Law 158/2008, makes the author, the producer of the advertising and the medium jointly liable with the advertiser ([Law 158/2008 art. 23](https://legislatie.just.ro/Public/DetaliiDocumentAfis/150055)). That is a reason to take no part in producing any Chain's advertising.

**Risk level: Low / not applicable**, while we neither advertise nor produce ads for anyone.

**Design implications.** Publish a short "using our results" policy (detailed in section 11). Media and NGOs may cite freely with date and Basket. If a Chain cites us in advertising, it must reproduce the date, the Basket, the price type and a link to the method, and we may publicly state that we do not endorse any Chain.

## 5. Chain names and logos on shareable cards

**Rule.**

- **The EU trade mark.** It lets the owner stop third parties "using in the course of trade" identical or similar signs (art. 9(2)). It does not let the owner stop use "for the purpose of identifying or referring to goods or services as those of the proprietor" (art. 14(1)(c)), provided the use is "in accordance with honest practices in industrial or commercial matters" (art. 14(2)). Recital 21 adds that the Regulation must respect "the freedom of expression" ([Regulation 2017/1001](https://eur-lex.europa.eu/eli/reg/2017/1001/oj/eng)).
- **"Course of trade"** means use "in the context of commercial activity with a view to economic advantage and not as a private matter" ([C-206/01 Arsenal v Reed, para. 40](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62001CJ0206)).
- **Use is not honest if** it gives the impression of a commercial connection with the owner, takes unfair advantage of the mark's repute, discredits or denigrates it, or presents goods as imitations ([C-228/03 Gillette](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62003CJ0228)).
- **Romania's Law 84/1998**, republished 2020 ([WIPO Lex record](https://www.wipo.int/wipolex/en/legislation/details/22204)), mirrors this. Infringement requires use "în activitatea lor comercială" ("in their commercial activity", art. 39(2)). Art. 45(1)(c) allows use of a mark "pentru a identifica sau a face o trimitere la produse sau servicii ca fiind ale titularului" ("to identify or refer to goods or services as those of the owner"), subject to "practicile loiale" ("honest practices", art. 45(2)). This text was read in a secondary consolidated copy ([euroavocatura](https://www.euroavocatura.ro/legislatie/1785/Legea_nr__84_1998__Republicata_si_actualizata_2020,_privind_marcile_si_indicatiile_geografice)).
- **Logos.** A logo can also be an original graphic work protected by copyright ([Law 8/1996 art. 7](https://legislatie.just.ro/Public/DetaliiDocument/7816)), and confusing use of another trader's emblem is a criminal offence ([Law 11/1991 art. 5(a)](https://legislatie.just.ro/Public/DetaliiDocument/1440)).

**How it applies to us.**

- **Names.** Naming a Chain is necessary to say whose prices these are. Non-commercial civic use is probably not "in the course of trade" at all, and even if it were, it is referential use.
- **Logos.** A logo is not needed to identify a Chain. It raises the impression of affiliation or endorsement, brings in the artwork's copyright, and on a card shared out of context could look like the Chain's own communication.

**Risk level: names Low; logos Low–Medium.**

**Design implications for cards.**

- Write Chain names in plain text in our own typeface. Use no Chain logos, colours, fonts, product photos or leaflet images; product photos and leaflet layouts are themselves copyright works.
- Make our own brand dominant and add a footer line: "Independent index. Not affiliated with or endorsed by any retailer. Names belong to their owners."
- Put the caveats on the card itself, as the Court required for advertisers in [C-562/15](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62015CJ0562): date, Basket name, city, price type (Shelf or Loyalty), data source and method URL.
- Use no superlatives that the data do not support, and no discount flags.

## 6. Press freedom and public-interest protections

- **Protective, but not a shield for false facts.** Constitution art. 30 ([Constitution](https://legislatie.just.ro/Public/DetaliiDocument/47355)), Civil Code art. 75 ([Civil Code](https://legislatie.just.ro/Public/DetaliiDocument/175630)) and Article 10 of the Convention protect public-interest speech. This includes speech by people who are not journalists, provided they act in good faith on accurate and reliable information ([Steel and Morris](https://hudoc.echr.coe.int/eng?i=002-4006)).
- **A narrower margin for speech that is not purely commercial.** States' margin to restrict speech is reduced where a speaker "had not made purely commercial statements, but had participated in a debate affecting the general interest" ([Hertel](https://hudoc.echr.coe.int/eng?i=002-6815)). Grocery prices during high food inflation are plainly a matter of general interest.
- **Equality of arms.** When a large company sues campaigners, procedural fairness and equality of arms are required, and the chilling effect is a relevant factor ([Steel and Morris](https://hudoc.echr.coe.int/eng?i=002-4006)).
- **No pre-publication bans.** A Romanian court cannot ban speech in advance in a personality-rights case. It can order only cessation and a declaration of unlawfulness (Civil Code art. 253(2)).
- **The anti-SLAPP Directive** protects persons engaged in "public participation" on "a matter of public interest" (art. 4) against manifestly unfounded or abusive civil proceedings ([Directive 2024/1069](https://eur-lex.europa.eu/eli/dir/2024/1069/oj/eng)). The transposition deadline was 7 May 2026 (art. 22). It covers only matters "with cross-border implications". A matter is domestic when both parties are domiciled in the court's Member State and all other elements are there too (art. 5(1)). A Romanian subsidiary of a Chain suing a Romanian project in a Romanian court is likely domestic. We did not verify whether Romania has transposed the Directive, or extended it to domestic cases.

**Risk relevance.** These protections lower the risk for honest, careful publication. They do not protect a wrong flag presented as fact.

## 7. Redistributing collected prices as open data

**Rule.**

- **Copyright.** Mere facts and data are not protected by copyright ("simplele fapte și date", [Law 8/1996 art. 9(f)](https://legislatie.just.ro/Public/DetaliiDocument/7816)).
- **The sui generis database right.** It protects a maker who made a "substantial investment in either the obtaining, verification or presentation of the contents" against extraction or re-use of all or a substantial part (art. 7(1)). It also covers "repeated and systematic extraction" of insubstantial parts that conflicts with normal exploitation of the database (art. 7(5)). A lawful user may always extract insubstantial parts "for any purposes whatsoever" (art. 8(1)), and contract terms to the contrary are void (art. 15) ([Directive 96/9/EC](https://eur-lex.europa.eu/eli/dir/1996/9/oj/eng)). Romania mirrors this in Law 8/1996 art. 140–142 ([Law 8/1996](https://legislatie.just.ro/Public/DetaliiDocument/7816)).
- **How the Court of Justice reads it:**
  - Investment in *creating* the data does not count; only investment in seeking out, collecting and verifying existing data does ([C-203/02 BHB v William Hill](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62002CJ0203)). A Chain creates its own prices.
  - A dedicated meta-search engine that reproduces a database's search function re-uses it ([C-202/12 Innoweb](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62012CJ0202)).
  - Extraction can be prohibited only where it is a "risk to the possibility of redeeming that investment through the normal operation of the database" ([C-762/19 CV-Online Latvia](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62019CJ0762)).
  - Where no database right exists, a website can still restrict use by contract ([C-30/14 Ryanair v PR Aviation](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0030)).
- **Exceptions.** The research exception covers extraction only, for non-commercial research, not making data available to the public ([Directive 96/9/EC art. 9(b)](https://eur-lex.europa.eu/eli/dir/1996/9/oj/eng); [Law 8/1996 art. 142(4)(b)](https://legislatie.just.ro/Public/DetaliiDocument/7816)). The text-and-data-mining exception also covers extraction, not re-use, and rightholders can opt out in machine-readable form ([Directive 2019/790 art. 4](https://eur-lex.europa.eu/eli/dir/2019/790/oj/eng)).

**How it applies to us.**

- **Scale.** Roughly 125 Basket items per Chain, set against catalogues of around 30,000 products ([project overview](https://github.com/exilonX/cart-compare/issues/1)), is a fraction of a per cent, so quantitatively insubstantial.
- **Substitution.** A Basket index does not substitute for a Chain's shop, so CV-Online's harm test is unlikely to be met.
- **The open point** is art. 7(5): a weekly, multi-year, item-level history of the same items. It never rebuilds the catalogue, but a lawyer should confirm.
- **The larger risk is contract, not database right.** Loyalty prices are visible only behind a Chain account whose terms we accept, and those terms may limit reuse (Ryanair). Publishing item-level Loyalty prices is the riskiest open-data choice. This overlaps with #9.
- **Licensing.** We can licence only rights we hold: our code, method, Basket definitions, matching tables and our compilation. The dataset licence should say we claim no rights in Chains' prices.

**Risk level:**

| Option | Risk |
|---|---|
| Basket totals and trends | Low |
| Item-level Shelf prices for Basket items | Low |
| Item-level Loyalty prices | Medium (contract) |
| A full-catalogue mirror (already out of scope) | High |

**How Comparables handle it.** In Croatia, Government Decision NN 75/2025 obliges retailers to publish price lists for direct price control. Open-source projects such as cijene-api (licensed AGPL) rely on that decision as their basis for downloading and redistributing prices ([cijene-api README](https://github.com/senko/cijene-api), *secondary for the Croatian decision*). We found no Romanian equivalent obliging retailers to publish machine-readable price lists for reuse. Monitorul Prețurilor is covered in section 10.

**Implications for #11 (open data or code only).**

- A defensible first step is to publish the code, the method, the Basket item lists and matching rules, Basket-level totals and history, and item-level Shelf prices for Basket items.
- Hold back item-level Loyalty prices until the account terms are reviewed.
- Use CC BY 4.0 or CC0 for our own contributions. These are the two licences Romanian open-data law recommends for public bodies ([Law 179/2022 art. 11(4)](https://legislatie.just.ro/Public/DetaliiDocument/256414)), which makes them a familiar choice.

## 8. Competition law

**Rule.**

- Art. 101 TFEU and Romanian Law 21/1996 art. 5(1) prohibit agreements and concerted practices between undertakings that restrict competition, in particular those that "stabilesc, direct sau indirect, prețuri" ("fix prices, directly or indirectly") ([TFEU art. 101](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:12016E101); [Law 21/1996](https://legislatie.just.ro/Public/DetaliiDocument/8005)).
- **The Commission's 2023 Horizontal Guidelines** ([2023/C 259/01](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52023XC0721%2801%29)) say:
  - Information can be exchanged indirectly "through a third party (such as a service provider, platform, online tool or algorithm)" (para. 368).
  - Information put in the public domain for legitimate reasons and "readily accessible … to all competitors and customers" is usually not commercially sensitive (para. 388).
  - A further exchange can still reduce uncertainty if it is more granular or more frequent than what is public (para. 389).
  - Aggregated data and historical data are less likely to restrict competition (paras. 391, 393).
  - The effect depends on how far the exchange changes the existing level of transparency (para. 424).
  - Publishing "price comparison data" is listed as an efficiency that helps consumers "make more informed choices" (para. 425).
- **Facilitators.** A third party that actively and knowingly contributes to a cartel can itself be liable ([C-194/14 P AC-Treuhand](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0194)).
- **The classic warning.** In 1993 the Danish authority published firm-specific *transaction* prices for ready-mixed concrete, and average prices rose 15–20% within a year. The authors attribute the rise to reduced oligopoly price competition ([Albæk, Møllgaard and Overgaard, 1997](https://doi.org/10.1111/1467-6451.00057)).

**How it applies to us.** We are not party to any agreement between Chains. Consumer shelf prices are already public to everyone, unlike the Danish transaction prices, so our incremental transparency is small: mainly Basket aggregation and history. The national competition authority runs Monitorul Prețurilor itself and lists it among its platforms ([consiliulconcurentei.ro](https://www.consiliulconcurentei.ro/)). Since 2020, Law 21/1996 obliges companies to send the Council their sale prices on request for "comparații de preț incluse în platformele on-line destinate informării consumatorilor" ("price comparisons included in online platforms intended to inform consumers") ([Law 21/1996 art. 4](https://legislatie.just.ro/Public/DetaliiDocument/8005)). We infer that the authority sees publishing retail prices as serving consumers.

**Risk level: Very low** for us. A theoretical facilitation risk arises only if we handle non-public data or become a channel between Chains.

**Design rules.**

- Publish only prices that every consumer can see.
- Accept no non-public data from Chains. If a Chain offers a feed, as the overview's partnership idea suggests, it should contain only what the Chain already shows consumers, and no Chain should see another's data before the public does.
- Publish nothing forward-looking, such as future prices or announced intentions, unless the Chain has already made it public to consumers.
- Offer no private dashboards, alerts or early access for any Chain. Everyone gets the same public data at the same time.
- Write no editorial commentary that could read as signalling, for example "Chain X has room to raise prices".

## 9. If the project changes shape (monetisation)

The Unfair Commercial Practices Directive applies to a "trader", meaning a person acting "for purposes relating to his trade, business, craft or profession" ([Directive 2005/29/EC art. 2(b)](https://eur-lex.europa.eu/eli/dir/2005/29/oj/eng)). Since the Omnibus Directive, traders that let consumers search products offered by different traders must disclose "the main parameters determining the ranking" and their relative importance ([Directive 2019/2161, inserting UCPD art. 7(4a)](https://eur-lex.europa.eu/eli/dir/2019/2161/oj/eng)). Romania transposed this through OUG 58/2022 ([DLA Piper](https://www.dlapiper.com/en-us/insights/publications/2022/05/change-of-an-era-geo-58-2022), *secondary*).

Ads, affiliate links or paid placements would likely make the project a trader for those practices, and the unfair-competition analysis in section 3 would change. Publishing our ranking parameters costs nothing and already matches the overview's plan.

## 10. Building on Monitorul Prețurilor data instead of our own collection

Ticket #8 found that the Competition Council owns and runs Monitorul Prețurilor, that the Chains upload the data, and that there is no licence, reuse terms, API or history. It also found that third parties already republish the data: the gov2-ro mirror and money.ro's Basket ranking with a CSV ([#8 findings](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md)).

### 10.1 What changes compared with collecting the data ourselves

**What the platform says about itself:**

- It aims to let consumers compare the price of a basket, but "nu își propune să fie un comparator de prețuri" ("does not aim to be a price comparator") ([Retail description](https://monitorulpreturilor.info/Home/Retail/Descriere)).
- Its prices are "pur informativ" ("purely informative") and are not offers. Prices at the point of sale "pot diferi" ("may differ"), and "prețurile valabile fiind întotdeauna cele afișate la punctul de vânzare" ("the valid prices are always those displayed at the point of sale").
- Some discounts are marked only in store or applied at the till.
- The Council and participants accept no liability for the information, nor "pentru utilizarea ilicită de către terți a informațiilor afișate pe site" ("for unlawful use by third parties of the information shown on the site") ([Monitorul Prețurilor home](https://monitorulpreturilor.info/)).

**Database right.** The Council invested public money in obtaining and presenting the data, so it could in principle be a database maker ([Law 8/1996 art. 140(4)](https://legislatie.just.ro/Public/DetaliiDocument/7816)). Two points cut against any claim:

- **The Council.** Romanian open-data law says public entities do not exercise the database maker's right "pentru a împiedica reutilizarea documentelor" ("to prevent reuse of documents") beyond the limits of that law ([Law 179/2022 art. 1(7)](https://legislatie.just.ro/Public/DetaliiDocument/256414); [Open Data Directive art. 1(6)](https://eur-lex.europa.eu/eli/dir/2019/1024/oj/eng)), provided the data fall within that law (see below).
- **The Chains.** Their claim to a database right in the prices they create and upload is weak under BHB ([C-203/02](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62002CJ0203)).

**Public-sector information and open-data law.**

- **Law 179/2022** makes documents within its scope "reutilizabile în scopuri comerciale sau necomerciale" ("reusable for commercial or non-commercial purposes", art. 3) ([Law 179/2022](https://legislatie.just.ro/Public/DetaliiDocument/256414)).
  - Any reuse conditions must be "obiective, proporționale, nediscriminatorii" ("objective, proportionate, non-discriminatory") and must not restrict competition (art. 11(1)).
  - Anyone may file a reuse request, which must be answered within 30 working days. A refusal must be reasoned within 15 working days and can be challenged at the Romanian Digitalisation Authority (ADR) (art. 4–5).
- **Exclusions:** documents on which third parties hold intellectual property rights (art. 1(2)(c)) and documents shielded by commercial secrecy (art. 1(2)(d)(iii)). The second hardly fits prices the platform already publishes.
- **The scope question.** The Romanian law covers documents held by public entities "pe care acestea le-au creat în cadrul activității proprii" ("which they created in their own activity", art. 1(1)). The Directive's wording is wider: "existing documents held by public sector bodies" ([Directive 2019/1024 art. 1(1)(a)](https://eur-lex.europa.eu/eli/dir/2019/1024/oj/eng)). Whether a compilation of prices uploaded by retailers counts as a document "created" by the Council is the key uncertainty for the lawyer.

**Contract.** The platform publishes no reuse terms ([#8 findings](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md)), so there is no contract equivalent to a Chain's account terms. #8 notes that the platform's searches are meant to work only from inside Romania; how to collect from it is a #9 question.

**Attribution duties.**

- No statute imposes attribution on reuse when no licence is set.
- If the Council adopts one of the two recommended licences, CC BY 4.0 would require attribution and CC0 would not ([Law 179/2022 art. 11(4)](https://legislatie.just.ro/Public/DetaliiDocument/256414)).
- Attribution is still good practice and evidence of good faith. So is making clear that the comparison is ours, because the Council says its platform is not a comparator. money.ro's wording is a ready model: "Comparația și calculele aparțin Money.ro, nu Consiliului Concurenței" ([money.ro](https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026)).
- Do not use the Council's name or logo in a way that suggests endorsement.

**Competition law.** The data are already public and compiled by the competition authority itself. Our added history is historical data, which is the less sensitive kind ([Horizontal Guidelines, para. 393](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52023XC0721%2801%29)). Risk stays very low.

**The glossary term.** A platform price is a price *reported by the Chain to the Council*, which the platform itself says may differ from the shelf. It is not the same thing as the Shelf price in the project glossary (CONTEXT.md): "the price any visitor sees without an account or loyalty card". Label it differently in the product and the data, for example "reported price".

### 10.2 Who is liable if a platform price is wrong

- **Toward the Council, the Chain answers for what it reported.**
  - In July 2022 the Council fined Mega Image 10.08 million lei for "furnizarea de informații inexacte privind prețurile" ("supplying inaccurate price information") in answers to a market inquiry. Its reported 3.69 lei/l sunflower-oil price was also shown in the app, but "produsul nu se regăsea, însă, în magazine la prețul indicat" ("the product could not be found in stores at that price").
  - The Council said this misled the authority and "consumatorii care folosesc Monitorul Prețurilor" ("consumers who use Monitorul Prețurilor").
  - The same release says the data "sunt încărcate de lanțurile de magazine" ("are uploaded by the store chains") ([Competition Council, July 2022](https://www.consiliulconcurentei.ro/wp-content/uploads/2022/07/amenda-Mega-Image-iul-2022.pdf)).
  - Since 2020, failing to send prices on request is itself fined 20,000–50,000 lei ([Law 21/1996 art. 4 and 54^2](https://legislatie.just.ro/Public/DetaliiDocument/8005)).
- **The Council disclaims liability** toward users ([Monitorul Prețurilor](https://monitorulpreturilor.info/)).
- **We remain liable for our own publications.** Civil liability for published information lies with the publisher or author ([Constitution art. 30(8)](https://legislatie.just.ro/Public/DetaliiDocument/47355)), and tort liability is fault-based ([Civil Code art. 1357](https://legislatie.just.ro/Public/DetaliiDocument/175630)).
  - Accurately reproducing a price the Chain itself reported to the regulator, and labelling it as such, is strong evidence that we were not at fault and acted in good faith (art. 75).
  - If the Chain's own wrong submission caused the harm, the Civil Code limits our liability to the part we caused. The victim's own fault (art. 1371(1)) or a third party's act (art. 1371(2)) reduces it.
  - The defence weakens if we knew, or should have known, that the data were wrong. #8 documents stale Cora prices and "0.0" prices ([#8 findings](https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md)). So data-quality checks are part of the legal defence, not only good engineering.
- **Rankings versus discount flags.**
  - **Rankings.** A ranking from platform data, worded as "prices reported by the Chains to Monitorul Prețurilor on [date]", is at Low risk, comparable to money.ro's approach.
  - **Flags.** A discount flag cannot rest on platform data alone. Art. 6a is triggered by the Chain's *announcement* of a reduction, made at the point of sale or in its own communications. As far as we and #8 could see, the platform shows a current reported price, not the announcement or the prior price the Chain displayed. It also warns that some discounts are marked only in store or applied at the till ([Monitorul Prețurilor](https://monitorulpreturilor.info/)). A flag therefore needs the Chain's own promotional display, captured from its site or leaflet. Platform history can only corroborate it.
  - **A potential advantage.** The platform is store-level, which matches HG 947/2000's "same sales area" better than a national website does ([HG 947/2000 art. 4^1(1)](https://legislatie.just.ro/Public/DetaliiDocumentAfis/255257)). This is worth exploring with the lawyer.
- **Comparables using platform data.** money.ro and the gov2-ro mirror republish platform-derived data. gov2-ro has no licence on its repository ([gov2-ro/monitorulpreturilor](https://github.com/gov2-ro/monitorulpreturilor)). We found no report of either being challenged. That is reassuring, but it is not legal authority.

**Risk level: Low** for rankings and Basket-level open data built on platform data with attribution and correct labelling. **Medium** for any discount flag that leans on platform data. **Unknown** for the formal reuse right, which a written request under Law 179/2022 would settle.

**A caution from Hungary.** Hungary's competition authority (GVH) runs Árfigyelő, a statutory equivalent of Monitorul Prețurilor. In 2023 it called an unofficial app that copied the data "az online Árfigyelő rendszer illetéktelen, engedély nélküli felhasználása" ("an unauthorised, unlicensed use of the online Árfigyelő system"), and announced civil and criminal steps against its makers ([Telex, 5 Aug 2023](https://telex.hu/belfold/2023/08/05/gvh-figyelmeztetes-kalozapplikacio-arfigyelo), *secondary*, via [#3 findings](https://github.com/exilonX/cart-compare/blob/research/cee-comparables/docs/research/cee-comparables.md)). A state operator can react badly to unannounced reuse. That is one more reason to ask the Council in writing before building on its data.

## 11. When a Chain quotes the index in its advertising

**What Comparables show** (from the #4 and #3 findings, *secondary*):

- **Chains advertise index wins.** Aldi UK issues a press release every month it tops Which?'s ranking ([#4 findings](https://github.com/exilonX/cart-compare/blob/research/western-comparables/docs/research/western-comparables.md)).
- **Regulators look hard at noise-level wins.** In March 2024 the UK advertising regulator (ASA) upheld a Sainsbury's complaint against an Aldi "Britain's cheapest Christmas dinner" ad that carried a Which? endorsement roundel. Which? had found 4p between Aldi and Lidl, and the ASA said: "While Aldi was technically the cheapest, this was by a negligible amount" ([Grocery Gazette, 20 Mar 2024](https://www.grocerygazette.co.uk/2024/03/20/aldi-ad-christmas-misleading)). Which? was not sanctioned, but said it was "disappointed that a Which? endorsement logo and our research was used" ([County Press/PA](https://countypress.co.uk/news/national/uk-today/24198333.aldi-cheapest-supermarket-advert-branded-misleading)).
- **Authorities can set a minimum gap.** In November 2025 the GVH closed a case over Lidl Hungary's "champion of low prices" slogan after Lidl made commitments, without finding an infringement. Lidl may make a monthly average-Basket claim only if it is at least 2.5% cheaper than the second-cheapest Chain, on the regulator's data ([Economx, 13 Nov 2025](https://www.economx.hu/magyar-gazdasag/2025/11/13/gvh-versenyhivatal-eljaras-lidl-arak-819279/), *secondary*, via [#3 findings](https://github.com/exilonX/cart-compare/blob/research/cee-comparables/docs/research/cee-comparables.md)).

### 11.1 Romanian rules for a Chain that cites a third-party index

**Comparative advertising (Law 158/2008).** An ad saying "cheapest according to the Grocery Basket Index" identifies competitors explicitly or implicitly, so it is comparative advertising (art. 3(c)). It must meet every condition of art. 6, including that it is not misleading and that it compares "în mod obiectiv" ("objectively") features that are "relevante, verificabile și reprezentative" ("relevant, verifiable and representative"), price included ([Law 158/2008](https://legislatie.just.ro/Public/DetaliiDocumentAfis/150055)). On a complaint, or on their own initiative, the Ministry of Finance or ANPC:

- ask the advertiser for "toate dovezile necesare privind exactitatea afirmațiilor" ("all evidence needed on the accuracy of the claims"), to be supplied quickly for comparative advertising (art. 9(1), (4));
- treat the claims as inexact if the evidence is missing, late or insufficient (art. 9(5));
- fine breaches 3,000–30,000 lei (art. 10);
- can order the ad stopped, or banned before it runs, without proof of actual harm or fault (art. 11);
- can require a corrective statement to be published at the advertiser's expense (art. 12).

Competitors, consumers and "asociațiile și organizațiile care au interes legitim" ("associations and organisations with a legitimate interest") can all complain (art. 7, 9). The Court of Justice's Basket cases set the bar for representativeness, disclosed differences and verifiable items ([C-159/09](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62009CJ0159), [C-562/15](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62015CJ0562)).

**Consumer law (ANPC).** A "cheapest" claim made to shoppers is also a commercial practice under the Unfair Commercial Practices Directive, transposed by Law 363/2007 ([Law 11/1991 art. 2^1(3)](https://legislatie.just.ro/Public/DetaliiDocument/1440) points to that law for consumers' economic interests). Two items on the Directive's blacklist matter here. A trader may not display "a trust mark, quality mark or equivalent without having obtained the necessary authorisation" (Annex I, point 2). Nor may it claim that it "has been approved, endorsed or authorised by a public or private body when he/it has not", or make such a claim "without complying with the terms of the approval, endorsement or authorisation" (point 4) ([Directive 2005/29/EC](https://eur-lex.europa.eu/eli/dir/2005/29/oj/eng)). A Chain presenting our ranking as an endorsement or badge risks both.

**Self-regulation (RAC).** The Romanian Advertising Council (Consiliul Român pentru Publicitate, RAC) approved the latest version of its Code of Practice in Commercial Communication on 15 December 2025 ([RAC Code](https://www.rac.ro/ro/cod/codul-de-practic%C4%82-%C3%8En-comunicarea-comercial%C4%82)). Under it:

- Communications must cite quantitative studies correctly, in a way "care să poată fi demonstrată și substanțiată pe toată perioada comunicării" ("that can be demonstrated and substantiated for the whole period of the communication"), and present statistics and their source "fără a exagera validitatea afirmațiilor" ("without exaggerating the validity of the claims") (art. 2(a)–(b)).
- The advertiser must be able to prove its data with evidence that is "actuale, relevante și documentate" ("current, relevant and documented") (art. 7.1).
- Comparison must meet conditions mirroring Law 158/2008 art. 6 (art. 12).
- The Ethics Committee can ask the advertiser for supporting documents (art. 42.6).

The Code binds RAC members, who agree to stop or change a communication the Ethics Committee finds in breach. We did not check which of the 8 Chains, or their agencies and media, are RAC members.

### 11.2 Does the index carry liability or a duty when a Chain quotes it?

- **Regulatory liability sits with the advertiser.** "Răspunderea revine comerciantului beneficiar al anunțului publicitar" ("liability lies with the trader who benefits from the advertisement", Law 158/2008 art. 17(1)), and the burden of proof is on the advertiser (art. 9) ([Law 158/2008](https://legislatie.just.ro/Public/DetaliiDocumentAfis/150055)).
- **Joint liability is limited to those who make or carry the ad.** Law 148/2000 art. 18, as amended, makes the author, the producer of the advertising and the medium jointly liable with the advertiser (Law 158/2008 art. 23). We stay outside that only if we take no part in making, approving or carrying any Chain's ad, and accept no payment or licence fee for the use of our results.
- **Civil liability does not grow, but the stakes do.** If our published figures are accurate and a Chain misquotes them, the misquote is the Chain's act. If our figures are wrong and a Chain advertises them, a competitor harmed by the ad could look to us in tort ([Civil Code art. 1357](https://legislatie.just.ro/Public/DetaliiDocument/175630)). This is the same exposure as in section 1, but an ad multiplies the harm.
- **No statutory duty to police use.** We found no rule requiring a publisher to monitor or correct how advertisers cite it.
- **Practical consequences remain.** A regulator or the RAC Ethics Committee examining a Chain's evidence will examine our method, as the ASA effectively did with Which?'s 4p result. Being associated with a misleading ad also damages a civic index's credibility.

**Risk level: Low** for us legally, while we stay out of ad production and payment. Reputational risk is **Medium** if noise-level wins are advertised.

### 11.3 What a published claims policy or tie threshold can do

Ranking facts are not copyright works ([Law 8/1996 art. 9(f)](https://legislatie.just.ro/Public/DetaliiDocument/7816)), so we cannot stop a Chain from stating them truthfully. A policy still helps in five ways:

1. **It removes noise-level "winners" at the source.** Define a tie threshold based on our measurement error: item substitutions, regional variation, sampling timing. Where two Chains' Basket totals differ by less than the threshold, show them as tied ("la egalitate"), not ranked. Optionally, show a "lowest total" label only after the lead holds for several consecutive weeks. The GVH's 2.5% gap for Lidl is one external reference point. Our own threshold should come from our error analysis (ticket #6), and Shelf and Loyalty rankings should each get their own.
2. **It gives regulators a benchmark.** If our published method says a gap is within a tie, a "cheapest" ad based on it is hard to substantiate under Law 158/2008 art. 9 or RAC Code art. 2(b). The policy does our enforcement work through the advertiser's burden of proof.
3. **It documents non-endorsement.** A clear "no endorsement, no badges" statement, together with UCPD Annex I point 4, makes any claim of endorsement by us a blacklisted practice by the Chain. If we licence our data under CC BY 4.0, its clause 2(a)(6) already says that nothing in the licence permits a user "to assert or imply that You are … connected with, or sponsored, endorsed, or granted official status by, the Licensor" ([CC BY 4.0 legal code](https://creativecommons.org/licenses/by/4.0/legalcode.en)). CC0 has no such clause, which is a point for the licence choice in #11.
4. **It sets citation conditions that reduce misquotes.** Cite the date, Basket, city and price type (Shelf or Loyalty), link the method, and do not extrapolate (for example, no "cheapest in Romania" from a Bucharest Basket). These conditions are enforceable only as licence terms on our data, or through a trademark in the index name if we register one. Otherwise they work as public norms that regulators and the press can point to.
5. **It commits us to correct misuse in public.** Publish a "misquote" note when a Chain overstates our results, and tell the Chain. Anyone may also complain to ANPC or the RAC. We should not offer a badge, roundel or "winner" logo at all: that is the device the ASA case turned on, and licensing one for money would make us commercial (section 3).

**Keep the policy unilateral.** We should set the threshold ourselves and publish it. We should not negotiate it jointly with the Chains: a collective arrangement among competing Chains about how they may advertise prices raises its own competition question, which belongs on the lawyer list.

## Questions for a Romanian IT lawyer

**Discount flag and consumer law**

1. Is a flag worded as in section 2.4 ("the prior price shown is higher than the lowest price we recorded in the previous 30 days") a defensible statement of fact? What evidence should we keep: our own timestamped captures, hashes, or periodic bailiff's reports of findings (procese-verbale de constatare)?
2. How does HG 947/2000 art. 4^1, framed around physical "suprafețe de vânzare", apply to online shops and to leaflet prices published on a website? Does Law 363/2007 cover the gap?
3. Which grocery products does ANPC treat as "susceptibile de a se deteriora sau a se perima rapid" (10-day window)? Has ANPC issued guidance?
4. Does ANPC follow the Commission guidance on loyalty programmes (s. 2.3)? Can we flag member-only app or card reductions, and against which reference price?
5. Should we notify the Chain and wait a few days before publishing a flag? Would that materially strengthen a good-faith defence (Civil Code art. 75) or reduce fault (art. 1357)? Should we also send flagged cases to ANPC, and does doing so before or after publication change our exposure?

**Liability, legal form and the unfair-competition perimeter**

6. Does Law 11/1991 art. 2 reach a non-profit, non-commercial publisher? Which facts would bring us within "întreprindere" or "practici comerciale": donations, grants, ads, affiliate links, or a maintainer employed in grocery retail or supply?
7. Which legal form limits personal liability for publications (an association under OG 26/2000, a foundation, or individual maintainers), and is media-liability insurance available to such a project?
8. Where can a Chain sue us, and could a country comparison that names a Chain's foreign sister company expose us to foreign defamation law?
9. Has Romania transposed the anti-SLAPP Directive 2024/1069, and does it extend to purely domestic cases?

**Trademarks and cards**

10. Is non-commercial civic use outside "activitatea comercială" (Law 84/1998 art. 39(2))? If we ever displayed Chain logos, would trademark, copyright or Law 11/1991 art. 5(a) be engaged?
11. Can we set binding conditions on Chains that cite our rankings in advertising, for example through the licence of our results?

**Open data and contracts (decision #11)**

12. Is a Chain's online shop a protected database under Law 8/1996 art. 140(4), given BHB (C-203/02)? Is a weekly Basket-level extract, and a multi-year item-level history, within art. 142(1), or could it be caught by art. 141(5)?
13. Do Chain account or app terms restrict publishing Loyalty prices, and are such terms enforceable against us? Does Law 8/1996 art. 142(1) override them, or does that depend on the database being protected (C-30/14)?
14. Which licence can we validly grant over a dataset containing Chains' prices (CC BY 4.0, ODbL or CC0), and what disclaimer must go with it?
15. Under what conditions could we accept data feeds from Chains without becoming a channel for information exchange under Law 21/1996 art. 5?

**Monitorul Prețurilor data (section 10)**

16. Is the Monitorul Prețurilor compilation a "document" the Council "created in its own activity" within Law 179/2022 art. 1(1), or does the Directive's wider "held by" wording govern? Do the Chains hold any rights that trigger the art. 1(2)(c) exclusion?
17. Absent any licence, may we republish platform prices and an open dataset derived from them? Should we file a reuse request under Law 179/2022 art. 4 to obtain a standard licence, and what happens if the Council refuses?
18. Do Law 21/1996 art. 4 (prices sent for "platformele on-line destinate informării consumatorilor") or art. 54^2 limit third-party reuse in any way?
19. If a Chain-reported price is wrong and our ranking repeats it with attribution, how is liability apportioned under Civil Code art. 1357 and 1371? Does the platform's own disclaimer that prices "may differ" weaken our good-faith defence?
20. Must or should we attribute the Council? How do we word attribution so it does not suggest endorsement, given the Council says the platform is not a comparator?

**Chains quoting the index in advertising (section 11)**

21. When a Chain cites our index in a comparative ad, is liability confined to the advertiser (Law 158/2008 art. 17)? Could any role on our side, such as a licence fee, approving copy, supplying data on request, or a media partnership, make us a "realizator" or medium jointly liable under Law 148/2000 art. 18?
22. Can a published claims policy (tie threshold, citation conditions, no-endorsement statement) be made binding on Chains? Possible routes are licence terms on our data (CC BY 4.0), a registered trademark in the index name, or website terms. Which is enforceable against a Chain that only reads our public pages?
23. If a Chain presents our ranking as an endorsement or badge, is that a blacklisted practice under the Law 363/2007 equivalent of UCPD Annex I point 2 or 4? Who should complain (ANPC, the Ministry of Finance, the RAC), and may we complain as an association with a "legitimate interest" (Law 158/2008 art. 7, 9)?
24. Would consulting the Chains on a common tie threshold, or hosting a joint code on how the index may be cited, raise competition concerns under Law 21/1996 art. 5? Is a purely unilateral policy safe?
25. If a regulator or court asks a Chain to substantiate a claim based on our index, can we be compelled to hand over our underlying data or captures? On what terms should we provide them voluntarily?

## Gaps and uncertainties

- **Search budget.** The shared web-search budget ran out midway through this research. Points we could not check:
  - Romania's transposition status of the anti-SLAPP Directive;
  - any ANPC guidance on loyalty prices or perishable goods;
  - whether Croatian price apps, DECO (Portugal), UFC-Que Choisir (France) or Stiftung Warentest (Germany) have faced legal challenges over price comparisons;
  - Romanian case law on NGOs or consumer groups criticising retailers' prices.

  We relied on direct fetches of known primary sources instead.
- **Law 84/1998.** It was read in a secondary consolidated copy (euroavocatura.ro). The official consolidated text on legislatie.just.ro was not retrieved. The article numbers (39, 45) follow that copy.
- **OUG 58/2022 and ANPC practice** rest on law-firm summaries (DLA Piper, Lynx Legal).
- **Versions.** HG 947/2000 was read as consolidated on 28 May 2022, the latest version the portal showed. The Civil Code page carries an older version label; the articles cited are stable as far as we know, but should be checked.
- **The Commission guidance is non-binding**, and Romanian courts and ANPC may read art. 6a differently.
- **Law 21/1996 numbering.** The duty to send prices appears as art. 4(5) in the consolidated text, while art. 54^2 cites it as art. 4(6).
- **Our own analysis.** The one-sided logic of the weekly-sampling test (section 2.4) is ours. A statistician and the lawyer should both check it.
- **Croatian decision NN 75/2025** is cited from a project README, not from the Narodne novine text.
- **Monitorul Prețurilor facts** (no licence, Romania-only access, data quality) come from ticket #8 and were not re-verified here, except for the platform's disclaimer, its description page and the Mega Image press release, which we read directly.
- **Advertising cases (section 11).** The ASA's Aldi ruling (2024) and the GVH's Lidl commitments (2025) are cited from media reports gathered by tickets #4 and #3. We could not retrieve the ASA ruling or the GVH decision themselves.
- **RAC membership.** We did not verify which of the 8 Chains, their agencies or their media are RAC members, so we do not know how far the RAC Code reaches them.
- **Tie threshold.** We give no specific value. It should come from our own measurement-error analysis.

## Sources

**EU law and guidance**

- Directive 98/6/EC on price indication, consolidated 28.05.2022 — https://eur-lex.europa.eu/eli/dir/1998/6/2022-05-28/eng
- Directive (EU) 2019/2161 (Omnibus) — https://eur-lex.europa.eu/eli/dir/2019/2161/oj/eng
- Commission Notice, Guidance on Article 6a of Directive 98/6/EC, OJ C 526, 29.12.2021 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52021XC1229%2806%29
- Directive 2005/29/EC (Unfair Commercial Practices) — https://eur-lex.europa.eu/eli/dir/2005/29/oj/eng
- Directive 2006/114/EC (misleading and comparative advertising) — https://eur-lex.europa.eu/eli/dir/2006/114/oj/eng
- Regulation (EU) 2017/1001 (EU trade mark) — https://eur-lex.europa.eu/eli/reg/2017/1001/oj/eng
- Directive 96/9/EC (databases) — https://eur-lex.europa.eu/eli/dir/1996/9/oj/eng
- Directive (EU) 2019/790 (copyright in the Digital Single Market) — https://eur-lex.europa.eu/eli/dir/2019/790/oj/eng
- Directive (EU) 2019/1024 (open data) — https://eur-lex.europa.eu/eli/dir/2019/1024/oj/eng
- Directive (EU) 2024/1069 (anti-SLAPP) — https://eur-lex.europa.eu/eli/dir/2024/1069/oj/eng
- TFEU art. 101 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:12016E101
- Guidelines on horizontal co-operation agreements, 2023/C 259/01 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52023XC0721%2801%29

**Court of Justice of the EU**

- C-330/23 Verbraucherzentrale Baden-Württemberg v Aldi Süd, 26.9.2024 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62023CJ0330
- C-159/09 Lidl v Vierzon Distribution, 18.11.2010 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62009CJ0159
- C-562/15 Carrefour Hypermarchés v ITM, 8.2.2017 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62015CJ0562
- C-206/01 Arsenal v Reed, 12.11.2002 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62001CJ0206
- C-228/03 Gillette v LA-Laboratories, 17.3.2005 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62003CJ0228
- C-203/02 British Horseracing Board v William Hill, 9.11.2004 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62002CJ0203
- C-202/12 Innoweb v Wegener, 19.12.2013 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62012CJ0202
- C-762/19 CV-Online Latvia v Melons, 3.6.2021 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62019CJ0762
- C-30/14 Ryanair v PR Aviation, 15.1.2015 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0030
- C-194/14 P AC-Treuhand v Commission, 22.10.2015 — https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:62014CJ0194

**European Court of Human Rights**

- Hertel v. Switzerland, no. 25181/94, 25.8.1998 — https://hudoc.echr.coe.int/eng?i=001-59366 (summary: https://hudoc.echr.coe.int/eng?i=002-6815)
- Steel and Morris v. the United Kingdom, no. 68416/01, 15.2.2005, Information Note 72 — https://hudoc.echr.coe.int/eng?i=002-4006

**Romanian law (legislatie.just.ro unless stated)**

- Constitution — https://legislatie.just.ro/Public/DetaliiDocument/47355
- Civil Code (Law 287/2009, republished) — https://legislatie.just.ro/Public/DetaliiDocument/175630
- Criminal Code (Law 286/2009) — https://legislatie.just.ro/Public/DetaliiDocument/109855
- HG 947/2000 on price indication, consolidated (incl. HG 686/2022) — https://legislatie.just.ro/Public/DetaliiDocumentAfis/255257
- Law 11/1991 on combating unfair competition — https://legislatie.just.ro/Public/DetaliiDocument/1440
- Law 158/2008 on misleading and comparative advertising, republished — https://legislatie.just.ro/Public/DetaliiDocumentAfis/150055
- Law 8/1996 on copyright and related rights — https://legislatie.just.ro/Public/DetaliiDocument/7816
- Law 21/1996 (Competition Law) — https://legislatie.just.ro/Public/DetaliiDocument/8005
- Law 179/2022 on open data and reuse of public-sector information — https://legislatie.just.ro/Public/DetaliiDocument/256414
- Law 84/1998 on trade marks, republished 2020: WIPO Lex record https://www.wipo.int/wipolex/en/legislation/details/22204; text read in a secondary consolidated copy https://www.euroavocatura.ro/legislatie/1785/Legea_nr__84_1998__Republicata_si_actualizata_2020,_privind_marcile_si_indicatiile_geografice

**Authorities and platforms**

- Consiliul Concurenței, home page listing Monitorul Prețurilor under its platforms — https://www.consiliulconcurentei.ro/
- Consiliul Concurenței, press release on the Mega Image fine, July 2022 — https://www.consiliulconcurentei.ro/wp-content/uploads/2022/07/amenda-Mega-Image-iul-2022.pdf
- Monitorul Prețurilor, home page disclaimer — https://monitorulpreturilor.info/
- Monitorul Prețurilor, retail description — https://monitorulpreturilor.info/Home/Retail/Descriere
- ANPC — https://anpc.ro/
- Consiliul Român pentru Publicitate (RAC), Codul de Practică în Comunicarea Comercială (version of 15.12.2025) — https://www.rac.ro/ro/cod/codul-de-practic%C4%82-%C3%8En-comunicarea-comercial%C4%82
- Creative Commons, CC BY 4.0 legal code — https://creativecommons.org/licenses/by/4.0/legalcode.en

**Comparables and secondary sources**

- Which?, "Aldi crowned the UK's cheapest supermarket in September", 5.10.2026 — https://www.which.co.uk/news/article/cheapest-supermarket-of-the-month-ag3nQ4J0v6ht
- money.ro, "Coșul cu 11 produse de bază în 7 supermarketuri", 10.10.2026 — https://www.money.ro/topul-zilei/acelasi-cos-in-7-supermarketuri-preturi-octombrie-2026
- gov2-ro, Monitorul Prețurilor alternative interface (repository) — https://github.com/gov2-ro/monitorulpreturilor
- cijene-api (Croatia), README — https://github.com/senko/cijene-api
- Albæk, Møllgaard and Overgaard, "Government-Assisted Oligopoly Coordination? A Concrete Case", Journal of Industrial Economics 45(4), 1997, 429–443 — https://doi.org/10.1111/1467-6451.00057
- DLA Piper, "Change of an era: GEO 58/2022", 11.5.2022 (secondary) — https://www.dlapiper.com/en-us/insights/publications/2022/05/change-of-an-era-geo-58-2022
- Lynx Legal, "Romania: 2022's Black Friday under review" (secondary) — https://lynx.legal/?p=6225
- Ticket #8 findings, "What does Monitorul Prețurilor do…" — https://github.com/exilonX/cart-compare/blob/research/monitorul-preturilor/docs/research/monitorul-preturilor.md
- Ticket #4 findings, Western basket indices and price apps — https://github.com/exilonX/cart-compare/blob/research/western-comparables/docs/research/western-comparables.md
- Ticket #3 findings, CEE Comparables — https://github.com/exilonX/cart-compare/blob/research/cee-comparables/docs/research/cee-comparables.md
- Grocery Gazette, "Aldi ad … misleading", 20.3.2024 (secondary) — https://www.grocerygazette.co.uk/2024/03/20/aldi-ad-christmas-misleading
- County Press (PA), "Aldi cheapest supermarket advert branded misleading", March 2024 (secondary) — https://countypress.co.uk/news/national/uk-today/24198333.aldi-cheapest-supermarket-advert-branded-misleading
- Economx, GVH and Lidl commitments, 13.11.2025 (secondary) — https://www.economx.hu/magyar-gazdasag/2025/11/13/gvh-versenyhivatal-eljaras-lidl-arak-819279/
- Telex, GVH warning on an unofficial Árfigyelő app, 5.8.2023 (secondary) — https://telex.hu/belfold/2023/08/05/gvh-figyelmeztetes-kalozapplikacio-arfigyelo
