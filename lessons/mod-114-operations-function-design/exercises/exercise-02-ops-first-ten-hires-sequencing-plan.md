# Exercise 02 — Ops first-ten-hires sequencing plan

> Estimated time: **~8 hours** · Related chapter: [02 — Sequencing the first ten operations hires](../02-first-ten-ops-hires-and-comp-benchmarks.md)

## Problem statement

Caldera Analytics is a US-headquartered venture-backed SaaS company — observability for data engineering teams. Current state: 72 employees, Series A ($18M, 14 months ago), on track to close Series B ($45M target) in 4–6 months. The founder-CEO is product-and-strategy heavy; the CTO co-founder runs engineering (28 people); the recent VP Sales (joined 5 months ago) runs a GTM team of 12; the VP People joined 7 months ago and runs a team of 2; a fractional CFO retains and runs with a Controller plus two accountants. The GC is contract (10 hours/week); the Head of Security is a Director reporting to CTO.

Operations is empty. The CEO has quietly been running operations herself, with occasional help from the VP People on ad-hoc projects. The board advisor has pushed her for a 24-month "operations function build-out plan" to accompany the Series-B investor conversations — one that is detailed enough to defend against a sceptical investor who sees the ops payroll grow from $0 to multi-millions.

The CEO has asked you to produce the ten-seat sequencing plan — one that lands at the following milestones:

- **Month 0 (today, pre-Series-B close).** Caldera is Series A, 72 FTE, operations function empty.
- **Month 4 (Series B closes).** Expected post-close headcount 90–100 FTE.
- **Month 12 (post Series B operating).** Expected headcount 160–200 FTE.
- **Month 24 (approaching Series C conversation).** Expected headcount 300–400 FTE.

For each of the ten seats, you must produce:

- A specific trigger (headcount, operating programme, systems-count, specific business event) that fires the hire.
- A target hire month (0–24).
- A comp band triangulated across Carta / Pave / Radford, with explicit `<!-- needs-research: ... -->` where current benchmark data is not available in chapter 02.
- The hire-vs-defer-vs-outsource call: full-time hire, fractional / contract, outsource to a managed firm, or defer with a bridge option.
- A leverage case — the specific operating leverage the seat produces in Year 1, expressed in a defensible way (cost saved, time freed, risk reduced, metric improved).
- The reporting line and the executive sponsor.

A twelfth deliverable is a cumulative fully-loaded cost model that shows the Caldera board the ops-function payroll trajectory over 24 months.

## Requirements

### Part A — The ten-seat sequencing table

For each of the ten seats in chapter 02 (CoS → BizOps analyst → Head of Workplace → Ops PM → Head of Procurement → Head of Business Systems → BizOps team lead → analyst backfills → international ops lead → COO), produce a one-page entry with the following fields:

1. **Seat.** Named per chapter 02.
2. **Target hire month.** 0, 3, 6, 9, 12, 15, 18, 21, 24+.
3. **Trigger.** The specific trigger that fires the hire — not "Series B" but "when headcount passes X and we have Y concurrent cross-functional programmes," or "when SaaS vendor count passes 50 and renewal-timing becomes a real problem."
4. **Comp band.** Base, bonus, equity, triangulated across Carta / Pave / Radford. Any specific number that is not in chapter 02 or the problem statement is flagged with `<!-- needs-research: ... -->` — do not invent compensation data.
5. **Hire-vs-defer-vs-outsource.** The chapter-02 call with Caldera-specific reasoning. If "fractional first," name the bridge mechanism and the trigger that converts to full-time.
6. **Leverage case.** One concrete paragraph answering "what does Caldera get in year 1 from this hire that it would not otherwise get, and is it worth the fully-loaded cost?" The leverage case must be specific to Caldera's facts — not a generic "runs the operating cadence."
7. **Reporting line and executive sponsor.** Who does this seat report to; who is the executive on the hook if the hire does not pan out.
8. **Risk flags.** The chapter-02 common-failure-mode most relevant to this specific hire (e.g., "premature COO," "deferring Business Systems until a crisis," "fractional ops leadership that should be full-time").

