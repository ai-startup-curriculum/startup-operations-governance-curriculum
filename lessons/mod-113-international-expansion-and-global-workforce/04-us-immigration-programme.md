# 4. The US immigration programme for foreign-national hires

> H-1B is not a hiring channel — it is a lottery. Design the group's immigration programme around the visas that are actually available on the timeline the group needs to hire on.

## Motivation

Most US startups discover the immigration programme reactively. A recruiter closes a candidate; the candidate reveals they are on an F-1 STEM OPT expiring in nine months; the head of engineering escalates to the CEO; the CEO forwards to the incoming COO / GC / Head of People with a note that says "figure out how we sponsor this person, we cannot lose them." At that point, the answer depends on the current calendar month, the candidate's country of birth, the candidate's academic and professional record, whether the group has a prior L-1-relationship, and whether the role is TN-eligible.

None of those inputs can be discovered on the day of the escalation. The immigration programme has to be designed in advance so the recruiter can screen candidates on a known set of visa options, the offer can be extended with a defensible sponsorship path, and the corporate calendar treats the H-1B lottery not as an event but as one of several parallel channels.

This chapter is the working map. It is not immigration-law advice — every visa filing is signed by counsel and every complex case (adjustment of status, extraordinary-ability petitions, PERM audits) requires an experienced immigration attorney. The goal is that the operator can (a) construct the sponsorship offer at hire time, (b) run the annual H-1B lottery cycle, (c) understand the trade-offs between visa categories, and (d) plan the green-card trajectory for retained employees.

**Ownership boundary before we begin:** this chapter owns the **US-side immigration programme** for foreign-national hires (H-1B, O-1, L-1, TN, E-3, F-1 OPT / STEM OPT, and the EB green-card categories). It defers back to [mod-104](../mod-104-hiring-onboarding-and-hr-operations/) for the general US onboarding workflow and I-9 / E-Verify substance, and to [chapter 05](./05-international-employment-law-variance.md) for the non-US inbound-worker frame.

## The federal-employment authorisation baseline

Every US employer, regardless of the worker's nationality, is subject to two baseline requirements every incoming operator should know:

- **Form I-9.** Under the Immigration Reform and Control Act of 1986 (IRCA), every US employer must complete a **Form I-9, Employment Eligibility Verification** for every new hire, verifying identity and employment authorisation from a specified list of documents. Section 1 completed by the employee on or before day one; Section 2 completed by the employer within three business days of the start date. Retention: three years after the hire date or one year after termination, whichever is later. USCIS I-9 guidance and current form: https://www.uscis.gov/i-9-central.
- **E-Verify** is the DHS/SSA electronic verification system that confirms the I-9 information against government records. E-Verify participation is **voluntary at the federal level**, but is **mandatory** for federal contractors (subject to specific FAR clause 52.222-54) and for private employers in a growing list of states (Arizona, Florida, Georgia, Mississippi, North Carolina, South Carolina, Tennessee, and Utah require E-Verify for most private employers; other states require it for public employers or specific industries). Substance in [mod-104](../mod-104-hiring-onboarding-and-hr-operations/); this chapter notes the federal baseline. <!-- needs-research: confirm current list of states requiring E-Verify for private employers as of 2025–2026. -->

Foreign-national hires layer a **visa-specific work-authorisation** analysis on top of the I-9 baseline. The employee's I-9 documentation for many nonimmigrant visa categories is the visa stamp, the I-94 arrival record, and the I-797 approval notice — not a US Social Security card or US passport.

## The nonimmigrant visa map for tech-startup hiring

Nine visa categories cover essentially every foreign-national tech-startup hire. Two categories (**H-1B** and **O-1**) are the workhorses; three (**L-1**, **TN**, **E-3**) fit specific fact patterns; the rest (**F-1 OPT / STEM OPT**, **J-1**, **E-2**, **H-1B1**) are edge cases or bridges.

### H-1B — specialty-occupation worker

The primary US nonimmigrant work visa for skilled foreign workers. Foundational authority: **INA § 101(a)(15)(H)(i)(b)**; regulations at **8 CFR § 214.2(h)**.

Core mechanics:

- **Specialty occupation.** The position must require theoretical and practical application of a body of highly specialised knowledge and require at least a US bachelor's degree (or foreign equivalent) in a specific specialty. Software engineering, ML research, data science, product management, and many quantitative roles typically qualify; some marketing and general-business roles do not.
- **Prevailing wage.** The employer must pay the higher of the actual wage paid to similarly-situated workers or the DOL-determined **prevailing wage** for the occupation and geographic area. The DOL's Wage and Hour Division and OFLC (Office of Foreign Labor Certification) maintain the prevailing wage determination process. **Level 1 (entry)** to **Level 4 (fully competent)** determines the prevailing wage; the OFLC's Occupational Employment and Wage Statistics (OEWS) data drives the numbers.
- **LCA (Labor Condition Application).** Before the H-1B petition is filed, the employer files an **LCA (Form ETA-9035)** with DOL certifying the wage, working conditions, and non-displacement of US workers. The LCA is posted at the worksite for 10 business days.
- **Cap.** The H-1B has an annual **statutory cap** of 65,000 (regular cap) plus 20,000 (US master's degree exemption), for 85,000 new H-1B numbers per fiscal year. INA § 214(g)(1)(A).
- **Cap-exempt categories.** Petitions filed by (i) **institutions of higher education**, (ii) related or affiliated nonprofit entities, (iii) **nonprofit research organisations**, and (iv) **government research organisations** are exempt from the cap. INA § 214(g)(5). Some AI research organisations are structured to qualify as cap-exempt; most for-profit startups are not.
- **Registration and lottery cycle.** USCIS runs an annual **H-1B registration** in March. Employers submit electronic registrations (a lightweight filing per candidate) during a defined registration window; USCIS conducts a **random selection (lottery)** among all timely registrations for the 85,000 available cap numbers. Selected registrants can then file a full H-1B petition between April 1 and June 30 for an October 1 start date (the start of the federal fiscal year). Unselected registrants must wait a year and try again. <!-- needs-research: confirm the current H-1B registration window, the FY2026 selection results, and any procedural changes (e.g., the beneficiary-centric selection reform introduced in 2024). -->
- **Duration.** Initial approval up to three years; renewable for a further three years (six-year statutory maximum). **AC21 § 106(a)** — the American Competitiveness in the Twenty-First Century Act — permits extensions beyond six years while a green-card process is pending, subject to specific milestone gates.
- **Filing fees.** Filing fees have moved substantially — the base I-129 fee, the ACWIA training fee, the fraud-prevention fee, the public-law 114-113 supplemental fee (for large H-1B / L-1 employers), and the USCIS Asylum Program Fee (as of April 2024) all layer up. A typical initial H-1B cap petition today runs several thousand dollars in filing fees; premium processing (I-907) is available for expedited adjudication at additional cost. <!-- needs-research: confirm current USCIS filing-fee schedule for I-129 (H-1B), I-907, and associated add-on fees as of the current effective date. -->

**Practical implications for startup hiring:**

- **H-1B is a lottery, not a channel.** Recruiting cannot promise a candidate that H-1B sponsorship equals work authorisation. It equals lottery entry.
- **The March registration is a corporate calendar event.** The immigration attorney assembles the candidate list in January/February; the CFO / GC / Head of People confirms the filings and pays the filing fees; registrations submitted in March; selection results in late March; petition prep April–June; start date October 1 (or later, per candidate).
- **Cap-exempt employers exist for a reason.** Universities, teaching hospitals, and qualifying nonprofit research organisations can file H-1B outside the lottery. Startups partnering with cap-exempt research institutions (e.g., visiting-fellow structures) can sometimes access the cap-exempt track — a specialist immigration-attorney call.
- **Change-of-employer H-1B (H-1B transfer).** An existing H-1B worker changing employers files a new petition; the worker can start work at the new employer as soon as the new petition is received by USCIS (INA § 214(n)). This is the primary channel for hiring an already-H-1B-holding candidate mid-year; it does not consume a lottery selection.

### O-1 — extraordinary ability

The **O-1A** visa for individuals of extraordinary ability in sciences, education, business, or athletics (and O-1B for arts / motion pictures and television). Foundational authority: **INA § 101(a)(15)(O)**; regulations at **8 CFR § 214.2(o)**.

Core mechanics:

- **Extraordinary-ability standard.** The petitioner (employer or agent) must demonstrate the beneficiary is one of a small percentage who has risen to the very top of the field. Evidence must satisfy at least **three of eight criteria** (nationally-or-internationally recognised awards; membership in associations requiring outstanding achievements; published material about the beneficiary in professional publications; participation as a judge of others' work; original scientific / scholarly contributions of major significance; authorship of scholarly articles; employment in a critical or essential capacity for organisations with distinguished reputations; command of a high salary relative to others in the field) or comparable evidence.
- **No lottery, no cap, no prevailing-wage requirement.** The O-1 avoids both the H-1B lottery and the LCA process.
- **Advisory opinion.** Petitions typically require a written **advisory opinion** from a peer group, labour organisation, or management organisation confirming the beneficiary's qualifications (8 CFR § 214.2(o)(5)). For an AI / research candidate, this is often coordinated with a professional society or with an academic advisor.
- **Duration.** Initial approval up to three years; extensions in one-year increments.
- **USCIS January 2022 policy update.** USCIS updated its Policy Manual (Volume 2, Part M) to clarify the O-1A criteria as they apply to STEM fields — publications in top-tier venues (e.g., peer-reviewed AI / ML conferences such as NeurIPS, ICML, ICLR, CVPR, ACL), citation counts, and involvement in peer review are among the STEM-relevant applications of the criteria. The clarification made O-1A a more accessible option for high-output AI / ML researchers.

**Practical implications for startup hiring:**

- **O-1 is the H-1B alternative for exceptional candidates.** No lottery, faster to file, no fiscal-year cliff. The trade is the higher evidentiary bar and the higher legal-preparation cost.
- **AI / ML researchers with strong publication records** — NeurIPS / ICML / ICLR papers with citation counts, invited talks, peer-review involvement, prior competition wins — often qualify for O-1A even at relatively early career stages.
- **The programme runs on the strength of the file.** Immigration counsel should assess the candidate's O-1A viability during the offer stage; the assessment is a specific document exercise, not a general read of the CV.

### L-1 — intracompany transferee

The **L-1A** visa for executives and managers, and the **L-1B** visa for specialised-knowledge employees, transferring from a foreign affiliate of a US company to the US company. Foundational authority: **INA § 101(a)(15)(L)**; regulations at **8 CFR § 214.2(l)**.

Core mechanics:

- **Prior foreign-employment requirement.** The beneficiary must have been employed **abroad** by the qualifying corporate entity for at least **one continuous year within the three years** preceding the L-1 filing, in an executive, managerial, or specialised-knowledge capacity.
- **Qualifying corporate relationship.** The US petitioner and the foreign employer must have a qualifying relationship — **parent, subsidiary, affiliate, or branch**. The relationship is fact-specific and requires documentation of the corporate structure and beneficial ownership.
- **L-1A vs. L-1B.** L-1A (executive / manager) supports a **7-year** maximum stay and correlates with the **EB-1C** (multinational executive / manager) green-card category. L-1B (specialised knowledge) supports a **5-year** maximum stay and correlates with EB-2 or EB-3 categories.
- **Blanket L petitions.** Larger multinationals with a demonstrated pattern of L-1 transfers can qualify for a **blanket L petition** (a pre-approved corporate framework), which permits streamlined individual L-1 filings without the full I-129 case. Most startups do not qualify; most established multinationals do.
- **No cap.** L-1 is not subject to the H-1B lottery or cap.
- **Duration.** L-1A up to 7 years; L-1B up to 5 years. Requires the qualifying foreign employment history at initial filing.

**Practical implications for startup hiring:**

- **L-1 is the workhorse for moving international-subsidiary employees to the US parent.** A UK Ltd engineer who has worked at the UK subsidiary for 12+ months can be transferred to the US parent via L-1B (specialised knowledge) or L-1A (if a manager). This is one of the practical reasons the direct international subsidiary structure ([chapter 02](./02-first-international-entity-setup.md)) matters — it creates the L-1 pathway.
- **L-1A / EB-1C is the fast track for genuine multinational executives.** The green-card path via EB-1C avoids the PERM labour-certification bottleneck and is measurably faster than EB-2 / EB-3.
- **Specialised knowledge (L-1B) is heavily scrutinised.** USCIS L-1B RFEs (Requests for Evidence) are common; expect substantial documentation of the "specialised knowledge" the beneficiary carries about the group's proprietary systems, processes, or methodologies.

### TN — USMCA professional (Canadian and Mexican citizens)

The **TN** visa under the **United States–Mexico–Canada Agreement (USMCA)** (successor to NAFTA). Foundational authority: **INA § 214(e)** and **8 CFR § 214.6**. USMCA Chapter 16 replaced NAFTA Chapter 16 with substantially the same TN framework.

Core mechanics:

- **Nationality.** Canadian or Mexican citizen (permanent residents do not qualify).
- **Profession.** The role must be listed in **USMCA Chapter 16, Appendix 2 (Professionals)** — the same list as the original NAFTA Appendix 1603.D.1. The list is finite (approximately 60 professions) and includes engineer, computer systems analyst, scientific technician / technologist, economist, management consultant, and many others. **Software developer is not on the list**; the workaround is typically to file as **computer systems analyst** or **engineer**.
- **Credentials.** Must satisfy the credential requirement for the profession — typically a US bachelor's degree or foreign equivalent, and in some cases a specific professional certification.
- **Duration.** Initial admission up to **3 years**; renewable indefinitely in 3-year increments as long as the underlying employment continues.
- **No lottery, no cap, no LCA.**
- **Filing mechanics.** Canadian citizens can apply at the port of entry (POE) with the employment support letter and credential documents; Mexican citizens file for TN visa at a US consulate. Change-of-status filings within the US via Form I-129 are also available.

**Practical implications for startup hiring:**

- **TN is the fastest, cheapest, most reliable work-authorisation channel for eligible Canadian / Mexican professionals.** Same-day port-of-entry admission is realistic for Canadian citizens with a clean case. Filing fees a fraction of H-1B.
- **The profession list is the constraint.** "Software developer" is not on the list — the case must be framed as computer systems analyst (which fits many but not all software-engineering roles) or engineer (which requires a specific engineering degree). Immigration counsel structures the case; the group's engineering-leveling and job-description discipline supports the case.
- **TN does not lead directly to a green card.** TN is nonimmigrant intent — a TN applicant / holder must not have immigrant intent at the time of admission or extension. Filing an I-140 or adjustment-of-status application can complicate future TN admissions, though the case law is mixed. Coordinate with immigration counsel before initiating a green-card process for a TN holder.

### E-3 — Australian professional

The **E-3** visa for Australian citizens in specialty occupations. Foundational authority: **INA § 101(a)(15)(E)(iii)**.

Core mechanics:

- **Nationality.** Australian citizen (permanent residents do not qualify).
- **Specialty occupation.** Same standard as H-1B (US bachelor's degree or equivalent in the specific specialty).
- **Annual cap.** **10,500** per fiscal year — historically undersubscribed, so effectively no lottery.
- **Duration.** Initial admission up to 2 years; renewable indefinitely in 2-year increments.
- **LCA.** Requires an LCA (Form ETA-9035), same as H-1B.

**Practical implications for startup hiring:**

- **E-3 is the H-1B for Australians without the H-1B lottery.** For Australian citizens in specialty roles, E-3 is faster, cheaper, and more predictable than H-1B.

### F-1 OPT and STEM OPT — recent graduates

**F-1** student visas permit **Optional Practical Training (OPT)** — up to **12 months** of work authorisation in the field of study, either during studies (pre-completion OPT) or after graduation (post-completion OPT). Foundational authority: **8 CFR § 214.2(f)(10)**.

**STEM OPT extension** — students who have earned a degree in a **DHS-designated STEM field** can apply for a **24-month extension** of post-completion OPT (a **36-month total OPT window**), provided the employer is enrolled in E-Verify and adheres to the training-plan and reporting requirements of the STEM OPT programme. 8 CFR § 214.2(f)(10)(ii)(C).

**Practical implications for startup hiring:**

- **The F-1 STEM OPT window is the recruit-and-sponsor bridge.** A recently-graduated foreign-national engineer typically has 12 months of OPT + 24 months of STEM OPT + potentially H-1B lottery attempts in years 1–3 of the OPT window before requiring a different visa. The group's recruiting operation should surface OPT / STEM OPT status early so the H-1B lottery calendar is planned in from the offer stage.
- **E-Verify is a STEM OPT prerequisite.** An employer hiring a STEM OPT worker must be E-Verify-enrolled. If E-Verify is not already in place at the group, enrol before the hire.

### H-1B1 (Chile / Singapore), TN (Canadians / Mexicans), E-3 (Australians) — the treaty-country cluster

Three visa categories tied to specific treaty relationships fit narrow but useful fact patterns:

- **H-1B1 — Chile / Singapore.** Free-trade-agreement H-1B derivative for Chilean and Singaporean citizens; 1,400 (Chile) / 5,400 (Singapore) annual cap that is essentially always undersubscribed. INA § 101(a)(15)(H)(i)(b1).
- **TN** — covered above.
- **E-3** — covered above.

Each is a fast, high-reliability alternative to H-1B for nationals of the specific treaty countries.

### J-1 exchange visitor — narrow fits

The **J-1** exchange-visitor programme covers research scholars, trainees, and interns. Foundational authority: **INA § 101(a)(15)(J)**; regulations at **22 CFR § 62**.

Practical fit for startups: limited. A J-1 research-scholar programme requires designation as a J-1 sponsor (or partnership with a designated sponsor); a J-1 trainee / intern programme fits summer / structured internship arrangements. Some J-1 categories carry a **two-year home-country residence requirement** (INA § 212(e)) that must be waived or served before the beneficiary can change to an H-1B or apply for a green card — a substantial constraint.

Most tech startups do not run a J-1 programme; those that do typically partner with an established sponsor organisation.

## The green-card categories

Long-term retention of foreign-national employees requires a green-card sponsorship trajectory. The employment-based (EB) categories:

### EB-1 — first preference (priority workers)

Three sub-categories:

- **EB-1A — extraordinary ability.** The green-card analogue to the O-1A visa; requires demonstration of sustained national or international acclaim. No PERM labour certification required. Self-petition permitted.
- **EB-1B — outstanding professor / researcher.** For academic / research positions with employer sponsorship. No PERM.
- **EB-1C — multinational manager / executive.** The green-card correlate to L-1A; requires prior qualifying foreign employment of at least one year in the three years preceding the US transfer, in an executive or managerial capacity. No PERM.

**EB-1 processing times** for the underlying I-140 are relatively short (premium processing available); however, priority-date backlog for oversubscribed countries (India, China) can add substantial time before adjustment of status is possible. <!-- needs-research: cite the current Visa Bulletin priority-date positions for EB-1 India, EB-1 China, and EB-1 rest-of-world as of the most recent monthly bulletin. -->

### EB-2 — second preference (advanced-degree professionals)

For positions requiring an **advanced degree** (US master's or higher, or US bachelor's + 5 years progressive experience) or for individuals with **exceptional ability**. Requires PERM labour certification (see below) unless the applicant qualifies for an EB-2 **National Interest Waiver (NIW)**.

**EB-2 NIW** — the National Interest Waiver — waives the PERM requirement for individuals whose work is deemed in the national interest of the US. The three-prong test from *Matter of Dhanasar*, 26 I&N Dec. 884 (AAO 2016), governs: (i) the endeavour has substantial merit and national importance; (ii) the applicant is well-positioned to advance it; (iii) on balance it would be beneficial to the US to waive the PERM requirement. AI / ML research work of national significance, work on critical infrastructure, work aligned with published administration priorities, and similar profiles frequently support NIW petitions. Self-petition permitted.

### EB-3 — third preference (skilled workers, professionals, and other workers)

For positions requiring at least a US bachelor's degree (professional) or two years of training / experience (skilled). Requires PERM. Priority-date backlogs for India / China are among the longest in the EB categories.

### EB-4 — special-immigrant categories

Ministers, religious workers, certain broadcasters, and other special-immigrant categories. Not typically relevant for tech startups.

### EB-5 — investor immigration

The investor / regional-centre programme; requires substantial capital investment ($800,000 in a TEA / $1,050,000 elsewhere as of the EB-5 Reform and Integrity Act of 2022). Not typically relevant for tech-startup employment.

### The PERM labour-certification path

For EB-2 (non-NIW) and EB-3, the employer must obtain a **Labor Certification (PERM)** from DOL before filing the I-140. The PERM process:

- **Prevailing wage determination.** Employer files ETA-9141 with DOL to determine the prevailing wage for the offered position.
- **Recruitment.** Employer conducts a specified recruitment sequence — job order at the state workforce agency, two Sunday newspaper ads (professional occupations require additional recruitment via campus recruiting, employer website, professional publications, etc.), internal job posting for 10 business days.
- **PERM application.** Employer files ETA-9089 with DOL certifying no qualified US workers applied for the position. DOL audits a percentage of filings; audits add 6–12 months to the timeline.
- **I-140 filing.** Certified PERM in hand, employer files I-140 with USCIS.
- **Adjustment of status (I-485).** Beneficiary files I-485 to adjust to permanent-resident status once the priority date is current — for India / China nationals in EB-2 / EB-3, this wait can be years or decades.

The PERM process is procedurally rigid; the recruitment requirements are audit-sensitive; the whole exercise is best run by immigration counsel with PERM experience.

## Designing the group's immigration programme

A practical operating pattern for a US startup with a foreign-national engineering workforce:

- **Retain immigration counsel.** A specialist firm — Fragomen, Berry Appleman & Leiden (BAL), Fisher Phillips, or a boutique — on retainer or on a per-case basis. The relationship survives multiple hires.
- **Run an intake at every offer.** For every candidate who is not a US citizen or permanent resident, the recruiter / HRBP asks the visa-status questions early — current status, expiration, prior H-1B history, prior L-1 history, country of birth (drives green-card priority-date exposure), citizenship — and hands to immigration counsel for a visa-strategy read before offer terms are finalised.
- **Set the sponsorship policy.** Publicly, the group's job postings should indicate whether visa sponsorship is available and for which categories. A common startup posture: sponsorship available for H-1B (subject to lottery), O-1, L-1 (if applicable), TN, E-3, and green-card sponsorship for retained employees after a defined tenure gate.
- **Enrol in E-Verify.** Required for STEM OPT hires. Also required for federal contractors and in an expanding list of state-mandated employers ([mod-104](../mod-104-hiring-onboarding-and-hr-operations/)). Register at https://www.e-verify.gov.
- **Calendar the H-1B lottery cycle.** Every October, immigration counsel identifies candidates for the following March registration. February–March: registrations submitted. Late March: selection results. April–June: full petitions filed for selected registrants. October 1: start date.
- **Design the green-card programme.** Common practice: after 12–24 months of employment (or on start for critical hires), initiate the green-card process. EB-2 NIW or EB-1 (extraordinary-ability / multinational-executive / outstanding-researcher) where the profile supports it; EB-2 / EB-3 with PERM otherwise.
- **Track priority dates.** For India / China nationals, the priority-date wait is a real dimension of the employment relationship and should be tracked as part of the retention conversation.

## Grace periods and terminations

Terminations of visa-holding employees carry a specific downstream mechanic every operator should know:

- **60-day grace period for terminated H-1B, L-1, O-1, TN, E-3, and other work-visa holders.** 8 CFR § 214.1(l)(2). A worker whose employment terminates has up to 60 consecutive days (or the remaining validity of their I-94, whichever is shorter) to find a new employer, change status, or depart the US.
- **Notification and repatriation.** For H-1B specifically, the terminating employer must notify USCIS of the termination (8 CFR § 214.2(h)(11)(i)(A)) and offer to pay the "reasonable cost of return transportation" to the worker's home country (8 CFR § 214.2(h)(4)(iii)(E)). Failure to do either can extend the employer's wage-payment obligation.
- **Green-card portability (AC21).** Workers with an approved I-140 whose adjustment-of-status (I-485) application has been pending 180 days or more can "port" to a same-or-similar occupation with a new employer without losing their priority date (AC21 § 106(c)). Retention planning for backlogged-country green-card cases sits on top of this rule.

The termination-side mechanics are picked up in [chapter 08](./08-international-workforce-reduction-playbook.md) alongside the international-side offboarding regimes.

## Anti-patterns

- **"We'll figure out the visa later."** A candidate is offered without an immigration-strategy read; the offer is accepted; the group discovers on onboarding that the sponsorship path is not viable in the available time. Screen at intake, not at signing.
- **Treating H-1B as a guaranteed channel.** Recruiters promise H-1B to a candidate; the March lottery does not select the registration; the candidate has no path and the group loses the hire. H-1B is a lottery.
- **Ignoring the country-of-birth green-card exposure.** An Indian-national or Chinese-national hire faces green-card priority-date waits that materially affect retention. Ignoring the exposure means losing the employee to a competitor with a better retention pitch (private-track EB-1, alternative visa strategies, or a same-or-similar-role portable I-140).
- **Missing the 60-day grace-period notification.** A terminated H-1B worker leaves the payroll and the group forgets to notify USCIS or offer return-transportation cost; the wage-payment obligation extends past the termination date. The immigration attorney should be looped into every termination of a visa-holding employee.
- **PERM run without immigration counsel.** The PERM recruitment process is audit-sensitive; a self-run PERM is a wasted 12 months and a compromised green-card case.

## Concrete example — a foreign-national ML researcher joins a US Series-B startup

A representative fact pattern:

- **Candidate.** ML researcher, PhD from a top UK institution, three years of postdoc research with multiple NeurIPS / ICML publications and citations. UK citizen. Currently on OPT-STEM extension at a US university.
- **Role.** Senior Research Scientist, US-based, reporting into the CTO. US bachelor's degree equivalent (PhD).
- **Initial sponsorship strategy.** Immigration counsel evaluates: (i) H-1B — feasible if selected in the March lottery; (ii) O-1A — likely feasible given the publication record and STEM Policy Manual clarification; (iii) TN — not eligible (UK national); (iv) E-3 — not eligible (UK, not Australia); (v) L-1 — not eligible (no prior foreign-affiliate employment). Recommendation: **file O-1A now**, run H-1B in parallel next March as insurance.
- **O-1A file.** Immigration counsel assembles the evidence — publications, citations, peer-review invitations, competition wins, advisory letters. Advisory opinion from a professional society or academic sponsor. Petition filed with premium processing. Approval typically within 15 days.
- **Green-card strategy.** After 12 months of employment, initiate **EB-1A** (extraordinary ability) or **EB-2 NIW** based on the strength of the file. Self-petition permitted; no PERM required.
- **Retention posture.** Green-card process telegraphed at hire; priority date established early; the candidate has visibility into a permanent-resident trajectory as part of the offer.

The programme's value is that this exact conversation is repeatable across candidates without inventing the strategy each time.

## Summary

- **US work-authorisation baselines (I-9, E-Verify)** apply to every hire; visa-specific work authorisation layers on top.
- **H-1B is the lottery.** March registration, April–June petitions, October 1 start; 85,000 statutory numbers, cap-exempt categories exist for university-affiliated / nonprofit-research employers.
- **O-1A is the H-1B alternative for exceptional candidates** — no lottery, no cap, but a higher evidentiary bar. Increasingly viable for AI / ML researchers under the January 2022 USCIS STEM policy clarification.
- **L-1 (A/B) is the intracompany-transfer channel.** Enables foreign-affiliate employees with one qualifying year abroad to transfer to the US parent. L-1A supports the fast EB-1C green-card path.
- **TN (Canadian / Mexican) and E-3 (Australian)** are the fast, cheap, high-reliability treaty channels for eligible nationals.
- **F-1 OPT / STEM OPT (12 + 24 months)** is the recruit-and-sponsor bridge for recent graduates; the H-1B lottery calendar must be planned in from offer.
- **Green-card categories.** EB-1 (A/B/C) — no PERM; EB-2 (with PERM or NIW); EB-3 (with PERM). PERM is a 12-month+ DOL process; priority-date backlogs for India / China nationals are years or decades in EB-2 / EB-3.
- **60-day grace period** applies to terminated H-1B, L-1, O-1, TN, and E-3 holders. Terminating employers of H-1B workers must notify USCIS and offer to pay return transportation.
- **Operating pattern:** retain immigration counsel, run visa-strategy intake at every offer, publish the sponsorship policy, calendar the H-1B lottery, design the green-card programme deliberately.
