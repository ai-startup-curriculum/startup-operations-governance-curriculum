# 6. D&O insurance program

> Directors and officers insurance is the financial backstop that makes the indemnification agreement worth signing — without a well-constructed tower, the fiduciary-duty framework in [chapter 05](./05-fiduciary-duties-of-directors.md) collapses onto personal balance sheets.

## Motivation

The corporation's promise to indemnify its directors and officers under DGCL § 145 and the NVCA-form indemnification agreement (see [chapter 03](./03-corporate-secretary-function.md)) is only as strong as the corporation's ability to pay. Insolvency, a hostile post-transaction board, or a derivative-suit settlement that DGCL § 145(b) prohibits the company from indemnifying will each strand a director without corporate reimbursement. The D&O tower exists to plug those gaps and to fund the defense of the fiduciary-duty claims — Van Gorkom, Caremark, Revlon, and the Chancery Court's growing docket of AI-oversight complaints — that the board is exposed to every meeting.

The corporate secretary, the CFO, and the general counsel jointly own the program. The board should treat the renewal as a governance event: the tower structure, retention, exclusions, and broker relationship materially affect whether a qualified director will accept a seat and whether a sitting director will vote conscience-first on a hard call. This chapter documents the mechanics of that program — three-part coverage design, tower construction, exclusion analysis, application warranties, IPO tail, renewal cadence, broker selection, private-versus-public differences, and the trip-wire checklist that determines whether coverage actually responds when a claim lands.

## Three-part coverage design

Modern D&O policies are written in three coverage grants, referred to as Sides A, B, and C. Each side addresses a different failure mode of corporate indemnification, and each interacts with the DGCL § 145 stack and the indemnification agreement's priority-of-payments clause in a specific way.

### Side A — individual protection

Side A pays defense costs, settlements, and judgments directly to individual directors and officers when the corporation *cannot* indemnify them. The paradigm scenarios are:

- **Insolvency.** The corporation is in bankruptcy or is contractually or statutorily prohibited from indemnifying.
- **Derivative-suit settlements.** DGCL § 145(b) bars a Delaware corporation from indemnifying an officer or director for amounts *paid in settlement* of a derivative action. Judgments in derivative actions are similarly barred; only defense costs are indemnifiable, and only if the director acted in good faith.
- **Hostile post-transaction refusal.** An acquirer's new board refuses to advance defense costs to former directors, notwithstanding a surviving indemnification agreement.

Because Side A is the last line of personal defense, boards typically stack a dedicated **Side A DIC** (difference-in-conditions) excess layer above the traditional ABC tower. Side A DIC drops down and pays when:

1. The underlying ABC carrier wrongfully denies coverage;
2. The underlying limits are exhausted; or
3. The corporation is financially or legally unable to indemnify.

Side A DIC also typically has broader terms than the underlying policies — narrower exclusions, no application warranties beyond the bare fact of the ABC placement, and often no retention.

### Side B — corporate reimbursement

Side B reimburses the *corporation* for indemnification payments it makes to directors and officers under DGCL § 145 and the NVCA indemnification agreement. Side B is where the retention sits — the corporation pays the first dollars of every indemnifiable claim before Side B attaches. When the corporation advances defense costs under the mandatory-advancement clause of the indemnification agreement (see [chapter 03](./03-corporate-secretary-function.md)), those advances hit the Side B retention first, then Side B reimbursement.

### Side C — entity coverage

Side C insures the corporation itself as a named defendant.

- **Public companies:** Side C is almost always limited to **securities claims only** — actions under §§ 10(b), 11, and 12 of the '33 and '34 Acts, plus state blue-sky analogs. The scope is narrow because insurers do not want to backstop general corporate liability, and because carving out non-securities entity claims keeps limits available for the individual directors under Sides A and B.
- **Private companies:** Side C is often written more broadly, as **entity coverage** that follows the corporation across a wider spectrum of wrongful-act claims. Private-company D&O forms sometimes include EPL (employment practices) coverage bolted on, though the market trend is to unbundle EPL into a standalone policy (see [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/)).

### Interaction with the indemnification agreement

The indemnification agreement's **priority-of-payments** clause typically sequences the sources of recovery as: (1) the D&O policy responds first, then (2) the corporation's own indemnification obligation, then (3) any indemnification the director may have from a fund sponsor or other secondary indemnitor. The insurance carrier does not get to argue that the director should seek indemnification from the corporation first — the agreement dictates the reverse.

