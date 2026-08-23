# 1. W-2 employee vs. 1099 independent contractor

> "They only work twenty hours a week, so they're a contractor" is a losing argument. Classification is a legal test with defined factors — not a preference.

## Motivation

The single most common structural mistake a startup makes with its non-founder workforce is calling somebody a "1099 contractor" who is legally a W-2 employee. The intuition is understandable — the corporation saves 7.65% in employer-side FICA, avoids state unemployment-insurance registration, sidesteps workers'-compensation coverage, avoids benefit-eligibility questions, and doesn't have to run payroll for the person. The worker often prefers it too, at least initially, because they get a bigger gross check and can deduct business expenses on Schedule C.

Everyone likes the arrangement — until an agency notices. When it does notice, the exposure is per-worker back employer-side FICA (7.65%) plus federal income-tax withholding the corporation should have made (24% supplemental rate is a common IRS assessment default), plus state income-tax withholding, plus state unemployment-insurance contributions with penalty and interest, plus workers'-compensation premium plus penalty, plus potentially unpaid overtime for the same worker if they were also FLSA-non-exempt (chapter 02), plus liquidated damages under 29 U.S.C. § 216(b), plus attorneys' fees, plus in California a Private Attorneys General Act (PAGA) representative action seeking penalties on behalf of all similarly-situated workers, plus (in the states with an ABC test) a rebuttable presumption of employee status that the corporation is now trying to overcome in court against an angry ex-worker who has filed for unemployment insurance and been denied because the corporation "wasn't their employer."

The economic gain from calling someone a contractor when they're an employee is between six and twelve months of avoided payroll-tax friction. The cost of losing the reclassification fight is between five and fifty times that amount. This chapter teaches the framework so the corporation makes the classification call correctly on day one and can defend it in an audit.

## The three federal tests, and why California adds a fourth

There is no single US "employee vs. contractor" test. There are at least three federal tests, each with a different statutory context, plus state-law tests that layer on top:

- **The IRS common-law test** (Rev. Rul. 87-41; current guidance in IRS Publication 15-A and Form SS-8) governs *payroll tax* — who owes FICA, federal income-tax withholding, and FUTA on the payments to the worker.
- **The FLSA "economic realities" test** (29 U.S.C. §§ 201 et seq.; 29 C.F.R. Part 795) governs *federal wage-and-hour law* — who is entitled to minimum wage, overtime, and record-keeping protection under the Fair Labor Standards Act. <!-- needs-research: 29 C.F.R. Part 795 was rewritten by the DOL's 2024 final rule restoring a six-factor totality-of-circumstances test; the rule has been challenged in litigation. Verify the current operative rule text and status before publishing. -->
- **The ERISA / benefit-plan test** (28 U.S.C. § 1002(6); *Nationwide Mutual Insurance Co. v. Darden*, 503 U.S. 318 (1992)) governs *benefit-plan eligibility* — who counts as an "employee" for purposes of the corporation's 401(k), health, and equity plans.
- **State-law tests** govern state unemployment insurance, state workers'-compensation, state wage-and-hour law, and state tax withholding. Some states import the FLSA / IRS test; some, notably California and Massachusetts, apply a stricter three-part ABC test that flips the burden of proof.

A worker who is a "contractor" under one test can be an "employee" under another. The prudent posture is: if the worker qualifies as an employee under *any* applicable test, treat them as an employee everywhere. Splitting the classification — "1099 for federal, W-2 for state" or "employee for FICA, contractor for benefits" — creates internally-inconsistent records that make every audit worse.

## The IRS common-law test (Rev. Rul. 87-41 and the current 20-factor formulation)

Revenue Ruling 87-41, published in 1987, listed twenty factors the IRS uses to determine whether a worker is a common-law employee. The current administrative formulation (in IRS Publication 15-A, "Employer's Supplemental Tax Guide") groups the twenty factors into three categories:

