# Grocery Basket Index

An open-source, civic-first index that prices the same grocery baskets across Romanian chains, regions and countries, so ordinary people and the press can see what a normal week of groceries really costs.

## Language

### The index

**Basket**:
A fixed, published set of quantities of Item specifications, standing for one household type's typical shop; several Baskets share one list of Item specifications.
_Avoid_: cart, shopping list

**Item specification**:
A written description of one Basket item (category, pack-size band and a quality tier set by measurable attributes) that the cheapest product on the shelf meeting it stands for, own brands included.
_Avoid_: product, SKU (one specific product)

**Price round**:
One week's visits to the named store of each Chain, in which every Item specification is priced from the shelf labels, all within the same 48 hours.
_Avoid_: scrape, crawl, snapshot

**Tie threshold**:
The smallest lead, as a share of the Basket total, at which a Chain may be named cheapest; below it the leading Chains are shown as tied.
_Avoid_: margin of error (until it is measured)

**Chain**:
A grocery retailer brand operating many stores, such as Lidl or Kaufland.
_Avoid_: store (one physical location), shop

**Shelf price**:
The price any visitor sees without an account or loyalty card.
_Avoid_: public price, list price

**Loyalty price**:
The price a Chain advertises to every holder of its loyalty card or app, obtained by identifying at the till; one number per product.
_Avoid_: member price, app price

**Personalised offer**:
A reduction that differs between loyalty members, such as targeted coupons, vouchers, points or bonus redemptions, spend-based discounts and test-group rates; never part of a Loyalty price.
_Avoid_: loyalty discount, coupon price

**Reported price**:
A price a Chain submits to Monitorul Prețurilor under its legal reporting duty; it may differ from the Shelf price actually on display. The index does not use Reported prices: Monitorul Prețurilor is not part of the project.
_Avoid_: official price, shelf price (when the source is Monitorul Prețurilor)

### The exploration

**Comparable**:
A public-facing initiative that compares grocery prices across chains for ordinary people or the press: a state transparency portal, a consumer-group basket index, or a private or indie app.
_Avoid_: competitor, similar app

**Social value**:
The good or harm a Comparable brought to people, judged on price outcomes, shopper behaviour, public discourse and policy, harms, and whether its cost-of-living comparisons told the truth.
_Avoid_: impact, benefit (they hide the harms)

**Demand signal**:
A product that shows people want to hunt grocery deals but does not compare baskets, such as a leaflet aggregator; evidence of appetite, not a Comparable.
_Avoid_: competitor

**Core**:
What the index must keep to still be this project: Baskets priced across Romanian Chains, updated regularly with history kept, by a published method anyone can check, run open source, civic and not for profit, and usable by shoppers directly (free, no account, readable on a phone).
_Avoid_: MVP, must-haves

**Kill criterion**:
A condition, set before reading the evidence, whose being met means we do not build the index.
_Avoid_: red flag, deal-breaker

**Pivot criterion**:
A condition, set before reading the evidence, whose being met means we build something quite different, because part of the index's core is lost.
_Avoid_: change of direction

**Cut**:
Dropping a feature outside the index's core; decided while re-scoping the MVP. A criterion can flag a Cut but never makes one.
_Avoid_: descoping

**Stop on notice**:
Pausing any activity a Chain or an authority objects to in writing, from the moment the objection arrives, while the IT lawyer reviews it.
_Avoid_: takedown, compliance request