The D&O tower must include an **"order of payments" endorsement** on Sides A / B / C so that when limits are being depleted, Side A payments to individual directors are made *before* Side B corporate reimbursements or Side C entity payments. Without that endorsement, an entity claim could exhaust limits before individual directors are paid.

## Tower construction

A D&O tower is built as a primary layer plus successive excess layers, each **following form** to the primary — meaning the excess layers adopt the primary policy's terms, exclusions, and definitions unless they explicitly override them.

### Structural mechanics

- **Primary layer.** Sits from dollar one above the retention. The primary carrier owns the claims-handling relationship, controls consent-to-settle decisions, and is the counterparty for most coverage disputes.
- **Excess layers.** Attach at the top of the underlying limit and provide additional limit above. Each excess layer is a separate contract with a separate carrier.
- **Concentration risk.** Splitting the tower across multiple carriers reduces the impact of any one carrier's insolvency, ratings downgrade, or coverage dispute.
- **Retention (self-insured retention / deductible).** Applies below the primary limit for Sides B and C. Side A commonly has **no retention** — the individual director should not have to fund a deductible when the corporation cannot indemnify.
- **Order of payments.** The order-of-payments endorsement (discussed above) applies across the tower to protect Side A limits.

### Worked example — Series-B tower

The following table illustrates a representative Series-B tower. Carriers are illustrative; limits and attachment points are structural rather than benchmarked.

| Layer | Carrier (illustrative) | Limit | Attaches at | Coverage sides | Retention |
|---|---|---|---|---|---|
| Primary | AIG | $5M | $0 | A / B / C | $250K B/C, $0 A |
| Excess 1 | Chubb | $5M x $5M | $5M | A / B / C | follow form |
| Excess 2 | Berkley | $5M x $10M | $10M | A / B / C | follow form |
| Side A DIC | Beazley | $5M x $15M | $15M | A only | $0 |

Total tower: $20M of limit, of which $20M is available to individual directors under Side A and $15M is available to the corporation under Sides B / C. The Side A DIC layer both extends limit and drops down to fill coverage gaps in the underlying ABC tower.

<!-- needs-research: typical Series-B primary premium ranges, retention benchmarks by company stage, and DIC-to-ABC ratio norms as reflected in Woodruff Sawyer or Aon market data -->

## Exclusion analysis

The value of a D&O policy is determined less by the limit than by the exclusions and their negotiated carve-backs. Each of the following exclusions warrants line-by-line attention at every renewal.

### Fraud and dishonesty

**What it says.** Coverage does not apply to loss arising from criminal, fraudulent, or dishonest acts of the insured.

**Why it matters.** A broad reading would let a carrier deny coverage the moment a complaint *alleges* fraud, which is nearly every securities-fraud case.

**Negotiated carve-back.** The exclusion should apply only after a **final, non-appealable adjudication** of fraud — and only in the underlying proceeding, not in a coverage action. Until that adjudication exists, the carrier must fund defense costs.

### Insured-vs-insured

**What it says.** Coverage does not apply to claims brought by one insured against another insured.

**Why it matters.** Without carve-outs, a shareholder derivative suit — technically brought "in the name of the corporation" (an insured) against directors (insureds) — would be excluded, defeating a core purpose of the policy.

**Negotiated carve-outs.** Standard carve-outs preserve coverage for:

- Derivative suits brought by stockholders on behalf of the corporation;
- Whistleblower claims (SOX § 806, Dodd-Frank § 922);
- Suits by a post-bankruptcy trustee, receiver, or examiner;
- Suits by a former officer or director after a specified separation period (commonly 2 years).

### Pending and prior litigation ("PPL")

**What it says.** Coverage does not apply to any matter pending or known as of the policy inception date, or to any claim arising from facts disclosed in the application.

**Why it matters.** PPL locks out matters known when the policy incepts. Combined with application warranties, PPL is the single biggest coverage-defeat vector — a claim the CEO or GC knew about but did not disclose can void coverage entirely for that matter.

**Negotiated posture.** PPL cannot be eliminated, but it can be scoped to actual pending litigation and specifically disclosed matters, rather than to "any circumstance that might give rise to a claim." Renewal timing matters — bind first, then update knowledge (see application discussion below).

### Regulatory and SEC exclusions

**What it says.** Some policies exclude or narrow coverage for regulatory investigations and SEC enforcement actions.

**Why it matters.** For a public company or a pre-IPO company preparing for a Wells notice, this exclusion can strip the tower of its most likely-to-be-used coverage.

