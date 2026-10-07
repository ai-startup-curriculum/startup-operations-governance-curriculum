# Exercise 07 — State-law variance across California, New York, Illinois, Washington, Colorado

> Estimated time: **~5 hours** · Related chapters: [08 — State-law variance across California, New York, Illinois, Washington, Colorado](../08-state-law-variance.md), with cross-references to [01](../01-w2-vs-1099-worker-classification.md), [02](../02-flsa-exempt-vs-non-exempt.md), [03](../03-offer-letter-architecture-and-pay-transparency.md), [06](../06-non-compete-landscape-and-alternatives.md), [07](../07-eeoc-protected-category-framework.md), and [09](../09-arbitration-and-class-action-waivers.md)

## Problem statement

Acme Robotics has grown from a single-state (California) workforce to a five-state footprint. Headcount is now 60 across California, New York (state and NYC), Illinois, Washington, and Colorado. The existing employee handbook, offer-letter template, PIIA, arbitration agreement, pay-transparency job-posting template, background-check process, biometric time-and-attendance system, and payroll / benefits program were all built California-first. The CEO has asked you (incoming COO / GC) to produce the corporation's **state-law compliance program** — the matrix of what applies where, the operating-policy decision (highest-common-denominator vs. per-state), the specific state-rider documents that need to be authored, and the maintenance discipline.

The deliverable is not a theoretical compliance map. It is the actual working document the Head of People, the Head of Finance, and outside employment counsel use to run the business — the kind of artifact the Series-A diligence counsel will read line-by-line.

## Facts

- **Corporation.** Acme Robotics, Delaware C-corp. HQ San Francisco. Employs in CA (28), NY state (6 upstate NY + 4 NYC), IL (4, all Chicago), WA (6, 4 Seattle + 2 remote), CO (5, 3 Denver + 2 Boulder). The 2 Texas employees and 5 Massachusetts employees from the exercise 05 scenario are deferred — this exercise covers the five chapter 08 jurisdictions only.
- **Current state footprint.** The corporation is registered as a foreign qualified employer in each of the five states. State unemployment-insurance accounts are open. Workers'-compensation coverage is state-specific. Payroll processes through a single HRIS vendor that supports per-state tax and leave-benefit calculations.
- **Specific operational facts that have state-law implications.**
  - The corporation uses a biometric fingerprint-based time-and-attendance system for its Chicago office (deployed when the corporation acquired a legacy ops vendor). The Chicago office has 4 employees.
  - The corporation reimburses WFH expenses only for California employees ($100/month flat stipend); other remote employees receive no reimbursement.
  - The corporation operates one centralised harassment-prevention training module, delivered once at new-hire and never refreshed, built against California AB 1825 content.
  - The corporation's standard offer letter includes a $75,000-floor-indexed non-solicit that the drafter copied from an Illinois-focused template; it has not been reviewed for California or Washington specifics.
  - The corporation posts salary ranges in some job postings and not others; the practice is ad hoc.
  - The corporation runs a candidate background check with FCRA consent but no state-specific Fair Chance addendum.
  - The corporation's standard payroll cadence is bi-weekly for all employees including NYC manual-worker-adjacent engineering staff.
- **Series-A diligence is 90 days out.**

## Requirements

### Part A — The state-law compliance matrix

Produce a comprehensive compliance matrix with:

- **Rows:** the nine recurring axes of state-law variance from chapter 08 — (1) worker classification, (2) wage-and-hour (daily overtime, meal-and-rest, salary-basis threshold, wage-statement and waiting-time penalties, expense reimbursement), (3) paid leave (family and medical, sick, pregnancy disability, bereavement, reproductive-loss, jury/voting/school-activities), (4) non-competes / restrictive covenants, (5) pay transparency and salary-history bans, (6) Fair Chance / ban-the-box, (7) anti-discrimination protected-category expansion, (8) biometric-information handling, (9) arbitration and dispute-resolution. Plus two Acme-specific rows: (10) expense reimbursement for remote workers, (11) harassment-prevention training requirements.
- **Columns:** California, New York State, New York City (separately where it adds law beyond state), Illinois, Chicago (separately where applicable), Washington, Seattle (where applicable), Colorado.
- **Cells:** the controlling statute(s) with citation, the specific requirement that applies, and a flag `[✓ compliant / ✗ non-compliant / ? review]` based on the Facts above.

