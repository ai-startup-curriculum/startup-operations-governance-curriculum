# Exercise 05 — Remote / hybrid / RTO operating policy authoring

> Estimated time: **~5 hours** · Related chapter: [05 — Remote / hybrid / RTO operating policy](../05-remote-hybrid-rto-operating-policy.md)

## Problem statement

Marcato Health is a Series-C vertical-SaaS corporation selling a revenue-cycle and prior-authorisation workflow product into mid-market US health systems. The corporation is 285 employees, Delaware C-corp, closed a $62M Series C fifteen months ago led by a growth-stage investor who sits on the board. Headcount split: 160 engineering (ICs plus eng-management), 55 go-to-market (AEs, SEs, CS), 40 product and design, 30 G&A. The corporation was founded fully-remote in Q2 2020 and operated remote-first through 2022, hiring aggressively against the remote-first pitch; the founder-CEO and founder-CTO sit in Austin, where the corporation holds a 14-person office that is day-use only. A second office opened in Toronto at Series-B as a Canadian-engineering pod (now 42 employees); the remainder of the workforce is spread across 28 US states and 4 Canadian provinces, with concentrations in NYC (18 employees), the Bay Area (14), Chicago (11), and Denver (9). Compensation is currently a 3-zone geo-tiered band structure authored under [mod-106](../../mod-106-compensation-architecture-and-total-rewards/) at Series-B: Zone 1 (SF / NYC / Boston / Seattle), Zone 2 (Austin / Toronto / Chicago / Denver / LA / DC), Zone 3 (remainder of US and Canada). The exec team is nine-strong: founder-CEO, founder-CTO, COO (external, 11 months in), CFO (external, 20 months in), CRO (external, 7 months in), CPO (external, 2 years), head of people (internal promote, 10 months in-seat), general counsel (external, 4 months in), head of design (internal promote, 18 months in-seat).

Three facts are forcing the posture decision now. First, the founder-CEO returned from a board offsite two weeks ago having been told by two board members and the lead-growth-stage investor that "the best companies in our portfolio are 5 days a week in office" and he has sent a Slack note to the exec team saying he wants to "move to 5 days in Austin and Toronto by end of Q1." Second, the CPO's org has quietly signalled a parent-cohort attrition risk — exit-interview data over the last six months shows four of six voluntary departures in product-and-design cited "being asked to come to an offsite that collided with school-pickup" or "the increasing in-person expectation" as a material factor; the head of people has correlated this against HRIS and roughly 38 of the 285 employees are primary caregivers of children under 10. Third, an accommodation request has been sitting in the head of people's queue for eleven days: a senior backend engineer in Zone 3 (rural Pennsylvania, hired fully-remote in 2021) has submitted a request citing a chronic autoimmune condition and immunocompromised status, with physician documentation, asking that her existing remote arrangement be preserved regardless of any posture change. The request names 42 U.S.C. § 12112(b)(5) and 29 C.F.R. § 1630 and is clearly drafted with the help of counsel. Separately, a cohort of 23 engineers were hired fully-remote in 2021–2022 at metros more than 100 miles from either Austin or Toronto; several have signalled, through their managers, that an in-office requirement would be a de-facto relocation demand they would decline.

The head of people has eight weeks to walk into an exec-team posture-decision meeting with (a) a defensible counter to the founder-CEO's 5-days-in-office push, (b) a written policy the corporation can publish through the handbook instrument in [chapter 02](../02-employee-handbook-nlrb-compliant-post-stericycle.md), (c) a specific disposition for the pending ADA accommodation, (d) a wired linkage to the geo-tiered pay strategy, (e) an in-person cadence calendar the CFO can price, and (f) a DE&I-impact assessment and rollout plan that the parent cohort, the caregiver cohort, the disability cohort, and the distant-metro cohort can read without concluding the corporation hired them under false pretences. Author the full package.

## Requirements

### Part A — Position memo

A one-page memo the head of people will circulate to the exec team before the posture-decision meeting. It must:

