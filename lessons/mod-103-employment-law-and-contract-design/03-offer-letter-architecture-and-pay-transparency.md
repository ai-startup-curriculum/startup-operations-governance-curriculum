# 3. Offer letters and pay transparency

> The offer letter is the smallest, most-read employment document the corporation ever writes. Get its architecture wrong and every subsequent employment issue is harder to litigate, defend, and unwind.

## Motivation

The offer letter is the first document a new hire signs — often the only one they read carefully. It sets the at-will framing, the compensation package, the reporting line, the start date, the pre-start contingent conditions, and (via cross-reference) the PIIA, NDA, arbitration agreement, benefits plan, and employee handbook. A well-architected offer letter is a page and a half of substance plus a page of cross-references and signatures. A poorly-architected offer letter is either a bloated pseudo-employment-contract that unwinds the at-will status the corporation thinks it has, or a napkin note that leaves every material term ambiguous.

This chapter authors the offer letter as a template. It also folds in the state-and-city **pay-transparency** rules that now govern job postings and, in a growing number of jurisdictions, the offer itself. The transparency wave — Colorado (2021), New York (2023), Washington (2023), California (2023), and more since — is one of the fastest-moving areas of US employment law and the one most likely to trip a corporation that hires across state lines.

## What the offer letter must do

A defensible offer letter accomplishes exactly this set of things:

1. **Identify the parties.** Corporation's legal name (the DE C-Corp from [mod-101](../mod-101-legal-entity-formation-and-corporate-structure/)) and the employee's full legal name.
2. **Position and reporting line.** Title, functional area, and the position the employee reports to (by title, not by named individual — a "reports to the VP of Engineering" line survives the departure of the current VP of Engineering).
3. **Start date.** A specific calendar date. If the start date is contingent on background check or work authorisation, state that.
4. **Employment status.** Full-time / part-time; W-2 employee; FLSA exempt or non-exempt (this is the [chapter 02](./02-flsa-exempt-vs-non-exempt.md) call, and it lives on the offer letter).
5. **Compensation.** Base cash compensation (annualised and per-pay-period expressed if useful); bonus structure if any; equity grant (see below); benefits eligibility summary.
6. **Pay-transparency-compliant salary-range disclosure** in the states and cities that require it (see the section below).
7. **At-will employment.** A clear statement that employment is at-will, terminable by either party at any time with or without cause and with or without notice — subject to the Montana carveout for Montana-based employees.
8. **Cross-references to standalone agreements.** The PIIA, the mutual arbitration and class-action-waiver agreement (if the corporation uses one — [chapter 09](./09-arbitration-and-class-action-waivers.md)), a relocation-assistance agreement (if applicable), a sign-on-bonus repayment agreement (if applicable), and the employee handbook (with a note that the handbook does not create a contract).
9. **Contingent conditions.** Employment is contingent on satisfactory completion of a background check, verification of work authorisation (Form I-9) within the statutory window, and any reference checks not yet completed.
10. **Governing law and dispute resolution.** Which state's law governs; which venue; if arbitration is required, which agreement controls.
11. **Integration and modification clauses.** Employment terms may be modified only by a signed writing from an authorised officer of the corporation.
12. **Signature blocks.** The corporation (by an authorised officer per DGCL § 142) and the employee. Countersignature returns the executed offer letter to the corporation.

Everything else is either handbook policy, standalone-agreement material, or noise.

## The at-will framing and the Montana carve-out

**At-will employment** is the default in every US state except Montana. It means either party can terminate the employment relationship at any time, for any reason (or no reason) that is not otherwise unlawful — no cause required, no notice required, no severance owed by operation of law.

The offer letter must state at-will status explicitly, in a form that a court reviewing an implied-contract wrongful-termination claim will read as an unambiguous disclaimer. The typical formulation:

> Your employment with the Company is at-will, which means that either you or the Company may terminate the employment relationship at any time, for any reason or for no reason, with or without cause and with or without notice. This offer letter is not a contract of employment for any specific duration, and nothing in this letter or in any other document, communication, or representation should be construed as guaranteeing employment for any specific period.

