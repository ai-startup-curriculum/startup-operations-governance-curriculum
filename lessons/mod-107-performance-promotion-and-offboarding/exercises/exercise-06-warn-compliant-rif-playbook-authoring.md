# Exercise 06 — WARN-compliant RIF playbook authoring

> Estimated time: **~7 hours** · Related chapter: [06 — The RIF / layoff playbook under WARN](../06-rif-and-layoff-playbook-under-warn.md)

## Problem statement

You are the head of people at Fibrelith Networks, a Delaware C-corp at Series-C, 320 employees. The corporation missed its Q3 revenue plan by 35%, extended runway is the board's priority, and the CEO and CFO have converged on the need for a 28% reduction in force — approximately 90 employees. The board has authorised the direction; you have four weeks to design and execute.

Fibrelith's workforce is distributed as follows:

- **California** — 130 employees (San Francisco HQ, 90; Los Angeles satellite, 25; San Diego satellite, 15). 45 employees are age 40+ across California.
- **New York** — 60 employees (NYC office, all in one building). 18 are age 40+.
- **Washington** — 35 employees (Seattle office). 12 are age 40+.
- **Illinois** — 20 employees (Chicago office). 7 are age 40+.
- **Texas** — 15 employees (Austin office). 4 are age 40+.
- **Remote across the rest of the US** — 60 employees (working from 22 additional states, no state with more than 8 employees). 20 are age 40+.

The cut has been sized by function: Engineering 25 of 110; Sales 25 of 60; Marketing 12 of 25; CS 10 of 30; G&A 12 of 40; R&D 6 of 55.

Two dependencies matter:

- **Compensation-committee involvement.** The executive-severance items in the RIF touch [mod-105](../../mod-105-equity-compensation-policy-and-comp-committee/); the comp committee needs to be brought in at the correct point.
- **Executive-level departures.** The RIF includes one VP-level departure (VP Marketing, tenure 3 years, age 51). The general-executive-offboarding playbook is [chapter 07](../07-executive-team-offboarding.md); the RIF interaction with an exec departure is the boundary you need to design.

Author the WARN-compliant RIF playbook end-to-end — board authorisation, impact analysis, WARN Act determination per state, OWBPA disclosure schedule, comms choreography, package design, and anti-signalling operating norms.

## Requirements

### Part A — Board-authorisation memo

Author the RIF memo from CEO to the board:

1. **Business rationale.** Revenue miss, extended-runway objective, cost-reduction commitment. Two-to-three paragraphs, board-audience-appropriate.
2. **Impact summary.** Percentage of workforce, function-by-function view, cost-savings (annualised salary + benefits; one-time severance cost; net savings in year 1).
3. **Recommended package.** Overview of severance-and-benefits structure at the highest level; comp-committee approval requested for VP-level executive severance.
4. **WARN Act analysis summary.** Federal and state per-site analysis; conclusion on whether formal WARN notice is required per jurisdiction; the plan if any state triggers 90-day notice (New York, New Jersey).
5. **Communications plan.** All-hands announcement date and CEO-delivery commitment; individual-conversation window; unaffected-employee comms; customer / investor / press comms.
6. **Board-consent request.** The specific consent asked of the board — unanimous written consent under DGCL § 141(f) for the RIF plan and the interim VP Marketing arrangement; comp-committee approval of the executive-severance package.

### Part B — Impact-analysis document

Author the internal impact-analysis document — the artifact the RIF is executed from and the artifact that survives a subsequent EEOC or wage-and-hour dispute.