1. **Recommend one of the four defensible postures** from chapter 05 — remote-first, hybrid-by-default, office-first, or RTO-with-exceptions — for Marcato Health specifically. Do not duck the choice; "flexible" is not a posture.
2. **Honestly state the trade-off paragraph** chapter 05 requires before announcing any posture: what hires it loses, what retention cost it accepts, what collaboration cost it incurs, what the recommended posture explicitly buys.
3. **Counter the founder-CEO's 5-days-in-office push** on the evidence. Reference Bloom, N., Han, R., & Liang, J. (2024). "Hybrid Working from Home Improves Retention Without Damaging Performance." *Nature*, 630, 396–401 as the canonical anchor on the retention-vs-performance evidence base, and reference GitLab's All-Remote Handbook as the canonical anchor on the operating discipline a non-office-first posture requires. Any benchmark number not in chapter 05 or resources.md gets `<!-- needs-research: ... -->`.
4. **Name the three populations most-exposed** to the proposed shift (parent / caregiver cohort, disability-accommodation cohort, distant-metro-hire cohort) and the retention cliff each represents in order of magnitude.
5. **State the decision rule** the memo asks the exec team to adopt — either accept the recommendation, counter with a specific alternative posture, or defer by a defined number of weeks pending additional data (and name the data).

### Part B — Written policy

The policy section Marcato Health will publish through the handbook instrument. Draft the operative text, not a summary. Cover:

1. **Posture statement.** The named posture from Part A, in plain language the workforce can read.
2. **Cadence.** Days per week in office; specific named days (Tuesdays and Thursdays, or similar) vs. "flexible within the week"; the discipline that supports the choice. If the posture is hybrid-by-default, the named commute radius for in-office expectation and the treatment of employees outside the radius.
3. **Geographic eligibility.** Who the posture applies to (metro-resident, distant-metro-remote, Toronto pod, international). How a new hire's posture is determined on offer.
4. **Exception / accommodation path.** The entry point to the accommodation process in Part C; the discipline that managers do not grant informal accommodations.
5. **Enforcement mechanic.** The published pattern — written conversation → written warning → separation — and the discipline that posture non-compliance absent an approved accommodation is treated as a performance matter, not a cultural matter. Pair the enforcement stance with the ADA interactive-process route so the policy does not read as coercive against employees with pending accommodation requests.
6. **Review cadence.** When the policy itself is reviewed and the triggers that force an earlier review.

### Part C — Accommodation process under the ADA

Author the written accommodation-process document the corporation will publish alongside the policy. Reference 42 U.S.C. § 12112(b)(5) and 29 C.F.R. § 1630 as the statutory and regulatory anchors. Defer the substantive employment-law architecture — the ADA-interactive-process discipline, the state-law overlay, the medical-certification standard, the retention of accommodation records — to [mod-103](../../mod-103-employment-law-and-contract-design/). The chapter-05-owned mechanics are:

1. **Intake.** The form, the inbox or HRIS surface where the request lives, the acknowledgement timeline (chapter 05 names 15 business days from complete submission as a defensible decision timeline; a shorter acknowledgement-of-receipt is expected).
2. **Interactive-process rhythm.** Who runs the conversation (head of people with HRBP support, per chapter 05); the cadence of exchanges with the employee; the role of the direct manager (route-and-acknowledge, not decide-informally).
3. **Documentation posture.** What is retained in the employee file; what is retained outside the file for legal-hold reasons; the discipline that written-accommodation-letter outcomes land in writing with named effective dates.
4. **Borderline-case escalation.** The named decision point at which the head of people routes the matter to employment counsel, deferring to [mod-103](../../mod-103-employment-law-and-contract-design/) for the substantive standard. Marcato Health has a general counsel; name whether general counsel is the first stop or whether external employment counsel is retained for the ADA-interactive-process review.
5. **Specific disposition for the pending request.** The named senior backend engineer with physician documentation, immunocompromised status, and a counsel-drafted request citing 42 U.S.C. § 12112(b)(5) is in-queue. Write the disposition: what the written-accommodation-letter outcome will be, the specific posture modification (preserved full-remote; preserved full-remote with named offsite-attendance accommodation; preserved full-remote with named medical-exception from in-person onboarding), and the effective-date-and-duration posture (open-ended; annual review; tied to the duration of the medical certification). Do not invent the ADA legal-test outcome — defer the legal determination to counsel — but author the operating disposition the head of people will publish once counsel signs off.

