# 1. Choose the US legal entity

> Pick the entity that will survive institutional-VC diligence — or pick the alternative deliberately, knowing the trade.

## Motivation

Entity choice is a one-time, low-reversibility decision that constrains everything downstream: what investors can buy, how founders and employees are taxed on their equity, what state law governs internal disputes, and how many post-hoc conversions or F-reorganizations you will pay for later. The venture-backed default is a Delaware C-corporation, and the reason is not "Delaware is fancy" — it is that every institutional term sheet, employee-option plan, and priced-round document set in wide use is *written against* the Delaware General Corporation Law and the federal C-corp tax regime. Choosing something else is choosing to (a) redraft or convert later, or (b) accept structural friction with the investors and employees you plan to bring in.

## The four candidates

For a US operating company, four entity shapes are actually on the table:

- **Delaware C-corporation.** Corporation formed under the Delaware General Corporation Law (DGCL, 8 Del. C. § 101 et seq.). Federal C-corp taxation under Subchapter C (IRC §§ 301–385). This is the venture-backed default.
- **Delaware LLC.** Limited liability company formed under the Delaware Limited Liability Company Act (6 Del. C. § 18-101 et seq.). Federal partnership taxation by default (or check-the-box to C-corp).
- **S-corporation.** Any state-law corporation (or LLC that elects corporate treatment) that further elects Subchapter S treatment under IRC § 1362. Pass-through tax with tight eligibility rules.
- **Delaware public benefit corporation (PBC).** A corporation formed under DGCL § 362 (or converted under § 363) that identifies one or more specific public benefits in its charter and legally binds directors to balance those benefits against stockholder interests.

Other geographies — a California corporation, a Nevada corporation, a Wyoming LLC — appear in specific fact patterns, but the default question is: **should this be a Delaware C-corp, and if not, why not?**

## Why Delaware

Three reasons drive the "why Delaware" default:

1. **Case law depth.** The Delaware Court of Chancery is a non-jury business court with over a century of corporate-law jurisprudence. Fiduciary-duty questions, appraisal proceedings, merger disputes, and stockholder litigation get resolved against a corpus that lawyers, judges, and investors already know. Predictability is the product.
2. **A modern, frequently-amended statute.** The Delaware Bar's Corporation Law Council proposes annual amendments to the DGCL, which the Delaware legislature typically adopts. The statute keeps pace with market practice (SAFE-like instruments, book-entry uncertificated shares, stockholder action by consent under § 228, forum-selection clauses).
3. **Investor and counsel muscle memory.** Every institutional venture term sheet, model NVCA document set, and standard employee-option plan is drafted against the DGCL. A Delaware C-corp saves the seed-stage cost of "translating" every downstream document; a non-Delaware entity pays that cost every round.

There is a real cost — the Delaware franchise tax (see [chapter 03](./03-corporate-record-and-compliance-calendar.md)) and a Delaware registered agent (8 Del. C. § 132) — but for a company that intends to raise institutional capital, the cost is the price of admission, not a decision variable.

## Why C-corp (and not S-corp or LLC)

The venture-backed answer is almost always C-corp because institutional venture funds structurally *cannot* hold pass-through equity:

- **S-corp is ineligible for VC ownership.** IRC § 1361(b) limits an S-corp to ≤100 shareholders, allows only one class of stock, and restricts shareholders to individuals, certain trusts, and certain estates. A venture fund (typically a limited partnership or LLC) is not an eligible S-corp shareholder. Preferred stock is a second class of stock and disqualifies the S election on its own. An S-corp that accepts a venture investment loses S status by operation of law.
- **LLC pass-through creates fund-level pain.** Institutional VC funds have tax-exempt LPs (endowments, pensions, sovereigns) and non-US LPs. A pass-through LLC pushes UBTI to the tax-exempts and ECI to the non-US LPs. Funds structurally avoid pass-through investments or force a blocker corporation in between — friction that a C-corp target does not create.
- **C-corp gives founders and employees IRC § 1202 QSBS exposure.** Only C-corp stock is eligible for Qualified Small Business Stock treatment under § 1202. QSBS is one of the single largest tax benefits available to founders and early employees of a venture-scale company; an LLC or S-corp forecloses it. <!-- needs-research: verify latest § 1202 gross-asset cap and per-issuer exclusion caps after the July 2025 One Big Beautiful Bill Act (OBBBA) amendments to Subchapter O; historically the cap was $50M gross assets with a $10M / 10x exclusion cap, but this was expanded. Cite the current IRC § 1202(a)–(d) text before publishing dollar amounts. -->
- **Employee equity is designed for C-corp shares.** ISOs (IRC § 422), NSOs, and RSUs all assume corporate stock. An LLC's equivalent — profits interests — carries different tax mechanics, different plan documents, and different employee-communication problems.

