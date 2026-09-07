# 8. State-law variance across California, New York, Illinois, Washington, Colorado

> The five most-consequential state-law overlays for a distributed US startup. Federal law is the floor; California, New York, Illinois, Washington, and Colorado routinely raise it — and the corporation has to choose whether to default to the highest common denominator or maintain per-state operating policy.

## Motivation

A hire in San Francisco, a hire in Manhattan, a hire in Chicago, a hire in Seattle, and a hire in Denver all sit under different statutory regimes. The federal core (chapter 07) covers all of them, but each of those five jurisdictions adds a stack of state-and-city law on top — a stack that a national employment-policy handbook, an offer letter template, a PIIA suite, and a payroll-and-benefits program has to accommodate.

The five jurisdictions covered here are picked because they are (a) where a disproportionate fraction of US startup workforces are located, (b) the most active source of new employment-law statutes over the last decade, and (c) the jurisdictions whose statutory choices frequently propagate to other states over time. A COO / GC who has this five-state layer clear can extend the same framework to any additional state the corporation hires into.

This chapter is not a comprehensive state-by-state matrix — that is a compliance-tool artifact, not a lecture. It is the practitioner's mental model for the recurring axes on which state law varies, the specific statutes in each of the five jurisdictions, and the highest-common-denominator versus per-state operating-policy decision.

## The recurring axes of state variance

Nine axes account for most of the state-law variance a startup encounters:

1. **Worker classification** — ABC test vs. common-law test (chapter 01).
2. **Wage-and-hour** — daily overtime rules, meal-and-rest breaks, minimum wage, salary-basis thresholds (chapter 02), waiting-time and wage-statement penalties.
3. **Paid leave** — paid family leave, paid sick leave, pregnancy disability leave, bereavement leave, jury and voting leave, school-activities leave.
4. **Non-competes and restrictive covenants** — bans, thresholds, notice requirements (chapter 06).
5. **Pay transparency and salary-history bans** — job-posting range disclosure, salary-history-inquiry bans (chapter 03).
6. **Fair Chance / ban-the-box** — criminal-history inquiry and adverse-action requirements.
7. **Anti-discrimination protected-category expansion** — sexual orientation, gender identity, marital status, source of income, criminal history, salary history, reproductive-health decisions, weight, height, hair texture, off-duty conduct, cannabis use (chapter 07).
8. **Biometric-information handling** — HR-adjacent biometrics for time-and-attendance, facility access, and identity verification.
9. **Arbitration and dispute-resolution** — carve-outs from mandatory arbitration for sexual-harassment / assault claims, whistleblower claims, and PAGA in California (chapter 09).

For each of the five focus jurisdictions below, the treatment is structured around these axes, plus jurisdiction-specific enforcement mechanisms and notable recent legislative activity.

## California

California is the strictest US employment-law jurisdiction and the source of the most-cited state statutory patterns. Every startup with any California workforce needs specific California-side compliance workstreams; a national handbook that treats California as one column in a state matrix will fail on multiple fronts.

### Worker classification — the ABC test and AB 5

**Cal. Lab. Code § 2775** codifies the ABC test from *Dynamex* (see chapter 01). Prong (B) — "outside the usual course of the hiring entity's business" — disqualifies almost every operational contractor at a technology startup. Statutory exceptions at Cal. Lab. Code §§ 2776–2784 return specified occupations and business-to-business relationships to the *Borello* multi-factor test, but the exceptions are narrow and each has conditions the engagement must satisfy.

Enforcement: EDD (payroll-tax and unemployment-insurance), Labor Commissioner (wage-and-hour), Attorney General (UCL / § 17200), city attorneys (San Francisco, Los Angeles, San Diego), and private plaintiffs (PAGA representative actions on behalf of the state under Cal. Lab. Code § 2698 et seq.).

### Wage-and-hour