### Part B — Reorder from the chapter 02 default where appropriate

Chapter 02 states the ten-seat default sequence but notes "reorder as the specific company's variables demand." Caldera's specifics may warrant reordering. For each seat that is reordered relative to chapter 02's default, explicitly justify the reorder.

Example reordering candidates to consider (not an exhaustive list — your plan may reorder differently):

- Caldera is a data-engineering observability company; its R&D infrastructure spend (cloud, data, observability) is likely a large category earlier than the generic chapter-02 trigger. Does Head of Procurement move earlier?
- Caldera has no COO on the plan at all — the problem statement implies the CEO is operating as the COO through month 24. Is that right? Does the COO seat land inside the 24-month window?
- The international ops lead — does Caldera have any international footprint in the 24-month plan? If not, defer explicitly; if yes, justify the trigger.

### Part C — The 24-month fully-loaded cost model

A single table showing the cumulative ops-function fully-loaded payroll over the 24-month window. Columns:

- Month (0, 3, 6, 9, 12, 15, 18, 21, 24).
- Seats active at month X (count).
- Seats added this quarter.
- Fully-loaded cost in-quarter (quarterly figure).
- Cumulative fully-loaded cost since month 0.
- % of total company payroll (require a company-payroll assumption; use the headcount trajectory in the problem statement and a US-SaaS-average fully-loaded cost per employee; cite the assumption).

Model fully-loaded cost at **1.5× base salary** per chapter 02 (base + bonus + employer taxes + benefits + equity burn + workspace + tools) unless you have a different defensible multiplier (name it and cite). <!-- Caldera is US-only; the chapter-02 benefits / employer-tax environment applies. -->

The model should let the board see — at each stage — what the operations function is costing, and what the incremental spend over the previous stage buys.

### Part D — The leverage case summary for the board

A 1–2 page memo you would send to the CEO before the Series-B investor conversation, explaining the ops-function build-out plan to a sceptical investor who asks "why does your operations payroll triple in year 2?" The memo must:

1. Open with the single sentence that frames the leverage case ("Caldera's operations function pays for itself through X / Y / Z savings and leverage, measurable against specific operating metrics...").
2. Cite the three or four highest-leverage seats and their specific Caldera leverage case.
3. Address the "could you outsource more?" counter — where fractional / outsourced bridges are being used, where they are explicitly being converted to full-time, and why.
4. Name the one or two seats where the leverage case is weakest and explain why they are still worth hiring (or why they are being deferred past the 24-month window).
5. Address the "could you hire slower?" counter — where the trigger is firm and where there is schedule slack.

### Part E — The Series-C diligence package preview

By month 24, a Series-C diligence lead will open the ops-function package. Author the one-page preview — the artefact that the Caldera COO (if hired by month 24) or the Chief of Staff (if the COO seat is deferred) would hand to the diligence lead.

The preview should include:

- A seat census (name, title, start date, prior role, reporting line).
- The approved approval-authority matrix per [chapter 05](../05-procurement-operating-model.md) (sketch, not the full matrix).
- The operating-cadence calendar per [chapter 06](../06-operating-cadence-and-okrs-rhythm.md) (weekly / monthly / quarterly / annual anchors).
- The systems-architecture register per [chapter 03](../03-systems-selection-meta-framework.md) (sketch — HRIS, ATS, CLM, spend, procurement, IT identified; owner named).
- The year-24 forward trajectory — the eleventh seat and beyond.

The preview is the "diligence will test the boundary" artefact from [chapter 10](../10-ownership-boundary-map.md).

## Starter guidance