### Part D — Geographic-pay interaction

Defer the comp-band mechanics — refresh cadence, band-width, mid-point-plus-range design, the specific zonal percentages — to [mod-106](../../mod-106-compensation-architecture-and-total-rewards/). The chapter-05-owned mechanics are the *posture* decisions that pin the pay strategy. Author a short memo covering:

1. **Linkage.** The posture from Part A pins Marcato Health's geo-tier strategy how, specifically? If hybrid-by-default anchored to Austin and Toronto, do the two offices become Zone 2 anchors or does the posture elevate Austin to Zone 1? If office-first, how does the three-zone structure collapse? If remote-first-preserved, does the three-zone structure survive unchanged?
2. **Relocation-eligible employees.** If the policy opens a relocation-eligible path (an employee outside the commute radius elects to move to Austin or Toronto to join the in-office cadence), does the employee land in the named-office-metro comp band on relocation, or is there a transitional treatment? Where does the mechanic live (mod-106) vs. the posture (chapter 05)?
3. **Employee-initiated moves across zones.** The HRIS currently records work-location and the location change routes to the comp-band lookup. When an employee moves from a Zone 1 metro to a Zone 3 location, what is Marcato Health's posture — grandfather the existing comp band, re-anchor to the destination zone, re-anchor at the next annual comp cycle? Chapter 05 owns the *posture*; defer the band mechanic to [mod-106](../../mod-106-compensation-architecture-and-total-rewards/).
4. **Transitional grandfathering.** If the posture shift materially changes any employee's comp-band eligibility, what is the written grandfathering treatment and what is the sunset date? Chapter 05's RTO-with-exceptions row names grandfathering as the defensible path; adopt or depart from that pattern explicitly.

### Part E — In-person-cadence calendar

Author the 12-month in-person calendar the head of people will publish to the workforce. Chapter 05's forum table (company all-hands offsite, function offsites, onboarding week, leadership summit, team on-site, exec offsite) is the spine. For each forum:

1. **Cadence.** How many per year under the Part A posture.
2. **Attendees.** Named population — full company, named function, directors-and-above, exec-only.
3. **Duration.** Days per event.
4. **Location.** Named city or rotation rule. Austin and Toronto are the two owned-office metros; chapter 05 does not require offsites to run from owned offices.
5. **Month placement.** The specific month (and, where relevant, week) each forum lands in the 12-month calendar. Bracket the leadership summits around the annual-planning cycle per chapter 05.
6. **Attendance norm.** The chapter-05 discipline that in-person forums are default-mandatory for the invited population, with travel accommodations (visa, caregiver, disability, medical) routed through the Part C accommodation process. Do not run optional offsites.

Present as a table or a month-indexed list. Reference the chapter 05 "cost side" note — Marcato Health's CFO is entitled to see the annual programme costed out — and name the specific line items the CFO's model should carry (travel, venue, F&B, swag, offsite ops), without inventing dollar figures.

### Part F — DE&I-impact assessment & rollout comms

Chapter 05 names an impact assessment on named populations as mandatory input to a posture-shift announcement. Author the full package:

1. **Impact assessment.** For each of four named cohorts, a short paragraph covering: cohort size (headcount, approximate percentage of workforce), the specific operating impact of the Part B posture on this cohort, the retention-risk estimate (qualitative — high / meaningful / low — not a fabricated number), the specific mitigations the Part B policy and the Part C accommodation process offer.
   - The **parent cohort** (approximately 38 primary caregivers of children under 10, per the problem statement).
   - The **caregiver cohort** (adults with eldercare, chronic-illness-adjacent, or single-parent responsibilities not already captured in the parent cohort — size unknown; name the data-collection step).
   - The **disability cohort** (employees with ADA-cognisable accommodations open, pending, or likely-to-arise under the new posture; the named senior backend engineer sits here).
   - The **distant-metro cohort** (approximately 23 engineers hired fully-remote in 2021–2022 at metros more than 100 miles from either owned office).