**Negotiated carve-back.** Public-company towers should narrow the exclusion to purely civil regulatory *penalties* that are uninsurable as a matter of public policy, and should preserve coverage for defense costs and for investigations. Side A layers should carve back regulatory exclusions more aggressively than the ABC tower.

### Personal-conduct exclusions (profit / personal-benefit)

**What it says.** Coverage does not apply to loss arising from an insured obtaining personal profit or advantage to which the insured was not legally entitled.

**Why it matters.** Read broadly, this exclusion swallows insider-trading and disgorgement claims (see [chapter 07](./07-insider-trading-policy-and-window-administration.md)).

**Negotiated carve-back.** Modern forms require **final, non-appealable adjudication** of personal profit in the underlying action before the exclusion attaches, and preserve defense-cost coverage until that adjudication.

### Bodily injury and property damage

**What it says.** D&O policies exclude bodily injury and property damage.

**Why it matters.** These risks belong on the CGL (commercial general liability), EPL, workers' comp, product-liability, and cyber towers — not on D&O.

**Negotiated carve-back.** D&O forms should carve back BI/PD exclusions to preserve coverage for **derivative claims** alleging that directors breached their oversight duty by allowing conduct that caused bodily injury (a Caremark theory). The primary policy pays defense costs for the derivative claim; the CGL and product-liability towers respond to the underlying tort. See [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) for the broader tower.

## Application, warranties, and prior-knowledge exposure

The D&O application asks the CEO, CFO, and general counsel to warrant that they have **no knowledge of any fact, circumstance, or situation that could reasonably give rise to a claim** under the policy. Signing the application binds the corporation and, in most forms, imputes the signer's knowledge to the entire pool of insured persons.

### Warranty consequences

A misstatement — even an innocent one — can void coverage as to the misstatement and, under some forms, void the whole policy as to all insureds. The severability provisions of modern forms cabin this by making the application knowledge non-imputable to *innocent* directors, but the CEO / CFO / GC signatories rarely benefit from severability.

### Bind first, warranty-letter second

The operational rule is: **bind coverage first, then update knowledge.** A "warranty letter" or "no-known-loss letter" freezes the state of knowledge as of the application date. Any post-application knowledge is preserved for the *next* renewal, not for the current bind. The corporate secretary should ensure that the application signing, the binder, and any late-breaking knowledge (e.g., a threatened suit from a departing employee) are calendared so that the application warranty does not straddle a new-knowledge event.

### Change-in-control

D&O policies contain a **change-in-control** clause that freezes the policy at the transaction date: no coverage for wrongful acts committed after closing, and the tail (run-off) must be purchased to preserve coverage for pre-close acts. Change-in-control is defined broadly — it includes mergers, majority-stock acquisitions, sales of substantially all assets, and often controlling-investor transactions. The corporate secretary should read the definition against the transaction structure before signing.

## IPO tail and run-off policy

The IPO tail (also called run-off) is the single most consequential D&O purchase after the initial placement.

### Triggers

The tail is triggered by an IPO, a de-SPAC transaction, a change-of-control merger, or an asset sale that constitutes a change-of-control under the policy. In each case the pre-transaction policy freezes and the tail is purchased to preserve coverage for wrongful acts committed *before* the trigger, for claims made *during* the tail period.

### Duration

The market convention is a **6-year tail**, matched to the statute-of-repose exposure from an IPO:

- **Securities Act § 11 claims** — 3-year statute of repose from the effective date of the registration statement.
- **Exchange Act § 10(b) claims** — 5-year statute of repose from the underlying violation (Sarbanes-Oxley § 804).

The 6-year tail therefore covers the full window in which pre-IPO conduct could give rise to a securities claim. Shorter tails (1-, 3-year) are available but rarely appropriate for an IPO.

### Pricing and timing

The tail is priced as a **multiple of the expiring annual premium** and must be purchased at policy expiration or at transaction close — there is no post-close cure. The corporate secretary and the CFO should have the tail quote in hand well before the S-1 goes effective or the merger closes.

<!-- needs-research: typical tail-premium multiples (percentage of expiring premium) for 6-year IPO run-off, as reflected in current broker market reports -->

### Interaction with acquirer coverage in M&A

In an M&A scenario the target's tail runs alongside the acquirer's ongoing D&O tower. The target's tail covers the target's former directors and officers for pre-close wrongful acts; the acquirer's tower covers the combined company's directors and officers for post-close wrongful acts. Where former target officers join the acquirer, they are covered by both — the target tail for pre-close acts, the acquirer tower for post-close acts. The corporate secretary should confirm named-insured status under the acquirer's tower and preserve access to the target's tail claims-notice channel.