**Montana.** Montana's Wrongful Discharge from Employment Act (Mont. Code Ann. § 39-2-901 et seq.) rejects the at-will default. After a probationary period (default 12 months if not otherwise set by the employer), termination requires good cause. The Montana version of the offer letter substitutes an appropriate probationary-period clause and either accepts the good-cause requirement or declines to hire in Montana.

**States with heightened implied-contract or public-policy exposure.** All at-will states recognise some limits: no termination in violation of an express employment contract, no termination in violation of statute (Title VII, ADA, ADEA, FMLA, whistleblower protection), no termination in violation of public policy (varies state to state). Some states also recognise an implied-in-fact contract based on employer-handbook language, oral representations by managers, or long duration of employment. The offer letter's at-will language is the corporation's primary defence against implied-contract claims; the handbook must not undermine it (a handbook that promises "progressive discipline before termination" without disclaiming that the promise creates a contract is a common source of implied-contract exposure — the handbook must include an explicit at-will disclaimer of its own).

**Language to avoid in the offer letter and in supplementary communications.**

- **"Annual salary of $X"** — read literally, invites an argument that the employment guaranteed at least a year. Prefer **"initial base salary of $X on an annualised basis"** or **"weekly / bi-weekly salary of $Y (equivalent to $X annually)"**.
- **"Permanent position"** — invites an implied-contract argument. Prefer **"regular full-time position."**
- **"You will always..."** — never.
- **"Guaranteed bonus"** — a bonus can be discretionary or targeted, but a "guaranteed" bonus loses discretionary status.
- **"You will only be terminated for cause"** — negates at-will.
- **"Long-term commitment," "career opportunity," "as long as you perform"** — implied-contract flags.

Managers should be trained to avoid these phrases in recruitment conversations. Recruiters who make oral promises that contradict the offer letter can create statements-of-a-party-opponent risk.

## Compensation section: cash, equity, benefits, one page

A one-page framing that most engineers, PMs, and operators can read at a glance:

- **Base cash compensation.** Annualised amount. Pay frequency (typically bi-weekly or semi-monthly). Exempt / non-exempt.
- **Sign-on bonus (if any).** Amount, payment timing, repayment obligation if the employee resigns or is terminated for cause within a defined window (usually 12 months, prorated). Cross-reference a standalone sign-on-bonus repayment agreement if the amount is meaningful.
- **Target performance bonus (if any).** Percent of base or fixed amount; performance criteria (with a cross-reference to a bonus-plan document); discretionary vs. formulaic; payment timing.
- **Commission (for sales roles).** Reference the commission plan document; note that the commission plan may be updated from time to time by the corporation.
- **Equity grant.** Number of stock options or restricted stock units, subject to board approval and issuance under the corporation's equity incentive plan. Vesting schedule (typical: 4-year vest, 1-year cliff, monthly thereafter). Exercise price / grant date = fair market value at the date of grant per the corporation's most-recent 409A valuation, subject to board approval. Cross-reference the stock option agreement or RSU agreement that will govern the grant. Note that the offer letter is not itself the grant; the grant is made by board consent under the plan ([mod-105](../mod-105-equity-compensation-policy-and-comp-committee/) has depth).
- **Benefits eligibility.** Standard summary — health / dental / vision (effective the first of the month following start date, or the equivalent as the plan specifies); 401(k) with any match or safe-harbor terms; FSA / HSA if offered; commuter benefits if offered; other. Cross-reference the benefits guide / SPD (Summary Plan Description) as the governing document.
- **Paid time off.** Vacation policy (accrued or flexible); sick leave (state-specific); holidays (calendar reference); parental leave (with cross-reference to the policy).
- **Expense reimbursement.** Reference the corporation's expense-reimbursement policy.
- **Relocation assistance (if applicable).** Reference a standalone relocation-assistance agreement.

The one-page compensation framing is a substantive commitment, not a summary. A discrepancy between what the offer letter says and what payroll actually pays is a labour-code violation in every state.

## Pay-transparency compliance

The state-and-city pay-transparency wave started in Colorado in 2021 and has expanded rapidly. As of the writing of this chapter, the operative statutes include:

- **Colorado — Equal Pay for Equal Work Act** (C.R.S. § 8-5-201 et seq., amended by the 2024 Ensure Equal Pay for Equal Work Act). Job postings must include the compensation range (hourly or salary), a general description of any bonuses / commissions / other compensation, and a general description of employment benefits. Applies to any position that can be performed in Colorado, including remote work. Colorado also requires internal-notice of promotional opportunities and disclosure of the salary of an internally-filled position after the hire.
- **New York — Labor Law § 194-b.** Job postings must include the range of compensation. Applies to jobs performed in New York (including remote work supervised from or performed at least in part in New York) at employers with four or more employees. The range must be a good-faith range the employer intends to offer.
- **Washington — RCW 49.58.110.** Job postings must include the wage scale or salary range and a general description of all benefits and other compensation. Applies to employers with 15 or more employees.
- **California — Cal. Labor Code § 432.3.** Requires employers with 15 or more employees to include the pay scale in job postings for positions that may be filled in California (including remote). Requires disclosure of the pay scale for a position to a current employee upon request, and imposes pay-data reporting to the Civil Rights Department for employers with 100 or more employees.
- **Illinois — 820 ILCS 112/10 (as amended by the 2024 Pay Transparency Act).** Effective January 1, 2025, employers with 15 or more employees must include the pay scale and benefits in job postings for positions physically performed at least in part in Illinois, or for positions the employee will report to a supervisor in Illinois.
- **Massachusetts — An Act Relative to Salary Range Transparency** (2024). Effective July 2025 for pay-range disclosure in job postings; effective 2025 for pay-data reporting.
- **Minnesota — Minn. Stat. § 181.173** (2024). Job postings must include a good-faith salary range and a general description of benefits.
- **Vermont, Rhode Island (specific request-based rule), Connecticut (request-based), Nevada (request-based on offer), Maryland (request-based)** and additional states have narrower rules requiring disclosure upon request or in specific circumstances.
- **Cities.** Jersey City, Ithaca (NY), Cincinnati, Toledo, and other cities have their own ordinances. NYC's Local Law 32 is subsumed by NY state Law § 194-b for most purposes.

<!-- needs-research: verify the full current list of state and city pay-transparency statutes, their effective dates, employer-size thresholds, and specific disclosure requirements before publishing a multi-state posting-compliance memo. This area changes materially every legislative session. -->

**Practical implications for the offer letter:**

- **Job postings** — the corporation must include a compensation range on every posting for a position that may be filled in a covered jurisdiction. The range must be in good faith — arbitrarily wide ranges (e.g., $50,000 to $500,000 for a mid-level engineer) can be enforcement targets.
- **Offer letters** — offer letters should reflect a compensation number that is consistent with (typically inside) the range disclosed in the posting. A candidate can compare the posted range to the offered number, and enforcement agencies do too.
- **Internal-transfer and promotion notices** — Colorado specifically requires internal notice of promotional opportunities and disclosure of the successful candidate's salary. Other states have narrower internal-disclosure rules; comply state by state.
- **Pay-data reporting** — Colorado, California, Illinois, and Massachusetts require aggregated pay-data reporting on a defined cadence. This is HR-operations work rather than offer-letter work, but the corporation must architect the reporting capability early.
- **Existing employees' access to the pay scale.** California § 432.3 and Washington RCW require disclosure of the pay scale for an existing employee's position upon request. The corporation should have a defined process for handling such requests without creating discrimination-adjacent conversations.

**The compliance choice: highest common denominator or per-state postings.** For a small remote-first corporation hiring across states, the two operating options are (i) apply the highest-common-denominator rule to every posting (include the compensation range on every job posting for every position, and include benefits) or (ii) tailor each posting by the applicable state's rules. The highest-common-denominator posture is administratively simpler and reduces the risk of a posting that violates a jurisdiction's rule; some corporations resist it because they view the compensation range as competitively sensitive. [Chapter 08](./08-state-law-variance.md) treats the highest-common-denominator vs. per-state decision more generally.

## Contingent conditions: I-9, background check, references

The offer letter conditions the start on satisfactory completion of a defined set of pre-start items:

- **Form I-9 (Employment Eligibility Verification).** 8 U.S.C. § 1324a requires the employer to verify the identity and work authorisation of every new hire within three business days of the start date. The offer letter should state that employment is contingent on the employee's completion of Form I-9 within the statutory window and on the employer's verification of the documents. E-Verify participation, where applicable, is separately disclosed. <!-- needs-research: verify the current I-9 form version and the state-by-state E-Verify participation rules (some states require E-Verify for all employers or for state contractors; federal contractors are subject to FAR E-Verify requirements). -->
- **Background check.** Contingent on satisfactory completion of a criminal-history and reference background check. The background check is governed by the federal **Fair Credit Reporting Act** (15 U.S.C. § 1681 et seq.) — the corporation must (i) provide a stand-alone written disclosure to the candidate that a consumer report will be procured, (ii) obtain the candidate's written authorisation, (iii) provide a pre-adverse-action notice with a copy of the report and the FCRA "Summary of Rights" before taking adverse action based on the report, and (iv) provide an adverse-action notice after the decision is final. State-specific requirements layer on top — California ICRAA (Cal. Civ. Code § 1786), New York, Illinois, and others have additional disclosures or timing requirements.
- **Ban-the-box and Fair Chance rules.** Federal contractors and a growing list of states and cities restrict when in the hiring process a criminal-history inquiry may be made, what convictions may be considered, and what individualised assessment is required before adverse action. California's Fair Chance Act (Cal. Gov. Code § 12952), New York City's Fair Chance Act, and Los Angeles's Fair Chance Initiative are examples. The offer letter should not disclose criminal history; the background-check process handles that with its own separate paperwork. <!-- needs-research: current federal Fair Chance Act coverage (contractor-only or broader), and a state-and-city ban-the-box matrix, before authoring a national background-check policy. -->
- **Drug testing.** Where the corporation drug-tests, contingent on satisfactory drug-test results. Increasingly restricted by state and city law with respect to marijuana (California AB 2188, NYC Local Law 91, New Jersey, and others). <!-- needs-research: current state and city marijuana-testing restrictions before authoring a drug-testing policy. -->
- **Reference checks (if not yet completed).** If references remain to be checked, condition the offer explicitly. Otherwise omit.
- **Return of a signed PIIA, arbitration agreement, and other on-boarding documents.**

Contingent-condition language example:

> This offer is contingent upon: (i) verification of your identity and eligibility to work in the United States, evidenced by your completion of Form I-9 within the statutory time period after your start date; (ii) satisfactory completion of a background check conducted in accordance with applicable law; (iii) your execution of the enclosed Proprietary Information and Inventions Assignment Agreement and Mutual Arbitration Agreement; and (iv) any additional items specified in this letter. If any of these conditions is not satisfied, this offer may be rescinded or your employment may be terminated.

## Cross-referenced standalone agreements

The offer letter references — but does not duplicate — these standalone agreements:

- **The PIIA** ([chapter 04](./04-employee-piia.md)). Signed on start date, before access to code or confidential information.
- **The mutual arbitration and class-action-waiver agreement** ([chapter 09](./09-arbitration-and-class-action-waivers.md)), if the corporation uses one. This is a policy choice. Where used, signed on start date. Some states (California) require specific opt-out or informed-consent formalities; some claim categories are non-arbitrable (sexual harassment and assault under the 2022 Ending Forced Arbitration Act).
- **A sign-on-bonus repayment agreement**, if the sign-on bonus exceeds a threshold that justifies a standalone document.
- **A relocation-assistance agreement**, if the corporation is paying relocation expenses (typically includes a claw-back if the employee resigns within a defined window).
- **The equity grant paperwork** — the stock option agreement or RSU agreement issued after board approval of the grant. The offer letter describes the grant; the agreement legally issues it.
- **The employee handbook**, with a prominent statement (both in the offer letter and in the handbook itself) that the handbook is not a contract and does not modify at-will status.

Each cross-referenced agreement stands on its own and can be updated without amending the offer letter.

## Common drafting failures

