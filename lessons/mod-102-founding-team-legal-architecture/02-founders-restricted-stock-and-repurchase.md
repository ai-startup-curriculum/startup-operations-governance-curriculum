# 2. Founders' restricted stock, vesting, and the repurchase right

> Vesting on paper is nothing. Vesting + a repurchase right at cost is what makes founder equity real.

## Motivation

The Stock Purchase Agreement (SPA) is the corporation's contract with each founder about how many shares that founder is buying, at what price, on what vesting schedule, and — crucially — under what circumstances the corporation can buy back the unvested shares. It is the operative document that turns the founder-agreement narrative from [chapter 01](./01-co-founder-equity-split-and-founder-agreement.md) into an instrument that Series-A counsel can read. Get it wrong, and the corporation either (a) has no lever when a founder walks (dead-equity), or (b) has a founder who owes ordinary-income tax on each vesting tranche because the mechanical details did not match what § 83(a) expects.

This chapter walks through the SPA end to end: purchase price and consideration, the 4-year / 1-year-cliff vesting default, the repurchase right at cost, the acceleration debate (with the change-of-control mechanics themselves deferred to `startup-exit-curriculum`), and the transfer restrictions that keep the cap table clean.

## Restricted stock, not options

Founders get *restricted stock*, not stock options. This matters.

- **Restricted stock** is stock issued to the founder today, subject to a vesting schedule and a corporation repurchase right on unvested shares. The founder is the record owner from day one; the § 83(b) election ([chapter 03](./03-83b-election-and-founder-tax-clock.md)) is available; the capital-gains holding clock starts today.
- **Stock options** are a contractual right to purchase shares in the future at a fixed exercise price. The employee is not a stockholder until exercise; the capital-gains clock does not start until exercise; ISO / NSO tax mechanics apply.

Founders get restricted stock because the corporation is at (or near) formation-day valuation — the fair market value is essentially par, the § 83(b) election recognises essentially zero ordinary income up front, and every dollar of future appreciation is capital gain on sale. Options are the right instrument for later employees hired against a higher 409A valuation, where a §83(b) election on restricted stock would recognise real ordinary income today.

If a founder joins after the corporation has grown enough that fair market value has materially appreciated above par, restricted stock is still often the right instrument (subject to their willingness to pay the FMV price today), but the §83(b) tax analysis becomes real and needs to be run before the grant.

## The SPA — a section-by-section walkthrough

### Purchase price and consideration

The founder pays the corporation for the shares. The two common consideration types:

- **Cash.** The founder writes a check (or wires funds) for the number of shares × the per-share purchase price. At formation, the per-share price is typically the par value or a small nominal amount above par. For 8,000,000 shares at $0.0001 per share, that is $800 in cash.
- **Contribution of pre-existing IP.** The founder contributes previously-developed code, designs, documentation, or other IP to the corporation in exchange for shares. The consideration section of the SPA describes the IP being contributed and assigns a value to it; the IP assignment mechanics themselves live in the PIIA ([chapter 04](./04-piia-mutual-ip-assignment.md)), but the SPA is where the *consideration* for the shares is documented.

Consideration must be real. DGCL § 152 requires the board to determine the consideration for and authorise the issuance of shares. Shares issued without consideration are voidable. Even for a small cash amount, the founder should retain proof of payment (the check image, the wire confirmation) and the corporation should archive it in the corporate record ([mod-101 chapter 03](../mod-101-legal-entity-formation-and-corporate-structure/03-corporate-record-and-compliance-calendar.md)).

Do not use the phrase "in exchange for services rendered" as consideration. Stock in exchange for services is compensation income taxable to the founder at fair market value; that is *not* the tax outcome founders want at formation, and it is not what a founder Stock Purchase Agreement is designed to produce. Founder shares are purchased for cash and/or IP.

### Vesting: the 4-year / 1-year-cliff standard

The market default for founders is 4-year vesting with a 1-year cliff:

- **Cliff.** The founder receives zero vested shares for the first 12 months of service. On the one-year anniversary, 25% (12 months' worth) of the shares vest in a single tranche.
- **Monthly (or quarterly) after cliff.** After the cliff, shares vest monthly (1/48th per month is common) or quarterly (1/16th per quarter) until 100% vesting at the 48-month mark.

Two things about this default deserve attention:

- **The cliff exists to protect the corporation and the co-founders.** A founder who leaves in the first 12 months exits with zero vested shares. Without the cliff, monthly vesting would give a founder who leaves in month three ~6.25% of their shares — enough to matter on the cap table but not remotely proportionate to the actual contribution.
- **Vesting counts from the vesting-start date, which is often the founder's start-of-service date, not the formation date.** For a founding team where all founders started before formation, backdating the vesting-start date to the earliest common-service date is defensible; the SPA should state the date explicitly and the corporate record should support it.

Non-default vesting is negotiable but should be justified on the record. Common variants:

- **Backloaded vesting** (e.g., 10 / 20 / 30 / 40 by year) — used to retain founders who might otherwise walk once "fully vested"; unusual.
- **Longer cliff** (e.g., 18 or 24 months) — used when the corporation wants a longer commitment before any vesting; unusual for founders.
- **Vesting with a prior-service credit.** A founder who worked on the project for 12 months pre-formation is granted a vesting-start date 12 months earlier and, in effect, begins day one of formation with 25% already vested (past the cliff). This is defensible if documented.

Do not create founders with wildly different vesting schedules without explaining why. A three-founder company with founder A on standard 4/1 vesting, founder B on 3/0 vesting, and founder C on 4/1 with 24 months of prior-service credit is legible only with a written rationale. Series-A diligence will ask.

### The repurchase right at cost — the mechanic that makes vesting real

The SPA grants the corporation a *right of repurchase* on the founder's unvested shares. The mechanics:

- **Trigger.** The founder's cessation of service to the corporation, for any reason. Some SPAs distinguish by reason (voluntary vs. involuntary; for-cause vs. without-cause); [chapter 01](./01-co-founder-equity-split-and-founder-agreement.md) discusses when acceleration alters the picture.
- **Scope.** All *unvested* shares as of the separation date. Vested shares belong to the founder outright, subject to standard transfer restrictions (see below).
- **Price.** The original purchase price paid by the founder (typically par), *not* the current fair market value. This is the "at cost" repurchase.
- **Mechanic.** The corporation delivers a notice to the founder within a defined window (often 90 days) exercising the repurchase, along with the repurchase price. The shares are cancelled on the corporation's books and returned to the pool of authorised-but-unissued shares.
- **Board approval.** The repurchase is authorised by the board via written consent as a matter of corporate hygiene. If the departed founder is (or was) a director, the DGCL § 144 interested-director rules ([chapter 06](./06-founder-conflict-of-interest.md)) apply.

Without the repurchase-at-cost mechanic, "vesting" is a nice number on a spreadsheet with no legal force. With it, the corporation can reclaim the unvested equity at nominal cost and either return it to the pool or reissue it to a replacement founder or key hire. The mechanic is what allows a company to survive a first-year founder departure without a permanent 25% dead-equity overhang.

### Right of first refusal and co-sale

Even for *vested* shares, the SPA typically imposes transfer restrictions:

- **Right of first refusal (ROFR).** If a founder proposes to transfer vested shares to a third party, the corporation has the right to purchase those shares first at the offered price. This keeps the cap table under the corporation's control.
- **Co-sale.** In some SPAs, other founders or investors have the right to participate proportionally in a founder's sale to a third party. More common in the priced-round Voting Agreement than in the founder SPA.
- **Right of first refusal on repurchase of vested shares at separation.** Some SPAs give the corporation a right (but not an obligation) to repurchase *vested* shares from a departing founder at fair market value on separation. Not standard; typically negotiated in and out based on the corporation's preference.
- **Transfer to permitted transferees.** Standard carveouts allow transfers to family members, trusts for family benefit, and (rarely) to charities without triggering ROFR.
- **Legend on the certificate / notation on the book-entry ledger.** All transfer restrictions are noted on the share record so a transferee cannot claim to have taken free of them.

### Standard representations and covenants

The SPA also includes founder representations that Series-A diligence will read:

- The founder has the legal capacity to enter into the agreement.
- The founder is not subject to any obligation to a former employer that would conflict with the founder's obligations to the corporation. (This dovetails with the PIIA's invention-carveout schedule — chapter 04.)
- The founder has not previously granted rights in the contributed IP to any third party.
- The founder has consulted (or had the opportunity to consult) their own tax advisor and understands the tax consequences of the purchase and the § 83(b) election.
- The founder is an accredited investor (or knowledgeable purchaser) for purposes of the § 4(a)(2) / Regulation D exemption under which the shares are being sold.

## Acceleration on change of control: the sideways deferral

Whether some or all of a founder's unvested shares vest on a change-of-control (CoC) is a design decision made at formation and captured in the SPA:

- **No acceleration** — the acquirer inherits the vesting schedule. Rare for founders; more common for later employees.
- **Single-trigger acceleration** — some fraction of unvested shares vest on CoC regardless of what happens to the founder's role afterwards. Investors typically resist single-trigger acceleration because it changes the acquirer's economics.
- **Double-trigger acceleration** — some fraction of unvested shares vest on CoC *and* the founder's involuntary termination (or resignation for good reason) within a defined window after the CoC. **This is the market-standard default for founders.**

Common double-trigger formulations:

- 100% of unvested shares accelerate on double trigger.
- 12 or 24 months of additional vesting on double trigger.