## Annual renewal preparation

The renewal is a 90-day project owned jointly by the CFO, the general counsel, and the broker.

### Timeline

- **T-90 days.** Broker circulates loss-run request and application questionnaire. Corporate secretary pulls prior-year board and committee minutes, litigation docket, regulatory correspondence, and material changes.
- **T-60 days.** Draft application to the CEO / CFO / GC for review. Broker begins market-check outreach.
- **T-30 days.** Underwriter meeting with CEO / CFO / GC. Terms and pricing indications from the primary carrier and select excess carriers.
- **T-14 days.** Final quotes. Broker delivers coverage-comparison memo — limits, retention, exclusions, endorsements — versus expiring program.
- **Bind.** Application signed, warranty letter executed, binders issued.

### Underwriter meeting

The underwriter meeting is a governance event. The underwriter is buying a management team as much as a risk. The CEO's answers to questions about strategy, litigation, and the AI / cyber / regulatory risk profile drive pricing and terms. The corporate secretary should prepare the CEO with the same rigor as a board pre-read (see [chapter 02](./02-board-cadence-and-materials.md)).

### Primary-carrier continuity

Primary-carrier retention is often desirable for claims-handling continuity, even at a modest premium premium. A new primary carrier will not have the file history on any pending matters and may re-litigate coverage questions the incumbent had already resolved.

### Market cycle

The D&O market cycles between hardening (rising rates, tightening terms, capacity withdrawals) and softening (falling rates, broader terms, new capacity). The broker's role includes calling the cycle and timing the market check accordingly.

<!-- needs-research: current D&O market conditions (hard / soft / transitioning) as of the applicable renewal year -->

## Broker selection

The D&O broker is a strategic advisor, not a transactional intermediary. For venture-backed and pre-IPO companies, the market is concentrated among a small set of specialist brokers:

- **Woodruff Sawyer** — deep venture and pre-IPO practice; publishes the annual D&O Databox market benchmark.
- **Marsh** — global scale, strong IPO tail and M&A run-off practice.
- **Aon** — global scale, extensive claims-advocacy resources.
- **Lockton** — strong middle-market and growth-stage practice.

### Selection criteria

- **Market access.** Relationships with the full slate of primary and excess carriers — Chubb, AIG, Beazley, Berkley, Argo, Sompo, AXA XL, Hiscox, and the Side A DIC specialists.
- **IPO-tail experience.** Documented track record placing 6-year run-offs, coordinating with underwriter's counsel, and handling the acquirer/target tail-alignment problem in M&A.
- **Claims-advocacy practice.** A dedicated claims-advocacy team that argues coverage on the insured's behalf against the carrier, distinct from placement brokers.
- **Coverage-analysis capability.** The broker should deliver a line-by-line coverage-comparison memo at renewal, not just quotes.
- **Ongoing service model.** Named service team, defined response SLAs for notice-of-circumstance events, quarterly review cadence.

### Market benchmarks

Woodruff Sawyer's annual D&O Databox is a widely cited benchmark for tower size, retention, and pricing by company stage, sector, and market-cap band. The corporate secretary should include current Databox data in the renewal board memo.

<!-- needs-research: most recent Woodruff Sawyer D&O Databox edition and headline benchmarks relevant to this company's stage and sector -->

## Private vs. public company D&O — comparison

| Dimension | Private company | Public company |
|---|---|---|
| Side C scope | Broad entity coverage; sometimes includes EPL bolt-on | Securities claims only (§§ 10(b), 11, 12) |
| Retention size | Lower — often $100K-$500K on Side B/C | Higher — scales with market cap and float |
| Application cadence | Annual | Annual; more detailed disclosures re: '34 Act filings |
| Run-off pricing | Standard change-of-control tail | 6-year IPO tail at multiple of expiring premium |
| SEC disclosure | Not required | Item 402 discussion of D&O premium and coverage in the proxy |
| Underwriter focus | Investor claims, employment, IP, contract | Securities-fraud class actions, SEC enforcement, derivative suits |
| Tower size | Scales with financing stage | Scales with market cap and float |

<!-- needs-research: specific retention benchmarks and tower-size benchmarks by stage and market-cap band -->

## Trip-wire checklist

The following are the ten most common ways D&O coverage fails when a claim actually hits. Each is preventable with disciplined program management.

