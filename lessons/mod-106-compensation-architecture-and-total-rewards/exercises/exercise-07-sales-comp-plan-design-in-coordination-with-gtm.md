# Exercise 07 — Sales comp plan design in coordination with GTM

> Estimated time: **~5 hours** · Related chapter: [07 — Sales-comp plan design (in coordination with GTM)](../07-sales-comp-plan-design.md)

## Problem statement

Highline Vectors, Inc. is a Delaware C-corp selling a developer-productivity analytics platform to mid-market and enterprise engineering orgs. The corporation closed a $56M Series-B eight months ago at a $230M post-money and has recently installed its first VP of Sales (formerly a Director of Enterprise Sales at a sector-adjacent Series-C corporation). Current headcount is **156 employees** with a GTM org of **38**: 14 AEs (8 Mid-Market, 4 Enterprise, 2 Strategic), 9 SDRs (including 2 Senior SDRs who manage the SDR-to-AE conversion), 6 Sales Engineers (SEs), 4 CS Managers, 3 Sales Operations ICs, and the VP Sales + 1 Director of Enterprise Sales.

Current state of the sales-comp plan:

- **No ratified plan.** OTE and commission structures were negotiated individually with each AE over the last three years. The plan carries nine different variants — some AEs are on a 50/50 base/variable split, some on a 60/40, some on a 65/35; some carry a 1.0× accelerator above quota, some 1.5×, some 2.0×, and one Strategic AE has a bespoke "deal-value-based" plan that pays a flat percentage of ACV with no quota.
- **The new VP Sales is proposing a full plan rewrite** effective Q1 2026 — a standardised 60/40 base/variable split for all AEs, a tiered accelerator structure (1.0× to 100% of quota, 1.5× from 100–150%, 2.0× from 150–200%, 2.5× above 200%), a ramp-comp policy (3-month 100%-of-OTE guarantee from start date, then stepping to 50% in month 4, 25% in month 5, no guarantee from month 6), a monthly spiff pool managed by the VP Sales, and a 12-month clawback on any commissioned deal that churns or is renegotiated.
- **Three specific coordination gaps** between the Head of Total Rewards and the VP Sales:
    1. **The base-salary side of OTE** — the VP Sales is proposing base-salary ranges that do not match the ratified band file from [exercise 02](./exercise-02-cash-and-equity-band-authoring-by-geography.md). Specifically, the proposed Enterprise AE base is ~8% above the Tier-1 band ceiling. The Head of Total Rewards believes the VP Sales is solving for OTE, not for the base / variable split, and is accidentally violating the band.
    2. **The quota-sizing side of the plan** — chapter 07 notes that the quota and the comp plan are two sides of the same instrument; a plan with an aggressive accelerator schedule but a quota set at an unreachable level is a comp-cost manageable plan but a retention disaster. The quota-setting conversation has not happened; the VP Sales is proposing the plan without the quota.
    3. **The clawback structure** — the 12-month clawback is above the market median (chapter 07 notes 6-month is more common at Series-B, with 12-month at Series-C and beyond) and the Head of Total Rewards is concerned the clawback will be challenged under state wage-and-hour law in CA (California Labor Code § 2751 requires commissions to be in writing and § 2802 requires expense reimbursement; the clawback may be challenged as either).
- **A pending Series-C process in Q3 2026** and a scheduled board compensation-committee review of the sales-comp plan in advance of the Q1 2026 effective date. The comp committee has asked for a jointly-authored plan from the VP Sales, the Head of Total Rewards, and the GC.

Your role: you are the **Head of Total Rewards** tasked with producing the sales-comp plan in coordination with the VP Sales and the GC. Produce the plan architecture (base / variable / OTE / accelerator / spiff / clawback), the quota-sizing-handoff boundary, the state wage-and-hour compliance posture, the specific disposition of the three coordination gaps, and the comp-committee presentation memo. **This exercise owns the compensation-architecture side; the quota-setting, territory-design, and plan-as-behaviour-shaping side is explicitly deferred to `startup-product-gtm-curriculum`**.

## Requirements

### Part A — OTE architecture and base / variable split

Produce the OTE and base / variable architecture. Cover:

1. **The base / variable split by role.** State the split per GTM role (AE Mid-Market, AE Enterprise, AE Strategic, SE, Sales Manager, Director of Sales, VP Sales, SDR, Senior SDR, SDR Manager). Chapter 07 notes the market cuts (`<!-- needs-research -->` for specific percentile cuts):
    - SDR: typically 70/30 to 80/20 base/variable (SDR variable is typically meeting-booking-based, not quota-revenue-based).
    - AE: typically 50/50 to 60/40 base/variable at Mid-Market, 50/50 at Enterprise, 60/40 at Strategic (Strategic AEs tend to carry a larger base because deal cycles are longer).
    - SE: typically 75/25 to 80/20 (SEs are typically paid a smaller variable with a team-based or deal-close component).
    - Sales Management: typically 70/30 to 80/20 (manager variable is tied to team quota, not individual).
