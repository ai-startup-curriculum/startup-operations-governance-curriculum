# 4. Reference checks and pre-employment background checks

> Reference calls confirm what you already believe. Background checks confirm what the candidate said. Get either wrong and the corporation either hires the wrong person or lands in an FCRA class action.

## Motivation

Between "we want to make an offer" and "we make the offer" the corporation should do two distinct things that are often conflated:

- **Reference checks** — the corporation talks to people who have worked with the candidate to confirm the picture built during the interview loop. Reference checks are *not* a legal-compliance surface; they are a hiring-quality tool.
- **Pre-employment background checks** — the corporation runs a formal background check (typically criminal-history, employment-history, education-verification, and — for certain roles — motor vehicle, credit, or professional-license checks) through a Consumer Reporting Agency (CRA) that operates under the Fair Credit Reporting Act (FCRA, 15 U.S.C. § 1681 et seq.). Background checks *are* a legal-compliance surface, with a specific FCRA-prescribed process the corporation must follow.

Both matter, and both have well-documented failure patterns:

- The "back-channel" reference (the founder calls their friend at the candidate's prior employer and asks "should we hire this person?") is fast but a compliance minefield — no consent, unstructured, prone to protected-category infection, and easily challenged in an EEOC or Title VII proceeding.
- The FCRA-non-compliant background check (bundled-disclosure form; unauthorised report pull; no pre-adverse-action letter; no waiting period; no adverse-action letter) is the *single most common wage-and-hour-style class-action trigger in HR compliance*. FCRA class actions targeting employers who buried the disclosure inside the offer packet, or skipped the pre-adverse-action process, have produced eight-figure settlements. <!-- needs-research: cite examples of high-profile FCRA-background-check class actions against employers (e.g., cases against major retailers and rideshare / logistics companies) to ground the exposure claim; do not fabricate case names or settlement amounts. -->
- The ban-the-box / fair-chance failure — asking about criminal history on the initial application in a jurisdiction that prohibits it, or making an adverse decision based on a criminal record without conducting the required individualised assessment — is an escalating state and city compliance surface.

This chapter builds the reference-check playbook, the FCRA-compliant background-check process, the ban-the-box / fair-chance overlay, and the international variance the corporation must factor if it hires abroad.

## Reference checks

### When to do them

Reference checks happen *after* the on-site loop and the debrief have produced a "we would extend" position, but *before* the offer is extended (or contingent on it). This ordering matters — reference checks are hiring-quality tools, not tie-breakers between candidates, and the corporation should not extend an offer without them.

### Who provides references

The candidate provides names — typically 2–4 references, weighted toward former managers and cross-functional peers. The corporation may also request "back-channel" references (people the corporation knows who worked with the candidate but were not named by the candidate); these have distinct sensitivity, discussed below.

### The reference-check playbook

A defensible reference call follows a structured template — often the same STAR / behavioural-question technique the corporation uses in the interview loop:

1. **Introduction and consent.** "Hi, I'm [name] from [corporation]. [Candidate] listed you as a reference — do you have 20 minutes to talk about working with them?" If the reference declines, do not pressure them.
2. **Relationship context.** How did you work with the candidate? For how long? In what capacity?
3. **Competency evidence.** For each of the top 3–4 competencies from the scorecard (see [chapter 03](./03-structured-interviewing.md)), ask a specific behavioural question: "Can you describe a time when [candidate] had to [competency-relevant scenario] — what did they do, what was the outcome?" This mirrors the interview loop's structured questioning and produces evidence, not opinions.
4. **Development areas.** "In what areas did [candidate] have the most growth over your time together?" and "In what areas did they still have room to grow?" Every honest reference has an answer here; the reference who says "no development areas, they were perfect" is either uninformed or unreliable.
5. **Rehire question.** "If you were in a position to hire [candidate] into a role at your current company, would you?" The rehire question is a single high-signal item that reveals what unstructured questions miss.
6. **Anything else.** "Is there anything I should have asked about that I didn't?" Frequently produces the most useful information in the entire call.

**What not to ask.** Anything protected under Title VII, the ADA, the ADEA, the PDA, or state-and-city equivalents. Questions about the candidate's family status, religion, national origin, health, or disability are prohibited even in a reference call. See [mod-103 chapter 07](../mod-103-employment-law-and-contract-design/07-eeoc-protected-category-framework.md).

### Back-channel references

The founder or hiring manager sometimes has a direct line to somebody who worked with the candidate but was not named by the candidate as a reference. There are two schools of thought:

- **Do them.** Back-channel references catch signals the candidate-selected references do not — the candidate does not name people who would give a bad reference. In competitive senior hiring, back-channels are common.
- **Do not do them, or do them cautiously.** Back-channels are done without candidate consent, they can breach the candidate's confidentiality about their job search, and they can introduce protected-category inference into the hiring decision.

The middle ground most corporations settle on: allow back-channels only for senior / exec hires (director+), only when the person contacted has an existing professional relationship with the reference-taker, and only with a documented adherence to the same structured-question rubric as an on-panel reference. Back-channel references from "friend of a friend" contacts should be off-limits.

### Reference-check writeup

Every reference call produces a short writeup stored in the ATS against the candidate record — the reference's name and relationship, the structured-question answers, and the rehire question response. The debrief and offer decision reference this writeup on the record.

## Pre-employment background checks — the FCRA framework

The Fair Credit Reporting Act, 15 U.S.C. § 1681 et seq., governs the use of consumer reports (including background-check reports) for employment purposes. The employer's obligations are precise and prescriptive.

### The four steps of an FCRA-compliant background check

**Step 1 — Disclosure and authorisation.**

Before ordering the background check, the corporation must provide the candidate with a **clear and conspicuous written disclosure that a consumer report may be obtained for employment purposes** (15 U.S.C. § 1681b(b)(2)(A)(i)) *in a document that consists solely of the disclosure* (the "standalone-disclosure requirement"). The candidate must then provide **written authorisation** for the corporation to procure the report (15 U.S.C. § 1681b(b)(2)(A)(ii)).

The standalone-disclosure requirement is the trapdoor. The corporation may not:

- Bury the disclosure inside a longer employment application.
- Add a liability-release / waiver-of-claims clause to the disclosure document.
- Add "extraneous" text — for example, state-law notices — to the *disclosure document itself*, though a separate state-law notice document is permitted.

Court decisions have repeatedly held that even *seemingly minor* additions to the disclosure document (a small liability release, a brand logo, an "acknowledgment" clause) can render the disclosure non-compliant, exposing the corporation to statutory damages of $100–$1,000 per willful violation (plus actual damages and attorneys' fees). <!-- needs-research: cite the leading FCRA standalone-disclosure cases (e.g., Syed v. M-I, LLC, 9th Cir. 2017, and subsequent cases) and the current FTC / CFPB guidance on FCRA disclosures. -->

The authorisation can be on the same document as the disclosure (this is expressly permitted by 15 U.S.C. § 1681b(b)(2)(A)(ii)) — but nothing else can.

**Step 2 — Ordering the report.**

The corporation orders the report from a Consumer Reporting Agency (Checkr, Sterling, HireRight, Accurate, GoodHire, and others). The CRA typically requires the corporation to complete a one-time certification under 15 U.S.C. § 1681b(b)(1) that (a) the corporation has provided the required disclosure, (b) the candidate has authorised, and (c) the corporation will follow the adverse-action process if it makes a decision adverse to the candidate based on the report.

The corporation does not decide *what to order* on autopilot — the scope of the background check must be job-related. A criminal-history-and-employment-history check is standard; a credit-history check is appropriate only for roles with financial or fiduciary responsibilities (and is prohibited or restricted in a growing set of jurisdictions — California, New York City, and others); a motor-vehicle-records check is appropriate for driving roles; a professional-license verification is appropriate for licensed roles.

**Step 3 — Pre-adverse-action process.**

If the report contains information that would cause the corporation to take an adverse action (rescind an offer, decline to hire), the corporation must, *before* taking the adverse action:

1. Provide the candidate with a copy of the consumer report (the actual report, not a summary), and
2. Provide the candidate with a copy of "A Summary of Your Rights Under the Fair Credit Reporting Act" (the FTC's model summary, updated periodically — check for the current version at consumerfinance.gov). <!-- needs-research: confirm the current version and correct citation for the CFPB's Summary of Rights document, and confirm CFPB (not FTC) is the current publishing authority. -->

The corporation must then **wait a reasonable period** — the FCRA does not fix a specific waiting period, but the FTC has historically guided that 5 business days is a common defensible baseline (some jurisdictions and some courts have implied longer, particularly under state analogues). <!-- needs-research: confirm the current FTC / CFPB guidance and case-law consensus on the pre-adverse-action waiting period; 5 business days is commonly cited but the specific number is not statutory. --> The wait period exists to allow the candidate to dispute inaccuracies in the report with the CRA before the corporation acts on the report.

**Step 4 — Adverse-action notice.**

If, after the waiting period, the corporation still intends to take the adverse action, it sends the candidate an **adverse-action notice** (15 U.S.C. § 1681m(a)) that includes:

1. Notice of the adverse action.
2. The name, address, and telephone number of the CRA that furnished the report.
3. A statement that the CRA did not make the decision and cannot explain the specific reasons for it.
4. Notice of the candidate's right to obtain a free copy of the report within 60 days.
5. Notice of the candidate's right to dispute the accuracy or completeness of the information.

The adverse-action process is process, not judgment. It applies whether the adverse decision is based on a criminal-history finding, an employment-verification discrepancy, a credit report, or any other item in the report.

### State-analogue FCRAs

Several states have their own analogues to the federal FCRA that add requirements on top of the federal baseline:

- **California** — the Investigative Consumer Reporting Agencies Act (ICRAA, Cal. Civ. Code § 1786) and the Consumer Credit Reporting Agencies Act (CCRAA, Cal. Civ. Code § 1785) impose additional disclosure requirements, including a right for the candidate to receive a copy of the report and, in many cases, a check-the-box on the disclosure requesting a copy.
- **New York** — Article 25 of the NY General Business Law imposes additional disclosure and adverse-action requirements.
- **Massachusetts, Minnesota, New Jersey, and others** — each impose additional variations.

<!-- needs-research: confirm the current text and applicability of each state analogue; the state landscape here shifts and any operating policy must be checked against a recent survey. -->

The operating implication: the corporation's background-check disclosure and adverse-action templates must be state-specific where the corporation hires, or the corporation must run the highest-common-denominator version of the templates that satisfies every applicable state (see the [mod-103 chapter 08 highest-common-denominator vs. per-state discussion](../mod-103-employment-law-and-contract-design/08-state-law-variance.md)).

## Ban-the-box and fair-chance-act constraints

"Ban the box" is a broad label for laws that prohibit or delay the employer's inquiry into a candidate's criminal history. The specifics vary sharply by jurisdiction:

- **California** — the California Fair Chance Act (Cal. Gov. Code § 12952) prohibits inquiry into criminal history until a conditional offer of employment has been extended, requires an individualised assessment before making an adverse decision based on criminal history, and requires specific written notices. Local ordinances (San Francisco, Los Angeles) impose additional requirements. <!-- needs-research: confirm current CFCA regulatory text and any 2023–2026 amendments. -->
- **New York City** — the Fair Chance Act (NYC Admin. Code § 8-107(11)) prohibits inquiry into criminal history until a conditional offer, requires an individualised assessment (the "NYC Fair Chance Act Notice"), and requires a specific waiting period before the offer can be withdrawn. New York State also has its own Fair Chance Act analog.
- **Illinois** — the Job Opportunities for Qualified Applicants Act ("Illinois Ban-the-Box Act," 820 ILCS 75) prohibits inquiry into criminal history until an interview has been conducted or a conditional offer has been extended.
- **Washington** — RCW 49.94 (Washington Fair Chance Act) prohibits inquiry until the corporation has initially determined that the candidate is otherwise qualified.
- **Federal contractors and federal agencies** — the federal Fair Chance to Compete for Jobs Act (2019) restricts federal executive-branch hiring and federal-contractor hiring for federal positions from inquiring about criminal history until a conditional offer is extended. State-and-local ban-the-box laws are separate from and often broader than the federal law.

Beyond timing, most fair-chance-act statutes require an **individualised assessment** before the corporation can rescind a conditional offer based on a criminal-history hit. The individualised assessment considers, at minimum:

1. The nature and gravity of the offence.
2. The time elapsed since the offence.
3. The nature of the job.

The EEOC's April 2012 Enforcement Guidance on the Consideration of Arrest and Conviction Records in Employment Decisions Under Title VII lays out the federal framework the state statutes generally track. <!-- needs-research: confirm that the 2012 EEOC guidance is still the current governing federal guidance and note any updates. -->

The individualised-assessment step, done in writing and stored against the candidate record, is the anchor of a defensible fair-chance decision.

## Employment verification and education verification

Beyond criminal history, the background check typically also verifies:

- **Employment history** — that the candidate held the positions and dates they represented. CRAs contact former employers directly or use payroll-database services (e.g., The Work Number by Equifax).
- **Education history** — that the candidate holds the degrees they represented. CRAs contact the institution's registrar or use the National Student Clearinghouse.
- **Professional licenses** — for licensed roles, verifying the license is active and unrestricted.

Discrepancies (candidate said "Director" but the previous employer confirms "Senior Manager"; candidate said "M.S. Computer Science 2018" but the university confirms "B.S. Computer Science 2018 only") are typical. The corporation's response is a judgment call — a minor title discrepancy is often benign; a fabricated degree is usually disqualifying. Whatever the response, it should be consistent across similarly situated candidates and documented against the candidate record.

## International background-check variances

The moment the corporation hires outside the US, the FCRA framework does not apply and per-country data-protection and background-check regimes take over. A few high-level patterns:

- **European Union / United Kingdom** — the GDPR (in the EU) and the UK GDPR + Data Protection Act 2018 (in the UK) impose strict lawful-basis, purpose-limitation, and minimisation requirements on background-check processing. Criminal-history data ("special-category data" under GDPR Article 10) is heavily restricted — the DBS (Disclosure and Barring Service) in the UK, and equivalent authorities in each EU member state, are the only lawful sources for criminal-history checks in most cases.
- **Canada** — federal and provincial privacy legislation (PIPEDA federally; PIPA in BC / Alberta; the Quebec Act Respecting the Protection of Personal Information in the Private Sector) govern background-check collection. Criminal-history checks typically require candidate consent and access is generally routed through the RCMP.
- **Australia** — the Privacy Act 1988 and the Australian Privacy Principles apply. National Police Checks are conducted through the Australian Criminal Intelligence Commission or accredited providers.
- **India, Singapore, and much of Asia** — the market is served by CRAs that partner with local authorities; each country has its own consent, scope, and permissible-use requirements. Consent forms are typically per-country.
- **Deeper coverage** — international background-check operating policy is a mod-113 topic; this chapter's role is to flag that "we'll just use the US template" is not viable.

<!-- needs-research: confirm the current DBS scope (Basic / Standard / Enhanced) and eligibility rules for UK employment background checks; confirm the PIPEDA + provincial-analogue landscape for Canadian pre-employment background checks. -->

## The ATS integration and the operating implementation

The FCRA process is the reason ATS integrations with background-check CRAs matter so much (see [chapter 02](./02-ats-selection-and-integration.md)). Well-integrated flows:

- Send the FCRA disclosure + authorisation to the candidate through the ATS at the correct pipeline stage (typically post-verbal-offer, contingent).
- Store the signed disclosure and authorisation against the candidate record.
- Order the report via API.
- Store the report against the candidate record.
- Kick off a pre-adverse-action workflow if the report has a flagged item, with a templated pre-adverse-action letter that satisfies the standalone-summary-of-rights requirement and starts the waiting-period clock.
- Kick off an adverse-action workflow if the corporation confirms the adverse decision, with the required notice content.

A background-check process that is not wired into the ATS is a process where the pre-adverse-action wait period is likely to be violated, the summary-of-rights document is likely to be forgotten, and the adverse-action notice is likely to be sent by an ad-hoc email that does not satisfy 15 U.S.C. § 1681m. This is where FCRA class actions are made.

## A worked example — a Series-A background-check policy

The corporation is at Series-A, hiring in California, Colorado, New York City, and Washington. It uses Ashby as the ATS and is deciding between Checkr and Sterling for the CRA integration.

**Operating policy.**

- **Scope.** Standard package: 7-year criminal-history check (subject to state limits — California's 7-year limit under the ICRAA, for example), employment verification (past 7 years), education verification (highest degree only), SSN trace and address history. Credit check is *excluded* except for roles with financial / fiduciary duties (CFO, controller, treasurer) — and where used, is subject to state credit-check-restriction laws. Motor-vehicle-records check is *excluded* except for driving roles.
- **Timing.** Ordered *after conditional offer acceptance*. Complies with the California, NYC, Washington, and Illinois fair-chance-act timing requirements.
- **Disclosure and authorisation.** Standalone disclosure sent from the ATS through the CRA-native workflow. State-specific supplementary notices sent as separate documents. The disclosure document contains no liability release, no logo, no extraneous text beyond the required statement.
- **Adverse-action process.** Pre-adverse-action letter with the actual report attached and the current CFPB Summary of Rights document. 5-business-day waiting period before the final adverse-action decision. Adverse-action letter with all 15 U.S.C. § 1681m(a) elements.
- **Individualised assessment.** For any criminal-history hit, an individualised assessment is completed in writing before the pre-adverse-action letter is sent. The assessment references the EEOC 2012 guidance three-factor framework (nature-and-gravity, time-elapsed, job-relatedness) plus any state-specific additional factors (California CFCA, NYC Fair Chance Act). Signed by the head of people, filed against the candidate record.
- **State-analogue notices.** ICRAA notices for California candidates (with the required check-box for the candidate to request a copy of the report). NYC Fair Chance Act Notice for NYC candidates. Washington-specific Fair Chance Act disclosures. All state notices maintained in a versioned template folder, reviewed annually.

The corporation runs this policy through Ashby's Checkr integration — end to end, from ATS to CRA to disclosure to report to adverse-action workflow — and never sends a background-check-related email that is not driven by the templated workflow.

## Summary

- Reference checks and background checks are different tools. References are hiring-quality; background checks are legal-compliance. Do both.
- The reference-check playbook is a *structured* call — the same STAR / competency-anchored questions the interview loop uses. The rehire question is high-signal. Written up in the ATS against the candidate.
- The FCRA-compliant background check is a four-step process: (1) standalone disclosure and authorisation, (2) ordering the report, (3) pre-adverse-action process (report + Summary of Rights + waiting period), (4) adverse-action notice with the 15 U.S.C. § 1681m(a) elements.
- The **standalone-disclosure requirement** (nothing but the disclosure and the authorisation on the disclosure form) is the single most litigated FCRA hiring compliance point. No liability releases; no logo; no state-law notices on the disclosure form itself.
- State-analogue FCRAs (California ICRAA/CCRAA, NY, Massachusetts, and others) impose additional requirements. Templates must be state-aware.
- Ban-the-box / fair-chance-act laws (California CFCA, NYC Fair Chance Act, Illinois Job Opportunities for Qualified Applicants Act, Washington RCW 49.94, federal contractor rules) restrict *when* the corporation may inquire about criminal history and require an **individualised assessment** before an adverse decision based on criminal history.
- International background checks operate under GDPR (EU/UK), PIPEDA (Canada), and per-country data-protection and criminal-record-access regimes. The US template does not port.
- Everything above lives in the ATS-CRA integration workflow. A background-check process that is not templated in the ATS is a process where FCRA class actions are made.