1. **Late notice.** Notice provisions require prompt reporting of claims and, in some forms, circumstances. Late notice is a per-se coverage defeat.
2. **Unauthorized settlement.** The consent-to-settle clause bars settlement without carrier consent. Settlement negotiations must loop in the primary carrier from the first substantive offer.
3. **Application misstatement or prior-knowledge issue.** A CEO / CFO / GC signature on the application warrants no known claims or circumstances. Post-signing knowledge belongs on the next application.
4. **Insured-vs-insured misfire.** A director-officer suit that does not fit a named carve-out (whistleblower, derivative, post-separation) can be excluded.
5. **Uninsurable conduct.** A final, non-appealable fraud adjudication triggers exclusion and clawback of advanced defense costs.
6. **Retention not met.** The corporation must fund the Side B/C retention before reimbursement — inadequate cash on hand can strand the director.
7. **Regulatory exclusion consumed.** A narrow or unnegotiated regulatory exclusion can strip coverage for an SEC or DOJ investigation.
8. **Pending-and-prior-litigation carve-out.** A pending matter or a disclosed circumstance is excluded from every subsequent renewal.
9. **Bodily injury / property damage push-back to CGL.** A claim initially noticed to D&O may be pushed to the CGL tower, delaying defense funding.
10. **Coverage tower depletion.** ABC limits exhausted with no Side A DIC leaves individual directors personally exposed for the tail of a large loss.

The corporate secretary should incorporate the trip-wire checklist into the annual governance rhythm (see [chapter 08](./08-annual-governance-rhythm.md)) and into the crisis-governance playbook (see [chapter 10](./10-crisis-governance-and-special-situations.md)).

## Coordination boundary

- **This chapter owns** the D&O tower and the officer/director-protection stack.
- **[Chapter 03](./03-corporate-secretary-function.md)** owns the corporate indemnification-agreement mechanics that D&O Side B reimburses.
- **[Chapter 05](./05-fiduciary-duties-of-directors.md)** defines the fiduciary-duty framework — Van Gorkom, Caremark, Revlon, DGCL §§ 102(b)(7), 144, 145 — that D&O protects against.
- **[Chapter 07](./07-insider-trading-policy-and-window-administration.md)** covers the personal-conduct exposure that the profit exclusion carves back.
- **[Chapter 09](./09-pre-ipo-readiness-governance-track.md)** covers the IPO tail placement as part of the pre-IPO governance track.
- **[Chapter 10](./10-crisis-governance-and-special-situations.md)** covers the notice-of-claim protocol in a live crisis.
- **[Mod-112](../mod-112-enterprise-risk-insurance-and-compliance/)** owns the broader insurance program — cyber, EPL, fiduciary liability (ERISA), crime, general liability, product liability, and R&W insurance for M&A.
- **[Mod-105](../mod-105-equity-comp-and-compensation-committee/)** and **[mod-106](../mod-106-compensation-architecture-and-benchmarking/)** own the compensation-committee interface for officer indemnification decisions.

## Summary

- D&O is a three-part product: **Side A** protects individuals when the corporation cannot indemnify, **Side B** reimburses the corporation for indemnification paid, and **Side C** insures the entity (securities-only for public companies, broader for private).
- Build a tower with multiple carriers, a following-form excess structure, an order-of-payments endorsement, and a **Side A DIC** layer above the ABC tower to protect directors against carrier denial and limit exhaustion.
- Negotiate exclusions to require **final, non-appealable adjudication** for fraud and personal-conduct, carve out derivative and whistleblower suits from insured-vs-insured, and preserve regulatory-defense coverage.
- The application is a warranty document — signed by CEO / CFO / GC — and misstatement voids coverage. Bind first, update knowledge second.
- The **6-year IPO tail** matches the § 11 / § 10(b) statute-of-repose exposure and must be purchased at closing or expiration.
- Run a 90-day renewal cycle with a specialist broker (Woodruff Sawyer, Marsh, Aon, Lockton), an underwriter meeting with the executive team, and a coverage-comparison memo to the board.
- Public and private towers differ meaningfully on Side C scope, retention size, disclosure obligations, and underwriter focus.
- The trip-wire checklist — late notice, unauthorized settlement, application misstatement, insured-vs-insured misfire, uninsurable conduct, retention shortfall, regulatory exclusion, PPL carve-out, BI/PD push-back, tower depletion — should be built into the annual governance rhythm.
- The D&O program is the operational bridge between the fiduciary-duty framework in [chapter 05](./05-fiduciary-duties-of-directors.md) and the indemnification-agreement machinery in [chapter 03](./03-corporate-secretary-function.md); the broader insurance program lives in [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/).