The founder-side conversation about *how much* acceleration and *what qualifies as "good reason"* is a live one at formation. This chapter records that the market-standard baseline is double-trigger, with 100% acceleration common for founders; the transaction-mechanics view (how acceleration flows through a merger agreement, escrows, indemnification hold-backs, revenue-based earn-outs) belongs to `startup-exit-curriculum`.

Single-trigger CoC acceleration is deferred to `startup-exit-curriculum` for the same reason: it is a negotiation that lives at the term-sheet stage of an M&A transaction, and the founder-side implications are best understood in the context of the transaction rather than at formation.

## The SPA has to match the founder agreement — and the board consent — and the cap table

At formation, four documents describe the same economic event:

- The **founder agreement** ([chapter 01](./01-co-founder-equity-split-and-founder-agreement.md)) — the founders' contract with each other about equity split, roles, and departure treatment.
- The **Initial Board Consent** ([mod-101 chapter 02](../mod-101-legal-entity-formation-and-corporate-structure/02-stand-up-the-entity.md)) — the corporation's authorisation of the issuance, the consideration, the form of SPA, and the vesting.
- The **Stock Purchase Agreement** (this chapter) — the executed contract between the corporation and each founder.
- The **share ledger** (Carta / minute book) — the record of who owns what.

If these four documents contradict each other, the corporate record is defective. Diligence will surface any inconsistency. Fixing it later usually requires a comprehensive ratifying board consent, sometimes an amended SPA, and — in the worst case — a founder who has moved on and now needs to sign paperwork.

## Concrete example: a three-founder SPA package

Three founders form a Delaware C-corp with 10,000,000 authorised common shares and $0.0001 par value. The initial board consent authorises the following issuances, each documented in a signed SPA:

- Founder A (CEO): 4,000,000 shares at $0.0001 per share = $400 cash consideration, plus assignment of pre-formation product IP; 4-year vesting, 1-year cliff, vesting start = 2025-11-01 (six months of prior-service credit).
- Founder B (CTO): 3,500,000 shares at $0.0001 per share = $350 cash consideration, plus assignment of pre-formation architecture documentation and prototype code; 4-year vesting, 1-year cliff, vesting start = 2025-11-01.
- Founder C (VP Product): 2,500,000 shares at $0.0001 per share = $250 cash consideration, no pre-formation IP contribution; 4-year vesting, 1-year cliff, vesting start = 2026-05-01 (C joined on formation day, no prior-service credit).

Each SPA:
- Grants the corporation a repurchase right at $0.0001 per share on unvested shares upon separation.
- Includes a narrowly-drafted "for cause" definition.
- Provides 6 months of accelerated vesting on termination without cause.
- Provides double-trigger acceleration on change-of-control (100% of unvested).
- Includes standard ROFR and transfer restrictions.
- Includes representations covering absence of conflicting obligations, previously granted rights, and § 83(b) acknowledgment.

Each founder writes a check to the corporation, receives their shares (uncertificated, recorded in the ledger), and — within 30 days of the SPA execution date — files their § 83(b) election ([chapter 03](./03-83b-election-and-founder-tax-clock.md)).

At month 11, Founder C decides the venture is not for them and resigns. C is short of the 12-month cliff — zero vested shares. The corporation delivers a repurchase notice within 30 days of the separation date, tendering $250 back to C, and the 2,500,000 shares return to the authorised-but-unissued pool. No dead-equity overhang. The cap table is clean; the corporation can reissue the shares to a replacement founder (with its own new SPA, vesting schedule, and 83(b)) or hold them in the pool.

Compare the counterfactual: if C's SPA had no repurchase right, C walks with 2,500,000 shares of common stock (25% of outstanding at that moment), and Series-A one year later is a negotiation with C's counsel before it is a negotiation with the lead investor. The difference is one clause in the SPA.

## Summary

- Founders get *restricted stock*, purchased today at par, vesting on a schedule, subject to a corporation repurchase right on unvested shares. Options are the wrong instrument for founders at formation.
- Consideration must be real — cash, contributed IP, or both. Not "services rendered." Retain the payment record.
- The market-standard vesting is 4 years with a 1-year cliff. Non-standard vesting is negotiable but must be justified on the record.
- **The repurchase right at cost is the mechanic that makes vesting real.** Without it, "vesting" is a spreadsheet decoration.
- Distinguish separation triggers in the SPA and use a *narrow* "for cause" definition to prevent weaponisation.
- **Double-trigger** CoC acceleration is the founder market-standard baseline; the transaction-mechanics view lives in `startup-exit-curriculum`.
- The SPA, the founder agreement, the initial board consent, and the share ledger all describe the same economic event and must agree. A discrepancy is a defect; fix it before Series-A finds it.