2. **The OTE anchor to the band file.** State the explicit rule — the OTE sits inside the ratified band (base + target variable = OTE; OTE midpoint anchors to the chapter-02 band midpoint for the equivalent level, with base and variable derived from the ratio chosen in Part A.1). Cross-reference [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md).
3. **The Enterprise AE base-salary gap.** The VP Sales' proposed Enterprise AE base is ~8% above the Tier-1 band ceiling. Diagnose the gap — is the VP Sales solving for OTE (and inadvertently stretching base), or is the OTE itself out-of-band? Propose the specific fix: either (a) adjust the base to the band and the variable up to maintain OTE, or (b) adjust the OTE midpoint if the current band is not market-competitive for Enterprise AE at this stage (which requires a band revision through the chapter-02 path, not a plan-authoring workaround).
4. **The role-levels × base / variable table.** Produce a table showing the floor / midpoint / ceiling base, target variable, and OTE for each GTM role at each level, per the ratified geographic tiers from [exercise 02](./exercise-02-cash-and-equity-band-authoring-by-geography.md). Flag every specific number with `<!-- needs-research -->`.

### Part B — Accelerator, decelerator, and ramp-comp mechanics

Produce the accelerator / decelerator and ramp mechanics. Cover:

1. **The accelerator schedule.** State the proposed accelerator schedule (the VP Sales' proposal is 1.0× to 100%, 1.5× from 100–150%, 2.0× from 150–200%, 2.5× above 200%) and compare against market cuts (`<!-- needs-research -->`). State whether the proposed schedule is market, above-market (aggressive overperformance incentive, risk of higher comp cost), or below-market (conservative overperformance incentive, risk of churning top performers).
2. **The decelerator or floor.** State whether the plan carries a decelerator below quota — some plans pay 0.5× below 50% attainment; some pay 0× below some floor. Chapter 07 notes the trade-off: a decelerator reduces risk-weighted comp but can push a struggling AE into a self-perpetuating death spiral where the deceleration makes it harder to fund the activities that would close the gap. State Highline's choice.
3. **The ramp-comp policy.** The VP Sales' proposal is 3-month 100%-of-OTE guarantee, stepping to 50% / 25% / 0%. Compare against market cuts (`<!-- needs-research -->`). State whether this is market for Series-B. Chapter 07 notes a 6-month ramp is common for Enterprise / Strategic AE with a longer deal cycle; evaluate whether the Highline proposal is adequate for the Enterprise and Strategic tiers.
4. **The spiff-pool structure.** The VP Sales' proposal is a monthly spiff pool. State the structure — who funds it (a % of total GTM comp budget held in reserve by the VP Sales), who allocates (the VP Sales with advisory input), the maximum per-AE per-month, the eligibility criteria (quota attainment above threshold, specific deal-type, specific product-line, logo-of-strategic-importance). State the governance — the spiff pool has an annual budget cap, reports to the comp committee at the quarterly review, and cannot be used to pay above-OTE-band commissions without comp-committee approval.
5. **The MBO / corporate-scorecard overlay.** State whether the AE plan carries a MBO or corporate-scorecard overlay in addition to the quota-based variable. Chapter 07 notes a modest MBO tranche (10–15% of variable) tied to CRM hygiene, pipeline-creation, or a strategic initiative can be an effective behaviour-shaping lever without eroding the quota focus. State Highline's choice.

### Part C — Clawback mechanics and state wage-and-hour compliance

Produce the clawback mechanics and the state wage-and-hour compliance posture. Cover:

1. **The clawback trigger scope.** State the specific events that trigger a clawback — customer churn within the clawback window, customer-initiated contract renegotiation to a lower value, customer bankruptcy, AE-caused contract termination (misrepresentation, fraud). State explicitly the events that do *not* trigger (routine expansion-revenue adjustments, product changes initiated by Highline, service-level failures by Highline).
2. **The clawback window.** The VP Sales proposed 12 months. State the window Highline will adopt — chapter 07 notes the market distribution: 3–6 months at seed, 6 months at Series-A, 6–12 months at Series-B, 12 months at Series-C and beyond. Pick a window with justification and flag `<!-- needs-research -->` against specific peer-cut distributions.
3. **The clawback mechanism.** State the mechanism — forfeiture of unpaid commissions (easy to administer), offset against future commissions (medium complexity), or demand for repayment from the AE (hard to administer, high state wage-law exposure in CA / NY). State the chosen mechanism with justification.
4. **The California compliance posture.** Address California Labor Code § 2751 — commissions must be in writing, with the method for determining and paying commissions clearly specified; the AE must receive a signed copy. Address California Labor Code § 2802 — the employer must reimburse the employee for necessary business expenses; a clawback that offsets against a *base-salary* wage instead of a *commission* is a potential § 2802 violation. Flag `<!-- needs-research -->` for the current-cut case-law position on clawback-against-commission vs. clawback-against-base-salary.
5. **The New York, Illinois, and Massachusetts compliance posture.** State the state-specific posture for each — NY Labor Law Article 6 (commission plans in writing; frequency-of-payment rules); IL Wage Payment and Collection Act (similar requirements); MA Wage Act (one of the strictest — attorney fees and treble damages for violations). Flag `<!-- needs-research -->` for state-specific wage-and-hour cuts.
6. **The AE commission-plan written agreement.** State the artifact every AE signs — the written commission-plan agreement, incorporated by reference in the offer letter, countersigned at hire and at each plan-year renewal. The agreement states the base, target variable, OTE, quota (incorporating the Part D hand-off), accelerator / decelerator schedule, clawback mechanics, and the interaction with the offer letter's at-will employment and termination terms. Cross-reference [mod-103 chapter 03](../../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md) for the offer-letter architecture.

### Part D — Quota-sizing hand-off boundary

Produce the explicit hand-off to `startup-product-gtm-curriculum` on the quota-sizing side. Cover:

1. **The boundary statement.** State clearly — the comp-plan architecture (base / variable / OTE / accelerator / clawback) is owned here; the quota-sizing (top-down from company revenue plan, bottom-up from territory / pod, individual-AE assignment, mid-year quota adjustment mechanics) is owned by `startup-product-gtm-curriculum`.
2. **The joint-authoring artifacts.** State the artifacts that are jointly authored between the Head of Total Rewards and the VP Sales / CRO:
    - The comp plan (this exercise).
    - The quota-sheet (the GTM-curriculum artifact).
    - The territory-assignment map (the GTM-curriculum artifact).
3. **The ratification path.** State the ratification path — the comp plan is ratified by the comp committee (this module's territory); the quota-sheet is ratified by the CEO + VP Sales + CFO (the GTM-curriculum's territory). The comp committee sees the quota-sheet as context but does not ratify its specific numbers.
4. **The mid-cycle plan-change rule.** State the rule — mid-cycle changes to the comp plan require comp-committee ratification; mid-cycle changes to the quota (quota relief, territory reassignment, mid-year reset) do not. Cross-reference `startup-product-gtm-curriculum` for the quota-change playbook.
5. **The specific quota-related inputs the comp plan requires.** The comp plan requires the quota to be defensible at the OTE midpoint — if the quota is set such that a 50th-percentile AE cannot reach OTE, the plan is a de facto deceleration and the comp architecture is violating the band promise. State the specific interaction and the forcing-function trigger that routes a quota-plan mismatch back through the comp committee.

### Part E — Three-coordination-gap disposition

Produce the specific disposition of the three coordination gaps in the problem statement. Cover:

1. **The Enterprise AE base-salary gap.** State the specific fix (from Part A.3) — either adjust base down and variable up to maintain OTE, or initiate a band revision through [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md). State the disposition decision and the communication path with the VP Sales.
2. **The missing quota-sizing conversation.** State how the comp plan ratification is conditioned on the quota-sheet being drafted in parallel. The comp committee cannot ratify the comp plan without seeing the quota-sheet; the VP Sales cannot draft the quota-sheet without the comp plan's OTE and accelerator structure. State the joint-drafting cadence (two-week sprint between the VP Sales, the Head of Total Rewards, and the CFO).
3. **The 12-month clawback.** State the disposition — reduce to 6 months per the Part C decision, or retain 12 months with a documented justification and a California-specific carveout. State the specific communication with the VP Sales and the GC on the state wage-law exposure.
4. **The communication sequence.** State the sequence — the Head of Total Rewards presents Parts A–D to the VP Sales for internal alignment, then the GC reviews Part C for wage-and-hour exposure, then the three jointly present to the comp committee with the quota-sheet as context.

### Part F — Comp-committee presentation memo

Produce the **1-page memo** attaching the sales-comp plan. Cover:

- The three coordination gaps (Part E) and the specific dispositions.
- The four ratification asks: the OTE architecture (Part A), the accelerator / decelerator / ramp / spiff mechanics (Part B), the clawback mechanics with state compliance posture (Part C), and the quota-sizing hand-off boundary (Part D).
- The explicit statement of the ownership-boundary carveout to `startup-product-gtm-curriculum` for quota-setting, territory design, and plan-as-behaviour-shaping.
- The Q1 2026 effective-date timing and the pre-effective-date AE-communication plan (every AE receives the new written commission-plan agreement countersigned before Q1 2026 start).
- The `<!-- needs-research -->` queue grouped by decision (OTE market cuts, accelerator-schedule market cuts, clawback-window market cuts, state wage-and-hour case-law positions).
- The forward-references to [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md) (band-to-OTE reconciliation), [chapter 08](../08-comp-architecture-failure-modes.md) (cross-function inversion, the "sales OTE exceeds engineering total cash at the equivalent level" failure mode), [mod-103 chapter 03](../../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md) (offer-letter commission-plan reference), and `startup-product-gtm-curriculum` (quota-sizing and territory-design ownership).

## Starter guidance

- Chapter 07 is the primary reference. Re-read the "OTE and base / variable split," "accelerator and decelerator," "ramp comp," "spiff mechanics," "clawback," and "state wage-and-hour compliance" sections before authoring.
- **This exercise explicitly does NOT own quota-sizing, territory design, or plan-as-behaviour-shaping.** Those are `startup-product-gtm-curriculum`'s territory. Reference the curriculum and the specific module; do not re-author.
- The three coordination gaps are the comp committee's anchor cases. The VP Sales' plan rewrite has to pass the band-reconciliation test, the quota-coordination test, and the state wage-and-hour test. Each disposition matters.
- **Do not manufacture market numbers.** Every base / variable ratio, every accelerator percentile, every ramp-period market cut, every clawback-window distribution must be flagged `<!-- needs-research -->`.
- The California § 2751 / § 2802 posture is the state-law anchor. Reference the specific Labor Code sections; do not re-derive the case law.
- The quota-sheet is a jointly-authored artifact. Do not invent its contents; defer to `startup-product-gtm-curriculum` and state the joint-drafting mechanics.

## Deliverables

- `ote-and-base-variable-architecture.md` — Part A.
- `accelerator-decelerator-ramp-spiff-mechanics.md` — Part B.
- `clawback-and-state-compliance.md` — Part C.
- `quota-handoff-boundary.md` — Part D.
- `three-coordination-gap-disposition.md` — Part E.
- `comp-committee-memo.md` — Part F (1 page).

## Acceptance criteria

The package is acceptable if:

1. Part A states the base / variable split per GTM role with market-cut comparisons flagged `<!-- needs-research -->`, states the OTE-to-band anchor rule, dispositions the Enterprise AE base-salary gap, and produces the role-levels × base / variable table.
2. Part B states the accelerator schedule with market comparison, the decelerator / floor decision, the ramp-comp policy with Enterprise / Strategic adjustment, the spiff-pool structure with governance, and the MBO / corporate-scorecard overlay decision.
3. Part C states the clawback trigger scope, the clawback window with market distribution, the clawback mechanism, the California Labor Code § 2751 and § 2802 compliance posture, the NY / IL / MA compliance posture, and the written AE commission-plan agreement artifact.
4. Part D states the quota-sizing hand-off boundary to `startup-product-gtm-curriculum`, the jointly-authored artifacts, the ratification path, the mid-cycle plan-change rule, and the specific quota-related inputs the comp plan requires.
5. Part E dispositions each of the three coordination gaps (Enterprise AE base, quota-sizing conversation, 12-month clawback) with specific fixes and a communication sequence.
6. The comp-committee memo is **one page**, names the three coordination gaps, the four ratification asks, the ownership-boundary carveout, the Q1 2026 effective-date timing, and the `<!-- needs-research -->` queue.
7. Every market cut (base / variable ratio, accelerator percentile, ramp-period cut, clawback window), every state wage-and-hour case-law position, and every OTE midpoint claim is flagged `<!-- needs-research -->`. The California § 2751 / § 2802, NY Labor Law Article 6, IL Wage Payment and Collection Act, and MA Wage Act citations are present.
8. Cross-references to [chapter 02](../02-cash-and-equity-bands-per-level-per-geography.md), [chapter 08](../08-comp-architecture-failure-modes.md), [mod-103 chapter 03](../../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md), and `startup-product-gtm-curriculum` are present.
9. Nothing left as `[TBD]` or `[FILL IN]`.