- **Cal. Lab. Code § 510 daily overtime** — 1.5× regular rate for hours over 8/day; 2× regular rate for hours over 12/day and over 8 on the seventh consecutive day. Applies to non-exempt employees only. This is materially more expensive than the federal weekly-overtime rule (chapter 02).
- **Meal and rest breaks** — Cal. Lab. Code § 512 (30-minute unpaid meal period before the end of the fifth hour; second meal period for shifts over 10 hours), Wage Order § 12 (10-minute paid rest period per four hours worked or major fraction thereof). Non-provision creates a one-hour-of-pay premium per work day (Cal. Lab. Code § 226.7); premiums are wages for purposes of § 226 wage-statement claims and § 203 waiting-time penalties.
- **Salary basis for exemption** — twice the state minimum wage for full-time employment. At the current state minimum wage this is materially higher than the federal $58,656/year. <!-- needs-research: current California minimum wage and the corresponding annual salary-basis threshold for exempt employees. -->
- **Cal. Lab. Code § 226** — itemised wage-statement requirements (nine specified data elements); non-compliance creates $50 first-pay-period / $100 subsequent-pay-period penalties per employee, aggregated across the workforce and multiplied through PAGA.
- **Cal. Lab. Code § 203 waiting-time penalties** — an employer that willfully fails to pay all final wages on the required day (termination — same day; resignation with 72+ hours notice — last day worked; resignation without notice — within 72 hours) owes the employee up to 30 days' additional pay as a penalty.
- **Cal. Lab. Code § 2802** — expense reimbursement. Employers must reimburse employees for all necessary business expenses. In the remote-work era, this drives a home-office / phone / internet reimbursement obligation that many national employers overlook. *Cochran v. Schwan's Home Service, Inc.*, 228 Cal. App. 4th 1137 (2014) requires reimbursement of *some* portion of a personal cell-phone bill used for work — a "reasonable percentage" — regardless of whether the employee incurred an incremental cost.

### Paid leave

