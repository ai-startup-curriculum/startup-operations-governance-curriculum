# 2. The ATS: selection, integration, and graduation triggers

> An ATS is not a spreadsheet you pay for. It is the corporation's system of record for every candidate, every conversation, every scorecard, every offer — and Series-A / Series-B people-ops diligence reads it end to end.

## Motivation

The Applicant Tracking System is the operational spine of the hiring function. Every candidate the corporation talks to should exist as a record in the ATS. Every scorecard from every interviewer should live there. Every offer should be sent through it. Every source-of-hire attribution, funnel-conversion metric, and time-to-fill statistic that the head of talent or CEO ever reports comes out of it.

An ATS is not just a convenience — it is a *compliance* and *diligence* artifact:

- **EEOC and OFCCP diligence** (for federal contractors) requires the corporation to demonstrate a defensible hiring process — one that applies the same evaluation criteria to comparably situated candidates. That defensibility lives in the ATS: the scorecard for every candidate at every stage.
- **State pay-transparency laws** (Colorado, New York, Washington, California, Illinois — see [mod-103 chapter 03](../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md)) require the corporation to show what range was disclosed and when. The ATS is where the disclosed range is captured against every posted req.
- **FCRA-compliant background checks** (see [chapter 04](./04-reference-and-background-checks.md)) are ordered through the ATS's background-check integration; the disclosure, authorisation, results, and adverse-action correspondence are stored against the candidate record.
- **I-9 workflow** (see [chapter 05](./05-i9-and-e-verify.md)) is typically kicked off from the ATS's onboarding module or handed off to the HRIS.

The corporation that runs hiring on a spreadsheet and an inbox for the first 40 hires will need to reconstruct all of the above for Series-B diligence — and cannot.

This chapter covers (a) the ATS product landscape and where each product fits, (b) the integration stack the ATS should be wired into, and (c) the graduation triggers between products.

## The ATS product landscape

Four ATS products dominate the venture-backed startup market from seed through Series-B / early growth:

- **Ashby** — modern, analytics-first ATS with a native ATS + CRM + scheduling + analytics + interview-intelligence architecture. Strong at ATS-native reporting and at reducing tool-stack sprawl. Increasingly the default for startups launching a hiring function in the 2020s.
- **Greenhouse** — long-established, structured-hiring-opinionated ATS with a deep integration marketplace and a strong track record with Series-A → post-IPO companies. Historically the "gold standard" for structured interviewing.
- **Lever** — CRM-forward ATS with strong outbound-sourcing tooling; merged product lines under the Employ Inc. umbrella (which also owns Jobvite). Historically strong at high-volume sourcing organizations.
- **Workable** — SMB-friendly, lower-cost ATS well suited to companies with modest hiring volume and standard needs. Common at pre-seed / seed startups looking for a low-friction starting point.

<!-- needs-research: confirm current pricing tiers, feature sets, and product-line ownership for Ashby, Greenhouse, Lever, and Workable; product positioning has shifted materially over 2022–2026 and needs a current source before quoting specifics. -->

There are other ATS products in the market — Recruitee, SmartRecruiters, Teamtailor, iCIMS, Workday Recruiting, SuccessFactors Recruiting — but they are typically outside the seed → Series-B window. iCIMS and the HCM-native ATS modules (Workday, SuccessFactors) show up at growth-stage / public-company scale, when the HRIS has already graduated to a full HCM (see [chapter 07](./07-hris-peo-payroll-stack.md)).

### Rough stage-fit map

| Stage | Headcount | Common ATS choice |
|---|---|---|
| Pre-seed / seed | 1–15 | Ashby, Workable, or Greenhouse — pick the one whose starting price and time-to-value match the founder's constraint. |
| Series-A | 15–50 | Ashby or Greenhouse most commonly. Some companies stay on Workable through Series-A. |
| Series-B | 50–200 | Ashby or Greenhouse. Lever remains in market for CRM-heavy sourcing orgs. |
| Growth stage | 200–1,000+ | Ashby or Greenhouse; some companies begin evaluating the HCM-native ATS as the HRIS graduates. |
| Post-IPO / enterprise | 1,000+ | Workday Recruiting, SuccessFactors Recruiting, iCIMS — HCM-native ATS becomes the norm. |