- [Chapter 02](../02-first-ten-ops-hires-and-comp-benchmarks.md) is the primary reference. The ten seats, triggers, comp bands, and the hire-vs-defer-vs-outsource matrix are all there.
- [Chapter 01](../01-coo-vs-cos-and-bizops-org-design.md) is referenced for the operations-function architecture that frames the seats.
- [Chapter 07](../07-scaling-up-greiner-adizes-org-evolution.md) is referenced for the stage-model framing (Caldera is in Phase 2 at Series A, moving into Phase 2-to-3 transition at Series B).
- [Chapter 10](../10-ownership-boundary-map.md) is referenced for the Part E diligence preview.
- Comp bands in chapter 02 are directional and flagged `<!-- needs-research: ... -->`. Do not sharpen them beyond what the chapter supports. The exercise is testing whether you can defend the bands as directional, not whether you can produce precise numbers.
- Where Caldera's data-engineering / observability nature matters, draw it out explicitly — the R&D-infrastructure spend trajectory, the SaaS-vendor-count trajectory in a data-heavy company, the Business-Systems-hire trigger in a data-stack company.
- Where the problem statement is silent (e.g., international footprint, specific GTM motion, specific customer-base profile), state the assumption explicitly rather than inventing.
- The CEO's product-and-strategy comparative advantage is relevant to Variable 1 of the chapter-01 framework; the CoS-first default from chapter 01's Series-A pattern applies.

## Deliverables

- `seat-01-chief-of-staff.md` through `seat-10-chief-operating-officer.md` — ten files, one per seat, each containing the Part A entry.
- `reordering-justifications.md` — Part B, where the Caldera plan reorders from chapter 02's default and why.
- `cost-model.md` — Part C, the 24-month fully-loaded cost model with the assumption named.
- `board-leverage-memo.md` — Part D, the 1–2 page memo to the board / investor conversation.
- `series-c-diligence-preview.md` — Part E, the diligence-package preview.

## Acceptance criteria

The package is acceptable if:

1. All ten seats are populated with specific target months, triggers, comp bands, hire-vs-defer-vs-outsource calls, Caldera-specific leverage cases, reporting lines, and risk flags. Generic answers that could apply to any company are unacceptable.
2. Comp bands cite chapter 02 or are flagged `<!-- needs-research: ... -->`; no comp numbers are invented beyond what chapter 02 states.
3. The leverage case for each seat is specific to Caldera — the data-engineering / observability nature of the business, the R&D-infrastructure spend, the specific executive-team shape, the specific stage trajectory — not a generic restatement of chapter 02.
4. Reordering from chapter 02's default (Part B) is explicitly justified for each seat that is reordered — Caldera-specific reasoning, not "this feels right."
5. The 24-month cost model (Part C) uses chapter 02's 1.5× fully-loaded multiplier (or a different multiplier that is explicitly cited), names the headcount and payroll assumptions, and shows the cumulative trajectory clearly.
6. The board memo (Part D) opens with a leverage case, cites specific seats, addresses the "outsource more" and "hire slower" counters, and names weak-leverage seats honestly.
7. The Series-C diligence preview (Part E) is populated with every element — seat census, approval matrix sketch, operating-cadence calendar, systems-architecture register, year-24 forward trajectory — and is formatted for diligence-lead readability.
8. The CoS seat is treated as a Caldera-specific hire, not a generic one — the problem statement's product-and-strategy-CEO profile shapes the specific CoS profile recommended (ex-operator with product background rather than generic ex-consultant, for example).
9. The COO seat question is answered specifically — hired inside the 24-month window with a specific trigger, or deferred past it with a reason, or merged with the CoS seat as the CoS-to-COO graduation.
10. The international-ops-lead seat is treated specifically — if Caldera has no international plan in the 24 months, defer explicitly with a reason; if yes, name the country and the trigger. The problem statement implies US-only in the first 24 months; justify your call.
11. Cross-references to chapters 01, 02, 05, 06, 07, and 10 are explicit where the reasoning draws from them.
12. No specific comp numbers are invented beyond what chapter 02 states. No real-company names are invented as "the finalist candidate." Nothing is left as `[TBD]` or `[FILL IN]`.