2. **CEO all-hands rollout script.** The founder-CEO's spoken rollout at the all-hands where the policy is announced. 400–600 words. The script must name the trade-off explicitly, name the three most-exposed cohorts explicitly, name the accommodation route explicitly, name the notice window explicitly, and avoid the "we trust our people" or "flexible" formulations chapter 05 identifies as anti-patterns. Draft the script in the founder-CEO's voice; do not draft the head of people's talking points as if the CEO were reading them.
3. **Written FAQ.** 5–8 anticipated workforce questions with Marcato-Health-specific answers. At minimum: the parent-cohort question (school-pickup / caregiver friction), the distant-metro-hire question (is this a de-facto relocation demand), the accommodation-process question (how do I request), the geo-pay question (what happens to my band), the notice-period question (when does the shift take effect), the enforcement question (what happens if I don't comply). Avoid the "legal-review softening" chapter 05 warns about — publish the honest answer, not a hedged one.
4. **Rollout sequencing.** The order in which populations learn about the shift: exec team → extended leadership → affected-population 1:1s → all-hands → written FAQ → handbook update. Chapter 05 does not script the sequencing in detail; apply the discipline that no employee learns about a policy change affecting them personally from an all-hands slide.

## Starter guidance

- Chapter 05 is the primary reference. The six operating decisions (position selection, geographic-pay interaction, collaboration norms, in-person cadence, tool stack, RTO shift framework) map directly to the parts above. Part A is Decision 1; Part B is the operating output; Part C is the chapter 05 side of the accommodation framework (with [mod-103](../../mod-103-employment-law-and-contract-design/) carrying the legal mechanics); Part D is Decision 2 as it defers to [mod-106](../../mod-106-compensation-architecture-and-total-rewards/); Part E is Decision 4; Part F includes the Decision 6 equity-and-inclusion implications.
- The founder-CEO push for 5 days in office is the forcing function on Part A. Ducking it — recommending "flexible hybrid" or "it depends by team" — is a fail. Chapter 05 is explicit that the fifth option is the absence of a posture, not an alternative to one.
- The named ADA accommodation request is the forcing function on Part C. The exercise wants the operating disposition, not the legal determination. Defer the legal test to counsel per [mod-103](../../mod-103-employment-law-and-contract-design/); do not author the ADA interactive-process standard from scratch.
- GitLab's All-Remote Handbook (see resources.md) is the canonical operating-discipline anchor for any non-office-first posture Part A recommends. Reference it; do not plagiarise it.
- Bloom, N., Han, R., & Liang, J. (2024) *Nature* 630:396–401 is the canonical retention-and-performance anchor the position memo can cite. Any specific figure from the paper not reproduced in chapter 05 gets `<!-- needs-research: ... -->` — refresh the citation before quoting the figure.
- Do not invent Buffer *State of Remote Work* benchmarks, SWAA survey percentages, or vendor-published retention statistics. Resources.md flags each with `<!-- needs-research: ... -->`; propagate the discipline into your draft.
- Do not invent real peer company names. Chapter 05's concrete example uses "a hypothetical B2B SaaS corporation" — follow the pattern.
- Part E's cost note is deliberate — chapter 05 warns against under-investing in cadence as a false economy. Do not under-sell the programme to the CFO in the calendar; name the forums the posture needs.
- The DE&I-impact assessment in Part F is the specific instrument chapter 05 requires before an RTO announcement. The engagement-measurement interaction (slicing manager-effectiveness, belonging, and career-development-confidence scores by remote vs. in-office population) lives in [chapter 04](../04-engagement-measurement-and-action-planning.md) — reference it where relevant; do not re-author it.
- Nothing in this exercise is a legal determination. The ADA interactive process, the state-law overlay on caregiver status, and the works-council / cross-border mechanics for the Toronto pod are deferred to [mod-103](../../mod-103-employment-law-and-contract-design/) and [mod-113](../../mod-113-international-expansion-and-global-workforce/) respectively. Flag the deferrals; do not author the mechanics.

## Deliverables

- `position-memo.md` — Part A.
- `written-policy.md` — Part B.
- `accommodation-process.md` — Part C.
- `geographic-pay-interaction.md` — Part D.
- `in-person-cadence-calendar.md` — Part E.
- `dei-impact-assessment-and-rollout.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. Part A names one of the four chapter-05-defensible postures (remote-first, hybrid-by-default, office-first, RTO-with-exceptions) for Marcato Health, carries an honest trade-off paragraph, and counters the founder-CEO's 5-days-in-office push on the evidence — citing Bloom et al. (2024) and GitLab's All-Remote Handbook as the canonical anchors from resources.md.
2. Part B's written policy is operative text (not a summary), covers posture, cadence, geographic eligibility, exception / accommodation path, enforcement mechanic, and review cadence, and avoids the "flexible" / "we trust our people" anti-patterns chapter 05 flags.
3. Part C's accommodation process references 42 U.S.C. § 12112(b)(5) and 29 C.F.R. § 1630, defers the substantive ADA-interactive-process standard to [mod-103](../../mod-103-employment-law-and-contract-design/), and specifies a named operating disposition for the pending senior-backend-engineer accommodation request — including the posture-modification outcome, the effective-date-and-duration posture, and the counsel-sign-off step.
4. Part D names the posture-to-geo-pay linkage, the relocation-eligible-employee treatment, the employee-initiated-move posture, and the transitional-grandfathering stance, deferring the band mechanics (refresh cadence, zonal percentages, mid-point-plus-range design) to [mod-106](../../mod-106-compensation-architecture-and-total-rewards/).
5. Part E's 12-month calendar covers each forum from the chapter 05 table (all-hands offsite, function offsites, onboarding week, leadership summit, team on-sites, exec offsite) with named cadence, duration, location, and month placement, and includes the CFO-side cost note without inventing dollar figures.
6. **Part F includes a concrete DE&I-impact assessment on each of the four named cohorts (parent, caregiver, disability, distant-metro) — cohort size, specific operating impact, qualitative retention-risk estimate, and specific mitigations tied to the Part B policy and the Part C accommodation process.** A generic "we considered DE&I impact" statement without the per-cohort analysis is unacceptable.
7. Part F's CEO all-hands rollout script is 400–600 words, in the founder-CEO's voice, names the three most-exposed cohorts explicitly, names the accommodation route, names the notice window, and avoids the chapter-05-flagged anti-patterns.
8. Part F's written FAQ covers at minimum the six anticipated workforce questions named in the requirements, each with a Marcato-Health-specific answer rather than a generic HR template answer.
9. Any benchmark or market number not in chapter 05 or resources.md is flagged with `<!-- needs-research: ... -->` — current-year Buffer *State of Remote Work* benchmarks, specific figures from Bloom et al. (2024) beyond those reproduced in chapter 05, SWAA survey percentages, travel-and-venue spend as a share of people-cost, and vendor pricing. No real peer company names are invented; nothing is left as `[TBD]` or `[FILL IN]`.
10. Deferrals to sibling modules are named explicitly where the chapter 05 ownership boundary assigns the mechanic elsewhere — [mod-103](../../mod-103-employment-law-and-contract-design/) for the ADA legal architecture, [mod-104](../../mod-104-hiring-onboarding-and-hr-operations/) for HRIS-side location-field configuration, [mod-106](../../mod-106-compensation-architecture-and-total-rewards/) for comp-band mechanics, [mod-113](../../mod-113-international-expansion-and-global-workforce/) for the Toronto pod's cross-jurisdiction overlay, [chapter 02](../02-employee-handbook-nlrb-compliant-post-stericycle.md) for the handbook-publication instrument, [chapter 04](../04-engagement-measurement-and-action-planning.md) for engagement measurement of the remote-vs-in-office experience, and [chapter 07](../07-internal-communications-operating-rhythm.md) for the cross-time-zone rhythm.