- **California Family Rights Act (CFRA)** — Cal. Gov. Code § 12945.2. Applies to employers with 5+ employees (compared to federal FMLA's 50-employee threshold). Provides 12 weeks of protected leave per 12-month period for the employee's own serious health condition, a family member's serious health condition (definition of "family member" is broader than FMLA — includes designated persons and adult independent children), or bonding with a new child.
- **Pregnancy Disability Leave (PDL)** — Cal. Gov. Code § 12945. Up to four months of pregnancy-related disability leave, in addition to (not concurrent with) CFRA bonding leave.
- **Paid Family Leave (PFL)** — Cal. Unemp. Ins. Code § 3300 et seq. State disability-insurance program (SDI) that provides partial wage replacement for up to eight weeks. PFL is a wage-replacement program, not a job-protection program; job protection comes from CFRA / FMLA / PDL layered on top. AB 1041 (2022) expanded the definition of "family member."
- **Paid sick leave** — Cal. Lab. Code § 246 (Healthy Workplaces, Healthy Families Act as amended by SB 616, effective January 1, 2024). Minimum 40 hours or 5 days per year of paid sick leave. San Francisco, Los Angeles, San Diego, Berkeley, Emeryville, Long Beach, Oakland, and other cities have local ordinances that add hours or coverage — a per-city payroll question.
- **Bereavement leave** — Cal. Gov. Code § 12945.7 (AB 1949, effective 2023) — up to five days of bereavement leave for a family member's death; may be unpaid if the employer's policy does not provide paid bereavement.
- **Reproductive-loss leave** — Cal. Gov. Code § 12945.6 (SB 848, effective 2024) — up to five days of leave for reproductive loss.

### Non-competes

Cal. Bus. & Prof. Code § 16600 has voided post-employment non-competes for over a century (see chapter 06). AB 1076 (2023) added a February 14, 2024 notice obligation. SB 699 (2023) voided non-competes signed anywhere and enforced against California employees, and provides fee-shifting to the employee.

### Pay transparency and salary history

- **Cal. Lab. Code § 432.3** — salary-history ban. Employers may not ask about or rely on prior salary in setting compensation; must provide the pay scale for the position upon reasonable request.
- **Cal. Lab. Code § 432.3(c) (SB 1162, effective January 1, 2023)** — pay-transparency requirement. Employers with 15+ employees must include the pay scale in any job posting; internal postings included; posting a range without a good-faith basis violates the statute. Private right of action for aggrieved applicants and employees; penalties from $100 to $10,000 per violation.
- **Cal. Gov. Code § 12999 (SB 1162)** — pay-data reporting. Employers with 100+ employees must file an annual pay-data report with the California Civil Rights Department (CRD) disclosing wage-band distribution by race, ethnicity, and sex for each job category, and a separate report on labor-contractor-supplied workers. Compliance is a specific annual workstream.

### Fair Chance

- **California Fair Chance Act — Cal. Gov. Code § 12952.** Prohibits pre-conditional-offer inquiry into criminal history; requires individualised assessment; requires specific pre-adverse-action and post-adverse-action notice; requires the employer to consider the nature and gravity of the offense, the time elapsed, and the nature of the job. Enforced by the CRD.
- **Los Angeles County Fair Chance Ordinance for Employers (effective September 3, 2024)** and similar local ordinances add procedural steps beyond the state Act.

### Protected-category expansion

FEHA (Cal. Gov. Code § 12900 et seq.) applies to employers with 5+ employees (compared to Title VII's 15-employee threshold) and covers a broader protected-category list than federal law: race (including CROWN Act protection for hair texture and protective hairstyles), color, religion (including religious dress and grooming), national origin, ancestry, physical or mental disability, medical condition, genetic information, marital status, sex (including pregnancy, childbirth, breastfeeding, and related conditions), gender, gender identity, gender expression, sexual orientation, age (40+), military and veteran status, reproductive-health decision-making. No damages cap.

### Biometrics

California does not have a BIPA-analog private right of action, but the CCPA / CPRA imposes disclosure and consumer-rights obligations on employer collection of biometric information under the "personal information" definition (Cal. Civ. Code § 1798.140(v)). Voluntary opt-in and clear notice are the operating floor. See [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) for depth.

### Arbitration and PAGA

California's Private Attorneys General Act (Cal. Lab. Code § 2698 et seq.) creates a representative-action mechanism for Labor Code penalties on behalf of the state, with 75% of penalties going to the state and 25% to aggrieved employees. Post-*Viking River Cruises, Inc. v. Moriana*, 596 U.S. 639 (2022), individual PAGA claims can be sent to arbitration, but non-individual (representative) PAGA claims remain in court — the California Supreme Court in *Adolph v. Uber Technologies, Inc.*, 14 Cal. 5th 1104 (2023), confirmed that an employee retains standing to pursue non-individual PAGA claims after individual claims are compelled to arbitration. See chapter 09 for depth.

## New York (state and NYC)

New York State and New York City each add their own layer. NYC has aggressive city-level statutes that frequently exceed state law and always exceed federal law.

### Worker classification

New York applies a common-law test analogous to the IRS test for state unemployment-insurance and wage-hour purposes, but industry-specific "freelance" and "construction" statutes add complexity. The **New York Freelance Isn't Free Act** (originally NYC Admin. Code § 20-927, extended statewide by Ch. 302 of 2023, effective 2024) requires written contracts for freelance work over $800, prompt payment (or on the date specified), and creates a private right of action with double damages and attorneys' fees for late or non-payment. The Act does not reclassify workers as employees, but it materially raises the friction of using contractors.

### Wage-and-hour

- **NY Lab. Law § 191** — weekly wage-payment requirement for "manual workers" (a category the New York courts and Department of Labor have interpreted broadly). Failure to pay weekly creates a private right of action with liquidated damages equal to 100% of the untimely-paid wages (*Vega v. CM & Associates Construction Management, LLC*, 175 A.D.3d 1144 (1st Dep't 2019)). Many employers pay bi-weekly and face material back-liability exposure. <!-- needs-research: track the current status of NY State legislative efforts and New York Court of Appeals treatment of the Vega private right of action for § 191 violations. -->
- **NY Lab. Law § 195** — wage-statement and wage-notice requirements (Wage Theft Prevention Act). Penalties for non-compliance.
- **NY Lab. Law § 652** — state minimum wage, with higher rates in NYC / Nassau / Suffolk / Westchester.
- **NY Lab. Law § 162** — meal-period requirements (30-minute meal period for shifts over 6 hours; specific timing rules).
- **12 NYCRR § 142-2.14 salary threshold for exemption** — the state has higher salary-basis thresholds than the federal floor for executive and administrative exemptions, with a NYC / Nassau / Suffolk / Westchester differential. <!-- needs-research: current-year NY State salary thresholds by region. -->

### Paid leave

- **NY Paid Family Leave (PFL)** — NY Workers' Comp. Law § 200 et seq. Job-protected paid leave (up to 12 weeks at 67% of average weekly wage, subject to cap) funded by employee payroll contributions. Bonding, family care, military exigency, and (2024 expansion) prenatal care.
- **NY State Disability Insurance (SDI)** — separate short-term disability program.
- **NY Paid Sick Leave — NY Lab. Law § 196-b.** Statewide paid sick leave (5 or 7 days depending on employer size).
- **NYC Earned Safe and Sick Time Act — NYC Admin. Code § 20-911 et seq.** NYC-specific paid sick and safe leave that layers on top of the state law.
- **NYC Temporary Schedule Change Law and Fair Workweek Law** — apply primarily to retail and fast-food but with broader-application analogs in other cities.

### Non-competes

New York State non-compete legislation passed in 2023 (S.3100A) was vetoed by Governor Hochul citing carve-out concerns. Narrower proposals have been introduced. See chapter 06. <!-- needs-research: verify the current status of New York non-compete legislation and any legislative or gubernatorial action after 2024. -->

### Pay transparency and salary history

- **NY Lab. Law § 194-a** — salary-history ban (statewide).
- **NYC Admin. Code § 8-107(32)** — NYC salary-history ban (predates state law).
- **NY Lab. Law § 194-b (effective September 17, 2023)** — statewide job-posting pay-range disclosure. Applies to employers with 4+ employees.
- **NYC Admin. Code § 8-107(32) — Local Law 32 of 2022** — NYC job-posting range disclosure, effective November 1, 2022; more prescriptive than state law in some respects.

### Fair Chance

- **NYC Fair Chance Act — NYC Admin. Code § 8-107(11).** Prohibits pre-conditional-offer criminal-history inquiry; requires individualised assessment; requires specific notice and rescission procedures. The 2021 amendments broadened coverage to include pending arrests and to strengthen the individualised-assessment requirement.
- **NY State — general Correction Law Article 23-A** — public policy against employment discrimination based on criminal history; requires individualised assessment.

### Protected-category expansion

**NY State Human Rights Law — Exec. Law § 296.** Applies to all employers regardless of size (as of the 2019 amendments). Adds sexual orientation, gender identity or expression, familial status, marital status, military status, predisposing genetic characteristics, domestic-violence-victim status, and others to the federal core.

**NYC Human Rights Law — NYC Admin. Code § 8-107.** Applies to employers with 4+ employees. Adds partnership status, arrest / conviction record (subject to Fair Chance rules), consumer credit history (NYC Stop Credit Discrimination in Employment Act), unemployment status, actual or perceived caregiver status, sexual and reproductive-health decisions, height and weight (Local Law 61 of 2023), and others. The NYCHRL is interpreted "independently" and "more broadly" than federal or state law; NYC Commission on Human Rights and private plaintiffs pursue aggressive damages.

### Biometrics

**NYC Biometric Identifier Information Law — NYC Admin. Code § 22-1201 et seq.** Consumer-facing; not principally aimed at HR biometrics but relevant to employer-issued visitor / customer check-in systems.

### Arbitration and dispute-resolution

**NY CPLR § 7515 (as originally enacted in 2018 and amended in 2019)** was intended to prohibit mandatory arbitration of harassment claims; the federal Ending Forced Arbitration Act of 2022 (see chapter 09) largely federalised this protection.

## Illinois

Illinois has aggressively expanded employment-law protections in the last five years, and has one of the most-consequential biometrics statutes in the country.

### Worker classification

Illinois applies an ABC test for wage-payment (820 ILCS 115/2) and workers'-comp (820 ILCS 305/1) purposes, and a variant test for unemployment insurance. The ABC test tracks the *Dynamex* / Massachusetts formulation, with prong (B) written as "outside the usual course of business or outside all places of business." Illinois enforcement is less publicised than California's but the exposure structure is similar.

### Wage-and-hour

- **Illinois Wage Payment and Collection Act — 820 ILCS 115.** Specific pay-frequency, wage-statement, and final-wage rules with statutory damages (2% per month of underpayment plus attorneys' fees; 5% for wilful conduct).
- **Illinois One Day Rest in Seven Act — 820 ILCS 140.** Weekly rest day, meal-period requirements.
- **Chicago Fair Workweek Ordinance — Chi. Mun. Code § 1-25.** Predictive-scheduling rules for covered industries.

### Paid leave

- **Illinois Paid Leave for All Workers Act — 820 ILCS 192 (effective January 1, 2024).** Requires most employers to provide up to 40 hours of paid leave per year for any reason (no requirement that the employee state the reason).
- **Chicago Paid Leave and Paid Sick and Safe Leave Ordinance — Chi. Mun. Code § 6-140 (effective July 1, 2024).** Layers additional hours and coverage on top of the state law.
- **Illinois Family Bereavement Leave Act — 820 ILCS 154.** Up to 10 days of bereavement leave.
- **Victims' Economic Security and Safety Act (VESSA) — 820 ILCS 180.** Leave for domestic-violence victims.

### Non-competes

**Illinois Freedom to Work Act — 820 ILCS 90 (as amended, effective January 1, 2022).** Non-competes void for employees earning under $75,000 per year (indexed); non-solicits void for employees earning under $45,000 per year (indexed). Notice and consideration requirements; see chapter 06.

### Pay transparency and salary history

- **Illinois Equal Pay Act — 820 ILCS 112** (amended by HB 3129, effective January 1, 2025). Job-posting pay-range disclosure for employers with 15+ employees; additional Equal Pay Registration Certificate for employers with 100+ employees.
- **Illinois salary-history ban — 820 ILCS 112/10(b).** Enacted 2019.

### Fair Chance

- **Illinois Job Opportunities for Qualified Applicants Act — 820 ILCS 75.** Ban-the-box; prohibits pre-interview or pre-conditional-offer criminal-history inquiry.
- **Employee Background Fairness Act — 820 ILCS 55/12 (2021 amendment to the Illinois Human Rights Act).** Requires individualised assessment before adverse action based on conviction record.

### Protected-category expansion

**Illinois Human Rights Act — 775 ILCS 5.** Broad protected-category list including race, color, religion, sex, national origin, ancestry, age (40+), marital status, order of protection status, disability, military status, sexual orientation, gender identity, pregnancy, work authorisation status, and reproductive-health decisions. Applies to employers with 1+ employees for some provisions, 15+ for others.

### Biometrics — BIPA

**Illinois Biometric Information Privacy Act — 740 ILCS 14.** The single most-consequential state biometric-privacy statute in the US. Requires **written informed consent** before collection of biometric identifiers or biometric information (fingerprints, faceprints, voiceprints, retina scans, hand-geometry), a written retention-and-destruction policy, prohibition on sale, and specific disclosure limits. Private right of action with statutory damages of $1,000 per negligent violation and $5,000 per intentional or reckless violation, plus attorneys' fees. In *Cothron v. White Castle System, Inc.*, 2023 IL 128004 (Ill. Feb. 17, 2023), the Illinois Supreme Court held that a separate BIPA claim accrues each time a biometric is collected or disclosed — driving the per-violation damages into the hundreds of millions in some cases. **HR-adjacent BIPA exposure** includes any time-and-attendance system using fingerprint punch-in, any facility-access system using facial recognition, or any identity-verification tool using biometric matching. Any Illinois-employee-facing biometric touchpoint requires a BIPA compliance workstream. <!-- needs-research: verify the current damages framework and any 2025–2026 amendments to BIPA following industry lobbying to cap or modify the per-violation damages. -->

### Arbitration

Illinois passed the **Workplace Transparency Act — 820 ILCS 96 (2019)** limiting mandatory arbitration of harassment claims; the federal EFAA largely federalises this protection. Illinois-specific statute continues to matter for non-harassment mandatory-arbitration analysis.

## Washington

Washington has become a leading source of pay-transparency and non-compete statutes, and has a robust paid-family-leave program.

### Worker classification

Washington applies a modified common-law test with statutory factor lists for wage-and-hour, unemployment-insurance, and workers'-comp purposes. The state Employment Security Department is an active enforcement agency. Industry-specific rules (construction, transportation, entertainment) add complexity.

### Wage-and-hour

- **RCW 49.46** — Minimum Wage Act; state minimum wage is materially above the federal floor. Seattle and SeaTac have local minimum-wage ordinances above the state rate.
- **RCW 49.46.210 salary basis for exemption** — Washington's exempt salary-basis threshold is calculated as a multiplier of state minimum wage (2.5× for large employers by 2028, phased in). This exceeds the federal $58,656 floor materially at Washington's minimum wage. <!-- needs-research: current-year Washington exempt salary-basis threshold by employer size. -->
- **Seattle Wage Theft Ordinance — SMC 14.20** — payroll penalties for late or unpaid wages.

### Paid leave

- **Washington Paid Family and Medical Leave — RCW 50A.** Up to 12 weeks of paid family or medical leave (up to 18 weeks combined in a year for pregnancy complications), funded by employer and employee premiums. Job-protected for employees who meet an eligibility threshold.
- **Washington Paid Sick Leave — RCW 49.46.200.** Statewide paid sick leave, minimum 1 hour per 40 hours worked.
- **Seattle Paid Sick and Safe Time Ordinance — SMC 14.16** and other local ordinances.

### Non-competes

**RCW 49.62** (effective January 1, 2020). Post-employment non-competes enforceable only above an annual-earnings threshold (indexed), with disclosure and duration limits. See chapter 06. <!-- needs-research: current-year Washington earnings threshold under RCW 49.62.020, indexed to the consumer price index. -->

### Pay transparency and salary history

- **RCW 49.58.110** (as amended by SB 5761, effective January 1, 2023). Requires job-posting wage-range and benefits disclosure for employers with 15+ employees. Private right of action.
- **RCW 49.58** — Washington Equal Pay and Opportunities Act. Extensive pay-equity, promotion-opportunity, and career-advancement provisions.

### Fair Chance

**Washington Fair Chance Act — RCW 49.94.** Prohibits criminal-history inquiry until after an initial determination that the applicant is otherwise qualified. Seattle has additional local requirements (Seattle Fair Chance Employment Ordinance — SMC 14.17).

### Protected-category expansion

**RCW 49.60 — Washington Law Against Discrimination.** Applies to employers with 8+ employees. Includes race, color, religion, national origin, sex, age (40+), marital status, sexual orientation, gender identity, disability, honorably-discharged-veteran status, use of a trained service animal, and pregnancy.

### Biometrics

**RCW 19.375** — Washington's biometric statute. Regulates commercial (not employer) use of biometric identifiers; consent requirement narrower than BIPA. HR-adjacent employer biometric use is not subject to the same private-right-of-action exposure as in Illinois, but general privacy-tort and CCPA-analog developments (see the Washington My Health My Data Act) are increasing scrutiny. <!-- needs-research: verify the current status of Washington's My Health My Data Act (RCW 19.373) and any employer-facing implications. -->

### Arbitration

**RCW 49.44.210** — restricts mandatory arbitration of discrimination and harassment claims for Washington employers. Post-federal-EFAA, the statute continues to apply outside the federal preemption zone.

## Colorado

Colorado has moved aggressively on pay transparency, restrictive covenants, and workplace protections since 2019.

### Worker classification

Colorado applies a modified common-law test for unemployment-insurance (C.R.S. § 8-70-115) and workers'-comp purposes. The state has been comparatively active in enforcement against misclassification in the construction and gig-economy contexts. The **Colorado Wage Act** (C.R.S. § 8-4-101 et seq.) applies employee-status determinations for wage-payment purposes.

### Wage-and-hour

- **Colorado Overtime and Minimum Pay Standards Order (COMPS Order 39)** — state overtime rules, meal-and-rest-break requirements, salary-basis threshold for exemption. State salary-basis threshold above the federal floor. <!-- needs-research: current COMPS Order salary-basis threshold and daily-overtime provisions. -->
- **Colorado minimum wage** — indexed annually; Denver has a higher local minimum wage.

### Paid leave

- **Colorado FAMLI — Family and Medical Leave Insurance Act (SB 20-205).** Statewide paid family and medical leave, up to 12 weeks (16 weeks for pregnancy complications), funded by employer and employee premiums. Benefits available since January 1, 2024.
- **Colorado Healthy Families and Workplaces Act (HFWA) — C.R.S. § 8-13.3-401 et seq.** Statewide paid sick leave.

### Non-competes

**C.R.S. § 8-2-113** (as amended by HB 22-1317, effective August 10, 2022). Non-competes void except for the sale-of-business exception, for a "highly-compensated" employee (indexed threshold), and for narrow trade-secret protection with an income threshold. Notice and duration requirements. See chapter 06.

### Pay transparency and salary history

- **Colorado Equal Pay for Equal Work Act — C.R.S. § 8-5-201 et seq. (effective January 1, 2021, expanded by SB 23-105, effective 2024).** Job-posting pay-range disclosure (including a general description of benefits and any additional compensation such as bonuses), promotion-opportunity disclosure, and record-keeping requirements. Enforced by the Colorado Division of Labor Standards and Statistics.
- **Colorado salary-history ban.**

### Fair Chance

**Colorado Chance to Compete Act — C.R.S. § 8-2-130.** Prohibits pre-interview or pre-conditional-offer criminal-history inquiry for most employers.

### Protected-category expansion

**Colorado Anti-Discrimination Act — C.R.S. § 24-34-401 et seq.** Includes race, color, religion, national origin, sex, sexual orientation (including transgender status), gender identity, gender expression, age (40+), disability, marriage to a co-worker, ancestry, creed. The **Protecting Opportunities and Workers' Rights (POWR) Act — HB 23-1075 (2023)** expanded harassment definitions, changed the "severe or pervasive" standard, and modified statute-of-limitations and remedies.

### Biometrics

Colorado Privacy Act (C.R.S. § 6-1-1301 et seq.) covers commercial biometric handling; employer-facing scope is narrower than BIPA. HR biometrics require consent and disclosure but do not have BIPA-scale private-right-of-action exposure.

### AI-driven hiring tools

**Colorado AI Act — SB 24-205 (2024, effective February 1, 2026).** Regulates "high-risk artificial intelligence systems" including those used in employment decisions. Imposes documentation, disclosure, and impact-assessment obligations on developers and deployers of covered systems. First state omnibus AI act with employment-decision scope. <!-- needs-research: track the current status of Colorado AI Act implementation, amendments, and enforcement rules from the Colorado AG's office. -->

## The highest-common-denominator vs. per-state operating-policy decision

A national employer with employees in each of the five focus jurisdictions has two coherent options for its handbook, offer letter, PIIA, arbitration provisions, background-check process, pay-transparency disclosures, and leave programs.

### Option A — highest common denominator

Adopt a single national policy that satisfies the strictest applicable rule everywhere.

**Advantages:**

- Simpler operations. One handbook, one offer letter, one PIIA, one background-check workflow, one pay-transparency disclosure format.
- Cleaner diligence. Series-A / Series-B counsel reviewing the corporation's employment file sees a coherent, defensible package rather than a state-by-state patchwork.
- Employee-relations optics. Employees in less-restrictive states receive more-protective terms than the local law requires, which is generally not a downside.
- Migration-proof. As states expand protections (which the trend clearly favors), the national policy already covers the expansion.

**Disadvantages:**

- Cost. Applying California's daily-overtime and meal-and-rest-break premium rules to a Texas workforce is over-inclusive; applying Illinois's Paid Leave for All Workers Act generously to a Delaware workforce is over-inclusive; extending California's expense-reimbursement rule to every remote worker is materially more expensive than doing so only in California.
- Bargaining position. Offering the highest-common-denominator to every employee reduces flexibility to differentiate compensation and benefits by location.
- Some California-specific rules (PDL, CFRA definition of family member, PAGA) don't cleanly extrapolate to other states in a way that adds employee value; blanket application creates operational complexity without proportionate benefit.

### Option B — per-state operating policy

Maintain a base national policy plus state-specific riders, addenda, or variants for each state the corporation employs in.

**Advantages:**

- Cost-efficient — the corporation pays only the compliance overhead each state requires.
- Precise — the corporation's package matches each state's actual statutory floor, avoiding accidental over-commitment.
- Flexible — state-specific programs can be sunset if the corporation exits a state without unwinding a national policy.

**Disadvantages:**

- Operational complexity. Payroll, benefits, PTO tracking, offer letters, handbooks, and background checks all have to accommodate per-state variance.
- Diligence complexity. Counsel has to review a stack of state variants, and cross-state consistency issues (an employee moving from state to state) surface as diligence questions.
- Employee-relations friction. When employees notice that their Texas colleagues receive different terms than their California colleagues, it creates fairness questions the corporation has to defend.
- Failure modes. Each state variant is an independent surface for a compliance failure — a missed handbook update, a stale offer-letter template, a payroll-system misconfiguration.

### The practitioner default

Most modern startups operate a hybrid: highest-common-denominator for the *national handbook* (paid sick leave applied across all states at the strictest rate, harassment training extended nationwide to satisfy the strictest state's requirement, salary-history questions banned nationwide even where not required, salary ranges disclosed in every posting even where not required), plus per-state variants for the *jurisdiction-specific* items (California-side wage-and-hour rules, Illinois-side BIPA compliance, Massachusetts-side non-compete formalities, NYC-side Fair Chance and salary-transparency procedures). The base offer letter is national; a state-specific addendum sheet covers the wage-and-hour, meal-and-rest, expense-reimbursement, and paid-leave elements per state. The base PIIA is national with state-law invention-assignment carveout riders per state.

Which elements go into the "national baseline" and which are handled per-state is a judgment call. The recurring axes:

- **National baseline candidates** — anti-harassment policy, EEO statement, salary-history ban, salary-range disclosure format, background-check individualised-assessment protocol, PIIA present-assignment language and DTSA notice, arbitration clause with EFAA carve-out.
- **Per-state variants** — daily overtime, meal-and-rest premiums, expense reimbursement, paid family leave benefits and eligibility, paid sick leave hours, non-compete enforceability, BIPA compliance if there is any Illinois biometric touchpoint, PAGA-specific arbitration-clause structure for California employees.

The right cut for a specific corporation depends on where its workforce actually lives — a corporation with 80% California employees may find California-first drafting more efficient than highest-common-denominator; a corporation with three-employees-per-state across ten states may find highest-common-denominator cheaper than maintaining ten variants.

## The maintenance discipline

State employment law changes constantly. A comprehensive state-law compliance program has, at minimum:

- **A state-law tracker.** For every state and city the corporation employs anyone in, a running list of applicable statutes and their current version, with dates of last review. Maintained by counsel (in-house or outside).
- **A quarterly refresh cadence.** Legislative sessions typically end in mid-year; late-summer and early-fall refreshes catch the majority of new statutes before January-1 effective dates.
- **A new-hire trigger.** When the corporation onboards a hire in a new state (or a state where headcount was previously below a statutory threshold), a compliance-review workstream is triggered — check the state-law tracker, add any applicable riders or state-specific benefits, register for state UI / SDI, confirm workers'-comp coverage, update the handbook and offer-letter templates.
- **An outside-counsel relationship** with an employment-law firm that has multistate coverage. State-specific specialists become important when the corporation reaches material headcount in specific jurisdictions.

## Summary

- The five focus jurisdictions — California, New York (state and city), Illinois, Washington, Colorado — cover a disproportionate fraction of US startup workforces and are the most-active source of state-and-city employment-law statutes. Nine recurring axes (classification, wage-hour, paid leave, non-competes, pay transparency, Fair Chance, protected-category expansion, biometrics, arbitration) organise the variance.
- California is the strictest and most-consequential — ABC test, daily overtime, meal-and-rest, salary-basis, expense reimbursement under § 2802, CFRA and PDL, non-compete void under § 16600, FEHA protected-category breadth, PAGA. Any California workforce requires California-side compliance workstreams.
- New York adds statewide and NYC layers. Weekly-pay under NY Lab. Law § 191, PFL, statewide and NYC salary-transparency and Fair Chance, NYCHRL protected-category breadth, and a growing set of proto-non-compete statutes.
- Illinois adds an ABC-test workstream, aggressive pay-transparency and Freedom-to-Work restrictions, and — critically — BIPA, whose per-violation damages structure demands a specific compliance workstream for any Illinois biometric touchpoint.
- Washington adds paid family and medical leave, an aggressive salary-transparency statute (RCW 49.58), and RCW 49.62 non-compete restrictions.
- Colorado adds FAMLI, the Equal Pay for Equal Work Act with promotion-opportunity disclosure, and the first state-level AI Act with employment-decision scope (SB 24-205).
- The highest-common-denominator vs. per-state operating-policy decision is a real trade-off — most modern startups operate a hybrid, with national-baseline elements where the national policy is cheap and per-state variants where state-specific compliance is materially different.
- State law changes constantly. A quarterly refresh cadence, a state-law tracker, a new-hire compliance trigger, and multistate outside counsel are the maintenance discipline.
