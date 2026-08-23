# 2. FLSA exempt vs. non-exempt

> Salary alone does not make an employee exempt. A "salaried" engineer who fails the duties test is a non-exempt employee whose unpaid overtime — plus liquidated damages, plus attorneys' fees — is the corporation's problem.

## Motivation

Once a worker is classified as a W-2 employee ([chapter 01](./01-w2-vs-1099-worker-classification.md)), the next classification question is whether they are **exempt** from the Fair Labor Standards Act's minimum-wage and overtime requirements — or **non-exempt** and therefore entitled to overtime pay at 1.5× the regular rate for all hours worked over 40 in a workweek (and, in California and a few other states, additional daily-overtime rules).

The mistake pattern is a familiar one at startups: pay everyone a "salary," assume "salary" means "exempt," don't track hours, don't pay overtime, and discover eighteen months later that the DevOps engineer, the two customer-success reps, the office manager, and the three inside-sales reps were all misclassified as exempt. The DOL FLSA collective action, the state wage-and-hour class action, or the individual Labor Commissioner claim then produces two years of back overtime (three years if wilful) plus 100% liquidated damages plus attorneys' fees plus, in California, meal-and-rest-period premium pay, wage-statement penalties, and PAGA representative-action penalties on top.

FLSA exempt status is a **two-part test.** Both parts must be satisfied. Failing either part means the employee is non-exempt regardless of what the offer letter says or what the payroll system codes them as.

## Part 1 — the salary basis test

An exempt employee must be paid on a **salary basis** at or above a defined weekly threshold. Being paid on a salary basis means:

- **A predetermined amount** each pay period, not calculated on hours worked.
- **Not subject to reduction** because of variations in the quality or quantity of work performed.
- **Paid the full salary** in any workweek in which the employee performs any work — subject to a narrow set of permissible deductions specified in **29 C.F.R. § 541.602**.

Permissible deductions include: full-day absences for personal reasons (other than sickness or disability); full-day absences for sickness or disability if pursuant to a bona fide plan of paid sick leave; unpaid disciplinary suspensions of one or more full days imposed in good faith for infractions of workplace-conduct rules; the first or last week of employment (proration allowed); unpaid leave under the Family and Medical Leave Act; and offset against jury/witness/military pay.

**Impermissible deductions** — deductions that break the salary basis, and, if a "pattern or practice" of impermissible deductions is found, cost the employee (and the entire job classification and workplace) the exempt status — include: deductions for partial-day absences; deductions for time when work is unavailable and the employee is ready to work; deductions for the quality or quantity of work; docking pay when the employee leaves early; and deductions for the corporation's operating losses.

The **weekly threshold** is where the DOL rulemaking of the last few years matters. As of the writing of this chapter:

- **The DOL's 2024 final rule** raised the federal salary threshold in two phases: to $844/week ($43,888/year) effective July 1, 2024, and to $1,128/week ($58,656/year) effective January 1, 2025, with subsequent inflation-indexed adjustments every three years. It also raised the "highly-compensated employee" annual threshold to $132,964 on July 1, 2024, and to $151,164 on January 1, 2025.
- **Litigation status.** The 2024 rule has been challenged in several federal courts. Portions have been vacated in some jurisdictions and remain contested. <!-- needs-research: verify the current operative federal salary-basis threshold and the highly-compensated-employee threshold as of the date you author a specific memo; the DOL's regulatory posture and the litigation outcome may have changed. -->
- **State thresholds are higher in some states.** California requires exempt executive, administrative, and professional employees to be paid at least twice the state minimum wage for full-time employment — a figure that, at the current state minimum wage, is materially higher than the federal $58,656. Washington and New York City also have thresholds above the federal floor. Colorado and Alaska have specific state rules. <!-- needs-research: current-year state salary thresholds for California, New York (including NYC/Nassau/Suffolk/Westchester differential), Washington, Colorado, and Alaska. -->

An employee paid below the applicable salary threshold — federal or state, whichever is higher — is **non-exempt regardless of duties**, and is entitled to overtime pay. Full stop.

