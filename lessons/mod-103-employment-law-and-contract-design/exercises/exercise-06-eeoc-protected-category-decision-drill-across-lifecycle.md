# Exercise 06 — EEOC protected-category decision drill across the employment lifecycle

> Estimated time: **~4 hours** · Related chapters: [07 — The EEOC protected-category framework across the employment lifecycle](../07-eeoc-protected-category-framework.md), [03 — Offer letters and pay transparency](../03-offer-letter-architecture-and-pay-transparency.md), [08 — State-law variance](../08-state-law-variance.md)

## Problem statement

Acme Robotics is running a Q4 recruiting cycle for seven roles across California, New York City, Illinois, Washington, and Colorado. The CEO has forwarded you (incoming COO / GC) a stack of real, concrete recruiting-and-employment artifacts — a draft job description, an ATS pre-screen configuration, four interview-scorecard rubrics, an offer-rescission email draft the Head of Finance wrote after a background check, a pregnancy-related accommodation request from an incumbent engineer, a RIF selection list from a 20% headcount reduction the board approved last week, and a draft separation agreement. Several of them have problems — some obvious, some subtle, some of them creating individual-plaintiff Title VII exposure, some creating class-action or state-FEPA exposure, some creating NLRB *McLaren Macomb* exposure, some creating ADA / PWFA / state-leave exposure.

Your job is to run each artifact through the chapter 07 lifecycle framework, identify what's wrong, cite the specific statute and (where applicable) case that controls, and produce a corrected version — plus a corporation-wide "manager-and-recruiter decision checklist" that the next person running this cycle can use without re-doing the analysis from scratch.

This exercise is not about catching every possible edge case. It is about internalising the lifecycle framework at each decision point and producing documented, defensible decisions.

## Facts