The trade the C-corp accepts is **entity-level tax**: a C-corp pays corporate income tax on its earnings, and dividends distributed to stockholders are taxed again at the stockholder level. For a startup that will reinvest all earnings and never distribute cash before an exit, "double taxation" is a theoretical concern. For a profitable, distributing business, it is a real cost — and that business is often better as an LLC.

## When the exception is right

- **LLC as a single-owner substrate or bootstrapped-services vehicle.** A solo founder building a services business, a two-founder consultancy, or an SPV to hold a specific asset can rationally be an LLC. If venture capital is not on the roadmap, the C-corp's franchise tax and Subchapter-C burden buys nothing.
- **LLC for R&D-heavy, tax-credit-optimising structures.** In narrow fact patterns, pass-through treatment lets founders use business losses against outside income, or channel research-tax-credit generation to individual returns. This is a CFO / tax-advisor call, and the analysis should be documented before formation — it usually is not correct for a company that intends to raise a priced round.
- **S-corp for a lifestyle / owner-operator business.** An S-corp lets an owner-operator take a "reasonable salary" plus distributions and save on self-employment tax. It cannot survive an institutional financing.
- **PBC for a mission-locked founding team.** Delaware PBC status legally binds directors to balance stockholder value against a specified public benefit (DGCL § 365(a)). For companies whose mission is central to their value proposition (climate, health-equity, education), PBC status is a credible signal and a governance anchor. Institutional venture investors do invest in PBCs; the marginal friction is (i) some public-market-focused investors have policy limits on PBCs and (ii) any subsequent conversion back to a standard corporation requires the same supermajority vote a conversion in requires (DGCL § 363(a)). Choose PBC deliberately, not fashionably.
- **Non-Delaware corporation for jurisdiction-specific tax reasons.** A California corporation with all operations in California pays California franchise tax anyway and saves the Delaware franchise tax and registered-agent cost. In practice, the moment institutional financing enters the picture, investors will require reincorporation to Delaware — and paying for that reincorporation is more expensive than paying the Delaware tax from day one. Non-Delaware formation is almost always a short-term saving and a long-term cost.

## The decision framework

For each candidate, answer four questions:

1. **Will this company raise institutional venture capital within 24 months?** If yes → Delaware C-corp. Full stop. Every other candidate creates a conversion event on the diligence schedule.
2. **Does the founder team need pass-through tax treatment right now?** If yes and (1) is no → LLC (Delaware if state-neutral, in-state otherwise).
3. **Is mission-lock a material commitment the founders want legally binding on the board?** If yes → Delaware PBC. Confirm the intended lead investor accepts PBC status.
4. **Does an S-corp election optimise tax without foreclosing option value?** Only if (1) is no *and* the founders are US individuals *and* there is no preferred stock. In a startup context, this is rare.

Document the answer in an entity-choice memo. See [exercise-01](./exercises/exercise-01-delaware-c-corp-vs-alternatives-decision-memo.md).

## Concrete example: the "we started as an LLC" pattern

A common pattern: two founders form a Delaware LLC in month 0 because it's cheap and the taxes-on-losses are useful. In month 14, a lead investor issues a term sheet contingent on "conversion to a Delaware C-corporation prior to closing." The conversion is executed under 6 Del. C. § 18-216 and DGCL § 265 (statutory conversion) or via a "check-the-box" election followed by a state-law conversion. The mechanics are well-understood — but they consume 30–60 days of counsel time, require re-executing every equity grant against the new capital structure, and can generate taxable gain on any appreciated assets contributed to the new corporation. The savings from starting as an LLC are frequently erased by the conversion cost. If the founders knew at month 0 they would raise institutional capital, starting as a Delaware C-corp was the correct choice.

## Summary

- **Default:** Delaware C-corp. It is what venture financings, standard equity plans, and Series-A diligence checklists are built for.
- **Delaware** because of Chancery Court, a modern statute, and universal counsel / investor familiarity.
- **C-corp** because VCs cannot own S-corp stock, pass-through creates fund-level pain, and only C-corp stock is § 1202-QSBS-eligible.
- **LLC, S-corp, or non-DE corp** are right in narrow, deliberate cases — most often when institutional capital is not on the roadmap.
- **PBC** is a governance commitment, not a marketing choice; adopt it when mission-lock is a real requirement and confirm investor alignment.
- Always document the entity-choice reasoning at formation. A one-page memo now prevents a "why didn't we do this?" conversation two years later.