Where current-year indexed figures are needed (CA minimum wage and exempt salary-basis threshold, NY State salary thresholds by region, WA RCW 49.46.210 multiplier for exempt salary basis, WA RCW 49.62.020 non-compete earnings threshold, CO C.R.S. § 8-2-113(2)(b) highly-compensated-worker threshold, IL 820 ILCS 90/10 and 90/15 non-compete and non-solicit earnings thresholds, CO FAMLI premiums), flag with `<!-- needs-research -->` and describe the compliance posture in general terms.

### Part B — Non-compliance remediation plan

For every cell marked `✗ non-compliant` in Part A, produce a specific remediation entry:

1. **The violation** — the specific statutory requirement that is not met.
2. **The exposure** — enforcement channel (private right of action, state agency charge, state attorney general, class action), potential damages, and the extent to which the violation has already materialised (e.g., *Vega v. CM & Associates* liability for the bi-weekly NYC pay cadence for any employee who could be classified as a "manual worker").
3. **The remediation** — the specific operational change required, with owner (Head of People / Head of Finance / outside counsel), timeline, and interim mitigation.
4. **The look-back exposure** — the number of pay periods / employee-days / covered events for which the violation has already run, and whether the corporation has an obligation to issue retroactive remediation (back wages, retroactive premium pay, retroactive reimbursements) or notice.

Address at minimum (from the Facts):