The stage-fit is a starting point, not a rule. A pre-seed team that will hire 20 people in the first 12 months is often best served picking the ATS they intend to stay on through Series-B rather than migrating twice.

## What the ATS must do

The ATS is not just a candidate database. A working ATS provides:

1. **Requisition management.** Every open role is a req with a job description, a hiring team, a scorecard, a target start date, an approved compensation range, and an approval chain.
2. **Candidate pipeline management.** Every candidate is a record moving through stages (sourced → applied → recruiter screen → hiring-manager screen → on-site loop → offer → hired / rejected). Every stage change is a timestamped, attributable event.
3. **Scorecards.** Every interviewer submits a structured scorecard against a pre-defined competency rubric (see [chapter 03](./03-structured-interviewing.md)). Scorecards are visible to the debrief, not to interviewers who have not yet completed their scorecard (to prevent cross-contamination).
4. **Interview scheduling.** Native or third-party, tied to interviewer calendars and to a room / video-call resource.
5. **Sourcing / CRM.** Candidate records exist before they apply — a sourced candidate is a candidate; the CRM tracks outbound outreach, response, and re-engagement.
6. **Referral tracking.** Employees can refer candidates through a portal; source-of-hire captures referrer for the bonus policy.
7. **Offer management.** Offer letters generated from a template with the disclosed compensation range, benefits summary, and any state-specific pay-transparency disclosures.
8. **Reporting and analytics.** Time-to-fill, source-of-hire, offer-accept rate, funnel-conversion by stage, EEO-1 self-identification (voluntary), interviewer bar (score distribution per interviewer), and pipeline health by req.
9. **EEO / diversity self-identification (voluntary).** Candidates may self-identify race, gender, veteran status, disability status. The corporation stores this data separately from the hiring-decision workflow (the ATS enforces this segregation).
10. **Integrations.** HRIS, calendar, email, LinkedIn Recruiter, background-check vendor, assessment tools, e-signature, and interview-scheduling tools.

## The integration stack

An ATS on its own is a database. An ATS wired into the surrounding stack is an operating system. The five integration surfaces every startup ATS must be wired into:

### Integration 1 — The HRIS / PEO

The ATS is the *pre-hire* system of record; the HRIS or PEO is the *post-hire* system of record. The hand-off happens when the offer is accepted. Every ATS in the seed → Series-B window integrates with the common HRIS / PEO products (Rippling, Gusto, Deel, Justworks, TriNet, Sequoia One — see [chapter 07](./07-hris-peo-payroll-stack.md)).

The hand-off should carry, at minimum: legal name, preferred name, email (personal for pre-boarding communications, work email once provisioned), start date, role / department / manager, compensation, equity grant details, work location, employment type (W-2 employee vs. contractor), and the accepted offer letter as an artifact. The HRIS then triggers the onboarding workflow — offer-letter countersign, I-9, PIIA sign-off, benefits enrollment (see [chapter 06](./06-first-90-day-onboarding.md)).

An unintegrated hand-off (recruiter emails the offer letter and the payroll admin manually types the new hire into the HRIS) is where new-hire records diverge from the source of truth in the ATS. Insist on the integration.

### Integration 2 — LinkedIn Recruiter (and LI Talent Insights)

LinkedIn Recruiter is the outbound-sourcing workhorse across every stage. The ATS-LinkedIn Recruiter integration (RSC — Recruiter System Connect) surfaces the corporation's ATS candidate records inside LinkedIn Recruiter's search UI, so that a sourcer searching LinkedIn can see whether a candidate is already in the pipeline, which stage, and who owns them. Without RSC, sourcers duplicate outreach and burn candidate goodwill.