- **Corporation.** Acme Robotics, Delaware C-corp. HQ San Francisco. Employs in CA, NY (state and NYC), IL, WA, CO, MA, TX.
- **Current headcount.** 60 employees. The 20% RIF below reduces headcount to 48.
- **Compliance tooling.** Standard ATS (unspecified vendor), standard payroll/HRIS, standard background-check vendor (FCRA-compliant per vendor's claim). No current harassment-prevention training program. No written interactive-process protocol for accommodation requests. No written RIF selection protocol. No separation-agreement template (the Head of Finance drafts them case-by-case from a 2019 template of unknown provenance).

## The artifact stack

### Artifact 1 — Draft job description for Senior Software Engineer (San Francisco, remote-OK)

> *"We're a young, scrappy, high-energy team of digital natives looking for a passionate, recent-grad-level Senior Software Engineer to join our mission to [redacted]. You should have 2–5 years of experience, native English fluency, be comfortable working late nights and weekends, and be able to lift up to 25 pounds. We're an EEO employer and consider all applicants regardless of race, gender, or orientation."*

### Artifact 2 — ATS pre-screen configuration for the SWE role

Required fields that candidates must answer to submit:

- Full name, address, phone, email.
- "What is your current compensation (base + total)?"
- "What are your salary expectations?"
- "What is your date of birth?" (The ATS vendor explains this is for I-9 preparation.)
- "Are you authorised to work in the United States?" (Yes / No.)
- "Will you require visa sponsorship now or in the future?" (Yes / No.)
- "Have you ever been convicted of a felony?" (Yes / No.)
- "What is your gender?" (Male / Female / Non-binary / Prefer not to say.)
- "What is your race / ethnicity?" (Dropdown with EEO-1 categories.)
- "Please upload a photo for identification purposes."

### Artifact 3 — Interview scorecards (four interviews for the SWE role)

Each interviewer writes free-form text in a "Notes" field. Sample notes from the last cycle on four candidates:

- *Candidate A* — "Strong technical interview. Mentioned she just got married and plans to start a family soon. Concerned about commitment. Not a culture fit."
- *Candidate B* — "Excellent problem-solving. Mentioned he's 54 and has been doing this for 30 years. Might struggle with our fast pace. Would prefer someone with more energy."
- *Candidate C* — "Good coding skills. His accent made it hard to understand him sometimes. Not sure he'd be able to communicate with customers. Note: he mentioned he's from Pakistan originally."
- *Candidate D* — "Weak behavioural interview. She mentioned she has a child with ADHD and needs flexibility for school pickup. We don't do flexible hours."

### Artifact 4 — Draft offer-rescission email from the Head of Finance

> *"Hi [Candidate],*
>
> *Thank you for your patience during our background-check process. Unfortunately, we've learned that you have a conviction from 2016 that we weren't aware of when we extended the offer. Based on this, we're rescinding the offer effective immediately. Please return any corporation property. We wish you the best in your job search.*
>
> *Best,*
> *[Head of Finance]"*

Facts about the candidate: California resident, offered Senior SWE role in San Francisco. 2016 conviction was for misdemeanor possession of a controlled substance; sentence completed in 2017; no subsequent convictions. The background check surfaced the conviction after the conditional offer. Role has no safety-sensitive duties and does not involve handling customer data of a sensitive nature.

### Artifact 5 — Pregnancy-related accommodation request

Incumbent engineer, Priya, works in the New York City office. 20 weeks pregnant. Doctor's note states: "Patient should not stand for more than 2 hours at a time; should avoid heavy lifting; should be permitted to take short breaks every 90 minutes; should work from home as needed for prenatal appointments and periods of fatigue." Priya's current job function is 90% remote-friendly software engineering, 10% in-office all-hands and whiteboard sessions. The engineering manager has pushed back: "We can't accommodate work-from-home outside of our standard hybrid policy, which is 3 days in-office. Priya should take unpaid leave until she's back to full capacity."

### Artifact 6 — RIF selection list from the 20% headcount reduction

The board approved a 20% RIF (12 employees). The CEO drew up a list of 12 names based on "performance, cultural contribution, and strategic fit." Review the list demographics (the following is the data you have — not what the CEO disclosed):

- 12 selected employees: 8 women, 4 men. Average age 52. 6 of 12 are age 50+. 2 of 12 are on PWFA / state-pregnancy accommodation or recent-return-from-parental-leave. 1 of 12 recently filed an internal complaint about a different manager's conduct. 1 of 12 is on an active ADA accommodation (ergonomic equipment and modified schedule).
- The remaining 48 employees who are not selected: skew male (60%), skew younger (average age 34), low rate of recent protected-leave usage.
- The RIF selection criteria are documented as: "performance review score (2024), cultural contribution (CEO's assessment), and strategic fit (CEO's assessment)."

### Artifact 7 — Draft separation agreement (RIF)

Standard template includes:

- Severance of 4 weeks' base salary.
- Release of all claims, including specifically "any claim under Title VII, the ADEA, the ADA, state fair-employment statutes, the Equal Pay Act, the Fair Labor Standards Act, or any other federal, state, or local law."
- Confidentiality clause: "Employee shall not disclose the existence or terms of this Agreement, nor any information about the terms of employee's separation, to any third party including coworkers, except employee's spouse and legal/financial advisors."
- Non-disparagement clause: "Employee shall not make any disparaging statement about the Corporation, its officers, employees, products, or services, in any medium."
- "In consideration for the above, employee has 7 days to sign and return this Agreement."
- "This Agreement is governed by Delaware law."

## Requirements

### Part A — Artifact-by-artifact teardown

For each of the seven artifacts, produce a structured review that includes:

1. **The problems**, enumerated. Each problem labelled with the lifecycle stage (chapter 07 § "the lifecycle") and the specific protected-category or statutory exposure (Title VII, ADA/PWFA, ADEA, PDA, EPA/state pay-equity, GINA, § 1981, NLRA, state FEPA, Fair Chance, salary-history ban, pay-transparency, FCRA).
2. **The controlling authority** for each problem — statute, regulation, case. Chapter 07 and chapter 08 are the primary references; cite the primary source, not the chapter.
3. **The corrected version** — a rewrite of the artifact (job description, pre-screen, scorecard rubric, offer-rescission email, accommodation response, RIF selection protocol, separation agreement) that eliminates the problems.

Be specific and ruthless. Where a problem creates a federal claim, state the claim. Where a problem creates a state-FEPA claim that would survive summary judgment because the state statute is broader than Title VII (e.g., FEHA, NYCHRL), state so.

### Part B — Priya's accommodation decision

Produce the interactive-process memo for Priya's accommodation request. The memo should:

1. Identify the applicable statutes — PWFA (Pub. L. No. 117-328), ADA (if any aspect of the pregnancy or related condition rises to a disability under the ADAAA-amended definition), NY State and NYC Human Rights Law pregnancy-accommodation provisions.
2. Address the "undue hardship" standard post-*Groff v. DeJoy*, 600 U.S. 447 (2023) (for the religious-accommodation standard, by analogy) and the PWFA's statutory undue-hardship framework.
3. Analyse the specific accommodations requested (no standing > 2 hours, no heavy lifting, breaks every 90 minutes, work-from-home as needed) against the essential functions of a software engineer (which chapter 07 § "the lifecycle — hiring and offer" and the ADA framework require the corporation to analyse before refusing an accommodation).
4. Reject the manager's "unpaid leave until back to full capacity" response and identify the specific violations of the PWFA, NY State Human Rights Law, and NYC Human Rights Law such a response would create.
5. Produce a draft written response to Priya accepting the accommodation (with specific terms — e.g., WFH as needed, breaks every 90 minutes, no in-office requirement during pregnancy, modified seating equipment if desired), the HR process going forward (job-protected leave entitlements under NY PFL at RCW 49.60, FMLA if applicable, and NYC paid safe-and-sick time; the interactive process remains open to additional accommodations as the pregnancy progresses), and the manager coaching that needs to happen.
6. Address the retaliation risk — the manager's refusal, if communicated to Priya, could independently support a retaliation claim; the response memo should address how the corporation internally resolves the manager's conduct.

### Part C — RIF adverse-impact analysis and selection-criteria rewrite

For the RIF, produce:

1. **An adverse-impact analysis** on the CEO's selection list, under the four-fifths rule and the standard EEOC guidance. Produce the selection rate for each protected class (sex, age 40+, protected-leave status, prior-complaint status, active-accommodation status). Where any protected class is selected at a rate materially different from its base rate, call out the exposure.
2. **A rejection of the CEO's criteria.** "Cultural contribution (CEO's assessment)" and "strategic fit (CEO's assessment)" are the textbook subjective-criteria disparate-impact failure mode (chapter 07 § "performance, promotion, and merit"). State the problem.
3. **A rewrite of the selection criteria** — a job-related, consistently-applied, documented RIF selection protocol. Chapter 07 and *mod-107 — Performance, Promotion & Offboarding* provide the framework. Options: position elimination (specific positions are being eliminated regardless of incumbent), ranked-by-performance-review-score within a defined cohort, seniority within a cohort, or a scored matrix combining role-criticality + performance + skill-match-to-future-roles. Pick one, document the rationale.
4. **A pre-decision legal review process** for the revised selection list — the chapter 07 "termination review" checklist adapted for a RIF — including the specific adverse-impact review, the specific review of any selected employee who is on protected leave, has recently filed a complaint, or has an active accommodation (which the four selected employees above collectively trigger).
5. **The OWBPA group-release analysis.** Twelve selected employees; the ADEA group-release formalities under 29 U.S.C. § 626(f)(1)(F)–(H) apply. The 45-day consideration period (not 7-day), the specific disclosure of the "decisional unit" (which group of employees was considered for selection), the ages and job titles of the selected and non-selected within the decisional unit, the 7-day revocation period, the right-to-consult-counsel advisement. Also address EEOC regulations at 29 C.F.R. Part 1625 governing the content and form of the OWBPA disclosure.
6. **WARN / mini-WARN analysis.** 12 selected employees at a 60-person corporation across multiple states. Is federal WARN triggered? Any state mini-WARN (California, New York, Illinois have the most-expansive)? For each state the corporation employs anyone in, apply the threshold analysis.

### Part D — Separation-agreement rewrite

Rewrite the separation-agreement template to comply with:

1. **OWBPA formalities** for the age-40+ selected employees — 45-day consideration period, specific disclosure of the decisional unit's ages and titles, 7-day revocation, consult-counsel advisement, specific reference to ADEA rights.
2. **The *McLaren Macomb* carve-outs** — the confidentiality and non-disparagement clauses must carve out (i) communication with coworkers about wages, working conditions, and the separation; (ii) filing charges with the EEOC, NLRB, SEC, or any state or federal agency; (iii) participating in a government investigation; (iv) exercising DTSA whistleblower immunity under 18 U.S.C. § 1833(b); (v) engaging in NLRA § 7 protected concerted activity. Draft the carve-outs explicitly.
3. **The Speak Out Act (Pub. L. No. 117-224, 2022)** — no pre-dispute confidentiality or non-disparagement clause may cover sexual-assault or sexual-harassment disputes.
4. **State-specific requirements** — for California employees, specific CCPA-related provisions on data return and the Cal. Lab. Code § 925 limit on forum-selection against California employees. For New York employees, the Section 5-336 ban on confidentiality clauses covering discrimination claims unless the employee specifically consents (and with a 21-day consideration and 7-day revocation period for that consent). For other states as applicable.
5. **The release scope.** The release can cover known-and-unknown-claims-up-to-the-signing-date in most states (with California adding Cal. Civ. Code § 1542 waiver language). Carve out any post-signing claims; address the FLSA / state wage-and-hour backward-looking release issue (DOL supervision is required for FLSA releases outside limited circumstances per *Lynn's Food Stores v. United States*, 679 F.2d 1350 (11th Cir. 1982), and some circuits).
6. **Consideration.** Four weeks of severance is thin; chapter 07 does not prescribe a specific severance amount, but the OWBPA requires "consideration in addition to anything of value to which [the employee] already is entitled." Document the design.

### Part E — Manager-and-recruiter decision checklist

Produce a one- or two-page checklist for the corporation's managers, recruiters, and interviewers that the Head of People can distribute as the standing reference. The checklist should cover (chapter 07 §§):

- **Job-posting review** — essential-functions-vs-proxy test, EEO statement with jurisdiction-specific protected-category list, salary-transparency range disclosure (chapter 03 cross-reference).
- **ATS and application-form configuration** — prohibited questions, voluntary EEO self-identification stored separately, salary-history-ban compliance per jurisdiction (chapter 03 cross-reference), ban-the-box compliance per jurisdiction (chapter 08 cross-reference).
- **Interview script and scorecard** — permitted and impermissible questions, structured scorecard mapped to essential functions, prohibition on "culture fit" / "executive presence" / "fit with the team" subjective fields.
- **Offer and background-check compliance** — FCRA pre-adverse-action notice, individualised-assessment write-up where Fair Chance Act applies, post-adverse-action notice.
- **Accommodation-request handling** — the interactive-process framework, the essential-functions analysis, the undue-hardship standard, the documentation obligation, the manager's role vs. HR's role.
- **Discipline / PIP / termination** — the chapter 07 "termination review" checklist, the retaliation review, the consistency-with-similarly-situated-employees review.
- **State-and-city escalation** — the state-law variance axes (chapter 08) and the escalation protocol when a role, offer, or termination crosses jurisdictions.

### Part F — Design-choices memo

A 2–3 page memo covering:

- The three decisions you found hardest and how you resolved them (likely candidates: the RIF selection-criteria rewrite, Priya's accommodation vs. the manager's hybrid-policy claim, the offer-rescission for the misdemeanor conviction).
- The highest-common-denominator vs. per-state operating-policy decision (chapter 08) applied to the lifecycle artifacts — e.g., is the ATS configured to the strictest state's Fair Chance rules nationally, or configured per-state?
- The manager-and-recruiter training program the checklist implies — frequency, trigger (new-manager onboarding, annual refresher, incident-driven), content, documentation.
- The AI-driven hiring tool question (NYC Local Law 144, Colorado SB 24-205) — whether the corporation uses any automated employment-decision tool anywhere in the ATS, and the compliance posture if so. Flag as `<!-- needs-research -->` if the ATS vendor's automated-decision-making profile is not known.
- Any `<!-- needs-research -->` items you flagged (current status of the Pregnant Workers Fairness Act regulations at 29 C.F.R. Part 1636, current status of the EEOC's harassment guidance, current status of state and NYC AEDT regulations, current status of the Washington My Health My Data Act for any HR / health-data touch).

## Starter guidance

- Chapter 07 is the primary reference, with chapter 08 providing the state-specific overlays. Chapter 03 provides the pay-transparency and Fair Chance interactions.
- When a question could be innocent in a vacuum but creates proxy evidence of a protected-category decision, treat it as impermissible. "When did you graduate college?" (age-proxy), "Where are you from originally?" (national-origin-proxy), "Do you plan to have children?" (sex/pregnancy-proxy) are all impermissible regardless of intent.
- The "culture fit" scorecard field is the most-cited disparate-impact failure mode in startup discrimination litigation. Rewrite the rubric to replace subjective fields with structured, job-related criteria.
- The offer-rescission email for the misdemeanor conviction is categorically defective under the California Fair Chance Act, Cal. Gov. Code § 12952 — the individualised-assessment, pre-adverse-action, and post-adverse-action procedural steps are all missing. The corrected process requires the full Fair Chance workflow, and may well end in reinstatement of the offer.
- Priya's accommodation request is the easier of the lifecycle calls — the PWFA, the ADA (to the extent any aspect qualifies as a disability), and the NY State / NYC Human Rights Laws clearly require the accommodation given the available-essential-function overlap. The manager's response is wrong on substance, procedure, and retaliation risk.
- The RIF selection-criteria "cultural contribution + strategic fit as the CEO assesses them" is a disparate-impact and disparate-treatment problem. Rewriting it is table-stakes. The adverse-impact analysis is the second step; even with revised criteria, the current selection list likely does not survive the four-fifths analysis.
- The separation-agreement template is defective on *McLaren Macomb*, Speak Out Act, OWBPA, Section 5-336, and consideration grounds. Rewrite it fully.
- Do NOT draft case-specific arguments for or against individual plaintiffs — the exercise is about compliance posture, not litigation strategy.
- Where a specific state-law citation is required and you cannot verify the current version (NY State salary-threshold figures, Washington salary-basis multiplier, Colorado Equal Pay Act posting elements), flag with `<!-- needs-research -->`.

## Deliverables

- `artifact-teardown-and-rewrites.md` — Part A, with each artifact clearly separated and both the teardown and the corrected version included.
- `priya-accommodation-memo.md` — Part B.
- `rif-adverse-impact-and-selection-rewrite.md` — Part C.
- `separation-agreement-template.md` — Part D (the corrected template).
- `manager-and-recruiter-decision-checklist.md` — Part E.
- `lifecycle-design-choices-memo.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. The job description's problems (age-proxies "young," "scrappy," "recent-grad-level," "digital natives"; disability-proxy "native English fluency" and "lift 25 lbs" where not job-related; religious-and-family-proxy "late nights and weekends") are identified with citations to Title VII, ADEA, ADA, and the EEOC's guidance on job-postings. The corrected version removes the proxies and lists the full jurisdiction-specific EEO statement.
2. The ATS pre-screen's problems (salary-history questions in CA, NY, IL, CO, WA ban jurisdictions; DOB; photo-upload; mandatory gender / race / ethnicity when voluntary EEO self-identification must be stored separately; "convicted of a felony" in ban-the-box jurisdictions) are identified with citations. The corrected configuration eliminates the prohibited fields.
3. The interview-scorecard notes' problems (pregnancy / family-plan commentary on Candidate A; age commentary on Candidate B; national-origin / accent commentary on Candidate C; disability / caregiver commentary on Candidate D) are identified with citations to Title VII, PDA, ADEA, § 1981, ADA, and state FEPA. The scorecard rubric is rewritten to be structured, job-related, and free of subjective "culture fit" fields.
4. The offer-rescission email is identified as a categorical Fair Chance Act violation (missing individualised assessment, missing pre-adverse-action notice, missing opportunity to respond, missing post-adverse-action notice, missing analysis of nature of offense / time elapsed / job-relatedness). The corrected process includes the full Fair Chance workflow per Cal. Gov. Code § 12952, and the likely outcome (reinstatement of the offer) is acknowledged.
5. Priya's accommodation is granted with specific terms. The manager's "unpaid leave until back to full capacity" response is identified as a PWFA / NY State / NYC Human Rights Law violation. Retaliation risk is addressed.
6. The RIF adverse-impact analysis correctly identifies the sex (women 67%), age (50%+ are 50+), and protected-leave/complaint/accommodation exposure in the CEO's selection list. The selection criteria are rewritten to be job-related, objective, and documented. The OWBPA 45-day group-release formality is addressed. WARN / state mini-WARN thresholds are analysed for each state.
7. The separation agreement is rewritten with OWBPA compliance, *McLaren Macomb* carve-outs, Speak Out Act compliance, Section 5-336 compliance (for New York employees), Cal. Civ. Code § 1542 waiver (for California employees), and documented consideration.
8. The manager-and-recruiter decision checklist is a usable, one-to-two-page reference that covers each lifecycle stage.
9. Statutory and case citations (Title VII at 42 U.S.C. § 2000e; ADEA at 29 U.S.C. § 621 and OWBPA at § 626(f); ADA at 42 U.S.C. § 12101 and § 12112(d); PDA at § 2000e(k); PWFA at Pub. L. No. 117-328; GINA at 42 U.S.C. § 2000ff; § 1981 at 42 U.S.C. § 1981; FCRA at 15 U.S.C. § 1681b(b)(3); Cal. Gov. Code § 12952; Cal. Civ. Code § 1542; Cal. Lab. Code § 925; NYCHRL at NYC Admin. Code § 8-107; NY Exec. Law § 296; NY Gen. Oblig. Law § 5-336; Illinois Human Rights Act at 775 ILCS 5; WA Law Against Discrimination at RCW 49.60; Colorado Anti-Discrimination Act at C.R.S. § 24-34-401; *Bostock v. Clayton County*, 590 U.S. 644 (2020); *Groff v. DeJoy*, 600 U.S. 447 (2023); *McLaren Macomb*, 372 NLRB No. 58 (Feb. 21, 2023); 29 C.F.R. Part 1625; 16 C.F.R. Part 910 N/A — do not cite the FTC non-compete rule in this exercise) are correct.
10. Nothing left as `[FILL IN]` or `[TBD]` — every field populated or explicitly flagged with a `<!-- needs-research -->` marker.