1. **By function.** For each function (Engineering, Sales, Marketing, CS, G&A, R&D), the percentage cut, the absolute headcount, the function-head justification for the cut, and the selection-criteria approach (position elimination vs. employee-selection).
2. **By level.** Distribution of the 90 affected employees across levels; whether the cut is concentrated at IC or manager levels or evenly distributed; the defence of the pattern.
3. **By tenure.** Distribution across tenure buckets (0–1 year, 1–3 years, 3+ years).
4. **By work location.** Per-state count of affected employees; the specific state-mini-WARN implication per state.
5. **By demographic slice.** Distribution across gender, race / ethnicity, age 40+, disability, and other protected categories, compared to the workforce baseline. Address explicitly what percentage of the affected pool is age 40+ (the exercise gives you the baseline: 45 CA + 18 NY + 12 WA + 7 IL + 4 TX + 20 remote = 106 of 320 = 33% of workforce). Address the workforce-baseline comparison. If a slice is over-represented, describe the specific selection-criteria review process.
6. **By cost savings.** Total annualised savings; one-time severance cost; net year-1 savings.
7. **Selection-criteria documentation.** For each function, the specific criteria used (performance rating, tenure, cross-functional utility, skill mix for go-forward organisation). The criteria must have been authored before names were placed against them — document the authoring date.
8. **HRBP and general counsel review.** Named review with named reviewer and date.

### Part C — WARN Act determination (federal + per-state)

Author the WARN Act analysis:

1. **Federal WARN — coverage threshold.** Confirm that Fibrelith (320 employees) is above the 100-employee threshold and is a covered employer.
2. **Federal WARN — per-site analysis.** For each Fibrelith site, apply the "single site of employment" test: are the 90 affected employees at any single site that hits 50+ full-time employees representing at least 33%, or 500+ regardless of percentage? Address the SF HQ (90 CA employees; need to know the affected count at SF specifically), LA (25), San Diego (15), NYC (60), Seattle (35), Chicago (20), Austin (15). For the remote population, address the "single site of employment" analysis — remote workers may or may not be treated as a single site depending on facts (see 20 C.F.R. § 639.3).
3. **Aggregation.** Address the 90-day aggregation rule under 29 U.S.C. § 2102(d) — Fibrelith cannot break the layoff into a series of sub-50-person cuts to escape notice.
4. **California WARN.** For each California covered establishment (SF, LA, San Diego), apply the Cal. Labor Code §§ 1400–1408 test: 75+ employees at the covered establishment (SF at 90 qualifies; LA at 25 does not; San Diego at 15 does not); 50+ employees terminated in any 30-day period. Address the affected count at SF specifically.
5. **New York WARN.** Apply NY Labor Law §§ 860–860-i: 50+ NY employees (Fibrelith at 60 qualifies); 25+ affected representing at least 33%, or 250+. 90-day notice required.
6. **Washington, Illinois, Texas.** Illinois WARN (75+ employees, 60-day notice for mass layoff of 33% or 250+): does Fibrelith's Chicago count (20) put Illinois under the state threshold? Washington has no state WARN analogue as of publication; Texas has none. Address for each.
7. **Practical execution.** For each triggered notice, the specific delivery mechanic — notice to affected employees, state dislocated-worker unit, chief elected official of the unit of local government. Notice content per 29 U.S.C. § 2102(a) and 20 C.F.R. § 639.7.
8. **Exceptions.** Whether any federal-WARN exception (faltering-company, unforeseeable business circumstances, natural disaster) applies to Fibrelith's fact pattern. The general read is that a planned revenue-miss-driven RIF does not qualify for the unforeseeable-business-circumstances exception; document the reasoning.
9. **Pay-in-lieu-of-notice.** Address whether Fibrelith will elect to give shorter notice with pay-in-lieu; the state-agency notice remains required.

### Part D — OWBPA disclosure schedule

Author the OWBPA disclosure schedule for the age-40+ pool:

1. **45-day consideration period.** Confirm that Fibrelith is offering the severance package as part of "an exit incentive or other employment termination program offered to a group or class of employees" — triggering the 45-day consideration period for age-40+ employees.
2. **7-day revocation period.**
3. **Written consultation notice.**
4. **Disclosure schedule.** For each age-40+ affected employee, in writing, the four disclosure items under 29 U.S.C. § 626(f)(1)(H): the class / unit / group of individuals covered, the eligibility factors, the applicable time limits, and the job titles and ages of all individuals eligible or selected for the program and the ages of all individuals in the same job classification or organizational unit who are not eligible or selected. Author an example disclosure schedule for the Engineering function.
5. **The definition of "organizational unit."** Fact-specific per chapter 06 — typically the smallest business unit within which the selection decisions were made (a team, a function, a department). Author Fibrelith's specific definition for each function.
6. **Strict-compliance rule per *Oubre v. Entergy Operations, Inc.***, 522 U.S. 422 (1998). Address the consequence of any omission — the release is unenforceable as to ADEA claims.
7. **Employment-counsel review.** Named review and date.

### Part E — Executive-communications choreography

Author the T-minus timeline and the delivery-day choreography:

1. **T-7 days.** Board / comp-committee confirmation; legal review of individual notice packets and severance-and-release agreements complete; HRBP / IT / finance-ops runbook aligned.
2. **T-2 to T-1.** Manager training (chapter 05 delivery-day script rehearsal per manager); notice packets prepared; individual conversations scheduled.
3. **T-day morning.**
   - All-hands or CEO video message announcing the RIF — timing and content.
   - Manager 1:1s with affected employees in a coordinated 60–90 minute window.
   - Manager check-ins with unaffected reports within hours.
4. **T-day + 1 to T-day + 3.** Q&A sessions; HRBP office hours; individual severance / COBRA / equity questions.
5. **T-day + 7 to T-day + 45.** Signed severance-and-release agreements returned within the OWBPA windows.

Author the specific words the CEO uses in the all-hands opening. Author the manager script for the individual notice conversation (per chapter 05 — 15 minutes, empathy + finality + clarity). Author the unaffected-employee follow-up communication.

### Part F — Package design

Author the severance-and-benefits package:

1. **Cash severance.** 3 weeks per year of service, minimum 12 weeks, per chapter 06's suggested more-generous-than-default framing. Address VP-level severance separately.
2. **COBRA subsidy.** Length in months tied to severance length; corporate-paid portion; how the subsidy is delivered (direct subsidy vs. cash gross-up).
3. **Equity treatment.** Post-termination exercise window extension — chapter 06 references 12–24 months as a material benefit. Cordwainer's specific choice; the mod-105 equity-policy handoff for approval.
4. **PTO payout.** Per corporation policy and California / New York state law.
5. **Bonus payment.** Prorated bonus if the RIF lands after the bonus performance period but before payment.
6. **Outplacement services.** Which provider (from the resources list — Randstad RiseSmart, LHH, INTOO, Careerminds); the specific service level (3-month, 6-month); the per-employee cost. Executive-level upgraded outplacement for the VP Marketing.
7. **References.** Written commitment to provide standard references; manager-authored LinkedIn recommendation opt-in.
8. **Alumni / re-hire signalling.** Chapter 08 handoff for the alumni programme and rehire-eligibility flag.
9. **VP Marketing package overlay.** The executive-severance items that require compensation-committee approval per [mod-105](../../mod-105-equity-compensation-policy-and-comp-committee/) — cash severance beyond policy default; equity-vesting acceleration if applicable; the CoC-trigger analysis if Fibrelith is in any early-stage strategic-transaction conversation.

### Part G — Anti-signalling operating norms

Author the anti-signalling policies during and after the RIF:

1. **During.** CEO leads all-hands and every subsequent follow-up. Head of people, GC, CFO visible in office hours. Managers trained and supported. Hiring-freeze theatre avoided (be honest about ongoing critical hiring). No same-week promotions or exec-comp announcements.
2. **After.** All-hands cadence every 1–2 weeks for the following 4–8 weeks. Retention risk management — head of people identifies retention risks in the remaining organisation; targeted retention conversations; retention-bonus authorisation through comp committee.
3. **The "no-second-cut" honesty.** Whether Fibrelith commits to no further cuts, or whether it declines to make that commitment. The honest position given the fact pattern.
4. **Alumni investment.** Explicit programme of outplacement, references, extended PTE window, alumni-network invitation.