LinkedIn Talent Insights is a separate LinkedIn product for talent-market analytics — headcount trends at competitors, hiring / attrition rates by function, geography, and skill. Distinct from Recruiter (which is candidate-facing); Talent Insights is a strategy tool for the head of talent and, at growth stage, the CPO.

<!-- needs-research: confirm the current LinkedIn Recruiter and Talent Insights pricing tiers and RSC integration requirements. -->

### Integration 3 — Interview scheduling

Interview scheduling is the single largest source of coordinator overhead in a growing recruiting function. Common products:

- **ModernLoop, GoodTime, Prelude** — dedicated interview-scheduling products that orchestrate multi-interviewer, multi-panel scheduling against interviewer calendars, load-balancing rules, and interview-training status.
- **Calendly, Cal.com** — general-purpose scheduling; sufficient at seed but stresses at Series-A once panels become multi-interviewer.
- **Native ATS scheduling** — Ashby, Greenhouse, and Lever all have native scheduling that has closed most of the feature gap versus the dedicated products. Ashby's native scheduling in particular is often cited as competitive with the dedicated products.

A common Series-A / Series-B pattern is to start on the ATS-native scheduler and evaluate a dedicated product only if / when the coordinator function is measurably over-loaded.

### Integration 4 — Background checks and identity verification

The ATS should trigger the background-check order (Checkr, Sterling, HireRight, Accurate, GoodHire, and others) at the appropriate stage in the pipeline (usually post-offer, contingent). The FCRA disclosure and authorisation forms should be sent through the ATS (with the standalone-disclosure requirement respected — see [chapter 04](./04-reference-and-background-checks.md)); the results should be attached to the candidate record; adverse-action correspondence should be initiated through the same integration.

The equivalent identity-verification integration is I-9 (Form I-9 and the E-Verify overlay — see [chapter 05](./05-i9-and-e-verify.md)). Most HRIS platforms (Rippling, Gusto, Deel, Justworks, TriNet) run I-9 workflow natively; the ATS hands off to the HRIS after offer acceptance.

### Integration 5 — Assessment and interview-intelligence tools

For engineering: CoderPad, CodeSignal, HackerRank, HackerEarth. For structured cognitive / behavioural: Wonderlic, Criteria, Predictive Index (with EEOC caveats — see [chapter 03](./03-structured-interviewing.md)). Interview-intelligence (recording + transcript + AI summary): Metaview, BrightHire, Pillar.

Interview-intelligence tools sit between the interview and the scorecard — they record the interview (with candidate consent — check state law, especially California and other two-party-consent states), transcribe it, and either replace or augment the interviewer's notes. Adoption has grown but consent, storage, and data-retention policies need to be aligned with mod-110 (privacy) and the interviewer-training playbook.

## The graduation triggers between products

Migrating ATS products is expensive — measured in weeks of recruiter time, at-risk pipeline data, and lost historical analytics — so the trigger to graduate should be real. Common triggers:

**Workable → Ashby / Greenhouse / Lever.** Trigger: hiring volume has passed ~5–8 concurrent open reqs, the interview panels are ≥4 people, and the corporation needs stronger structured-scorecard workflow, deeper reporting, or a specific integration Workable does not support well. Migration typically fits inside a 4–8-week window at Series-A hiring volume.

**Greenhouse → Ashby.** Trigger: the corporation is heavy on analytics and wants ATS-native reporting rather than a Greenhouse + BI-stack combination; or the corporation is heavy on outbound sourcing and wants a stronger native CRM. Not automatic — Greenhouse is a durable long-term ATS and many growth-stage corporations stay on it through IPO.

**Lever → Ashby / Greenhouse.** Trigger: the CRM-forward workflow that made Lever attractive at seed is no longer the primary constraint; the corporation needs a structured-hiring workflow the panel can trust.

