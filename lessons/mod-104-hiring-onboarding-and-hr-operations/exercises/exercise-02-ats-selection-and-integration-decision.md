# Exercise 02 — ATS selection and integration decision

> Estimated time: **~4 hours** · Related chapter: [02 — The ATS: selection, integration, and graduation triggers](../02-ats-selection-and-integration.md)

## Problem statement

You are the Head of Talent at Blueharbor Robotics, a Series-A robotics startup that just closed a $28M round. Today the company runs hiring on a Google Sheet, a shared Gmail label, and a founder-owned LinkedIn Recruiter Lite seat. Blueharbor has 26 employees across California, Massachusetts, Washington, and New York, and plans to hire 40+ additional employees in the next 18 months across engineering (mechanical, ML, firmware), product / design, GTM, ops, and G&A. The corporation has enterprise-customer engagements pending a SOC 2 Type I attestation and expects Series-B people-ops diligence within 24 months.

The CFO has approved a recruiting-tooling budget for the first 12 months. Board expectations: the corporation adopts an ATS within 60 days of your start, wires it into the corporation's other systems, and stands up the compliance and diligence artifacts (structured scorecards, EEO self-identification, background-check workflow, pay-transparency logging). No preferred vendor has been selected.

The corporation also has one specific complication: two of the four founders were previously on Greenhouse at a prior startup and prefer it; the CEO has heard "Ashby is the modern choice" from a peer CEO and is leaning that way; the incoming VP Engineering used Lever at their last two companies. Everyone has an opinion; nobody has yet made the decision on the merits.

Produce (a) an ATS selection decision, (b) an integration-stack design, (c) a graduation-trigger memo, and (d) an implementation plan for the first 90 days.

## Requirements

### Part A — ATS selection

Produce a decision memo picking one ATS from the seed → Series-B window (Ashby, Greenhouse, Lever, Workable) for Blueharbor. Cover:

1. **The decision framework** you applied — analytics needs, sourcing intensity, structured-hiring opinionation, existing tooling relationships, recruiter familiarity, HRIS integration story, budget. (Chapter 02 names these; use them as the axes.)
2. **The scoring or comparison** across at least three of the four candidates. Do not pretend this is a data-driven optimum; it is a judgment call. Show the judgment.
3. **The final selection** with a short justification (2–4 sentences). Address the internal politics — the two founders on Greenhouse, the CEO's Ashby lean, the VP Eng's Lever history — either accommodating or explicitly overriding.
4. **The rejected options** — for each, the specific reason it was not chosen. Do not write "not as good"; write the specific constraint.
5. **The graduation horizon** — what stage of company Blueharbor should be at before considering the next ATS, and what would trigger a graduation earlier than that. (For a Series-A pick, a defensible answer is "we intend to stay on this ATS through Series-B; graduation triggers before that are covered in Part C.")

### Part B — Integration stack design

Produce the integration-stack design for the chosen ATS. For each of the five integration surfaces the chapter names, specify:

1. **HRIS / PEO integration.** Which HRIS or PEO the ATS will hand off to at offer acceptance (defer the deep HRIS decision to exercise 07, but name what the corporation is on today and where the handoff goes). What data is handed off (legal name, preferred name, personal email, work email once provisioned, start date, role, department, manager, compensation, equity, work location, employment type, signed offer letter). How the handoff is validated (automated field mapping vs. manual review).
2. **LinkedIn Recruiter (RSC) and LinkedIn Talent Insights.** Which LinkedIn Recruiter tier the corporation buys, how many seats and for whom, whether the corporation licenses Talent Insights, and how the RSC integration is configured (which candidates surface in-app, dedupe rules, ownership assignment).
3. **Interview scheduling.** Whether the corporation uses the ATS-native scheduler or a dedicated product (ModernLoop, GoodTime, Prelude, Calendly). Justify against the panel complexity and interviewer count. Specify the load-balancing rules the corporation will operate against and the interviewer-training-status gate (only certified interviewers can be scheduled for a given interview type — see [chapter 03](../03-structured-interviewing.md)).
4. **Background-check integration.** Which CRA the corporation uses (Checkr, Sterling, HireRight, Accurate, GoodHire) and how it is wired into the ATS's post-offer workflow. Specify the pipeline stage at which the disclosure and authorisation are sent, how the standalone-disclosure requirement is honoured (see [chapter 04](../04-reference-and-background-checks.md)), and how pre-adverse-action and adverse-action workflows are templated.
5. **Assessment / interview-intelligence tools.** Which engineering assessment platform the corporation uses (CoderPad, CodeSignal, HackerRank, HackerEarth), whether the corporation deploys interview-intelligence recording (Metaview, BrightHire, Pillar), and — critically — the two-party-consent posture for California, Massachusetts, and Washington candidates. Reference the consent-capture flow before recording begins.

### Part C — Graduation-trigger memo

Produce a short memo naming the graduation triggers between ATS products Blueharbor will monitor over the next 24–36 months. Cover:

1. Triggers that would prompt a mid-Series-A migration (nearly always a bad idea — say why, and name the failure modes that would nevertheless justify it).
2. Triggers that would prompt a Series-B or growth-stage migration (analytics gap, sourcing-CRM gap, HRIS-graduation coincidence).
3. The trigger that would prompt a move to an HCM-native ATS (Workday Recruiting, SuccessFactors Recruiting, iCIMS) — this is a growth-stage decision Blueharbor will not face for years but should name.
4. A written migration playbook for whichever future graduation the corporation might face — the chapter's migration checklist walked through end-to-end (locked cut-over date, full candidate + pipeline data export, req-by-req import, source-of-hire mapping, integration re-configuration, shadow-run period, retention of source-ATS data export).

### Part D — 90-day implementation plan

Produce a Gantt-style or milestone-list plan for the first 90 days of ATS deployment. Cover:

1. **Weeks 1–2 — Vendor selection and contract.** Vendor meetings, reference checks, contract execution.
2. **Weeks 2–4 — Implementation kickoff.** Requisition-and-scorecard schema, user roles and permissions, EEO self-identification setup, offer-letter templates (including state-specific pay-transparency disclosures — see [mod-103 chapter 03](../../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md)).
3. **Weeks 3–6 — Integration wiring.** HRIS / PEO handoff, LinkedIn Recruiter RSC, scheduling, background-check CRA, assessment tools.
4. **Weeks 4–8 — Data migration.** Every candidate currently in the Google Sheet, LinkedIn message inbox, or founder email folder is migrated into the ATS with source-of-hire attribution preserved where possible.
5. **Weeks 6–10 — Interviewer training and rollout.** All current interviewers trained on the ATS (submitting scorecards, refusing to interview without a scorecard, cross-contamination prevention). Structured-hiring workflow gates enabled (see [chapter 03](../03-structured-interviewing.md)).
6. **Weeks 8–12 — Compliance and diligence artifacts.** State pay-transparency logging turned on, EEO-1 self-identification captured, FCRA disclosure templates state-aware, adverse-action templates versioned. Diligence-readback pilot with one closed req to confirm the artifact set is coherent.
7. **Week 12 — Sunset the spreadsheet.** No new candidate goes into any system other than the ATS. Old spreadsheet archived to the corporate record.

Each milestone has an owner, a target date (relative to your Day 0 start), and a definition of "done."

## Starter guidance

- Chapter 02 is the primary reference. The five-integration-surface framing (HRIS, LinkedIn, scheduling, background check, assessment) is the design skeleton.
- The chapter's worked example (Series-A SaaS company choosing between Ashby and Greenhouse) is directly analogous. Blueharbor's specifics — the CEO / VP Eng preference conflict, the enterprise-customer SOC 2 posture, the California / Massachusetts / Washington two-party-consent footprint — are what make it a real decision.
- Do not manufacture ATS pricing. Where you cite a per-seat cost, name it as a `<!-- needs-research -->` item and specify what the corporation will confirm before contract signature.
- The "which ATS is best" answer is almost never "objectively X." The right answer is "the one the Head of Talent will run day-in / day-out through the next 24 months." Own the recommendation.
- The migration checklist in the chapter is deliberately conservative; a corporation running a first-time ATS deployment (not a migration between ATSes) can compress most of it, but the compliance-artifact steps (Week 8–12) are not optional even for a first deployment.
- Do not confuse the ATS decision with the HRIS decision — the chapter draws a bright line between the two (pre-hire system of record vs. post-hire system of record). The HRIS decision is exercise 07.
- The two-party-consent state list is not exhaustive in the chapter; refresh it before deploying an interview-intelligence tool.

## Deliverables

- `ats-selection-decision.md` — Part A.
- `integration-stack-design.md` — Part B.
- `graduation-trigger-memo.md` — Part C.
- `90-day-implementation-plan.md` (or `.xlsx` / `.csv` if you prefer a Gantt view) — Part D.

## Acceptance criteria

The package is acceptable if:

1. Part A explicitly picks one ATS and rejects the others with specific reasons; it does not say "either would work."
2. The decision engages with the internal politics (two founders' Greenhouse preference, CEO's Ashby lean, VP Eng's Lever history) rather than ignoring them.
3. All five integration surfaces are covered in Part B with a specific product / vendor named for each.
4. The FCRA-integration design references the standalone-disclosure requirement and the state-analogue FCRA landscape (California ICRAA, others). It does not just say "we'll use Checkr."
5. The interview-intelligence deployment (if included) explicitly addresses two-party-consent for California, Massachusetts, and Washington candidates.
6. The graduation-trigger memo names at least one *quantitative* trigger (concurrent open reqs, panel size, time-to-fill, functional pipeline volume) for each transition.
7. The 90-day plan has ≥15 milestones with owners and target dates; it is not a bullet list of intentions.
8. The plan ends with the spreadsheet sunset — no new candidate goes anywhere other than the ATS after week 12.
9. Compliance artifacts (state pay-transparency logging, EEO-1 self-identification, FCRA disclosure templates, adverse-action templates) are called out as their own workstream rather than assumed.
10. Every market price / feature claim is either cited to chapter 02 or flagged with a `<!-- needs-research -->` marker.