1. **Behavioural control.** Does the corporation have the *right* to direct and control how the worker performs the work? Indicators: instructions the worker is required to follow (when, where, how); training the corporation provides; evaluation systems that measure how the work is done (as opposed to only the end result); the degree to which the worker is integrated into the corporation's operations.
2. **Financial control.** Does the corporation have the right to direct the *business* aspects of the worker's activity? Indicators: significant unreimbursed business expenses of the worker; a real investment by the worker in tools or facilities; the worker's services are available to the relevant market (not exclusive to the corporation); how the worker is paid (regular wage vs. flat fee per project); whether the worker can realise a profit or incur a loss on the engagement.
3. **The type of relationship.** How do the parties view their relationship? Indicators: written contracts describing the relationship (though the contract label is not dispositive); whether the corporation provides employee-type benefits (insurance, pension, paid leave, holidays); the permanency of the relationship (indefinite vs. project-based); the extent to which the services performed are a key aspect of the regular business of the corporation.

**No single factor is dispositive.** The twenty individual factors from the original ruling — instructions, training, integration, personal services requirement, hiring/firing/paying assistants, continuing relationship, set hours of work, full-time-required, doing work on employer's premises, order or sequence set, oral or written reports, payment method, payment of business/traveling expenses, furnishing tools and materials, significant investment, realisation of profit or loss, working for more than one firm at a time, making service available to the general public, right to discharge, right to terminate — are all still relevant, and the IRS applies them holistically.

**The Form SS-8 pathway.** Either the worker or the corporation can file **Form SS-8** ("Determination of Worker Status for Purposes of Federal Employment Taxes and Income Tax Withholding") asking the IRS to make a formal determination. The corporation almost never voluntarily files SS-8; a *worker* files SS-8 when they suspect they've been misclassified. An SS-8 determination that a worker is an employee is often the trigger for a broader IRS worker-classification examination of the corporation, and it is a fact the IRS shares with state agencies.

**The "safe harbour" of § 530.** Section 530 of the Revenue Act of 1978 (uncodified, but binding on the IRS) provides a defence to reclassification for corporations that (i) have a reasonable basis for the classification (a court decision, an IRS ruling, an IRS audit of the corporation for the same worker type, or "long-standing recognised practice of a significant segment of the industry"), (ii) have consistently treated the worker and all similarly-situated workers as contractors, and (iii) have filed all required Forms 1099. § 530 relief is narrow and does not apply to certain worker types (technical services workers under § 530(d)). Most startup contractor arrangements do not have the industry-practice or IRS-ruling basis that § 530 requires; assume § 530 will not save you.

