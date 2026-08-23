# 5. Form I-9 and E-Verify

> The Form I-9 is a three-day deadline the corporation loses in ways it does not notice — the new hire started remote, HR never met them in person, the "we'll fix it later" period turned into six weeks, and the eventual ICE audit reads every one of those files.

## Motivation

Every US employer is required by the Immigration Reform and Control Act of 1986 (IRCA), 8 U.S.C. § 1324a, to verify that every employee hired in the United States is authorised to work — regardless of the employee's citizenship. That verification happens on **Form I-9, Employment Eligibility Verification**, issued by U.S. Citizenship and Immigration Services (USCIS).

The rules are simple to state and easy to break at scale:

- The employee must complete **Section 1** of Form I-9 no later than the first day of employment (i.e., by the day they start).
- The employer must complete **Section 2** — physically examining the employee's original identity and work-authorisation documents — no later than **the third business day after the first day of employment** (or, if the employee is hired for fewer than three days, by the first day of employment).
- Retention: the completed I-9 must be retained for **three years after the date of hire, or one year after the date of termination, whichever is later**.

Failure exposes the corporation to civil penalties per violation, which are indexed for inflation and rise sharply for repeat and willful violations. <!-- needs-research: confirm the current civil-penalty schedule under 8 C.F.R. § 274a.10 as most recently updated for inflation (the DHS Federal Civil Penalties Inflation Adjustment adjusts these annually); do not quote specific dollar figures without confirming the current-year schedule. --> Beyond civil penalties, "knowing hire" of unauthorised workers is a separate criminal exposure under 8 U.S.C. § 1324a(f).

**E-Verify** is a separate federal system that layers on top of Form I-9. It is a Department of Homeland Security / Social Security Administration web-based service that compares the employee's Form I-9 information against DHS and SSA records to confirm work authorisation. E-Verify is **optional for most employers under federal law** but **mandatory for federal contractors and subcontractors** subject to the FAR E-Verify clause (FAR 52.222-54, 48 C.F.R. § 52.222-54) and **mandatory for all or specified employers in a set of states** (with the state list expanding over time). E-Verify participation triggers additional employer obligations — the tentative-nonconfirmation (TNC) process, additional recordkeeping — that must be operated correctly.

This chapter builds the I-9 operating procedure, walks the acceptable-documents list and the reverification triggers, describes the retention and audit-readiness posture, and layers on the E-Verify overlay.

## The Form I-9 process

### The current form

Employers must use the **currently valid edition of Form I-9**. USCIS publishes an edition date and expiration date on the form itself; using an expired edition is a violation. Check https://www.uscis.gov/i-9 for the current edition before every new-hire cycle. <!-- needs-research: confirm the current I-9 form edition (e.g., 08/01/23 edition or successor); do not hard-code an edition number that may have been superseded. -->

### Section 1 — Employee information and attestation

The employee completes Section 1 no later than the first day of employment. The employee attests, under penalty of perjury, to one of the following categories:

1. A citizen of the United States.
2. A noncitizen national of the United States.
3. A lawful permanent resident (with Alien Number / USCIS Number).
4. A noncitizen authorised to work (with expiration date if applicable, and either an Alien / USCIS number, Form I-94 admission number, or foreign passport number).

Section 1 also captures name, address, date of birth, SSN (voluntary unless the employer is enrolled in E-Verify, in which case SSN is required), email, and phone number. If the employee had assistance completing Section 1 (e.g., a translator), the preparer/translator certification section must also be completed.

### Section 2 — Employer review and verification

Within three business days of the first day of employment, the employer (or an authorised representative — see below) must:

1. Physically examine the original documents the employee has presented from the Lists of Acceptable Documents (see below).
2. Verify that the documents reasonably appear to be genuine and to relate to the employee presenting them.
3. Record the document title, issuing authority, document number, and expiration date on Section 2.
4. Sign, print name, title, and date Section 2 — attesting under penalty of perjury that the documents were examined.