- **The NYC bi-weekly pay cadence** under NY Lab. Law § 191 and the *Vega* decision. For any employee who meets the "manual worker" definition (chapter 08 flags this), the bi-weekly cadence creates liquidated-damages exposure. Produce the analysis.
- **The California-only WFH stipend** under Cal. Lab. Code § 2802 and *Cochran v. Schwan's Home Service*. For California remote workers, the stipend is likely non-compliant on amount; for other-state remote workers, no state law requires reimbursement, but some do — flag the Illinois Wage Payment and Collection Act and the few other states that may apply.
- **The Chicago biometric time-and-attendance system** under BIPA, 740 ILCS 14. Written informed consent, written retention-and-destruction policy, sale-and-disclosure limits. Per-collection private right of action with statutory damages per *Cothron v. White Castle System, Inc.*, 2023 IL 128004. Multi-year look-back exposure is substantial. Produce the specific remediation (replace with non-biometric system or come into BIPA compliance; retention-and-destruction policy; written consent; disclosure framework) and the look-back exposure analysis.
- **The harassment-prevention training program** — California requires AB 1825 / SB 1343 compliant training for supervisory employees every two years and non-supervisory employees every two years. New York State requires annual training per NY Lab. Law § 201-g. NYC requires annual training per NYC Admin. Code § 8-107(29). Illinois requires annual training under IHRA § 2-109. Chicago requires annual bystander-intervention training. Washington requires training by rule for certain employers. Address each state's training requirement and produce the compliance remediation.
- **The one-size-fits-all non-solicit** — defaulted to the Illinois $75,000 earnings-threshold formulation. For California employees, void under *AMN Healthcare* and chapter 06; for Washington employees, must comply with RCW 49.62; for Colorado employees, must comply with C.R.S. § 8-2-113. Produce the remediation (cross-reference exercise 05's output if relevant).
- **The ad hoc salary-range disclosure practice.** California SB 1162 / Cal. Lab. Code § 432.3(c), NY Lab. Law § 194-b, NYC Local Law 32, IL HB 3129 / 820 ILCS 112, WA RCW 49.58.110, CO C.R.S. § 8-5-201 all apply (chapter 03). Produce the remediation (universal range disclosure, consistent format, documented good-faith-range methodology).
- **The background-check Fair Chance addendum.** California (Cal. Gov. Code § 12952), NYC (Admin. Code § 8-107(11)), Illinois (820 ILCS 75), WA RCW 49.94, CO C.R.S. § 8-2-130 all apply (chapter 07). Produce the remediation.

### Part C — The highest-common-denominator vs. per-state operating-policy decision

For each of the eleven matrix rows in Part A, decide whether Acme adopts:

- **National baseline** — the strictest state's rule applied everywhere; or
- **Per-state variant** — jurisdiction-specific rules at each location.

For each decision, justify under chapter 08's trade-off framework (cost, operational complexity, employee-relations optics, diligence posture, migration-proofing, over-commitment risk). Expected pattern per chapter 08:

- **National baseline candidates** — anti-harassment policy and training (schedule to the strictest state's cadence; content covers the strictest state's required material), EEO statement (union of protected categories), salary-history ban (national), salary-range disclosure in postings (national), Fair Chance individualised-assessment protocol (national), PIIA present-assignment and DTSA notice (national), arbitration clause with EFAA and PAGA carve-outs (national).
- **Per-state variants** — daily overtime (California only), meal-and-rest premiums (California only), state salary-basis threshold for exemption (per state), expense reimbursement (California; other states where applicable), paid family and medical leave benefits (per state's statutory program), paid sick leave hours (per state; Chicago overlay), state-law invention-assignment carveout language (per state as in chapter 04), BIPA compliance (Illinois only), non-compete / non-solicit specifics (per state as in chapter 06 and exercise 05), AI-driven hiring tool bias audit (where applicable — NYC, Colorado as it comes into effect).

For each decision, state the design choice and the one-sentence rationale.

### Part D — The state-rider document pack

Produce the content outline (not full drafts) for the state-rider documents the corporation needs. Each rider is a short state-specific supplement to the national-baseline document, delivered to employees at hire (and to existing employees as part of a Part E remediation campaign). The riders include:

1. **California wage-and-hour, leave, and reimbursement rider.** Daily overtime per Cal. Lab. Code § 510; meal-and-rest premiums per Cal. Lab. Code §§ 226.7, 512; expense reimbursement per § 2802; CFRA eligibility per Cal. Gov. Code § 12945.2; PDL per § 12945; PFL per Cal. Unemp. Ins. Code § 3300; paid sick leave per Cal. Lab. Code § 246 as amended; bereavement per § 12945.7; reproductive-loss leave per § 12945.6; waiting-time penalties per § 203; wage-statement requirements per § 226.
2. **New York State and NYC rider.** NY Lab. Law § 191 pay-frequency and the manual-worker analysis; § 195 wage-notice and wage-statement; § 652 state minimum wage with regional differentials; § 162 meal-period requirements; 12 NYCRR § 142-2.14 salary thresholds for exemption; NY PFL per Workers' Comp. Law § 200; NY State and NYC paid sick leave; NYCHRL protected-category breadth; NYC Fair Chance Act procedures; NYC and state salary-transparency; NYC AEDT bias-audit (NYC Local Law 144).
3. **Illinois and Chicago rider.** Illinois Wage Payment and Collection Act; 820 ILCS 90 non-compete / non-solicit earnings thresholds; Illinois Paid Leave for All Workers Act (820 ILCS 192); Illinois Human Rights Act protected-category breadth; Illinois ban-the-box (820 ILCS 75); Illinois Equal Pay Act salary-transparency amendments; **BIPA** (740 ILCS 14) with the written-consent and retention-and-destruction-policy template; Chicago Fair Workweek Ordinance (if applicable); Chicago Paid Leave Ordinance.
4. **Washington and Seattle rider.** RCW 49.46 minimum wage and overtime; RCW 49.46.210 salary-basis multiplier; RCW 50A PFML; RCW 49.46.200 paid sick leave; RCW 49.62 non-compete; RCW 49.58 Equal Pay and Opportunities Act and salary-transparency; RCW 49.94 Fair Chance; RCW 49.60 WLAD; RCW 49.44.210 arbitration restriction post-EFAA; Seattle Wage Theft Ordinance; Seattle Paid Sick and Safe Time Ordinance; Seattle Fair Chance Employment Ordinance.
5. **Colorado rider.** COMPS Order 39 overtime and meal-and-rest; Colorado FAMLI; HFWA paid sick leave; C.R.S. § 8-2-113 non-compete; C.R.S. § 8-5-201 et seq. Equal Pay for Equal Work Act as amended; C.R.S. § 8-2-130 Chance to Compete; CADA protected-category breadth and the POWR amendments; **Colorado AI Act (SB 24-205)** as it comes into effect February 1, 2026 for high-risk AI employment-decision systems.

Each rider's outline specifies: the governing statute(s) with citation, the employee-facing content (what the employee needs to know), the operational content (what the corporation does differently in that state), and the referenced documents (benefit-plan summary, handbook rider, PIIA state-carveout schedule).

### Part E — The maintenance discipline

Produce the corporation's state-law maintenance program per chapter 08's "maintenance discipline" section:

1. **State-law tracker.** Format and content of the running state-law tracker (per-state, per-statute, current-version-and-amendment date, next-review-trigger). Specify owner and review cadence.
2. **Quarterly refresh cadence.** Document the quarterly review process — what is reviewed, who signs off, how changes propagate to the matrix / riders / handbooks / offer-letter templates / ATS configuration / payroll settings.
3. **New-hire trigger.** The onboarding workflow for a hire in a new state (or in a state where headcount is now above a statutory threshold that didn't previously apply). Specify the trigger thresholds (e.g., Cal. Gov. Code § 12952 Fair Chance Act applies to employers with 5+ employees; Cal. Gov. Code § 12945.2 CFRA applies to employers with 5+ employees; NY Exec. Law § 296 and NYCHRL now apply to all employers; NY Lab. Law § 194-b salary-transparency applies at 4+ employees).
4. **Outside-counsel relationship.** The scope of the retained-outside-counsel relationship (primary firm with multi-state coverage; specialist firms by state) and the trigger for engagement (new-state hire, new-state statute, state-agency charge, pre-RIF review).
5. **Legislative-session triggers.** The timing of state legislative sessions (most end spring / early summer; late-summer / early-fall is the critical refresh window for January-1 effective dates).
6. **A "state-of-the-handbook" annual memo.** The corporation produces an annual memo documenting that the handbook, offer-letter template, PIIA, arbitration provision, and state-rider documents have been reviewed and updated. This memo becomes a diligence artifact.

### Part F — Series-A diligence response package

Produce the compliance-program section of the Series-A diligence response:

1. The matrix from Part A (as of the diligence date, with cells marked `✓ compliant` where remediation is complete, `in-progress` where it is scheduled, or `scheduled` where remediation is planned post-funding).
2. The remediation plan from Part B, with status.
3. The highest-common-denominator vs. per-state operating-policy decisions from Part C.
4. The state-rider document pack from Part D (final drafts in a separate repository the corporation will share).
5. The maintenance discipline from Part E.
6. A short memo listing the outstanding compliance risks (anything in Part B that is not yet remediated) and the mitigation posture (reserves, insurance coverage, documented management attention).

### Part G — Design-choices memo

A 2–3 page memo covering:

- The three design choices you found hardest (likely: biometric time-and-attendance remediation vs. system replacement; universal salary-range posting vs. per-state; the harassment-training frequency and content design).
- The hybrid highest-common-denominator / per-state model you chose and the rationale.
- The practical mechanism for the state-law tracker — spreadsheet, specialised vendor tool, outside-counsel-maintained artifact.
- The migration vector — how the corporation handles state-to-state employee moves, which trigger a new state's compliance surface (chapter 08 "new-hire trigger" extended to transfers).
- The relationship between this exercise and mod-104 (hiring and HR operations), mod-106 (total rewards), mod-107 (performance and offboarding), mod-110 (privacy and biometric compliance at depth), mod-112 (enterprise risk and insurance) — note the hand-offs explicitly per chapter 10.
- Any `<!-- needs-research -->` items you flagged — current indexed thresholds (CA minimum wage; WA salary-basis multiplier; WA RCW 49.62 non-compete threshold; CO C.R.S. § 8-2-113 highly-compensated threshold; IL 820 ILCS 90 thresholds; NY State salary thresholds by region; BIPA damages framework after any 2025–2026 amendments; Colorado AI Act (SB 24-205) implementing regulations and enforcement posture); current state-and-city AEDT regulations; current Washington My Health My Data Act employer-facing implications; current PWFA regulations at 29 C.F.R. Part 1636.

## Starter guidance

- Chapter 08 is the primary reference. Cross-references to chapters 01, 02, 03, 06, 07, and 09 and the mod-102 chapter 04 PIIA carveout schedule are expected.
- The matrix is a working artifact. Expect it to be in a tabular / spreadsheet form conceptually; you may present it in Markdown-table form or in a structured per-row / per-column outline — the format should be auditable and copy-able.
- The biometric remediation is substantial. BIPA's $1,000 / $5,000 per-violation damages structure plus the *Cothron* per-collection accrual rule means a four-employee system that has run for 18 months of twice-daily fingerprint scans represents a facially material exposure. The remediation choice (replace with non-biometric vs. come into compliance) is a judgment call; document it.
- The harassment-training analysis is subtle. California's cadence (every two years for supervisors and non-supervisors) is less frequent than New York State (annual) and NYC (annual) and Illinois (annual). The national baseline should match the strictest (annual, with content covering each applicable state's required elements).
- The NY Lab. Law § 191 manual-worker analysis is the single highest-exposure item. For software engineers, product managers, and the usual startup workforce, the "manual worker" definition applies to a specific class of workers; the NY DOL's historical interpretation covers more workers than the statute's text might suggest at first read. Flag as `<!-- needs-research -->` the specific DOL and Court of Appeals interpretation; conservatively assume any employee whose job involves substantial physical activity (even in a software context — e.g., hardware testing, lab work, warehouse ops) may fall within the definition. In the Acme fact pattern, likely no engineer falls within the definition, but address the question explicitly.
- The highest-common-denominator decision is per-row, not whole-document. Apply chapter 08's framework row by row.
- Do NOT invent current-year thresholds. Flag with `<!-- needs-research -->` and operate on the chapter 08 framework in general terms.
- The Chicago biometric remediation and the NY Lab. Law § 191 analysis are substantial individual decisions — produce specific memos for each.

## Deliverables

- `state-law-compliance-matrix.md` — Part A.
- `non-compliance-remediation-plan.md` — Part B, with discrete sub-sections for biometric remediation, pay-cadence remediation, harassment-training remediation, non-solicit remediation, salary-range disclosure remediation, Fair Chance remediation, expense-reimbursement remediation.
- `highest-common-denominator-decisions.md` — Part C.
- `state-rider-document-pack-outline.md` — Part D.
- `maintenance-discipline-memo.md` — Part E.
- `series-a-diligence-compliance-package.md` — Part F (table-of-contents).
- `state-law-variance-design-choices-memo.md` — Part G.

## Acceptance criteria

The package is acceptable if:

1. The matrix covers the nine chapter 08 axes plus the two Acme-specific rows across all eight columns (CA, NY State, NYC, IL, Chicago, WA, Seattle, CO).
2. Each cell cites the controlling statute by section number (not just "California FEHA" — the specific Cal. Gov. Code section).
3. The compliance flags `✓ / ✗ / ?` are supported by the Facts, with no hand-waving.
4. The remediation plan covers at minimum: NYC Lab. Law § 191 pay-cadence, BIPA Chicago time-and-attendance, harassment-training program redesign, non-solicit retrofit, universal salary-range disclosure, Fair Chance background-check addendum, Cal. Lab. Code § 2802 expense-reimbursement review.
5. The BIPA remediation memo addresses the per-collection *Cothron* damages exposure, the written-informed-consent requirement, the retention-and-destruction-policy requirement, the no-sale-or-disclosure requirement, and the look-back exposure for the four Chicago employees over the deployment period.
6. The NY Lab. Law § 191 analysis addresses the manual-worker definition, the *Vega* liquidated-damages private right of action, and the pay-cadence remediation (switch to weekly for any employee who meets the manual-worker definition, or document the engineering-staff analysis for why the definition does not apply).
7. The highest-common-denominator vs. per-state decisions are per-row and justified under chapter 08's framework.
8. The state-rider document outlines cover the governing statutes, employee-facing content, operational content, and referenced documents per rider.
9. The maintenance discipline addresses the state-law tracker, quarterly refresh, new-hire trigger, outside-counsel relationship, legislative-session timing, and the state-of-the-handbook annual memo.
10. Statutory citations (Cal. Gov. Code §§ 12945.2, 12952, 12900 et seq.; Cal. Lab. Code §§ 2775, 203, 226, 226.7, 246, 432.3, 510, 512, 2802; Cal. Bus. & Prof. Code §§ 16600, 16600.1; Cal. Unemp. Ins. Code § 3300; NY Exec. Law § 296; NY Lab. Law §§ 191, 194-a, 194-b, 195, 196-b, 201-g, 652; NY Workers' Comp. Law § 200; NY Gen. Oblig. Law § 5-336; NYC Admin. Code §§ 8-107, 20-911, 22-1201; 775 ILCS 5; 820 ILCS 75, 90, 112, 115, 140, 180, 192; 740 ILCS 14; RCW 49.44.210, 49.46, 49.46.200, 49.46.210, 49.58, 49.58.110, 49.60, 49.62, 49.94, 50A; C.R.S. §§ 8-2-113, 8-2-130, 8-4-101, 8-5-201 et seq., 8-13.3-401, 24-34-401; *Dynamex Operations West, Inc. v. Superior Court*, 4 Cal. 5th 903 (2018); *Cochran v. Schwan's Home Service, Inc.*, 228 Cal. App. 4th 1137 (2014); *Vega v. CM & Associates Construction Management, LLC*, 175 A.D.3d 1144 (1st Dep't 2019); *Cothron v. White Castle System, Inc.*, 2023 IL 128004) are correct.
11. Nothing left as `[FILL IN]` or `[TBD]` — every field populated or explicitly flagged with a `<!-- needs-research -->` marker.
