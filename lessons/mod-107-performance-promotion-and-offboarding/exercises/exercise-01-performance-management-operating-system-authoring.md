# Exercise 01 — Performance-management operating system authoring

> Estimated time: **~5 hours** · Related chapter: [01 — The performance-management operating system](../01-performance-management-operating-system.md)

## Problem statement

Fernstone Health is a Delaware C-corp at Series-A, 55 employees, headquartered in Austin with distributed engineering and a small go-to-market team in New York. The corporation has a first-time head of people (promoted six months ago from a senior HR-generalist role) and a first-time CEO. Today, Fernstone's "performance-management operating system" is:

- Managers hold 1:1s "when they can" — cadence varies from weekly to monthly, no shared template.
- One informal "check-in" happened last spring, using a Google Doc that different managers filled out differently.
- No formal review has ever run to completion; the previous attempt (in Q3 last year) stalled at the calibration step because no one had decided what a rating meant.
- The corporation adopted Lattice six months ago on a peer-CEO's recommendation and has used ~15% of its capabilities; managers describe it as "another tool we have to log into."
- The annual comp cycle has landed in Q1 based on manager-gut merit recommendations, with no rating input.

The board has asked the head of people to have a defensible performance-management operating system live by Q4 this year (six months out) — one that feeds the Q1 comp cycle authored in [mod-106 chapter 04](../../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md). Two constraints matter:

- **Fernstone has one HRBP-adjacent employee** — the head of people herself. There is no HRBP layer, no L&D lead, no dedicated calibration facilitator.
- **The 12-person management corps has zero formal training on writing or delivering a performance review.** Six of the twelve became managers for the first time in the last 12 months.

Author the performance-management operating system that Fernstone will operate, calendared to the Q4 review / Q1 comp-cycle timeline.

## Requirements

### Part A — Cadence memo

A 1–2 page memo covering the three cadence layers from chapter 01:

1. **Formal review cadence.** Recommend semi-annual, annual-only, or quarterly; defend the choice against Fernstone's stage, manager maturity, and the comp-cycle anchor.
2. **Continuous informal cadence.** Define the 1:1 cadence, the shared 1:1 doc template, and any monthly written check-in mechanism. Anchor the continuous cadence to the formal cadence — the point is that nothing in a formal review should be new information.
3. **Comp-cycle anchor.** A month-by-month calendar showing when self-reviews open, when manager reviews are due, when calibration meets, when ratings lock, when comp cycle opens, when statements are delivered. Land the review closure at least 30 days before comp cycle begins per chapter 01.

### Part B — Format-by-level design

Author the review format matrix Fernstone will operate against its current levels. Since Fernstone has adopted the [mod-106 chapter 01](../../mod-106-compensation-architecture-and-total-rewards/01-job-architecture-and-leveling-framework.md) leveling framework, use L1 through L6 (junior IC through second-line manager). For each level, specify:

1. Which of the canonical inputs apply — self, manager, peer, upward, skip-level, 360.
2. The peer-review mechanic (how many peers per review, who nominates them, whether the peer set is disclosed to the employee).
3. The rating scale — three-point or five-point, with the defence of the choice against manager maturity and the comp-cycle mechanics. Include a "Not Yet Rateable" edge case.
4. The competency-anchor — a specific paragraph on how the review reads against the level rubric versus subjective narrative.

### Part C — Calibration design

Author the calibration protocol:

1. **Function-level calibration.** Which functions Fernstone will calibrate (Engineering, Product, GTM, G&A, or some collapsed structure given the 55-person size); who sits in each function-level meeting; the meeting agenda; the specific output artifact (a signed function-level rating distribution).
2. **Cross-function calibration.** Attendees; agenda; who chairs; specific decisions the room is authorised to make (re-anchor across functions, escalate borderline cases, surface pattern-of-manager concerns).
3. **Distribution guardrail.** A specific soft guardrail — e.g., "no function reports more than 30% at 'Above Expectations' without a written justification from the function head." Justify against the anti-inflation objective from chapter 01 without adopting a forced curve.
4. **Anti-bias step.** The specific demographic-slice review the head of people will run, the specific slices reviewed (gender, race / ethnicity, tenure, work-location, age 40+), and the escalation path if a pattern is found. Refer to [mod-103 chapter 07](../../mod-103-employment-law-and-contract-design/07-eeoc-protected-category-framework.md) for the substantive protected-category framing.

### Part D — Manager-training curriculum

Given Fernstone's zero-trained manager corps, author the manager-training curriculum for this first cycle:

1. **Review-writing workshop.** 60-minute session outline — SBI (situation / behaviour / impact) framing, level-rubric anchoring, distinguishing outcome from effort, supporting the rating with evidence. Include 2–3 discussion cases (e.g., "an engineer who shipped consistent product but under-collaborated"; "an AE who hit quota but blew up two customer accounts").
2. **Delivery workshop.** 60-minute session outline — opening, handling disagreement, transitioning to the development plan. Include 2–3 role-play prompts.
3. **Hard-conversation workshop.** 60-minute session outline — coaching vs. pre-PIP conversations (see [chapter 04](../04-pip-mechanics.md)), documentation practice, HRBP escalation. Include one role-play prompt.
4. **Rollout calendar.** When each workshop lands relative to the review cycle. Specify who delivers each workshop (head of people; outside facilitator; asynchronous video; combination).

### Part E — Tool decision memo

A 1-page memo answering: does Fernstone keep Lattice, migrate to a competitor, or fall back to a Google Sheet / Notion database for the Q4 cycle?

Address:

1. The chapter's five-part selection criteria — HRIS integration, comp-cycle integration, manager UX, calibration workflow, data export.
2. The specific cost of Lattice (or the alternative) against Fernstone's ~$X per-employee licence spend (flag as `<!-- needs-research -->` if you cite a specific number and cannot source it).
3. The manager-adoption problem — the honest read on why Lattice is underused today, and whether that changes with the operating system this exercise designs.
4. A recommendation and a 90-day migration or entrenchment plan.

### Part F — Cycle-one runbook

A single-page runbook the head of people will operate against for the Q4 cycle:

- Week-by-week calendar (from self-reviews opening in October to comp statements delivered in April).
- Owner-by-owner responsibilities (head of people, manager, employee, executive team).
- Escalation paths for the three most-likely failure modes — manager falls behind on writing reviews; calibration meeting fails to converge; employee disputes their rating in the delivery conversation.

## Starter guidance

- Chapter 01 is the primary reference. The cadence, format, calibration, manager-training, and tooling decisions are the chapter's five-part frame.
- The mod-106 chapter 04 comp-cycle calendar is load-bearing. Fernstone's Q4 review must close before the Q1 comp cycle begins; back the calendar off from the mod-106 comp-cycle open date.
- Fernstone has no HRBP layer. The head of people plays the HRBP role directly this cycle. That constraint should show up in Parts C (calibration) and D (manager training) and in the cycle-one runbook.
- Do not invent Lattice pricing, Fernstone financials, or industry benchmarks. Where you cite a specific number, either take it from chapter 01 or flag `<!-- needs-research -->`.
- The rating-scale choice (three-point vs. five-point) is a real trade-off with different downstream comp-cycle mechanics. Pick one and defend it.
- The demographic-slice review in Part C is a pattern-detection instrument, not a quota. The exercise wants the specific mechanic and the escalation path, not a policy debate.
- The calibration room design must survive the corporation's size — a function-level meeting for a 4-person function is different from one for a 25-person function.
- The manager-training curriculum is the highest-ROI investment Fernstone will make this cycle per chapter 01. Do not shortcut this part.

## Deliverables

- `cadence-memo.md` — Part A.
- `format-by-level.md` — Part B, including the level-by-format matrix and the rating scale.
- `calibration-protocol.md` — Part C.
- `manager-training-curriculum.md` — Part D, plus 2–3 discussion cases and 3–4 role-play prompts.
- `tool-decision-memo.md` — Part E.
- `cycle-one-runbook.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. The cadence memo (Part A) picks a specific formal-review cadence and defends it; specifies a continuous-informal cadence; and lands the calendar so the review closes at least 30 days before the mod-106 comp cycle opens.
2. The format-by-level matrix (Part B) covers every level from L1 through L6, is specific about which of the six canonical inputs apply at each level, picks a rating scale, and explains the trade-off.
3. The calibration protocol (Part C) authors a function-level meeting, a cross-function meeting, a distribution guardrail, and a demographic-slice review with a specific escalation path.
4. The manager-training curriculum (Part D) has three concrete workshop outlines, discussion cases, role-play prompts, and a rollout calendar tied to the Q4 review cycle.
5. The tool-decision memo (Part E) reaches a Lattice-keep, migrate, or spreadsheet-fallback recommendation, addresses the chapter's five selection criteria, and includes a 90-day plan.
6. The cycle-one runbook (Part F) is a single page with a week-by-week calendar, owner-by-owner responsibilities, and named failure-mode escalations.
7. Every reference to another module (mod-103 protected-category framework, mod-106 leveling framework and comp cycle, chapter 04 PIP handoff) is specific — the exercise names *what* is being handed off, not just that a handoff exists.
8. Any market number cited (Lattice pricing, industry-benchmark percentages, comp-band sizes) is either taken from a chapter or flagged with `<!-- needs-research -->`.
9. Nothing left as `[TBD]` or `[FILL IN]`.
