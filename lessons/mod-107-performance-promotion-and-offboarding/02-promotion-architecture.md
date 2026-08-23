# 2. Promotion architecture

> Who decides, on what evidence, at what cadence, communicated how — and what happens to the two-thirds of the pool that did not get promoted this cycle.

## Motivation

Promotion is the single decision that most tests whether a corporation's leveling framework is actually load-bearing. The comp cycle in [mod-106 chapter 04](../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md) reads the ratings from [chapter 01](./01-performance-management-operating-system.md) and applies a merit-budget curve; that mostly runs itself. Promotion is where competing narratives, sponsor politics, function drift, and manager favouritism collide with a fixed budget and a public outcome. The failure modes are expensive:

- Every manager writes their own promotion case, no committee vets it, and by year two the engineering team has three "Staff Engineers" who would not clear the bar at any peer company.
- The corporation runs a promotion committee that only meets when a manager pushes a case, so promotions become a function of manager assertiveness rather than employee readiness.
- Promotions are announced by email with no supporting narrative, and the twelve people who did *not* get promoted read the announcement as evidence they are not being seen.
- Nothing systematic happens to the not-promoted pool. Six months later, three of them have accepted external offers.

The promotion architecture is the mechanism that turns promotions into a predictable, defensible operation whose output is a promotion decision the corporation is willing to stand behind for the next twelve months.

## The five operating decisions

1. **Committee construction.** Who sits in the room; how function-level committees compose into cross-function calibration.
2. **Criteria authoring.** What the level rubric actually requires (competencies), who sponsored the promotion inside and above the manager (sponsor), what the employee's business impact has been (impact).
3. **Cadence.** Semi-annual as the default, with an off-cycle exception path for genuinely exceptional cases.
4. **Communication.** How promotions are announced to the promoted employee, to their team, to the corporation.
5. **Not-promoted-signal management.** What happens to the two-thirds of the pool that did not get promoted this cycle.

## Decision 1 — Committee construction

Promotion decisions are made by a *committee*, not by a manager. The reasons:

- A committee normalises across managers within a function so that Manager A's "Senior" bar looks like Manager B's "Senior" bar.
- A committee normalises across functions so that Engineering's "Staff" bar and Product's "Group Product Manager" bar look meaningfully similar.
- A committee creates the documentary record that survives a legal challenge if a rejected promotion candidate later files an EEOC charge alleging discrimination.

**Function-level promotion committee.** For each function (Engineering, Product, Design, Data / ML, Sales, Marketing, CS, Ops, Finance, People, Legal), a standing committee that includes:

- The function head (chair).
- 2–4 senior ICs and managers from within the function.
- The HRBP assigned to the function.
- Optionally, a rotating seat from an adjacent function to add outside perspective.

Committee members should rotate on a 12–18 month cadence to (a) spread the calibration signal across the function and (b) prevent a small clique from becoming the "kingmakers" of the promotion process.

**Cross-function calibration.** After each function-level committee has produced its slate, the function heads meet as a cross-function calibration group (typically the CEO or the head of people chairs) to re-anchor "Staff" or "Senior" or "Principal" across functions. The cross-function meeting does not typically overturn a function-level decision; it exists to surface cross-function drift ("Engineering is promoting 15% of the L4 pool to L5, Product is promoting 3% — why?") and to force the function heads to defend their distributions.

**Executive-level promotions.** Promotions to VP or above are handled outside the function committee — by the CEO with input from the head of people, and, for material officer-level promotions, with a compensation-committee or board consent per [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/). See [chapter 07](./07-executive-team-offboarding.md) for the exec-level end of the same operating system.

## Decision 2 — Criteria authoring

The two failure modes at the criteria layer:

- **Too vague.** The rubric says "Staff engineers drive company-wide impact" and every promotion is a debate about what "company-wide" means.
- **Too mechanical.** The rubric is a 40-line checklist and managers game it by manufacturing checkbox-shaped work rather than by developing the engineer.

The mainstream pattern is a **three-anchor criteria set**:

1. **Competency-anchored.** The employee demonstrably operates at the next level's competencies (per the leveling framework in [mod-106 chapter 01](../mod-106-compensation-architecture-and-total-rewards/01-job-architecture-and-leveling-framework.md)) — not for a single project, but sustained across the review period. "Operating at" is not the same as "aspiring to"; the promotion recognises work already being done, not work the employee might do if promoted.
2. **Sponsor-anchored.** At least one senior person outside the direct-manager relationship (a skip-level, a peer team's lead, a cross-functional executive) will actively vouch for the promotion. A promotion whose only advocate is the direct manager is a promotion that is going to blow up in cross-function calibration.
3. **Impact-anchored.** The employee has produced business impact commensurate with the target level. Impact framing must be concrete and legible to a non-specialist ("shipped X, which produced Y outcome") not narrative-only ("has been a trusted partner across the org").

The three anchors are *conjunctive* — a candidate needs all three. Competency without impact is a "great engineer stuck in maintenance," impact without competency is a "great hack that does not repeat," sponsor without either is a friendship promotion. Any two without the third is a red flag.

**Level-specific criteria.** The rubric per level is authored by the function head with the head of people; it should reference the leveling framework, name the specific competencies the level requires, and give 2–3 concrete examples of what "operating at this level" looks like in this function. Rubrics should be published to the whole function — an employee who cannot read the rubric for their target level is an employee who cannot self-evaluate readiness.

## Decision 3 — Cadence

**Semi-annual promotion cycle** is the mainstream default:

- **Q4 promotion cycle** — reviewed in the November calibration window, announced in December, effective for the January comp cycle in [mod-106](../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md).
- **Q2 promotion cycle** — mid-year cycle, announced in July, effective July or August, funded from the mid-year promotion budget carved out of the annual comp-cycle allocation.

Two cycles per year strike a balance: often enough that a strong employee does not wait 18 months for recognition, rare enough that the committee overhead does not swamp the calendar.

**Off-cycle promotion exception path.** A minority of promotions genuinely cannot wait — a rising Staff engineer who is entertaining an external offer, a VP-level hire being promoted internally at a rate the market is about to force. The exception path:

- **Trigger.** Manager and function head both agree the promotion cannot wait for the next cycle; HRBP concurs.
- **Bar.** The off-cycle promotion must clear the same three-anchor criteria as an on-cycle promotion. The point of the exception is *speed*, not *lower bar*.
- **Approval.** Function-level committee reviews via written motion or a called meeting; cross-function calibration is skipped in favour of a written notice to peer function heads.
- **Volume cap.** No more than ~10% of the function's annual promotions should be off-cycle. Higher than that means the cadence is broken; drop the on-cycle cycle to quarterly or fix the calibration process.

Off-cycle promotions are load-bearing when the corporation is scaling fast enough that six-month cycles genuinely lag; they are pathological when they become the norm and the on-cycle process becomes ceremonial.

## Decision 4 — Communication

Promotions are announced along three axes:

**To the promoted employee.** The direct manager delivers the news in a scheduled 1:1, with a written summary in follow-up: the new title, the new level, the effective date, the comp change (from the comp-cycle output in [mod-106](../mod-106-compensation-architecture-and-total-rewards/04-annual-comp-cycle.md)), any equity refresh (from the grant guidelines in [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/)), and a short paragraph on what the promotion recognises. The manager should also name the sponsors — the promoted employee should know who advocated for them in the room.

**To the team.** A short announcement in the team channel or all-hands meeting, focused on impact — "X is now Y, in recognition of the work they led on Z." Avoid announcements that read as a list of names; each promotion should have a one-sentence rationale.

**To the corporation.** A single all-hands announcement or company-wide email at the end of each cycle lists the promotions. Content: promoted employee names, new titles, one-line impact rationales. This is *the* mechanism by which the corporation signals what it values. If the promotion list runs 40 names deep and no one can remember any of the rationales two weeks later, the announcement was too diffuse to send.

**Timing.** Communicate the promoted-employee news first, the team news second (within 24–48 hours), the corporation-wide news last (typically as a batch at the end of the cycle). Never let a promoted employee find out from an all-hands slide.

## Decision 5 — Not-promoted-signal management

Every cycle, more people are not promoted than promoted. The corporation's job at that boundary is not to hide the outcome — the employees know whether they were considered — it is to prevent the *not-promoted* signal from being read as *not-valued* or *not-progressing*.

**The three not-promoted patterns:**

1. **Not considered this cycle.** Employee is on-track for the next level but not yet ready; manager and employee agreed at the previous check-in that this cycle was too early. The manager confirms the plan for the next cycle in the post-cycle 1:1.
2. **Considered, not promoted, on-track.** Employee was reviewed by the committee; the committee's read is that they are close but not yet operating consistently at the target level. The manager delivers this news in a scheduled 1:1, with a specific paragraph on what would move the decision at the next cycle, framed against the three-anchor criteria (competency, sponsor, impact) so the employee can act on it.
3. **Considered, not promoted, not on-track.** Employee was reviewed and the committee's read is that they are not currently on a promotion trajectory. The manager delivers this news with more care — this is not a PIP conversation (see [chapter 04](./04-pip-mechanics.md)), but it is a career-honesty conversation. The manager should also be honest with themselves about whether this is a leveling problem, a role-fit problem, or an early-signal PIP conversation to plan for.

**The not-promoted communication cadence.** Every employee who was reviewed by the committee — promoted or not — gets a scheduled 1:1 with their manager within one week of the outcome, in which the manager delivers a summary of the committee's read. Employees who were not reviewed (not considered this cycle) get a shorter 1:1 in which the manager confirms the plan for the next cycle. Nobody should be silent on their promotion outcome after a cycle closes.

**Attrition risk.** The single highest attrition-risk moment in the year is the two to eight weeks after a promotion cycle closes, concentrated in the "considered, not promoted, on-track" pool. The head of people should get a report from each manager on this pool within two weeks of cycle close, and should look at retention risk (external offer, expiring vest, disengagement signals) explicitly. Waiting until three of the pool have resigned is waiting too long.

## Concrete example: a Series-B engineering promotion committee

A 30-person engineering organisation at Series-B, split across five teams, running a Q4 promotion cycle.

- **Committee.** Chair: VP Engineering. Members: two Staff engineers (rotating from different teams than the candidates), one Engineering Manager, one Principal engineer (rotating in from Platform), the People Business Partner for Engineering. Optionally: the Head of Product as the cross-function seat.
- **Timeline.** Nominations open in mid-October. Nominators (manager + at least one sponsor) submit a promotion packet — self-narrative from the candidate, manager narrative, sponsor letters, impact evidence, competency-rubric assessment. Committee meets in three sessions during the second and third week of November.
- **Criteria.** Three anchors per candidate — competency (per the E1–E7 engineering-level rubric imported from `cto-curriculum`), sponsor (at least one senior sponsor outside the direct-manager chain), impact (concrete outcomes over the six-month review period).
- **Decisions.** Each candidate is voted: Promote / Not this cycle / Not on-track. Written rationale captured for each. Deferred candidates get a specific paragraph on what would move the decision.
- **Communication.** Managers deliver news to reports in the first week of December, before the corporation-wide all-hands announcement in the second week of December. Comp and equity changes are communicated via the Q1 comp-cycle statement in February.
- **Not-promoted follow-through.** VP Engineering and the People Business Partner review the deferred pool in the fourth week of December for retention risk; the manager of any employee flagged as at-risk gets HRBP support for a 1:1 conversation before the holiday break.

This process runs in ~40 hours of committee time, ~4 hours of manager time per candidate packet, and it produces a defensible outcome the company will stand behind for the next six months.

## Summary

- Promotion is a committee decision, not a manager decision — function-level committee inside each function, cross-function calibration on top.
- The criteria are conjunctive: competency + sponsor + impact. Any two without the third is a red flag.
- Semi-annual cadence is the default; an off-cycle exception path exists but should stay under ~10% of annual promotions.
- Communicate the promotion in three layers — to the employee, to the team, to the corporation — with a one-sentence impact rationale each.
- The not-promoted pool is the highest-attrition-risk cohort of the year. Every reviewed employee gets a debrief 1:1 within a week; the head of people should get a retention-risk report from managers within two weeks.
- See [exercise-02](./exercises/exercise-02-promotion-committee-and-criteria-authoring.md) for the authoring drill.