- **Guaranteeing the equity grant amount.** The offer letter can describe the target grant, but the grant is not effective until the board approves it under the plan. Language: "We will recommend to the Board of Directors that you be granted an option to purchase X shares of the Company's common stock, subject to the terms of the Company's Equity Incentive Plan and a stock option agreement to be delivered upon Board approval." Avoid absolute language that promises the grant regardless of board action.
- **Promising a specific 409A valuation.** The strike price is fair market value on the grant date; the grant date is the board-approval date. Do not promise a strike price in the offer letter, because the strike price is determined at grant, not at offer.
- **Guaranteeing bonuses that are supposed to be discretionary.** "Guaranteed" wording removes the discretion.
- **Promising future promotions or raises.** Any promise beyond the current package invites implied-contract exposure.
- **Vague severance language.** If severance is offered, be specific: cause / no cause definitions, dollar amount, duration, treatment of unvested equity, treatment of benefits, release requirement (see [mod-107](../mod-107-performance-promotion-and-offboarding/)). If severance is not offered, omit — do not gesture toward it.
- **Mismatching the exempt classification.** The offer letter's "exempt / non-exempt" line must match the actual classification analysis from [chapter 02](./02-flsa-exempt-vs-non-exempt.md). Do not code inside-sales reps as exempt on the offer letter to make the compensation package look more prestigious.
- **Omitting the state-specific required disclosures.** New Hampshire, Rhode Island, and other states have specific offer-letter or notice-of-hire requirements. New York's Wage Theft Prevention Act (N.Y. Labor Law § 195) requires a Notice of Pay and Payday to every new hire; the offer letter can incorporate the required disclosures or the notice can be delivered separately. <!-- needs-research: state-by-state notice-of-hire requirements before finalising a multi-state offer-letter template. -->

## Concrete example: an offer letter for a full-stack engineer in California

Corporation: Acme Robotics, Inc., Delaware C-Corporation, principal place of business San Francisco.
Candidate: Priya Patel, joining as a Full-Stack Software Engineer, based in San Francisco, reporting to the VP of Engineering.

Offer letter (sketched, not full form):

> **May 15, 2026**
>
> **Priya Patel**
> [address]
>
> Dear Priya,
>
> On behalf of Acme Robotics, Inc. (the "Company"), I am pleased to offer you the position of **Software Engineer** on the Engineering team, reporting to the **VP of Engineering**. Your start date will be **June 15, 2026**, and your position will be based in **San Francisco, California**, with a hybrid schedule as specified by the Company's remote-work policy.
>
> **Compensation.**
> - **Base salary:** $200,000 on an annualised basis, paid on the Company's regular bi-weekly payroll schedule (equivalent to approximately $7,692.31 per bi-weekly pay period). You are classified as an **exempt** employee under the FLSA and California Labor Code § 515.5 (computer professional).
> - **Sign-on bonus:** $10,000, payable on your first regular payday, subject to the enclosed Sign-On Bonus Agreement (which provides for repayment if you resign or are terminated for cause within 12 months).
> - **Equity grant:** We will recommend to the Board of Directors that you be granted an option to purchase **20,000 shares** of the Company's common stock, at an exercise price equal to the fair market value on the date of grant as determined by the Board in accordance with the Company's most-recent Section 409A valuation. The grant will vest 25% on the first anniversary of your start date and monthly thereafter over the following 36 months, subject to your continued service and to the terms of the Company's 2024 Equity Incentive Plan and the applicable stock option agreement.
> - **Benefits:** You will be eligible for the Company's standard benefits program, including medical, dental, and vision coverage effective the first of the month following your start date; participation in the Company's 401(k) plan; and paid time off in accordance with the Company's PTO policy.
>
> **Pay range.** The pay range for this position in California is **$180,000 – $240,000** annualised, plus the equity grant, sign-on bonus, and benefits described above. The specific amount offered reflects our assessment of your experience and qualifications.
>
> **At-will employment.** Your employment with the Company is at-will, which means that either you or the Company may terminate the employment relationship at any time, for any reason or for no reason, with or without cause and with or without notice. Nothing in this letter should be construed as guaranteeing employment for any specific period.
>
> **Standalone agreements.** As a condition of employment, you will be required to sign the enclosed **Proprietary Information and Inventions Assignment Agreement** (the "PIIA") and **Mutual Arbitration Agreement** (the "Arbitration Agreement"), each on or before your start date.
>
> **Contingent conditions.** This offer is contingent upon (i) verification of your identity and eligibility to work in the United States pursuant to Form I-9 within the statutory time period; (ii) satisfactory completion of a background check conducted in accordance with applicable law; and (iii) execution of the PIIA and Arbitration Agreement.
>
> **Governing law.** This offer letter is governed by the laws of the State of California. Any disputes are subject to the terms of the Arbitration Agreement.
>
> **Integration.** This letter, together with the PIIA, the Arbitration Agreement, the Sign-On Bonus Agreement, and the equity documents when issued, sets forth our entire offer. Any modification must be in a signed writing from an authorised officer of the Company.
>
> Please indicate your acceptance by countersigning below and returning a copy to me by **May 22, 2026**.
>
> Welcome to Acme.
>
> [Signature block for CEO or authorised officer]
> [Countersignature block for Priya Patel with acceptance date]