### Part H — Executive-team offboarding overlay (VP Marketing)

The VP Marketing departure is a RIF-scoped executive departure and needs the [chapter 07](../07-executive-team-offboarding.md) executive-offboarding overlay applied. Author:

1. **CEO-VP-Marketing difficult conversation.** Held before the general all-hands; separate from the manager-line RIF conversation; the CEO delivers, head of people joins for the package walkthrough.
2. **Board choreography.** Notice to the board before the general employee announcement; comp-committee approval of any above-policy severance items.
3. **Indemnification continuation.** Reaffirmed in the separation agreement per DGCL § 145.
4. **D&O coverage.** Confirmed continuing during the executive's period of service.
5. **Board-seat resignation.** Not applicable (VP Marketing does not hold a board seat), but confirm.
6. **Employee announcement.** Written announcement from CEO; recognition paragraph co-authored with departing VP; live all-hands within 24 hours of the announcement.
7. **External comms.** Fibrelith is Series-C but not yet public — no 8-K obligation. IR outreach to lead investors before the general announcement (chapter 06 anti-signalling norm: lead investor should not read about a material RIF on LinkedIn).

## Starter guidance

- Chapter 06 is the primary reference. The seven operating decisions plus the exec-departure interaction with chapter 07 are the frame.
- The WARN Act analysis is the load-bearing legal spine. Get the "single site of employment" test right per 20 C.F.R. § 639.3; do not aggregate across sites you should not aggregate; and do not fail to aggregate the individual losses in the 90-day window per 29 U.S.C. § 2102(d).
- The California WARN Act has a lower threshold than federal (75-employee covered-establishment vs. 100-employee federal-employer). The Cal-WARN "unforeseeable business circumstances" exception was narrowed by California courts — assume the exception does not apply to a planned revenue-miss-driven RIF.
- The New York WARN Act requires 90-day notice (not 60); Fibrelith has 60 NY employees, over the 50-employee threshold; the affected count needs to be 25+ representing at least 33%, or 250+. Do the math against the specific affected NYC count.
- The OWBPA 45-day consideration period is triggered by the "group or class of employees" test. Do not use a 21-day consideration period for age-40+ RIF-affected employees.
- The OWBPA disclosure schedule under § 626(f)(1)(H) is unforgiving — omission voids the ADEA waiver per *Oubre*. Get the four elements right and get the definition of "organizational unit" right.
- The remote-employee analysis under WARN is fact-specific. 20 C.F.R. § 639.3(i) treats a "single site of employment" as either a single geographic location or a group of contiguous locations; remote employees may be treated as reporting to the location that is their primary base of operations. Assume Fibrelith's remote employees report administratively to SF HQ for benefits and payroll purposes; flag `<!-- needs-research -->` and cite the ambiguity if you cannot resolve the question against 20 C.F.R. § 639.3.
- The VP Marketing departure is an executive offboarding per chapter 07 running inside a RIF per chapter 06. Both frameworks apply; the exercise wants the overlay executed cleanly.
- Do not fabricate specific selection criteria for functions — the exercise gives you the aggregate cut per function, and you author the general selection-criteria pattern. Do not invent specific individuals or performance data.
- Do not invent specific WARN Act state-agency contacts or notice-content boilerplate. Chapter 06 and resources.md have the framework; the exercise wants the recognition of the framework and the specific triggers per state, not the boilerplate.
- Every severance-and-release agreement in the RIF has to satisfy chapter 05 (Speak Out Act, state Silenced No More, *McLaren Macomb* NLRA) plus the OWBPA group-release additions from chapter 06. The chapter-05 template is the base; the OWBPA additions layer on.
- Equity treatment on separation, including any extended PTE window and any executive-severance-triggered acceleration, defers to [mod-105](../../mod-105-equity-compensation-policy-and-comp-committee/). Name the handoff points; do not author the equity-policy substance.
- The CoC-trigger analysis for the VP Marketing (if Fibrelith is in any pre-transaction conversation) is chapter 07 and mod-105 territory. The exercise notes it — you do not need to author it, but you need to name the question so the comp committee reviews before signing.