## Part 2 — the duties tests

Above the salary threshold, exempt status also requires that the employee's *primary duty* fits one of the five statutorily-defined exemptions. "Primary duty" means the principal, main, major, or most important duty the employee performs (29 C.F.R. § 541.700), evaluated as a totality of the circumstances. It is not a strict percentage-of-time rule, though time spent on exempt-qualifying work is a relevant factor.

### The executive exemption (29 C.F.R. § 541.100)

Primary duty is management of the enterprise, or a customarily recognised department or subdivision. The employee must:

- Customarily and regularly direct the work of two or more other full-time employees (or the equivalent).
- Have the authority to hire or fire other employees, or the employee's suggestions and recommendations as to hiring, firing, advancement, promotion, or other status change of other employees are given particular weight.

At a startup this covers the CEO, CTO, VPs of engineering / product / sales / marketing / operations, and department heads who have real management responsibility for two or more direct reports. It does *not* cover a "lead engineer" whose title implies management but whose actual duty is individual-contributor engineering work.

### The administrative exemption (29 C.F.R. § 541.200)

Primary duty is the performance of office or non-manual work directly related to the management or general business operations of the employer or the employer's customers, *and* the primary duty includes the exercise of discretion and independent judgment with respect to matters of significance.

This is the most-litigated and most-abused exemption. The requirements matter:

- **"Directly related to management or general business operations"** — the work must be in a functional area that supports the running of the business, not the production of the corporation's product. Examples the DOL identifies: HR, employee benefits, labour relations, PR, government relations, computer network / database administration, legal and regulatory compliance, procurement, quality control, safety and health, research (as opposed to production), tax, finance, accounting, budgeting, auditing, insurance, marketing, and similar activities.
- **"Discretion and independent judgment"** — the employee must have the authority to make an independent choice among possibilities, free from immediate direction or supervision, on matters of consequence. Following detailed procedures is not discretion. Applying skill in performing well-established techniques is not discretion. The bar is meaningful.
- **"Matters of significance"** — the decisions the employee makes must have consequence to the business. The DOL cites examples: making decisions that affect the business's operations; formulating, interpreting, or implementing management policies; carrying out major assignments; committing the employer in matters that have significant financial impact; waiving or deviating from established policies without specific authorisation.

Positions that *frequently qualify* at a startup include: senior finance and accounting roles (controller, senior FP&A), senior HR roles (HR business partner, head of HR at a small company), senior marketing roles (marketing manager, brand strategist), and senior operations roles.

Positions that *frequently do not qualify* despite being "salaried" and holding a manager-adjacent title:

- **Customer success reps** — typically execute defined playbooks for account management; discretion is limited.
- **Inside-sales reps** — the "sales" exemptions (outside sales below) are strict; inside sales is generally non-exempt.
- **Recruiters (non-managerial)** — execute a defined recruiting workflow; discretion is limited.
- **Office managers and executive assistants** — support functions; discretion is typically limited to scheduling and administrative logistics.
- **Junior marketing, junior finance, and junior operations roles** — execute assigned work; do not exercise discretion on matters of significance.
- **Content writers, editors, and social-media coordinators** — creative or communications work often does not meet the "discretion on matters of significance" test.

The single most common misclassification at a Series-A-through-Series-B company is treating customer-success reps and inside-sales reps as exempt "salaried" employees.

### The professional exemption — learned and creative (29 C.F.R. § 541.300–541.303)

Two sub-types:

- **Learned professional.** Primary duty is work requiring advanced knowledge in a field of science or learning, customarily acquired by a prolonged course of specialised intellectual instruction (a bachelor's or higher degree in a relevant field, or equivalent). The DOL identifies fields including law, medicine, theology, accounting, actuarial computation, engineering (architects and engineers with recognised professional certifications), teaching (in a school system or accredited institution), and various scientific specialities. The requirement is *advanced knowledge* and *specialised academic training* — not just a college degree.
- **Creative professional.** Primary duty is work requiring invention, imagination, originality, or talent in a recognised field of artistic or creative endeavour. Journalism, music composition, writing (some categories), acting, and visual arts qualify. Standard journalism and content-marketing work does *not* automatically qualify; the DOL requires genuine originality and creativity.

Software engineering *may* qualify under the learned-professional exemption in principle, but the DOL and courts have historically preferred to analyse software engineers under the **computer-employee exemption** (below), which has its own specific requirements. Do not assume that every engineer with a CS degree qualifies as a learned professional.

### The computer-employee exemption (29 C.F.R. § 541.400)

Applies to computer systems analysts, computer programmers, software engineers, and other similarly-skilled workers in the computer field whose primary duty is:

- Application of systems-analysis techniques and procedures, including consulting with users, to determine hardware, software, or system functional specifications; *or*
- Design, development, documentation, analysis, creation, testing, or modification of computer systems or programs, including prototypes, based on and related to user or system design specifications; *or*
- Design, documentation, testing, creation, or modification of computer programs related to machine operating systems; *or*
- A combination of the above requiring the same level of skill.

The exemption **does not** apply to employees engaged in the manufacture or repair of computer hardware and related equipment, or to employees whose work is highly dependent upon computers or computer software (e.g., engineers, drafters, or others whose work products are dependent on a computer, but who are not primarily engaged in computer-systems analysis and programming).

**Compensation floor for the computer-employee exemption** — 29 C.F.R. § 541.400(b) allows salary basis at the § 541.600 threshold *or* hourly pay at not less than **$27.63/hour**. This is the one place the FLSA permits hourly pay to satisfy the compensation prong of an exemption.

**Practical implications for startup engineers:**

- A senior backend engineer who designs, develops, and modifies computer programs based on product specifications and who is paid a salary above the federal threshold is exempt under the computer-employee exemption.
- A junior "software engineer" whose actual work is largely QA test execution or click-through testing of a UI — without design, development, or modification of programs — may not satisfy the primary-duty test.
- A DevOps engineer whose primary duty is systems administration (maintaining production systems, running deployments, responding to alerts) may fall outside the computer-employee exemption, which is about *design and programming*, not operations. The DOL has taken a narrow view of computer-employee-exemption coverage for pure system-administration roles. Analyse carefully.
- A data analyst whose primary duty is executing queries and building dashboards from defined specifications may not qualify. A data scientist who designs and modifies machine-learning systems more plausibly does.
- **Support engineers, IT-helpdesk staff, and technicians** are generally non-exempt regardless of the "engineer" title.

### The outside-sales exemption (29 C.F.R. § 541.500)

Primary duty is making sales or obtaining orders or contracts for services or use of facilities, *and* the employee is customarily and regularly engaged **away from the employer's place of business** in performing this primary duty.

The "away from the place of business" requirement is dispositive. **Inside-sales reps who work from the corporation's office or from their home office (calling / emailing customers from that base) are not "outside sales" employees** — they may satisfy the retail-and-service commissioned-employee exemption under 29 U.S.C. § 207(i) in specific configurations, or they may simply be non-exempt.

A B2B account executive who spends 60% of their time on-site with customers and prospects is a plausible outside-sales candidate. A B2B account executive who spends 90% of their time on Zoom calls from home is not.

### The highly-compensated-employee exemption (29 C.F.R. § 541.601)

A short-cut for employees who make above the highly-compensated-employee threshold (currently $151,164/year federal per the 2024 rule, subject to litigation; state thresholds may be higher) and who customarily and regularly perform at least one of the duties of an executive, administrative, or professional exempt employee. The salary threshold is high, and one duty from any of the three primary exemptions suffices. Useful for senior individual contributors who almost — but not quite — hit the full duties test of one exemption.

## The California variations that matter

California's Industrial Welfare Commission wage orders and Labor Code impose additional and different rules that the federal FLSA does not:

- **Daily overtime.** In California, non-exempt employees are entitled to overtime at 1.5× for hours worked over 8 in a day, and double-time for hours worked over 12 in a day (Cal. Labor Code § 510). A workday that runs 9 hours triggers overtime under California law even if the workweek stays at 40 hours.
- **Seventh-consecutive-day overtime.** 1.5× for the first 8 hours on the seventh consecutive day of work in a workweek, and double-time thereafter.
- **Salary threshold for the executive, administrative, professional exemptions.** Twice the state minimum wage on a full-time basis. At the current state minimum wage, this is above the federal $58,656 threshold and requires an update every time the minimum wage moves. <!-- needs-research: current California state exempt-salary threshold based on the operative state minimum wage. -->
- **Meal and rest periods.** Cal. Labor Code § 512, § 226.7, and IWC Wage Order § 11 require a 30-minute unpaid meal period before the fifth hour of work and a 10-minute paid rest period per four hours worked (or major fraction). Failure to provide either results in a premium payment of one hour's pay per workday for each type of missed break (up to two hours per day). Class actions and PAGA representative actions built on meal-and-rest-period violations dwarf the underlying overtime exposure in many cases.
- **Waiting-time penalties.** Cal. Labor Code § 203 — if the corporation fails to pay all wages due at termination, the employee's wages continue as a penalty at the daily rate for up to 30 days.
- **Wage-statement penalties.** Cal. Labor Code § 226 — every itemised wage statement must include specific information; each defective statement is a per-employee penalty capped at $4,000 per employee, plus PAGA representative-action penalties on top.
- **Duties-test formulation** — California uses a "more than 50% of time on exempt work" quantitative rule for the executive, administrative, and professional exemptions, which is stricter than the federal "primary duty" totality test. An employee who spends 45% of their time on exempt work and 55% on non-exempt work is non-exempt under California law even if their "primary duty" is technically the exempt work.
- **Computer-employee exemption.** California has a separate statutory computer-professional exemption at Cal. Labor Code § 515.5 with its own compensation threshold that is updated annually and its own duties test (broadly similar to the federal, with California-specific tweaks). <!-- needs-research: current California computer-professional exemption compensation threshold under Cal. Labor Code § 515.5 as set by the Department of Industrial Relations. -->

## The misclassification-exposure math

Assume a startup that pays an inside-sales rep a $75,000 annual "salary," treats them as exempt, and doesn't track hours. The rep actually works 50 hours per week. Two years later, the rep files a complaint alleging misclassification.

- **Regular hourly rate.** $75,000 / (52 weeks × 40 hours) = $36.06/hour.
- **Overtime rate.** $36.06 × 1.5 = $54.09/hour.
- **Weekly overtime hours.** 10 (50 worked − 40 threshold).
- **Weekly overtime pay owed.** 10 × $54.09 = $540.90.
- **Annual overtime pay owed.** $540.90 × 52 = $28,127.
- **Two-year back overtime.** $56,254.
- **Liquidated damages** (equal amount under 29 U.S.C. § 216(b)). $56,254.
- **Attorneys' fees** (mandatory to prevailing plaintiff under 29 U.S.C. § 216(b)). Often exceed the underlying damages in litigated cases.
- **State overtime** — if in California, add daily-overtime for any day worked over 8 hours, meal/rest-period premiums, and waiting-time and wage-statement penalties.
- **PAGA representative penalties in California** — additional civil penalties on a per-pay-period basis for each Labor Code violation, aggregated across all similarly-situated aggrieved employees.

For one misclassified inside-sales rep in California working 50 hours a week for two years, all-in exposure — before attorneys' fees — commonly clears $150,000. Times ten reps.

## Practical implications for startup roles

A working baseline classification for common startup roles, subject to the case-by-case duties-test analysis:

- **CEO, CTO, VPs with direct reports** — exempt executive.
- **Senior backend / frontend / infra engineers** — typically exempt computer-employee (subject to duties analysis and salary threshold).
- **Junior engineers / associate engineers / new-grad engineers** — analyse carefully. Salary must clear the threshold; duties must include design or development of programs (not just QA execution or click-testing).
- **DevOps / SRE** — analyse carefully. Pure operations work may not satisfy the computer-employee exemption; may qualify as administrative if the role involves genuinely-discretionary decision-making about infrastructure architecture and reliability programs.
- **Data scientists / ML engineers** — typically exempt (learned professional or computer employee, depending on the role's specific facts).
- **Data analysts / BI analysts** — analyse carefully. Executing defined queries may not meet the exemption; building analytical frameworks may.
- **Product managers** — typically exempt administrative (product management directly relates to general business operations; discretion is meaningful).
- **Designers (product, UX, UI, brand)** — analyse carefully. Creative-professional exemption may apply for genuinely original creative work; more routine visual-design work may not.
- **Marketing managers, growth managers** — typically exempt administrative.
- **Content writers, social-media coordinators, community managers** — often non-exempt.
- **Recruiters (individual contributor)** — often non-exempt. Head of Talent / VP of People — exempt if managerial.
- **Customer-success managers (individual contributor)** — often non-exempt despite the "manager" title.
- **Sales development reps (SDRs), business development reps (BDRs), account executives working inside sales** — non-exempt as a default. Analyse retail-and-service commissioned-employee exemption in specific configurations.
- **Field-sales / outside-sales account executives** — potentially exempt outside-sales if the "customarily and regularly away from the place of business" test is met.
- **Office managers, executive assistants** — non-exempt as a default.
- **Support engineers, IT helpdesk, technicians** — non-exempt.
- **Finance / accounting individual contributors** (senior FP&A, controller, senior accountant) — typically exempt administrative. Junior AP/AR clerks — non-exempt.
- **HR business partners, senior HR generalists** — typically exempt administrative. HR coordinators — analyse carefully.

The rule of thumb: when in doubt, classify as non-exempt, pay overtime, and track hours. Non-exempt classification is easy to administer once the corporation has a functioning time-tracking system, and it eliminates the misclassification exposure. Exempt classification is the risk category.

## The operational plumbing: what a compliant program looks like

Correct classification is only half the job. The corporation must also:

- **Track hours worked for non-exempt employees.** A time-tracking system (integrated with the payroll platform — Gusto, Rippling, Justworks, Deel, ADP) that captures start, stop, and meal-break times. Voluntary "salaried non-exempt" workers still need hours tracked; a non-exempt "salary" is a device for smoothing pay across pay periods, not an escape from hour-tracking.
- **Pay all hours worked, including "off-the-clock" work.** Non-exempt employees who check email, take after-hours calls, work on documents at home, or attend voluntary training must be paid for that time. Corporate policies that "prohibit" off-the-clock work but tacitly encourage it are FLSA-liability generators.
- **Pay overtime automatically for hours over 40 (and, in California, over 8 in a day).** Do not require the employee to request overtime; the FLSA does not permit that structure.
- **Maintain records** as required by 29 C.F.R. Part 516 — personal information, hours worked each day and week, wage rate, overtime pay, additions to and deductions from wages, total wages per pay period, dates of payment and pay period covered. Records must be retained for at least three years.
- **Issue compliant wage statements** — federal has a light itemisation requirement; California, New York, and several other states require detailed itemised statements with specific fields. In California a defective wage statement is a per-pay-period penalty per employee.
- **Post the required workplace notices** — federal (FLSA, EEOC, OSHA, FMLA where applicable), state (California DIR wage-order posters, etc.), and city (San Francisco, LA, NYC and other city-specific posters). At a remote-first company, the DOL's guidance allows electronic posting where all employees "customarily receive information from the employer" electronically. <!-- needs-research: confirm current DOL and state guidance on electronic workplace-notice posting for remote workforces before advising a fully-remote corporation on posting compliance. -->

## Concrete example: three "salaried" hires, three classifications

- **Backend engineer, $175,000 salary, San Francisco.** Salary clears the California and federal thresholds. Primary duty is designing and developing programs from product specs. Classification: **exempt** under the computer-employee exemption. No hour-tracking required. Overtime not owed.
- **Customer-success rep, $75,000 salary, Chicago.** Salary clears the federal $58,656 threshold. Primary duty is executing account-management playbooks (following defined procedures to renew customers, handle escalations, and drive adoption metrics). Discretion is limited. Classification: **non-exempt**. Must track hours. Overtime owed for hours over 40 in a workweek. Note: even though the offer letter said "salaried, exempt," the offer letter is not dispositive. Payroll system codes the employee as non-exempt; time-tracking begins day one.
- **Inside-sales rep, $60,000 base plus commission, Los Angeles.** Base salary is below California's exempt-salary threshold (which is above the federal $58,656 by a meaningful margin at the current California minimum wage). Even if base cleared the threshold, the employee is inside-sales, not outside-sales, so the outside-sales exemption does not apply. The retail-and-service commissioned-employee exemption at 29 U.S.C. § 207(i) has narrow requirements the corporation likely does not meet. Classification: **non-exempt**. Must track hours. Overtime owed for hours over 40 in a workweek, over 8 in a day, and on the seventh consecutive workday. Meal-and-rest-period compliance required. California-specific wage statements required.

## The retroactive-cleanup pattern

A common inheritance for an incoming HR / GC / COO: an employee-population spreadsheet where every role is coded "exempt" and no one is tracking hours. The cleanup playbook:

1. **Audit the population.** Categorise every current employee against the salary-basis test (part 1) and the duties tests (part 2), state by state.
2. **Reclassify prospectively.** For any employee who is currently misclassified as exempt, reclassify to non-exempt effective a specific date; begin hour tracking; brief the manager and the employee on the change and why (avoid framing that suggests the reclassification is a demotion — it isn't).
3. **Address the back-liability question with counsel.** Options range from "do nothing and hope no one files" (imprudent), to a self-audit under FLSA § 216(c) with DOL supervision, to a voluntary back-pay computation and offer to the affected employees, to a full VCSP-style disclosure. The right answer depends on how many workers, how much back exposure, how likely a whistleblower complaint is, and how it will be perceived at Series-A diligence.
4. **Update the offer-letter and handbook templates.** New hires get the correct classification from day one. The offer-letter template ([chapter 03](./03-offer-letter-architecture-and-pay-transparency.md)) has an explicit "exempt / non-exempt" field.
5. **Update the payroll system.** Employee records reflect the correct classification; overtime calculations enabled for non-exempt employees; time-tracking integrated.
6. **Update the compliance calendar.** State minimum wages, salary thresholds, and wage-statement rules update annually. The calendar tracks each state's effective date.

## Summary

- FLSA exempt status is a two-part test. **Part 1 — salary basis:** employee must be paid a predetermined salary above the applicable threshold (federal $58,656/year per the 2024 rule, subject to litigation; higher in California, Washington, New York, and other states), with only permissible deductions. **Part 2 — duties:** primary duty must fit one of the five statutorily-defined exemptions (executive, administrative, professional, computer employee, outside sales), or the highly-compensated-employee short-cut.
- The administrative exemption is the most-misused. "Discretion and independent judgment on matters of significance" is a meaningful bar; executing defined playbooks does not meet it.
- The computer-employee exemption covers *design and development of programs* — not operations, QA execution, or IT helpdesk work. It uniquely allows an hourly rate ($27.63/hour) to satisfy the compensation prong instead of a weekly salary.
- The outside-sales exemption requires that the employee is *customarily and regularly away from the employer's place of business*. Inside-sales reps do not qualify.
- California adds daily-overtime, seventh-day overtime, meal-and-rest-period premiums, waiting-time and wage-statement penalties, and PAGA representative actions on top of the federal FLSA baseline. The California exempt-salary threshold and computer-professional threshold are set by state law and change annually.
- Misclassifying one non-exempt employee as exempt for two years commonly creates $50,000–$150,000+ of exposure per employee including back overtime, liquidated damages, state penalties, and attorneys' fees.
- When in doubt, classify as non-exempt, track hours, and pay overtime. Non-exempt classification is easy to administer and eliminates the risk. Exempt classification is the risk category.
- The operational plumbing — hour tracking, compliant wage statements, workplace-notice posting, records retention, off-the-clock-work policy — is as important as the classification itself.