**Ashby / Greenhouse / Lever → HCM-native ATS (Workday Recruiting, SuccessFactors Recruiting).** Trigger: the HRIS has graduated to a full HCM (see [chapter 07](./07-hris-peo-payroll-stack.md)); the CFO / CPO want a single vendor across recruit-to-retire; the enterprise-controls and audit requirements of the HCM apply to recruiting as well. This is a growth-stage / pre-IPO decision and is often *not* the right call — the specialised ATS often outperforms the HCM-native ATS on hiring-team ergonomics for years past the point where the finance / HR org has moved to Workday.

### Migration checklist

A defensible ATS migration produces:

- A locked cut-over date and a communications plan for the recruiting team and hiring managers.
- A full candidate-and-pipeline data export from the source ATS, with a plan for what fields do not map cleanly (rejected candidates from >12 months ago, stalled candidates, notes in free-text fields).
- A req-by-req import plan into the target ATS with scorecards re-created and interview kits re-linked.
- A source-of-hire mapping so historical attribution is not lost.
- An integration re-configuration checklist — HRIS, LinkedIn Recruiter (RSC), background-check vendor, scheduling, assessment tools, e-signature — each re-connected and tested end-to-end with a pilot req.
- A shadow-run period (typically 2–4 weeks) where both systems are updated in parallel before the old system is deprecated.
- Retention of the source-ATS data export in the corporate record so that a diligence request can reconstruct historical hiring activity.

## A worked example — a Series-A SaaS company choosing an ATS

A Series-A company (22 → 55 hires in 18 months, see [chapter 01](./01-sourcing-operating-model-by-stage.md)) is choosing between Ashby and Greenhouse. Both would work.

**The decision framework.**
- **Analytics.** How much does the head of talent care about ATS-native reporting? If deeply — Ashby's advantage in ATS-native analytics is real. If reporting will be done in the corporation's BI stack anyway — Greenhouse's integration ecosystem is deeper.
- **Sourcing intensity.** How much of the pipeline will be sourced (vs. inbound)? Heavy sourcing favours Ashby's native CRM; balanced pipelines make either work.
- **Interview-panel discipline.** How opinionated does the corporation want the structured-hiring workflow to be? Greenhouse historically has the most opinionated structured-hiring workflow; Ashby has closed the gap.
- **Existing tooling relationships.** If the corporation is already on Rippling or Gusto, both products have first-class integrations. If the corporation is on a less-common HRIS, check the integration.
- **Recruiter familiarity.** Recruiters coming from a Greenhouse shop are productive on day one. Recruiters coming from an Ashby shop are similarly productive on day one. Familiarity is a real tiebreaker.

**Recommendation.** The Head of Talent picks the product they will personally operate day-in / day-out, given the corporation's specific hiring plan. Either product will get the corporation from Series-A through Series-B. The wrong decision is choosing neither and staying on the spreadsheet through the first 40 hires.

## Summary

- The ATS is the corporation's hiring system of record and a compliance / diligence artifact from day one. Adopt one at seed even at low volume.
- The seed → Series-B window is dominated by Ashby, Greenhouse, Lever, and Workable. Growth-stage / enterprise moves toward the HCM-native ATS (Workday Recruiting, SuccessFactors Recruiting, iCIMS).
- The ATS must be wired into five integration surfaces: HRIS / PEO, LinkedIn Recruiter (RSC) + LI Talent Insights, interview scheduling, background checks / identity verification, and assessment / interview-intelligence tools.
- Graduation between ATS products is real work — 4–8 weeks at Series-A hiring volume — and should be triggered by a specific operating constraint, not preference. Migrate once, migrate deliberately.
- The ATS decision at seed is less about "which product is best" and more about "which product will we still be on at Series-B?" Migration costs favour the product the head of talent can live with through the next 24 months.
