# 4. The employee-engagement measurement programme

> Measure on a defensible cadence, publish results fast, force a visible executive-team response, cascade to manager-level action, and hold the question set stable — anything else is survey theatre and destroys the response rate you rely on.

## Motivation

Engagement measurement is the single most-frequent way a well-intentioned people-ops function makes things worse. The failure mode is not that the survey is badly designed. The failure mode is that the survey runs, a slide deck is published, and then nothing visible happens for a year. Employees learn — correctly, from evidence — that filling in the survey does not change the workplace. The response rate craters and the signal degrades until the survey is a report on how few people still bother to respond.

Four concrete failure patterns to build against:

- **Response-rate collapse from silence.** The corporation launches an engagement survey with an 82% response rate. The next cycle prints results, the executive team receives a briefing, and no company-wide action lands. The next cycle response rate is 63%. The one after that is 41%. The head of people escalates that "we have an engagement problem" — the actual problem is that the executive team never closed the loop on the previous three cycles.
- **Redesign every cycle destroys year-over-year comparison.** A new head of people arrives, dislikes the previous question set, adopts a new vendor with a different question bank, and the corporation loses the ability to compare this year's belonging score against last year's. Two years later a new hire in the seat repeats the exercise. The company has run engagement surveys for five years and can compare no metric across any two consecutive cycles.
- **Anonymity violation at small team size.** A team of three receives its own team-level anonymous results. Everyone on the team can back-solve who said what. One employee raised a concern about their manager; the manager reads the result, works out who it was, and the trust cost of the survey is now negative. The rule that team-level slices require a minimum team size (>=5 hard, >=8 safer) exists because of exactly this pattern.
- **Executive silence read as disinterest.** The survey closes. Results are shared with the executive team. Five months pass with no executive-team communication about what they heard and what they intend to do. Employees infer — again, correctly — that the executive team either did not read the results or does not care. The next survey cycle response rate reflects that inference.

The purpose of an engagement-measurement programme is not "to measure engagement." It is to run a **calendared, disciplined loop** — measure, respond fast, force manager action, hold the question set stable, protect anonymity, and track that promised actions actually shipped — so that filling in the next survey is a rational thing for the employee to do.

## The cadence — four survey types

An engagement-measurement programme is not a single instrument. It is a portfolio of four surveys, each with a different purpose and cadence.

| Survey | Length | Frequency | Purpose |
|---|---|---|---|
| Quarterly pulse | 10–15 questions, 5–10 minutes | Every quarter | Detect movement between annuals; test targeted interventions |
| Annual deep-dive | 50–80 questions plus open-text | Once per year | Full dimensional read; year-over-year comparison; benchmark anchor |
| Onboarding pulse | 8–12 questions, ~5 minutes | Day 30 and Day 90 post-hire | Detect onboarding failure early; feed into hiring / onboarding fixes |
| Exit / alumni | 15–25 questions plus structured interview | On departure; alumni follow-up 6–12 months later | Regretted-attrition root-cause; alumni network health |

**Quarterly pulse.** A short instrument sent to the full company. The point is trend detection, not full-dimensional coverage. Keep 4–6 anchor questions constant across every pulse (eNPS is the obvious one) and rotate 4–8 topical questions to test whatever the executive team is investing in this quarter (a new career framework, a return-to-office policy, a manager-training rollout).

**Annual deep-dive.** The full instrument. This is the one that produces the dimension-level scores in the section below, the manager-level cascade, and the year-over-year comparison. It is long enough to hurt if the respondent does not believe it matters — which is why the action-planning workflow further down is not optional.

**Onboarding pulse (30-day and 90-day).** New hires are the population whose engagement signal changes fastest and whose feedback is the most-actionable. Two short pulses — one at ~30 days (initial impressions, manager clarity, tooling) and one at ~90 days (role fit, ramp support, retention risk) — feed directly into the hiring and onboarding programme in [mod-104](../mod-104-hiring-onboarding-and-hr-operations/). Do not lump onboarding pulses into the quarterly pulse cohort; the question set is different and the signal degrades if it is diluted.