**The Voluntary Classification Settlement Program (VCSP).** Announcement 2011-64 and subsequent guidance let a corporation prospectively reclassify workers as employees in exchange for paying a fraction of the employment-tax liability that would otherwise be owed (roughly 10% of one year's employment-tax exposure). VCSP is available if the corporation has consistently treated the workers as non-employees, has filed all required 1099s for the last three years, and is not currently under IRS audit for the workers in question. VCSP is worth considering when the corporation identifies a misclassified population before an audit finds them. <!-- needs-research: confirm the current VCSP eligibility rules and payment computation before recommending it to a client; the IRS has updated the program terms multiple times since 2011. -->

## The FLSA economic-realities test

The Fair Labor Standards Act does not use the IRS common-law test. It uses an "economic realities" test that asks whether the worker is, as a matter of economic reality, dependent on the corporation for employment (employee) or is truly in business for themselves (contractor). The DOL's current regulation — 29 C.F.R. Part 795, as rewritten by the 2024 final rule — lists six factors:

1. Opportunity for profit or loss depending on the worker's managerial skill.
2. Investments by the worker and the potential employer.
3. Degree of permanence of the work relationship.
4. Nature and degree of control the potential employer has over the work.
5. Extent to which the work performed is an integral part of the potential employer's business.
6. Skill and initiative.

The 2024 rule directs a totality-of-circumstances analysis with no factor pre-weighted. This restored the pre-2021 approach, replacing the 2021 rule that had elevated two "core" factors. Litigation over the 2024 rule is ongoing. <!-- needs-research: 29 C.F.R. Part 795 status after any 2025–2026 rulemaking or litigation; verify the operative test formulation and the DOL's current enforcement posture before authoring an FLSA-side classification memo. -->

For a startup, the practical implication of the FLSA test is that it is *no easier* than the IRS test — often stricter, because the DOL's remedial statute is interpreted broadly. A worker who is a "1099 contractor" under a strict IRS common-law analysis may still be an "employee" under the FLSA if the totality of factors shows economic dependence. This matters because FLSA classification determines minimum-wage and overtime rights — and a misclassified employee who was denied overtime can recover two years of back overtime (three years if the violation was wilful), plus an equal amount as liquidated damages, plus attorneys' fees.

## The California ABC test (*Dynamex* and AB 5)

California is the most restrictive state on worker classification, and its rule flips the burden of proof onto the hiring entity. In **Dynamex Operations West, Inc. v. Superior Court**, 4 Cal. 5th 903 (2018), the California Supreme Court adopted the "ABC test" for wage-order claims. The California Legislature codified and extended it via **AB 5** (2019), now in **Cal. Labor Code § 2775**.

Under the ABC test, a worker is presumed to be an employee unless the hiring entity establishes **all three** of the following:

- **(A)** The worker is free from the control and direction of the hiring entity in connection with the performance of the work, both under the contract and in fact.
- **(B)** The worker performs work that is outside the usual course of the hiring entity's business.
- **(C)** The worker is customarily engaged in an independently established trade, occupation, or business of the same nature as the work performed.

Prong **(B)** is the sharpest. It disqualifies most engineering, product, design, sales, and operational contractors at a technology startup, because their work is the exact "usual course of business" of the corporation. A software engineer doing software-engineering work at a software company fails prong (B) as a matter of law — no matter how much personal autonomy the engineer has and no matter how many other clients they serve.

**Statutory exceptions to AB 5** exist for specific professions and business-to-business relationships:

- **Cal. Labor Code § 2778** — "professional services" carve-out that returns to the *Borello* multi-factor test for specific occupations: marketing, human resources administrator, travel agent, graphic design, grant writer, fine artist, IRS-enrolled agent, payment-processing agent, some photographer / videographer / editor / illustrator categories, freelance writer / editor / newspaper cartoonist (subject to conditions), and others. Each carve-out has specific conditions the engagement must satisfy.
- **Cal. Labor Code § 2776** — "business-to-business" carve-out that returns to *Borello* if twelve specific conditions are met (contractor is a business entity, the contractor is free from control, the work is outside the usual course of the hiring entity's business, the contractor has its own business license, the contractor maintains a separate location, the contractor contracts with other businesses, etc.). This is a narrow safe harbour that most startup engagements fail on multiple prongs.
- **Referral-agency, motor-carrier, construction-subcontractor, and other industry-specific carve-outs** — largely irrelevant to a technology startup.

Where a statutory exception applies, the older *S.G. Borello & Sons v. Department of Industrial Relations*, 48 Cal. 3d 341 (1989) multi-factor test governs — which is close to the IRS common-law test. Where no exception applies, the ABC test governs and prong (B) is the key.

**California enforcement.** The California Employment Development Department (EDD) runs periodic worker-classification audits driven by unemployment-insurance claims (a former "contractor" files for UI, the EDD investigates whether the corporation should have been paying UI contributions on the worker's wages). The California Labor Commissioner enforces wage-and-hour law and adjudicates individual wage claims. The California Attorney General and city attorneys can bring UCL (Cal. Bus. & Prof. Code § 17200) actions. And private plaintiffs can bring **Private Attorneys General Act (PAGA)** representative actions on behalf of the state seeking civil penalties for Labor Code violations, including misclassification — with 75% of the penalties going to the state and 25% to the aggrieved employees (see [chapter 09](./09-arbitration-and-class-action-waivers.md) for PAGA's arbitration-carveout status).

## Other state ABC tests and the state variance

California is not alone. **Massachusetts** applies a stricter version of the ABC test under M.G.L. c. 149 § 148B for wage-and-hour purposes (prong B is "outside the usual course of business" *or* "performed outside all the places of business," which is stricter still than California). **New Jersey** applies an ABC test under N.J.S.A. § 43:21-19(i)(6) for unemployment-insurance purposes. **Illinois** applies an ABC test for wage-payment and workers'-comp purposes. **Connecticut** applies an ABC test for unemployment-insurance and workers'-comp purposes. **New Hampshire, Delaware, Nebraska, Vermont, and several other states** apply ABC or ABC-adjacent tests in specific contexts. <!-- needs-research: publish a current state-by-state matrix of which classification test applies for which regulatory purpose (wage-hour, unemployment insurance, workers' comp, wage payment) before drafting a multi-state classification memo. -->

The pattern to internalise: state law is at least as strict as federal law and frequently stricter. A corporation with employees in more than one state cannot rely on a single "we use the IRS test" answer.

## The agency-audit surface

Worker-classification exposure surfaces through several distinct enforcement channels. Understand which agency does what:

- **IRS worker-classification examination.** Triggered by an SS-8 filing from a worker, by a randomly-selected employment-tax audit, or by an IRS review of a Form 1099 that appears to relate to services that look like employment. Remedy: back employer FICA, back employer FUTA, back federal income-tax withholding the corporation should have collected (assessed at supplemental wage rate absent proof of the worker's actual tax liability), penalties (§ 6656 failure-to-deposit, § 6672 trust-fund recovery penalty against responsible officers personally), interest.
- **State employment-tax agency audit** (California EDD, Texas Workforce Commission, New York Department of Labor, etc.). Triggered by a worker's UI claim, by a random audit, or by inter-agency data sharing from the IRS. Remedy: back state unemployment-insurance contributions, back state income-tax withholding (states with wage withholding), penalties, interest. In California, EDD audits also feed into Labor Commissioner and Franchise Tax Board actions.
- **US Department of Labor (Wage and Hour Division) investigation.** Triggered by a worker complaint, by DOL initiative in targeted industries, or by media reporting. Remedy: back overtime and minimum-wage under FLSA (2- or 3-year lookback), civil money penalties for willful or repeated violations under 29 U.S.C. § 216(e), and — critically — DOL supervision of settlement.
- **State labour agency / attorney general action.** State-specific: California Labor Commissioner, New York AG's Labor Bureau, Massachusetts AG's Fair Labor Division. Remedy: back wages, penalties, injunctive relief, sometimes criminal referrals for wilful conduct.
- **Private civil litigation.** A former worker sues for unpaid wages, overtime, benefits, or misclassification. In California, add PAGA representative actions on behalf of the state. FLSA collective actions under 29 U.S.C. § 216(b) allow one worker to sue on behalf of all "similarly situated" workers who opt in.
- **Workers'-compensation carrier audit.** The corporation's workers'-comp policy is priced on covered payroll. A missing "contractor" payroll surface, discovered on a carrier audit or after a "contractor" gets hurt and files a claim, produces a retroactive premium assessment plus penalties. Some states impose criminal liability on employers who fail to carry workers'-comp coverage on legitimate employees.

The tell-tale sign that a "contractor" is actually an employee: they file for unemployment insurance after the engagement ends, are told they aren't eligible because the corporation didn't pay UI contributions on their behalf, and appeal that determination. The appeal is the first domino.

## The consequences of misclassification, quantified

Assume a startup that treats a full-time software engineer as a 1099 contractor for a year at $180,000. If reclassified:

- **Employer FICA** (Social Security 6.2% on wages up to the annual base, Medicare 1.45% on all wages plus Additional Medicare 0.9% over $200k) — approximately $12,300 for one year. <!-- needs-research: verify current Social Security wage base and Medicare thresholds before quoting exact dollar figures. -->
- **Federal income-tax withholding the corporation should have collected** — assessed at 24% supplemental wage rate absent proof the worker paid the underlying income tax; roughly $43,200 gross, reducible to zero under IRC § 3402(d) and Rev. Proc. 2004-56 if the corporation can obtain the worker's payment records. In practice the reduction is only partial.
- **FUTA** — 6.0% on the first $7,000, less state credits (typically to 0.6%) — small: $42.
- **State unemployment insurance** — state-specific. In California, the SUI rate for new employers is 3.4% on the first $7,000, so ~$238; but with penalty and interest, the assessment can run 1.5–2× the base amount.
- **Workers'-compensation premium** — industry-rate-dependent. For a technology-industry worker at $180k, roughly $500–$1,500 in annual premium, plus a large-scale penalty (California can impose stop-work orders and civil penalties of $1,500 per employee for willful failures).
- **Back overtime and liquidated damages under FLSA** — if the engineer, though salaried at $180k, was non-exempt (chapter 02) and worked over 40 hours in a week, back overtime for two years at 1.5× the regular rate for all hours over 40, plus an equal amount as liquidated damages, plus attorneys' fees. Six-figure exposure is common.
- **State wage-and-hour equivalents** — California adds daily-overtime (over 8 hours in a day), meal-and-rest-period premiums, waiting-time penalties (Cal. Labor Code § 203), wage-statement penalties (Cal. Labor Code § 226), and PAGA per-pay-period penalties.
- **Benefits catch-up** — the misclassified employee may claim retroactive entitlement to health coverage, 401(k) participation, equity grants, PTO, and other benefits. This depends on plan-document language and eligibility rules; a well-drafted plan document that ties eligibility to the corporation's classification decision can limit this exposure, but ERISA-fiduciary risk remains.
- **§ 6672 personal liability.** The IRS can assess the trust-fund recovery penalty against any officer or employee with "responsibility" for the withholding failure — a personal, non-dischargeable liability equal to the unpaid trust-fund portion of the tax.

For a single misclassified full-time engineer at $180k, the combined exposure — pre-negotiation — is commonly $60,000 to $150,000+. Multiply by every "contractor" the corporation has misclassified and add PAGA/class action multipliers in California, and the total can run into seven figures.

## The narrow cases where 1099 is genuinely defensible

The framework does not say "never use 1099." It says "use 1099 only when the classification survives the applicable tests." Genuinely-defensible 1099 engagements typically share a set of features:

- **Discrete, project-based scope.** A defined deliverable (a redesigned marketing site, a specific integration, a set of illustrations) with a defined completion criterion, not open-ended ongoing services. The engagement letter is a Statement of Work with milestones, not an employment agreement with a start date.
- **Contractor's own tools, workspace, and methods.** The contractor brings their own equipment, works from their own location, and controls how the work is done.
- **Contractor operates as a business.** Registered business entity (LLC, S-Corp, sole proprietorship with a DBA), business license, general-liability insurance, marketing materials, other clients. Ideally the contractor invoices from a business account, not their personal one.
- **Multiple concurrent clients.** The contractor is not economically dependent on the corporation. This directly answers the FLSA economic-realities test and helps on prong (C) of the ABC test.
- **Specialised trade outside the usual course of business.** A software startup engaging an outside accountant, an outside patent attorney, an outside videographer, an outside PR consultant — the contractor's trade (accounting, law, video production, PR) is distinct from the corporation's usual course of business (building and selling software). This is prong (B) of the ABC test.
- **Duration is limited.** A three-month engagement to complete a project reads as a contractor engagement. An indefinite ongoing engagement at 30–40 hours a week reads as an employment relationship regardless of the paperwork label.
- **The engagement letter reflects all of the above.** Present-tense SOW, milestones, payment on delivery, no fixed schedule, no benefits, no company laptop, no company email address, IP-assignment language appropriate to a contractor (see [chapter 04](./04-employee-piia.md) for the founder-side language and the contractor-specific carveouts).

The "twenty hours a week and they only have one client" contractor almost never survives this filter. The "we called them a contractor because they preferred it" contractor never survives it. And the "we can't afford to make them an employee yet" contractor especially never survives it — the affordability of correct classification is not a defence.

## Concrete example: three engagements, three classifications

- **Engineer A, hired to build the corporation's core product, working 40 hours a week from home in San Francisco, using corporation-issued laptop, attending daily standups, reporting to the CTO, no other clients, "consulting" for six months and then "we'll see."** Classification: employee under IRS common-law (behavioural control, integration, permanence), under FLSA (economic dependence), and under California's ABC test (fails prong B — engineer's work is the usual course of business). Legal answer: W-2, from day one. The "consulting" framing does not save the classification. If misclassified, exposure per the section above.
- **Videographer B, a Delaware LLC operating as "B Films LLC," engaged to produce a 90-second recruiting video, works from her own studio using her own equipment, invoices on delivery, has five other clients that quarter, engagement is a three-page SOW with a milestone.** Classification: contractor under IRS common-law (no behavioural or financial control, project-based relationship), under FLSA (no economic dependence, opportunity for profit / loss on the project), and — critically — under California's ABC test if the corporation qualifies for the business-to-business carveout (§ 2776) or if the video production doesn't fall into any of the ABC-covered contexts (which turns on where the wage-order coverage lands). Legal answer: 1099 is defensible; papers should reflect the LLC-to-LLC engagement, IP assignment via a mutual work-for-hire + assignment backstop, no benefits, no company-issued equipment.
- **Sales representative C, described as an "independent sales agent" paid on straight commission, uses corporation's CRM, is territory-assigned by the VP of Sales, attends the corporation's weekly sales meeting, has a corporation email address, has been "consulting" for eighteen months in Texas.** Classification: employee under IRS common-law (behavioural control via CRM, integration, permanence, indefinite duration), under FLSA (economic dependence), and under Texas's IRS-common-law-adjacent test. Legal answer: W-2. The "independent sales agent" label does not save the classification; the operational facts govern.

## The consultant-to-hire transition trap

A common startup pattern: hire someone as a "1099 contractor" for a three-month trial, then convert to W-2 if they work out. The trap: during the trial period, the corporation exerts behavioural control, integrates the worker into the team, provides tools, sets hours, and treats the worker exactly as an employee — but calls them a contractor. The trial-period 1099 arrangement is almost always misclassified. If the trial is a genuine try-before-you-buy — the corporation makes an informed decision after 90 days about whether to extend an offer — the correct paper structure is: hire the person as a W-2 employee from day one, on an at-will basis, with an explicit "introductory period" acknowledgement in the offer letter if that framing is useful for internal expectations. The at-will termination right is what the trial period gives the corporation; a 1099 label does not add anything except misclassification exposure.

## The "engineering is a contractor because they only work 20 hours a week" argument, and why it loses

Some founders reason: the engineer only works 20 hours a week, so they are not "full-time" and therefore they are a contractor. This is not how any of the tests work. Hours worked per week is not a factor in the IRS common-law test. It is not among the six factors in the DOL's economic-realities test. It is not one of prongs A, B, or C of the ABC test. A part-time worker who is directed by the corporation on how to perform the work, whose work is the usual course of business, and who has no independent trade is a part-time employee — not a contractor.

Similarly, arguments like:

- "We call everyone contractors at this stage." — Industry practice is not a defence under any test. § 530 requires the practice to be a "long-standing recognised practice of a significant segment of the industry," which no startup can credibly demonstrate.
- "The engineer prefers 1099." — Worker preference is not a factor. Classification is a legal test, not a bargaining outcome.
- "We signed a contract that says they're a contractor." — The contract label is not dispositive under any test. The operational facts govern.
- "They incorporated an LLC, so we're paying an LLC, so they're not our employee." — Wrong. The corporate form the worker uses to receive payment is one factor in the ABC test (prong C) and in the IRS financial-control analysis, but by itself it does not overcome behavioural control, integration into operations, and lack of an independent trade. The California courts have specifically rejected the "LLC-to-LLC papering" defence when the underlying relationship is employment.

## The decision framework, distilled

Ask, in order:

1. **What does the worker do?** If the work is the usual course of the corporation's business (engineering at a software company, sales at a sales-driven company, product at a product-led company), the worker is almost certainly an employee under the ABC test if the corporation has any workforce in an ABC-test state, and is likely an employee under the IRS common-law and FLSA tests as well.
2. **How much control does the corporation exert?** If the corporation controls when, where, and how the work is done — sets hours, assigns work, provides tools, requires participation in team meetings — the worker is likely an employee under the IRS common-law and FLSA tests.
3. **How permanent is the relationship?** An indefinite, ongoing arrangement is an employment relationship. A defined-scope, defined-duration project is a contractor engagement.
4. **Is the worker in business for themselves?** A worker with multiple clients, a registered business, business insurance, a separate workspace, and the ability to realise a profit or loss on the engagement is more plausibly a contractor. A worker who is economically dependent on the corporation is more plausibly an employee.
5. **What state?** If any state involved applies an ABC test (California, Massachusetts, and others), prong (B) — the "outside the usual course of business" prong — is the tightest constraint and usually the dispositive one.
6. **What is the cost of being wrong?** If reclassification exposure is meaningful — and for any full-time, ongoing worker it is — the presumption should be W-2 unless the corporation can affirmatively demonstrate contractor status under all applicable tests.

**Default the corporation to W-2 for any worker who is not manifestly, obviously a genuine outside contractor operating a real business with multiple clients on a discrete project.** The cost of W-2 (payroll, benefits, unemployment insurance, workers'-comp) is a known, budgetable operating expense. The cost of misclassification is an unquantified tail-risk that lands on the officer, the corporation, and the audit trail Series-A diligence will read.

## Summary

- Worker classification is a legal test with defined factors, not a preference or a bargaining outcome. Three federal tests (IRS common-law, FLSA economic-realities, ERISA/*Darden*) apply in different regulatory contexts; state tests (California ABC per *Dynamex* / AB 5, and analogues in Massachusetts, New Jersey, Illinois, Connecticut, and others) add strictness.
- California's ABC test (Cal. Labor Code § 2775) presumes employee status and requires the hiring entity to prove all three prongs — A (freedom from control), B (work outside the usual course of business), and C (independently established trade). Prong B disqualifies most engineering, product, design, sales, and operational contractors at technology startups.
- Misclassification exposure combines back employer FICA, federal and state withholding, unemployment-insurance contributions, workers'-compensation premium, FLSA back overtime and liquidated damages, state-specific wage-hour penalties (California adds PAGA), potential benefit-plan claims, and personal liability for responsible officers under IRC § 6672. Per-worker exposure for a full-time misclassified engineer commonly reaches $60,000–$150,000+.
- Genuinely-defensible 1099 engagements share discrete scope, contractor-owned tools and workspace, contractor-operated business, multiple concurrent clients, specialised trade outside the corporation's usual course of business, and a limited duration. Engagement letters read as SOWs with milestones, not as employment agreements.
- "The engineer only works 20 hours a week, so they're a contractor" is not an argument under any test. Hours worked is not a factor. Worker preference is not a factor. Contract labels are not dispositive. Operational facts govern.
- The prudent default at a startup is **W-2 from day one** for any worker performing the corporation's usual course of business, unless the engagement clearly and demonstrably satisfies every applicable test for contractor status.