## Deliverables

- `board-authorisation-memo.md` — Part A.
- `impact-analysis.md` — Part B, the internal analytical document.
- `warn-act-determination.md` — Part C, federal + per-state analysis with specific triggers noted per site.
- `owbpa-disclosure-schedule.md` — Part D, including an example disclosure for the Engineering function.
- `comms-choreography.md` — Part E, T-minus timeline, CEO all-hands opening words, manager script, unaffected-employee follow-up.
- `package-design.md` — Part F, general-workforce package plus the VP Marketing overlay.
- `anti-signalling-norms.md` — Part G.
- `exec-offboarding-overlay-vp-marketing.md` — Part H, applying chapter 07 to the RIF's exec departure.

## Acceptance criteria

The package is acceptable if:

1. The board-authorisation memo (Part A) is board-audience-appropriate, requests a specific DGCL § 141(f) consent, and separates the general RIF authorisation from the comp-committee approval of executive severance.
2. The impact analysis (Part B) covers all six slices (function, level, tenure, work location, demographic, cost savings); documents selection criteria authored before names were placed; and includes HRBP and general counsel review with dates.
3. The WARN Act determination (Part C) applies both federal and per-state (California, New York, Washington, Illinois, Texas, remote) tests site-by-site; addresses the 90-day aggregation rule; addresses each state-mini-WARN's specific threshold; and reaches a specific triggered / not-triggered conclusion per notice statute.
4. The remote-employee "single site of employment" question is addressed with reference to 20 C.F.R. § 639.3, with any residual ambiguity flagged with `<!-- needs-research -->` and specific counsel-review requested.
5. The OWBPA disclosure schedule (Part D) covers the 45-day consideration period, 7-day revocation, written consultation notice, the four § 626(f)(1)(H) items, a specific example disclosure for Engineering, and the definition of "organizational unit" per function. The *Oubre* strict-compliance rule is acknowledged.
6. The comms choreography (Part E) has the T-minus timeline, specific CEO all-hands opening words, a manager script, and unaffected-employee follow-up communication.
7. The package design (Part F) covers cash severance, COBRA subsidy, extended PTE window, PTO payout, bonus, outplacement (with specific vendor from resources.md), references, and alumni signalling — plus the VP Marketing overlay with executive-severance items requiring comp-committee approval.
8. The anti-signalling norms (Part G) address during-and-after; include the honest treatment of the "no-second-cut" question; include the retention-risk management with retention-bonus authorisation through comp committee.
9. The VP Marketing exec-offboarding overlay (Part H) applies chapter 07 — CEO-executive conversation, board choreography, indemnification / D&O reaffirmation, employee announcement with recognition paragraph, IR outreach to lead investors before the general announcement.
10. Every severance-and-release agreement in the RIF satisfies the chapter 05 requirements (Speak Out Act, state Silenced No More per state, *McLaren Macomb* NLRA) plus the OWBPA group-release additions.
11. Equity treatment on separation defers to [mod-105](../../mod-105-equity-compensation-policy-and-comp-committee/); executive-severance-triggered acceleration defers to mod-105 and comp committee; the CoC-trigger analysis is named as a comp-committee review item.
12. Any specific statute cited (29 U.S.C. §§ 2101–2109; 20 C.F.R. Part 639; Cal. Labor Code §§ 1400–1408; NY Labor Law §§ 860–860-i; 29 U.S.C. § 626(f)) is verifiable against [resources.md](../resources.md) or flagged.
13. Nothing left as `[TBD]` or `[FILL IN]`.
