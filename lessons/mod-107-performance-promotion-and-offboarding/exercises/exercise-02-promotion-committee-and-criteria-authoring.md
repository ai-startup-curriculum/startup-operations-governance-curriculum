# Exercise 02 — Promotion committee and criteria authoring

> Estimated time: **~5 hours** · Related chapter: [02 — Promotion architecture](../02-promotion-architecture.md)

## Problem statement

Longshore Analytics is a Delaware C-corp at Series-B, 145 employees, running a rapidly-scaling engineering, product, and design organisation plus a growing GTM function. The head of people is preparing for the corporation's first-ever formal promotion cycle in Q4 this year. Historically, promotions at Longshore have been:

- Manager-initiated in a 1:1 with the CEO ("I want to promote Priya to Senior Engineer — okay?"), decided within a week, announced in the next all-hands.
- Not tied to any documented level rubric.
- Announced to the team with a one-line Slack message.
- Concentrated in Engineering (which is 60% of headcount) — Product and Design have promoted almost no one in two years.
- Uneven — the highest-performing SDR at Longshore has been passed over four times because "Sales promotions happen after quota-club, not the review cycle."

Three specific pressures make this cycle load-bearing:

1. **A staff-plus engineering promotion candidate** — Tomás, an L5 engineer who has been at Longshore for 4 years and has led two multi-team programmes. Tomás's manager wants to promote him to Staff (L6); the VP Engineering is supportive; the CTO thinks it is a full level too early. Two other L5 engineers with similar tenure and stronger business impact were not promoted last cycle either.
2. **A cross-function calibration risk.** Engineering wants to promote 8 of 45 L4-eligible engineers to L5 (~18%); Product wants to promote 1 of 8 L4-eligible PMs to L5 (~13%); Design wants to promote 3 of 5 L4-eligible designers (~60%). The CEO has flagged the ratios as needing scrutiny.
3. **A retention risk.** Amaya, an L4 designer, has an external offer at a competitor for a Senior title and a 30% comp lift. Longshore's manager thinks Amaya should be considered off-cycle; the head of people is worried this becomes the norm.

Author the promotion architecture Longshore will run for this cycle — committee construction, criteria, cadence, communication, and not-promoted-pool management.

## Requirements

### Part A — Promotion-committee construction

Author a written specification for the promotion-committee architecture:

1. **Function-level committee per function** — Engineering, Product, Design, GTM, G&A. For each, specify: chair (typically the function head), member roster (roles, seniority, rotation cadence), HRBP seat, optional adjacent-function seat, and the meeting agenda.
2. **Cross-function calibration meeting.** Attendees; chair; frequency (per-cycle); what the room can decide vs. escalate.
3. **Executive-level promotions.** How VP+ promotions are handled outside the function-committee track — CEO, head of people, compensation-committee involvement per [mod-105](../../mod-105-equity-compensation-policy-and-comp-committee/), and the material-officer promotion process from [mod-101](../../mod-101-legal-entity-formation-and-corporate-structure/).
4. **Committee-member rotation policy.** 12–18 month rotation; how new members are selected; how the corporation prevents the "kingmaker clique" failure mode.
5. **Documentary record.** What the committee documents per candidate and per decision — the artifact that survives a subsequent legal challenge (see [mod-103 chapter 07](../../mod-103-employment-law-and-contract-design/07-eeoc-protected-category-framework.md)).

### Part B — Three-anchor promotion criteria

Author the promotion-criteria rubric for L5 → L6 (Senior → Staff / equivalent). The rubric must be legible to a candidate reading it in isolation and calibrated across functions. For each of the three anchors:

1. **Competency anchor.** Reference the leveling framework in [mod-106 chapter 01](../../mod-106-compensation-architecture-and-total-rewards/01-job-architecture-and-leveling-framework.md); name the specific competencies the target level requires in each of the four functions; give 2–3 concrete "operating at this level" examples per function. Address explicitly what "sustained over the review period" means at Longshore given a 6-month cycle.
2. **Sponsor anchor.** Define who counts as a sponsor (skip-level, peer function lead, cross-functional executive); how many sponsors are required; how sponsor letters are collected and weighted; the pitfall of the direct-manager-only sponsor case and how the committee filters for it.
3. **Impact anchor.** Define what "business impact commensurate with the target level" means in each function. Include specific examples of impact framing that would qualify vs. narrative-only impact that would not.

The rubric must make explicit that the anchors are conjunctive — all three required, any two without the third is a red flag.

### Part C — Cycle cadence and off-cycle exception policy

1. **Semi-annual cadence.** Author the Longshore Q4 / Q2 promotion-cycle calendar, anchored to the [mod-106 chapter 04](../../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md) comp cycle in Q1 and the mid-year budget carve-out in Q3.
2. **Off-cycle exception policy.** Written policy: trigger criteria (external offer, extraordinary performance, retention risk), decision path (manager → function head → HRBP → head of people concurrence), bar (same three-anchor criteria as on-cycle — speed, not lower bar), volume cap (chapter 02 suggests ~10% of annual promotions). Address Amaya's case specifically: does the external offer qualify, and what is the process now that the offer has surfaced?
3. **Tomás's case (level-up-early scenario).** How the committee will handle a promotion where the direct manager supports, the function head is supportive, but the second-line function executive thinks it is a level too early. Describe the deliberation process and the specific evidence the committee will require to overturn the CTO's read.

### Part D — Promotion-communication playbook

Author the three-layer communication playbook per chapter 02:

1. **To the promoted employee.** The manager-delivery script and follow-up email; the specific fields communicated (title, level, effective date, comp change per mod-106 output, equity refresh per mod-105 grant guidelines, sponsors named); the "we promoted you because" paragraph.
2. **To the team.** Team-channel or all-hands announcement pattern; the one-sentence impact rationale per promotion; the avoidance of the "list of names" failure mode.
3. **To the corporation.** End-of-cycle all-hands announcement; format and length; the signal the announcement sends about what Longshore values.
4. **Sequencing.** The rule that the promoted employee is told first (never learns from an all-hands slide), the team is told second, and the corporation is told third.

### Part E — Not-promoted signal-management playbook

Chapter 02 identifies three not-promoted patterns — not considered this cycle, considered / not promoted / on-track, considered / not promoted / not on-track. Author the mechanic Longshore will operate for each:

1. **Debrief-1:1 within one week** for every reviewed employee; template for the conversation; the specific paragraph the manager delivers per pattern.
2. **Attrition-risk report to the head of people.** What managers report on the "considered / not promoted / on-track" pool within two weeks; the specific signals monitored (external-interview activity, expiring-vest cliff, disengagement).
3. **Retention interventions.** Specific tools available — a retention conversation, a targeted growth-plan revision, a spot-bonus authorised through the head of people, a retention grant authorised through the compensation committee per [mod-105](../../mod-105-equity-compensation-policy-and-comp-committee/).
4. **The specific "considered / not promoted / not on-track" pattern.** How the manager delivers this without collapsing it into a PIP conversation (see [chapter 04](../04-pip-mechanics.md)); the honest coaching path forward and the escalation point if the underlying signal is role fit rather than performance.

### Part F — Cross-function calibration decision on the divergent ratios

Longshore's Engineering (18%), Product (13%), and Design (60%) L4 → L5 promotion ratios are the specific case for the cross-function calibration meeting. Author the memo the head of people will write for the CEO before the meeting:

1. The specific questions the room will ask each function head.
2. What evidence the room requires to accept the Design 60% ratio (or to challenge it back to a lower number).
3. The three-anchor criteria as the reset — a Design promotion pool that clears all three anchors at 60% is defensible; a pool where three of five clear all three anchors is defensible; a pool selected on tenure or manager preference is not.
4. The specific decisions the CEO can make: accept the ratios; require Design to re-defend and reduce; require Engineering to re-defend and reduce; require Product to re-defend and expand.

## Starter guidance

- Chapter 02 is the primary reference. The three-anchor framework (competency + sponsor + impact) is the substantive spine and applies at every level.
- The leveling framework in [mod-106 chapter 01](../../mod-106-compensation-architecture-and-total-rewards/01-job-architecture-and-leveling-framework.md) is the substance of the "competency anchor." The exercise wants a rubric that reads against the mod-106 framework, not a new one authored from scratch.
- The comp change (base + target bonus) and the equity refresh on a promotion are mod-106 and mod-105 territory respectively. The exercise names the outputs but does not author the sizing.
- The demographic-slice review across the promotion pool matters but is not the exercise's centre-of-mass — reference [mod-103 chapter 07](../../mod-103-employment-law-and-contract-design/07-eeoc-protected-category-framework.md) and stay disciplined about the pattern-detection framing.
- Tomás's case is a real dilemma. The exercise wants the committee-deliberation mechanic, not the answer. The committee should reach a defensible decision on the evidence; whether that is promote or defer is not scored.
- Amaya's case tests the off-cycle exception. An external offer alone should not automatically trigger promotion — the three-anchor criteria still apply. The exercise wants the honest read.
- The Design 60% ratio is the calibration case. The right answer is not "60% is too high" — it is "the anchors either clear or they do not, and the room should require the evidence."
- The GTM promotion mechanic differs from the engineering / product / design pattern (quota-attainment, ramp, and role-specific competencies matter). Refer to `startup-product-gtm-curriculum` for the substance; this exercise stays inside the general framework.
- Chapter 07 references executive-level promotions; anything VP+ hands off to the CEO-and-comp-committee track and is out of scope for this exercise.

## Deliverables

- `promotion-committee-construction.md` — Part A.
- `promotion-criteria-l5-to-l6.md` — Part B, the three-anchor rubric per function.
- `cycle-cadence-and-off-cycle-policy.md` — Part C.
- `promotion-communication-playbook.md` — Part D.
- `not-promoted-signal-management-playbook.md` — Part E.
- `cross-function-calibration-memo.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. The committee-construction spec (Part A) covers function-level committees, a cross-function meeting, executive-level promotion handling, rotation policy, and the documentary record.
2. The three-anchor rubric (Part B) is specific per function, is legible to a candidate, and explicitly requires all three anchors. Vague competency descriptions ("has impact") are unacceptable.
3. The cycle cadence (Part C) ties to the mod-106 comp cycle; the off-cycle policy has a decision path, a bar, and a volume cap; Tomás's and Amaya's cases each get a specific deliberation-mechanic answer (not a "yes/no" answer).
4. The promotion-communication playbook (Part D) has the three-layer structure and the sequencing rule that the employee learns first.
5. The not-promoted playbook (Part E) covers all three patterns, has a specific attrition-risk-report mechanic, and named retention interventions with the correct authorisation path.
6. The cross-function calibration memo (Part F) surfaces the specific questions the room will ask, defines the evidentiary bar, and gives the CEO a specific decision surface — not just "call it out."
7. The comp change on promotion (base + target bonus) is deferred to mod-106; the equity refresh is deferred to mod-105; both deferrals are named explicitly.
8. Executive promotions above VP-level are deferred to the CEO / comp-committee track referenced in chapter 07.
9. Any market number cited (promotion ratios industry benchmark, retention-grant sizing, comp lift on promotion) is either taken from a chapter or flagged with `<!-- needs-research -->`.
10. Nothing left as `[TBD]` or `[FILL IN]`.