**Exit and alumni.** The exit survey is the last chance to hear from a departing employee, and the alumni survey (sent 6–12 months post-departure) captures the more-honest reflection that people give once they are no longer worried about a reference. Both feed into the alumni / rehire-eligibility loop in [mod-107 chapter 08](../mod-107-performance-promotion-and-offboarding/08-alumni-rehire-eligibility-and-feedback-loop.md). Do not double-count exit responses in the main engagement scores — leavers are a different population and mixing them distorts the trend.

## The tool landscape

The mainstream vendors, with the axes that actually matter for selection:

| Vendor | Strong at | Weak at | Typical stage fit |
|---|---|---|---|
| [Culture Amp](https://www.cultureamp.com/) | Question-bank quality, benchmarking data, action-planning workflow | Price at low headcount; can feel heavy for pulse-only use | Series-A → growth |
| [Lattice Engagement](https://lattice.com/) | Integration with Lattice performance / 1:1 / goals | Benchmarking depth vs Culture Amp | Series-A → Series-B if already on Lattice |
| [15Five Engage](https://www.15five.com/) | Manager-level workflow; lightweight | Deep-dive dimensional analysis | Seed → Series-A |
| [Officevibe (Workleap)](https://workleap.com/officevibe/) | Weekly pulse cadence; low-friction UX | Enterprise reporting; benchmark customisation | Seed → Series-A |
| [Peakon (Workday Peakon Employee Voice)](https://www.workday.com/en-us/products/employee-voice/overview.html) | Continuous listening; sophisticated driver analysis; Workday integration | Cost; complexity at small scale | Growth (particularly if on Workday HCM) |
| [Glint (LinkedIn / Microsoft Viva Glint)](https://www.microsoft.com/en-us/microsoft-viva/glint) | Manager-level reporting UX; Microsoft ecosystem integration | Vendor roadmap volatility through the LinkedIn → Viva transition <!-- needs-research: current Viva Glint roadmap and general-availability status as of authoring date --> | Growth |
| [Qualtrics EmployeeXM](https://www.qualtrics.com/employee-experience/) | Survey-design flexibility; deep analytics; enterprise scale | Overkill and expensive below several-hundred headcount | Growth → enterprise |

**Selection criteria to actually weight** (borrow the discipline from [mod-107 chapter 01](../mod-107-performance-promotion-and-offboarding/01-performance-management-operating-system.md) on tool selection):

1. **Question-bank quality.** A vetted, validated bank of items with published psychometric properties beats questions the head of people writes on a Friday afternoon. Every mainstream vendor supplies one; check that the vendor will let you keep anchor items constant across cycles even if they update the rest of the bank.
2. **Benchmarking data availability.** External benchmarks (industry, stage, geography) are useful for context but dangerous as a target — do not run the programme against a benchmark. Weight this criterion after the year-over-year comparison capability.
3. **Manager-level reporting UX.** Managers will not action results they cannot easily read. The manager dashboard is the single feature that determines whether the action-planning workflow below actually happens.
4. **HRIS integration.** The vendor needs to pull org chart, level, tenure, location, and reporting-line from the HRIS ([mod-104](../mod-104-hiring-onboarding-and-hr-operations/)) so that team-level and slice-level cuts are correct without manual data wrangling.
5. **Action-planning workflow.** Structured prompts for the team-level action conversation, a visible tracker for committed actions, and a re-check mechanism at the next cycle. This is the feature that separates "we ran a survey" from "we ran a programme."
6. **Data-export capability.** Never buy a vendor that will not export your raw response data. You will change vendors.

**Stage decision:**

- **Seed (≤~20 employees).** A Google Form (or Typeform) is the right answer. Question bank is copy-pasted from the vendor benchmarks or from an open reference like the Q12. The head of people (often the founder) runs analysis in a spreadsheet. Cost: zero. This is not primitive — at that headcount, a dedicated tool's per-seat cost is not defensible and the analytical horsepower is wasted.
- **Series-A (~30–75 employees).** A dedicated tool becomes worthwhile. Manager cascade, anonymity guarantees at team-level slice, and a validated question bank are the reasons; do not defer past this point or you will bake bad habits into a growing organisation.
- **Series-B → growth (~75–300 employees).** The dedicated tool is now load-bearing. Manager-level reporting UX and action-planning workflow are the two features that determine renewal.
- **Growth stage and beyond (~300+ employees).** The HCM engagement module (Workday Peakon, SuccessFactors, Dayforce equivalents) may make sense — particularly if you already operate the HCM for payroll and HRIS. Whether to consolidate or keep a dedicated vendor alongside the HCM depends on whether the HCM's manager UX is competitive. Frequently it is not.

## Dimension design

The annual deep-dive should cover the dimensions below. Keep an anchor set of items constant across years; add new items rather than replacing anchors.

### eNPS (employee Net Promoter Score)

A single-question 0–10 item: "How likely are you to recommend {Company} as a place to work?" Score is computed as % promoters (9–10) minus % detractors (0–6). eNPS is easy to run, easy to trend, and easy to over-interpret — it is a *coarse* number and should never be the only engagement metric the executive team looks at. But it is a defensible anchor across cycles and it is broadly understood, so it earns its place.

### Engagement (multi-item)

A composite of typically 4–8 items covering pride in the company, motivation, discretionary effort, and intent-to-stay. Avoid conflating engagement with satisfaction — an employee can be highly satisfied (comfortable pay, easy work) and not engaged (no discretionary effort, no pride). Sample item shapes:

- "I am proud to work at {Company}."
- "I am motivated to go above and beyond in my role."
- "I see myself working at {Company} in 12 months."
- "I would recommend {Company} to a friend looking for a job."

### Manager effectiveness (multi-item)

A composite covering the manager relationship. Typically 6–10 items. This is the dimension that drives the manager-effectiveness feedback loop further down. Sample item shapes:

- "My manager gives me actionable feedback on a regular basis."
- "My manager supports my career development."
- "My manager sets clear expectations about my work."
- "I feel comfortable raising concerns with my manager."
- "My manager treats me with respect."

### DEI / inclusion

Post-SFFA (see [chapter 03](./03-dei-programme-design-post-sffa.md) for the full legal frame), the safer design measures **inclusion outcomes** — belonging, fairness, voice — rather than making programmatic inferences from race / gender. Items should ask about the employee's experience of the workplace, not about the demographics of who was hired or promoted. Sample item shapes:

- "I feel a sense of belonging at {Company}."
- "People at {Company} treat each other with respect."
- "I feel that I can be my authentic self at work."
- "I believe that people at {Company} are treated fairly regardless of background."
- "My perspective is heard and valued by my team."

The inclusion score can and should be sliced by demographic dimension (with the anonymity thresholds in the action-planning workflow) to detect experience gaps. What the corporation *does* about those gaps is a programme-design question addressed in [chapter 03](./03-dei-programme-design-post-sffa.md) — the survey's job is to expose the gap, not to prescribe the remedy.

### Wellbeing

A composite covering workload, burnout risk, and mental-health support. Wellbeing is the dimension most likely to move in a bad direction during a growth spike or a difficult quarter, and the one whose movement most directly predicts regretted attrition. Sample item shapes:

- "My workload is sustainable."
- "I am able to disconnect from work when I need to."
- "I have the support I need to manage stress at work."
- "{Company} genuinely cares about my wellbeing."

### Leadership / executive-team confidence

A composite covering trust in the executive team, confidence in decision-making, and clarity of company direction. This is often the dimension the executive team is least keen to see printed and the one that most requires them to respond visibly. Sample item shapes:

- "I have confidence in the executive team's leadership."
- "The executive team makes decisions that are good for the long-term health of the company."
- "The executive team is transparent about the company's direction."

### Strategy clarity

A composite covering whether employees understand the company's strategy and how their work contributes. High engagement in the absence of strategy clarity is a warning sign — employees are motivated but rowing in different directions. Sample item shapes:

- "I understand {Company}'s strategy."
- "I understand how my work contributes to {Company}'s goals."
- "Priorities are clear across the organisation."

## The action-planning workflow

This is the section that separates programmes from theatre. The workflow is a **calendared response loop** with published deadlines.

| Milestone | Deadline (from survey close) | Owner | Output |
|---|---|---|---|
| Raw results processed; anonymity thresholds applied | 3 business days | People-ops analyst | Cleaned dataset; slice-level cuts prepared |
| Results briefing to executive team | 2 weeks | Head of people | Full deck; dimension trends; slice highlights; open-text themes |
| Executive-team response drafted and prioritised | 3 weeks | Executive team collectively | 3–5 company-level commitments with owners and dates |
| Company-wide communication of results + executive response | 4 weeks | CEO + head of people | All-hands presentation; written follow-up; question channel open |
| Manager-level cascade (team results delivered where team size >=5) | 5 weeks | People-ops + managers | Manager dashboard access; briefing session for managers |
| Team-level action conversations completed | 8 weeks | Every manager | Structured team discussion; 1–3 team-level commitments logged |
| Action tracker published (company-level + team-level commitments) | 9 weeks | Head of people | Visible tracker; quarterly re-check schedule |

**The executive-team-response-timing norm.** The four-week deadline between survey close and company-wide response is not arbitrary. Anything longer than that reads as disinterest to employees; anything shorter typically means the response is a reflex rather than a considered position. Hold the line on the deadline even when the results are difficult — a difficult response delivered on time is orders of magnitude better than a polished response delivered late.

**The anonymity threshold for team-level cascade.** Team-level results are only shared where the team is large enough that individual responses cannot be back-solved. The mainstream rule is a minimum team size of 5; a safer rule is 8. Below that threshold, the manager receives an aggregated view against the next-level-up team, but not their own team's discrete results. Configure the vendor to enforce this at the platform level — do not rely on the head of people to remember.

**The structured team action-planning conversation.** Managers are not researchers. Do not hand them a dashboard and hope for the best. Provide a scripted 45-minute agenda:

1. **Share the results** (5 minutes). Manager walks through the team's scores against company benchmark.
2. **Identify the top 1–2 areas of strength** (10 minutes). The team names what is working. This is not a warm-up — anchoring on strengths gives context for the improvement conversation.
3. **Identify the top 1–2 areas to improve** (15 minutes). The team names what is not working. Manager listens more than they talk.
4. **Commit to 1–3 team-level actions** (10 minutes). Specific, owner-attributed, deadline-attached. "The manager will publish a written team charter by end of month" is a valid commitment; "we will improve communication" is not.
5. **Log the commitments in the tracker** (5 minutes). Live, in the room, before the meeting ends.

**The visible action tracker.** Every commitment — company-level from the executive team, team-level from the manager conversations — lands in a tracker that any employee can view. The tracker shows: commitment, owner, deadline, status. The next survey cycle explicitly re-checks whether committed actions shipped, and the results are read against that record. This is the single mechanism that most reliably prevents survey theatre.

## Year-over-year comparison discipline

The temptation to move questions between surveys — because a new head of people prefers a different framing, or a new vendor's question bank is subtly different, or the executive team wants to "freshen up" the instrument — is real and near-constant. Resist it.

- **Baseline metrics must persist across at least three years to be interpretable.** A dimension score with two years of data is a slope, not a trend. Three years is the minimum to distinguish a real movement from a survey-artefact fluctuation.
- **Add new questions rather than replacing anchor items.** If a topic emerges that the anchor set does not cover, extend the instrument. The cost of a longer survey (some completion-rate drag) is much lower than the cost of losing a year-over-year anchor.
- **Document the anchor set explicitly.** Maintain a written list of the anchor items — the ones that never change — and require any change to those items to be approved by the head of people and reviewed against the year-over-year cost.
- **Do not switch vendors casually.** A vendor switch usually means an anchor break. If the switch is justified, run one cycle in parallel — same population, both instruments — so that the corporation can calibrate the old-vendor score against the new-vendor score and preserve trend interpretation.

## Response-rate discipline

Response rate is a direct measure of programme health. A programme with declining response rate is a programme that employees have stopped believing in.

- **Series-A / Series-B target: 70%+ response rate on the annual deep-dive.** Below 70% the results start losing reliability at slice-level cuts. Below 50% the results are anecdotal and should be flagged as such.
- **Pulse response rate is typically lower** than deep-dive response rate (shorter instrument, more frequent ask). A ~60% pulse response is a reasonable working target; a persistent decline is the leading indicator of survey theatre.
- **Diagnose falling response rate as an action-planning failure, not a communication failure.** The reflex when response rate drops is to send more reminder emails. The correct response is to audit whether the last cycle's committed actions shipped, and to communicate the audit result.
- **Do not pressure managers to hit team-level response targets.** Once managers are incentivised on response rate, they lean on their teams to respond, and anonymity guarantees erode. The right lever is executive-team visibility on the action loop, not manager pressure on the survey.

## The manager-effectiveness feedback loop

Manager-effectiveness scores are one of the highest-signal outputs of the engagement programme. They connect back into manager development and, in the tail, into performance management.

- **Development-first response for the average case.** A manager with a middling-or-low manager-effectiveness score gets coaching and a development plan (see [mod-107 chapter 03](../mod-107-performance-promotion-and-offboarding/03-development-growth-plans-and-l-and-d-programme.md)). The score is one input to the development plan, not a rating in itself.
- **Coaching engagement for materially-low scores in a single cycle.** A score meaningfully below the company distribution in a single cycle triggers an HRBP-led conversation with the manager, a specific coaching engagement, and a shared plan of what will change before the next cycle.
- **Performance-system engagement for sustained low scores.** If manager-effectiveness scores remain materially low across multiple cycles despite coaching, the pattern feeds into the performance-management operating system in [mod-107 chapter 01](../mod-107-performance-promotion-and-offboarding/01-performance-management-operating-system.md). Sustained inability to manage a team is a performance issue and needs to be treated as one; masking it with "engagement is complicated" fails both the manager and their reports.
- **Do not publish manager-effectiveness scores publicly.** They are shared with the manager, the manager's manager, and the HRBP. Public ranking of managers by team engagement score is a reliable way to turn the survey into a political instrument and destroy the honesty of responses.

## Concrete example: a Series-B, 200-person company

A B2B SaaS company, Series-B, ~200 employees across three geographies. HRIS on Rippling; performance on Lattice; engagement on Culture Amp. Head of people plus one people-ops analyst; five-person executive team; twenty-eight managers.

**Cadence.** Quarterly pulse in weeks 4 of each quarter (13 anchor items plus 5 rotating items). Annual deep-dive in Q3 (weeks 36–38; 62 items plus open-text). Onboarding pulse at day 30 and day 90 for every new hire (automated in Culture Amp). Exit survey administered by people-ops on last day of employment; alumni survey sent nine months post-departure.

**Twelve-month operating calendar:**

| Week | Event |
|---|---|
| Week 4 | Q1 pulse opens; runs 10 days |
| Week 7 | Q1 pulse results to executive team; brief written response to company by week 8 |
| Week 17 | Q2 pulse opens; runs 10 days |
| Week 20 | Q2 pulse results to executive team; brief written response to company by week 21 |
| Week 36 | Annual deep-dive opens; runs 12 days |
| Week 38 | Deep-dive closes |
| Week 40 | Results briefing to executive team (2 weeks from close) |
| Week 41 | Executive-team response drafted; 3–5 company commitments logged |
| Week 42 | All-hands company communication (4 weeks from close) |
| Week 43 | Manager-level cascade opens (dashboards live; manager briefing) |
| Week 46 | Team action conversations completed (8 weeks from close); commitments logged |
| Week 47 | Action tracker published |
| Week 4 (next year) | Q1 pulse re-checks progress on committed actions |

**Manager cascade rules.** Team size threshold set to 5 in the Culture Amp configuration; managers with teams below the threshold receive their next-level-up view only. Manager-effectiveness scores shared with manager, manager's manager, and HRBP. Culture Amp action-planning workflow used for team action conversations; commitments export to an Asana tracker accessible to all employees.

**Feedback loop into manager development.** Two managers show manager-effectiveness scores materially below the company distribution across the Q1 pulse and the annual deep-dive. HRBP runs a coaching engagement with each; development plans logged in Lattice; re-checked at Q3 the following year. One manager's scores improve on the next annual; one does not, and the pattern moves into the [mod-107 chapter 01](../mod-107-performance-promotion-and-offboarding/01-performance-management-operating-system.md) performance conversation.

This programme runs in roughly one FTE-day per week of people-ops analyst time, an average of one hour per manager per quarter, and ~15 minutes of employee time per pulse plus ~45 minutes for the annual. It is boring and predictable, which is again the point.

## Ownership boundary

- **Engagement measurement (this chapter)** owns the instrument, the cadence, the anonymity guarantees, the executive-response loop, and the action tracker.
- **Manager development and the performance system ([mod-107](../mod-107-performance-promotion-and-offboarding/))** own what happens to a manager whose team engagement is materially low across multiple cycles. This chapter surfaces the signal; that module acts on it.
- **DEI programme design ([chapter 03](./03-dei-programme-design-post-sffa.md))** owns the response to inclusion-dimension gaps. This chapter measures belonging and fairness; that chapter designs the interventions in a post-SFFA legal frame.
- **Onboarding programme ([mod-104](../mod-104-hiring-onboarding-and-hr-operations/))** owns the response to the day-30 and day-90 pulses. This chapter runs the instrument; that module fixes the onboarding.
- **Role-specific engagement nuance** — the engagement dynamics of a product / GTM organisation versus an engineering / infrastructure organisation differ meaningfully. See `startup-product-gtm-curriculum` for the product-and-GTM-side nuance and `cto-curriculum` for the engineering-org-side nuance. This chapter provides the cross-functional operating spine; those curricula provide the role-specific overlay.

## Summary

- Engagement measurement is a programme, not a survey. The programme's health is measured by whether committed actions ship, not by the topline score.
- Run four surveys with different purposes: quarterly pulse, annual deep-dive, onboarding pulse (day 30 / day 90), and exit / alumni. Do not lump them together.
- Buy a Google Form at seed, a dedicated tool at Series-A, and consider the HCM engagement module at growth stage. Weight manager-level reporting UX and action-planning workflow above benchmarking depth in selection.
- Design the instrument around dimensions — eNPS, engagement, manager effectiveness, inclusion, wellbeing, leadership confidence, strategy clarity — and keep an anchor item set constant across years.
- Anonymity threshold at team size >=5 (safer at >=8); configure the vendor to enforce it. Never publish manager-effectiveness scores publicly.
- The action-planning loop is calendared: results to executive team within 2 weeks; executive response and commitments within 4 weeks; manager-level cascade within 5 weeks; team action conversations within 8 weeks; visible action tracker published within 9 weeks.
- Year-over-year comparison discipline: add questions, do not replace anchors; document the anchor set; do not switch vendors casually.
- Response rate is a leading indicator of programme health. 70%+ at Series-A / Series-B is the working target. A declining response rate is a symptom of an action-planning failure, not a communication failure.
- Manager-effectiveness scores feed into manager development ([mod-107 chapter 03](../mod-107-performance-promotion-and-offboarding/03-development-growth-plans-and-l-and-d-programme.md)) and, for sustained low scores, into the performance system ([mod-107 chapter 01](../mod-107-performance-promotion-and-offboarding/01-performance-management-operating-system.md)).
- See [exercise-04](./exercises/exercise-04-engagement-survey-and-action-planning-drill.md) for the drill.