The employee chooses which documents to present — the employer may not require specific documents from the list.

### The acceptable-documents list

Form I-9 lists documents in three categories:

- **List A** — documents that establish both identity and employment authorisation. Presenting a single List A document is sufficient. Common examples: U.S. Passport or Passport Card; Permanent Resident Card (Form I-551); Employment Authorisation Document (Form I-766); foreign passport with a Form I-94 endorsement.
- **List B** — documents that establish identity only. Common examples: state driver's license or ID card; school ID with photograph; U.S. military ID.
- **List C** — documents that establish employment authorisation only. Common examples: Social Security Card (unrestricted); certified copy of a birth certificate issued by a U.S. state or territory; U.S. Citizen ID Card (Form I-197).

If the employee does not present a single List A document, they must present **one document from List B and one document from List C**.

Full lists (with detailed acceptable-form specifications, including exceptions and updates) are published in the USCIS **Handbook for Employers M-274** (https://www.uscis.gov/i-9-central/handbook-for-employers-m-274). The M-274 is the authoritative reference for edge cases (receipts for lost documents; documents for minors; H-1B and other work-visa holders; expired documents; etc.).

### The remote-hire and authorised-representative workflow

Historically, Section 2 required in-person physical examination of documents. The COVID-era temporary flexibility permitted remote examination in some circumstances; that flexibility was superseded in 2023 by a **permanent alternative remote procedure** available to employers enrolled in E-Verify and in good standing with certain compliance criteria. <!-- needs-research: confirm the current status, eligibility criteria, and procedural requirements of the DHS "alternative procedure" for remote document examination (announced in 2023 via 88 Fed. Reg. 47990); the eligibility is narrower than the COVID flexibility and requires E-Verify enrollment. -->

For employers not eligible for the alternative remote procedure, the standard operating pattern for a remote new hire is:

- The employer designates an **authorised representative** near the employee's location to physically examine the documents and complete Section 2 on the employer's behalf.
- The authorised representative can be *any* individual the employer designates (a notary, an HR service, a family member of the employee, a neighbour) — but the *employer* remains liable for any errors or violations in the completion of Section 2.
- Practical implementation: many HRIS platforms (Rippling, Gusto, Deel, Justworks, TriNet — see [chapter 07](./07-hris-peo-payroll-stack.md)) and dedicated I-9 vendors (Equifax I-9 Anywhere, WorkBright, HireRight I-9, and others) provide authorised-representative networks (notaries or agents) as a paid service.

### Section 3 — Reverification and rehires

Section 3 is completed when:

1. An employee's work authorisation is expiring and must be reverified before the expiration date. The employee presents unexpired List A or List C documentation establishing continued authorisation to work.
2. An employee has a legal name change (Section 3 is *optional* in this case, though recommended for recordkeeping).
3. A former employee is rehired within three years of the date of the original Form I-9 (Section 3 may be used to update the form, or a new Form I-9 may be completed).

**What must not be reverified.** The corporation may **not** reverify permanent-resident-card (green-card) expiration dates. A permanent resident's authorisation to work does not expire when the physical card expires; the person is a lawful permanent resident.

The corporation may **not** reverify List B documents (driver's licenses, state IDs) even if they expire. List B documents establish identity, not authorisation to work, and identity does not expire.

**Reverification triggers a calendar obligation.** The corporation must have a tickler system — typically in the HRIS or the ATS's onboarding module — that flags upcoming work-authorisation expirations and initiates the reverification workflow before the expiration date. Failing to reverify by the expiration date and continuing to employ the person is a violation.

## Storage, retention, and audit-readiness

### Retention

Form I-9s must be retained for **three years after the date of hire, or one year after the date of termination, whichever is later**. So for a two-year employee, the I-9 must be kept for one year after termination. For a five-year employee, the I-9 must be kept for one year after termination. For a one-month employee, the I-9 must be kept for three years after the date of hire (which will be longer than one year after termination for a short-tenured employee).

### Storage — separate from personnel file

I-9s are typically stored **separately from the general personnel file**. The reason: in an ICE audit (see below), the auditor demands only the I-9s (and, if applicable, the E-Verify records). Storing I-9s separately makes production straightforward and avoids inadvertent disclosure of unrelated personnel information.

Storage may be paper, electronic, or a combination. Electronic storage must meet the requirements of 8 C.F.R. § 274a.2(e) — including reasonable controls to ensure integrity, accuracy, reliability, indexing, and the ability to reproduce legible paper copies on demand. Most modern HRIS platforms handle electronic I-9 storage in a compliant manner as a core feature, and store the I-9 in a segregated area from the general employee record.

### Audit-readiness

The corporation should be able to, within three business days of a Notice of Inspection (NOI) from ICE Homeland Security Investigations (HSI), produce **every I-9 currently in the retention window** in the format the auditor requests. Three business days is the statutory response window — 8 C.F.R. § 274a.2(b)(2)(ii).

Preparation:

- **Internal I-9 audit** — annually or when the corporation is preparing for a diligence event (Series-B, Series-C, acquisition, IPO). A trained internal reviewer or external counsel walks every I-9 for common errors: missing signatures, unexamined documents, expired forms, incorrect document combinations (List B + List B instead of List B + List C), improperly recorded document details, and reverification misses.
- **Error correction protocol** — Errors are corrected by drawing a single line through the incorrect information, entering the correct information, initialling and dating the correction. Errors are **not corrected by white-out, by re-typing, or by back-dating**. The USCIS M-274 Handbook is the reference for the correct correction technique.
- **Missing I-9s** — For an employee whose I-9 cannot be found, the corporation must complete a new I-9 immediately, using the *current* date (not the original hire date), and note the circumstances of the correction. A missing I-9 is a violation; a new I-9 completed on the current date at least demonstrates good-faith correction and reduces the exposure at audit.
- **Retention housekeeping** — Employees who have been terminated and whose I-9 retention window has expired can have their I-9 removed from the corporate record. Documented destruction (rather than accumulating years of past-employee I-9s) reduces the audit surface.

### ICE Notice of Inspection

An ICE HSI audit typically begins with a Notice of Inspection served to the employer, giving three business days to produce the I-9s. The employer's counsel should be involved from day one. Audits commonly proceed as follows:

1. **Notice of Inspection.** Three business days to produce.
2. **Audit.** ICE reviews the I-9s (and any E-Verify records if the employer is enrolled). Common findings: technical violations (missing information, expired forms), substantive violations (missing I-9s, unverified documents), and — most seriously — indicators of "knowing hire" of unauthorised workers.
3. **Notice of Suspect Documents** or **Notice of Discrepancies** — for employees whose documents ICE could not verify.
4. **Notice of Intent to Fine (NIF)** or **Warning Notice** — the enforcement action.
5. **Response and negotiation** — the employer typically has 30 days to respond to the NIF and can negotiate the fine amount.

The corporation that prepared for the audit before it arrived — internal audits complete, corrections properly documented, retention discipline in place — typically settles the audit within the technical-violations band. The corporation that ignored I-9 hygiene for years faces exposure that scales rapidly.

## E-Verify

### What E-Verify is

E-Verify is a free, web-based system operated by USCIS in partnership with the Social Security Administration that compares information from an employee's Form I-9 against records held by DHS and SSA to confirm employment eligibility. It is *complementary to* Form I-9, not a substitute — every E-Verify-enrolled employer still completes Form I-9 for every new hire.

An E-Verify case is created for every new hire (of an enrolled employer) within three business days of the first day of employment. The case is submitted through the E-Verify web interface (https://www.e-verify.gov) or through an HRIS integration that connects to E-Verify.

### The tentative-nonconfirmation (TNC) process

Most E-Verify cases result in **Employment Authorized** within seconds. A small percentage result in a **Tentative Nonconfirmation (TNC)** — the DHS or SSA record does not match the information submitted. On a TNC:

1. The employer notifies the employee of the TNC and provides the "Further Action Notice" printed from E-Verify.
2. The employee decides whether to take action to resolve the mismatch (contest the TNC) or not (self-terminate).
3. If the employee contests, the employer must give the employee eight federal government working days to contact DHS or SSA to resolve the mismatch.
4. The employer must not terminate, suspend, delay training, withhold pay, or take other adverse action against the employee during the TNC resolution period. This is a specific, enforceable E-Verify obligation.
5. Once DHS or SSA updates the case (to Employment Authorized, or Final Nonconfirmation), the employer proceeds accordingly. On Final Nonconfirmation the employer may terminate.

### E-Verify obligations beyond the TNC process

- **Notice.** Employers must display the required E-Verify participation posters (in English and Spanish) in a location visible to prospective employees.
- **Nondiscrimination.** Employers may not use E-Verify to pre-screen job applicants, may not selectively use E-Verify for some employees and not others (except that federal contractors may verify their existing workforce under the FAR clause), and may not use E-Verify for reverification (permanent-resident-card expirations are excluded from E-Verify entirely).
- **Recordkeeping.** E-Verify case numbers should be recorded on the Form I-9 (or in the E-Verify system's own record), and E-Verify records are retained for the same period as the underlying I-9.

### E-Verify — optional federally, mandatory in specific contexts

**Optional at the federal level for most employers.** The federal government does not require the private sector broadly to use E-Verify.

**Mandatory for federal contractors and subcontractors** subject to the FAR E-Verify clause (FAR 52.222-54) — the corporation performing under a contract with the E-Verify clause must (a) enroll in E-Verify within 30 days of the contract award, (b) begin using E-Verify for all new hires within 90 days of enrollment, and (c) verify all existing employees assigned to the contract within 90 days of enrollment (or, at the corporation's option, all existing employees).

**Mandatory in specific states.** The list of states that require E-Verify for some or all employers has grown and now includes (with variance in scope — private-sector broadly, public-sector only, employers of a certain size, employers with state contracts, etc.):

- **Alabama** — Beason-Hammon Alabama Taxpayer and Citizen Protection Act.
- **Arizona** — Legal Arizona Workers Act.
- **Florida** — Fla. Stat. § 448.095 (mandatory for private employers with 25+ employees for hires on or after July 1, 2023).
- **Georgia** — O.C.G.A. § 36-60-6 and related statutes (varies by employer size and public-contract status).
- **Mississippi** — Mississippi Employment Protection Act.
- **Missouri** — for state contractors.
- **North Carolina** — for employers with 25+ employees.
- **South Carolina** — S.C. Code § 41-8-20 (all employers).
- **Tennessee** — Tenn. Code § 50-1-703 (varies by employer size).
- **Utah** — Utah Code § 63G-11-103 (private employers of 15+ and public contractors).

<!-- needs-research: this state list is drawn from long-standing E-Verify mandates but the exact scope, employer-size threshold, and effective-date landscape shifts frequently. Verify each state's current statute and any 2024–2026 amendments before publishing operating policy. -->

**Operating implication.** The corporation must know, for every state where it hires, whether E-Verify is mandatory (and if so, for which employers) — and configure the HRIS or E-Verify workflow accordingly. Multi-state employers commonly enroll in E-Verify once and use it for all hires in all states, both because the operating simplicity outweighs the compliance nuance and because E-Verify enrollment is a prerequisite for the DHS alternative remote-examination procedure discussed above.

## The intersection with the HRIS

Nearly every modern HRIS runs the I-9 (and, if applicable, E-Verify) workflow natively or through a tight integration:

- Employee completes Section 1 in the HRIS onboarding workflow before day one.
- Employer or authorised representative completes Section 2 in the HRIS after physically examining documents (or, where eligible, using the DHS alternative remote procedure).
- E-Verify case is created via the HRIS-E-Verify integration.
- I-9 stored electronically in the HRIS's compliance module, segregated from the general personnel file.
- Reverification calendar-managed by the HRIS, with automated alerts to HR before work-authorisation expiration.

The HRIS-I-9-E-Verify workflow is one of the strongest reasons the corporation adopts an HRIS rather than running payroll on spreadsheets — the compliance surface without an HRIS is one the corporation will not cover on its own at any real hiring rate. See [chapter 07](./07-hris-peo-payroll-stack.md).

## A worked example — a Series-A I-9 operating procedure

The corporation has employees in California, Colorado, New York, Washington, and Florida. It is on Rippling as its HRIS. It is not a federal contractor.

**Operating procedure.**

1. **E-Verify enrollment.** The corporation enrolls in E-Verify because (a) it has employees in Florida (mandatory for private employers with 25+ employees as of July 1, 2023) and expects to cross that threshold within the fiscal year, (b) it wants operating simplicity across states, and (c) it wants access to the DHS alternative remote-examination procedure. Enrollment is via https://www.e-verify.gov; the required posters are printed and posted in the physical office and the corporation's remote-employee handbook links to the electronic version.
2. **I-9 workflow.** Rippling's onboarding module sends Section 1 to the employee at offer acceptance, with a target completion date of the day before the start date. Section 2 is completed within three business days of the start date. Remote hires complete Section 2 through Rippling's authorised-representative network (or, once the corporation qualifies for the DHS alternative procedure, remotely via E-Verify).
3. **E-Verify case.** Rippling submits the E-Verify case within three business days. TNCs (rare) route to the head of people, who follows the Further Action Notice workflow.
4. **Storage.** I-9s and E-Verify records stored in Rippling's compliance module, segregated from the general employee record.
5. **Reverification calendar.** Rippling flags upcoming work-authorisation expirations (for H-1B / EAD holders) 90 days in advance. The head of people initiates the reverification workflow.
6. **Retention.** I-9s retained for the statutory period. Rippling manages retention against the schedule.
7. **Annual internal audit.** In Q4, the head of people (with external counsel review) runs the annual internal I-9 audit. Errors are corrected using the M-274-approved technique. The audit report is filed with the corporate record.
8. **NOI response plan.** In the event of an ICE NOI, external immigration counsel (name and contact on the compliance card) is engaged on day one. Rippling produces the full I-9 dataset in the requested format within the three-business-day window.

## Summary

- Every US employer must complete Form I-9 for every new hire — **Section 1 by day one**, **Section 2 within three business days of the first day of employment**.
- The employee chooses which documents from the Lists of Acceptable Documents to present. The employer verifies that the documents reasonably appear genuine and relate to the employee. The USCIS M-274 Handbook is the operating reference.
- Retention: **three years after date of hire, or one year after date of termination, whichever is later**. Store separately from the general personnel file. Electronic storage is fine if it meets 8 C.F.R. § 274a.2(e) requirements.
- Reverification is triggered by expiring work authorisation. Do **not** reverify green cards. Do **not** reverify List B identity documents. Reverification requires a calendar system.
- Remote hires complete Section 2 through an authorised representative (with employer liability) or, if the corporation is E-Verify-enrolled and eligible, through the DHS alternative remote-examination procedure.
- E-Verify is optional federally for most employers, but **mandatory for federal contractors** under FAR 52.222-54 and **mandatory in a specific set of states** including Alabama, Arizona, Florida, Georgia, Mississippi, Missouri, North Carolina, South Carolina, Tennessee, and Utah (subject to state-specific size thresholds and effective-date variations). Confirm current state law.
- E-Verify enrollees have additional obligations — the TNC process, no adverse action during TNC resolution, poster requirements, no pre-hire prescreening, no selective use.
- The HRIS is the operating substrate for I-9 and E-Verify at scale. Insist on native or tight-integration workflow. Doing this on paper does not survive.
- Annual internal audit + response-plan-on-file is the corporation's insurance against ICE NOI exposure.