The offer letter is about a page and a half. The PIIA, arbitration agreement, sign-on bonus agreement, and equity plan documents run separately.

## Ancillary hires: contractors, interns, advisors, part-time

The offer letter template is for W-2 employees. Adjacent hire types get analogous but different documents:

- **Contractors.** Independent Contractor Agreement — Statement of Work — no "at-will," no benefits references, IP assignment via mutual work-for-hire + assignment backstop, per-project scope and payment terms. Cross-reference to a mutual NDA if confidential information is exchanged.
- **Interns.** Intern offer letter, but note the DOL "primary beneficiary" test (Fact Sheet #71) for whether the intern must be paid. For-profit corporations should generally pay interns as W-2 non-exempt employees; unpaid internships at for-profit corporations are legally fragile under the seven-factor primary-beneficiary test.
- **Advisors (technical, business, or industry).** Advisor Agreement — typically the FAST (Founder / Advisor Standard Template) form or a similar model — describes scope of advice, term, equity or cash compensation, and confidentiality. Not an employment agreement; not a contractor engagement in the § 530 or ABC sense (usually).
- **Board directors.** Director offer letter or director appointment package (see [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/)) — director compensation, indemnification, D&O coverage, expected time commitment, conflict-of-interest disclosure.
- **Part-time employees.** Same offer-letter template with the "part-time" flag; hours-per-week disclosed; benefits eligibility may differ per plan terms; FLSA and state wage-and-hour analysis identical.

## Summary

- The offer letter is a short, structured document that identifies the parties, states the position and reporting line, sets the start date, states the compensation (cash, equity, benefits) at a one-page-legible level, states FLSA exempt / non-exempt status, states at-will (with the Montana carveout), cross-references standalone agreements (PIIA, arbitration, sign-on, relocation, equity, handbook), enumerates contingent conditions (I-9, background check, references), and closes with governing law and integration language.
- The at-will language must be unambiguous. Managers and recruiters must be trained to avoid implied-contract phrasing in written and oral communications.
- Pay-transparency compliance is state-specific and moving fast: Colorado, New York, Washington, California, Illinois, Massachusetts, Minnesota, and additional states require compensation-range disclosure on job postings; several require internal disclosures on request and pay-data reporting to state agencies. The highest-common-denominator posting posture is administratively simpler than per-state variance for a small remote-first corporation.
- The compensation section describes the *equity grant* rather than legally issuing it; the grant is made by board consent under the equity incentive plan, at a strike price equal to the 409A fair market value on the grant date. Do not promise a strike price in the offer letter.
- Contingent conditions must be enforced. Form I-9 is federally required within three business days. Background checks are governed by FCRA and its state analogues; ban-the-box and Fair Chance rules restrict when and how criminal history may be considered.
- Standalone agreements — PIIA, arbitration, sign-on repayment, relocation, equity documents — are cross-referenced from the offer letter, signed separately, and archived alongside it in the employee's personnel file.
- Common drafting failures: guaranteeing the equity grant or the 409A strike price, guaranteeing discretionary bonuses, promising future promotions or raises, vague or generous severance gestures, mismatching the exempt classification, and omitting state-specific notice-of-hire disclosures.
