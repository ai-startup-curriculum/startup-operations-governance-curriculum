# 4. The employee PIIA

> Every founder signed one on formation day ([mod-102 chapter 04](../mod-102-founding-team-legal-architecture/04-piia-mutual-ip-assignment.md)). Every employee signs one on day one. Without it, the corporation does not actually own the code its people write.

## Motivation

The Proprietary Information and Inventions Assignment (PIIA) for employees is the direct extension of the founder-side PIIA authored in [mod-102 chapter 04](../mod-102-founding-team-legal-architecture/04-piia-mutual-ip-assignment.md). The mechanics are the same: present-assignment language ("hereby assigns"), work-made-for-hire + assignment backstop, Prior Inventions schedule, state-law invention-assignment carveouts, DTSA whistleblower-immunity notice, confidentiality obligations that survive termination, and further-assurances / power-of-attorney language for perfecting the corporation's ownership.

This chapter does not re-teach the founder-side chapter. Instead it authors the parts that are *different* for the employee context: the drafting pattern for pre-employment invention carveouts that preserve a genuine side project without dragging it into corporate ownership; the operational discipline of getting every employee to sign before they touch code; the standardised, no-negotiation posture for junior hires; the accommodations for senior hires who arrive with meaningful pre-existing IP; the multi-state carveout pattern for a remote-first workforce; and the Series-A "personnel matrix" that the corporation will be asked to produce.

Read [mod-102 chapter 04](../mod-102-founding-team-legal-architecture/04-piia-mutual-ip-assignment.md) first for the underlying anatomy. This chapter picks up where that one left off.

## What the employee PIIA does — recap

Six things, same as the founder PIIA:

1. **Assigns IP to the corporation** via present-assignment language (*Stanford v. Roche*, 583 F.3d 832 (Fed. Cir. 2009) — "hereby assigns," not "will assign").
2. **Confirms copyright work-made-for-hire** under 17 U.S.C. § 101, with an assignment backstop for anything that does not qualify. For W-2 employees the § 101 employee-authored-work path is generally strong; the backstop is defensive.
3. **Carves out pre-employment inventions** on a schedule (Schedule A / Prior Inventions).
4. **Imposes confidentiality obligations** on the corporation's Confidential Information, running during and after service.
5. **Requires disclosure of inventions** made during service.
6. **Provides post-termination obligations** — continuing confidentiality, return of property, assignment of trailing inventions using confidential information, and the state-law-adjusted non-solicitation / non-compete surface treated in [chapter 06](./06-non-compete-landscape-and-alternatives.md).

Every employee — engineer, PM, designer, marketer, salesperson, HR person, finance person, operations person, executive assistant — signs one. Every advisor, intern, and contractor signs an equivalent document with the appropriate variant language ([chapter 03](./03-offer-letter-architecture-and-pay-transparency.md) covers the cross-referencing pattern).

## The when: day one, before access

The employee PIIA must be signed **on or before the start date, before the employee is granted access to code, systems, or confidential information**. This ordering is critical for two reasons:

- **Consideration.** The employment itself is the consideration for the PIIA. Signing the PIIA on the start date, alongside the offer letter and the I-9, means the PIIA is supported by the initial employment as consideration. A PIIA signed after employment has begun requires additional consideration (a bonus, a raise, continued employment for some period) to be enforceable in some states — a doctrine most restrictively applied in states like Illinois that require adequate consideration for restrictive covenants. Signing at the start avoids the additional-consideration question.
- **Coverage of the first day's work.** Any work the employee performs, or confidential information they access, before signing the PIIA is arguably outside the PIIA's coverage. A signed PIIA prospectively covers work from the effective date; retroactive coverage is arguable but never as clean.

Operationally, the on-boarding checklist bundles the offer letter, the PIIA, the arbitration agreement (if any), the I-9, and other day-one paperwork into a single packet the employee signs before their laptop is provisioned and before their access to code repositories and internal systems is granted. HR and IT are the enforcers of this ordering; the PIIA-first rule is one of the few day-one hard gates that should never be waived.

## The pre-employment invention carveout: preserving genuine side projects

The single most common negotiation on an employee PIIA — especially for engineers, researchers, and product-people arriving from other technology companies — is the Prior Inventions schedule.

The corporation's default posture: *fill it in or forfeit it.* The employee signs the PIIA with a blank schedule at their own risk; anything they later claim was "prior work" is presumptively covered by the assignment.

The employee's genuine interest: *list every pre-existing project, open-source contribution, personal website, and technical writing they want to keep as their own.* A well-run corporation supports this listing because it protects both sides:

- The corporation gets a clean, documented record of what the employee is *not* assigning — so a downstream dispute about ownership is resolved by reference to the schedule.
- The employee's side projects and open-source contributions are protected from being swept into the corporation's ownership.
- The employee is put on notice, in writing, of what they *are* assigning: everything else made during service.

The drafting pattern that keeps a side project a side project without dragging it into corporate ownership has four components:

1. **List the specific project on the schedule** with enough detail to identify it: name, brief description, current state (public GitHub URL, private repo, personal blog, etc.).
2. **Confirm the project relates to a field distinct from the corporation's business.** This tracks the California Labor Code § 2870 carveout: an invention that "does not relate to the employer's business or actual or demonstrably anticipated research or development" is not assignable to the employer even if the employee developed it during the employee's tenure.
3. **Confirm the employee will not use the corporation's equipment, supplies, facilities, or trade secret information on the project.** This tracks the second half of § 2870. Working on a side project from a corporate laptop, on corporate wifi, in corporation-issued Google Docs, taints the project.
4. **Confirm the corporation acknowledges the side project.** A short "the Company acknowledges the following as prior work of the Employee not assigned hereby" recital on the schedule, initialed by the corporation's authorised signer, gives the employee a clean record.

**When a side project genuinely relates to the corporation's business**, no clever drafting can save it. If a corporation making enterprise-collaboration software hires an engineer with a personal open-source collaboration library, and the engineer continues to develop the library during the employment, the library falls inside the corporation's scope under Cal. Lab. Code § 2870(a)(1) and inside the PIIA's assignment. The employee has three genuine options: (i) fully assign the library to the corporation as prior work identified on the schedule, (ii) stop working on the library during the employment, or (iii) not join the corporation.

For a senior hire who arrives with genuinely meaningful pre-existing IP — a patent portfolio, published research, a company-relevant open-source project — the offer negotiation should surface this early and the corporation may agree to (i) a specific license grant from the employee to the corporation for pre-existing IP, (ii) a broader carveout for continued personal work on defined pre-existing projects, or (iii) an outright acquisition of pre-existing IP for consideration. All three arrangements are documented in a side letter or amendment to the PIIA, and the amendment goes into the personnel file.

## The state-law invention-assignment carveout schedule

[Mod-102 chapter 04](../mod-102-founding-team-legal-architecture/04-piia-mutual-ip-assignment.md) catalogues the state statutes: California Labor Code § 2870, Delaware 19 Del. C. § 805, Illinois 765 ILCS 1060/2, Kansas K.S.A. § 44-130, Minnesota Minn. Stat. § 181.78, North Carolina N.C. Gen. Stat. § 66-57.1, Utah Utah Code § 34-39-3, Washington RCW 49.44.140. Each statute exempts from any employee assignment inventions the employee developed on their own time, without using the employer's resources, unless the invention relates to the employer's business or the employee's work for the employer.

For a *remote-first, multi-state workforce*, the practical drafting choice is one of:

- **The California-plus multi-state schedule.** Include the California § 2870 language and the § 2872 written-notification requirement, plus an appended list of every applicable state's carveout, keyed to the employee's state of residence at the time of signing. This is the highest-common-denominator posture for a corporation that does not want to maintain a per-state PIIA library.
- **The per-state PIIA library.** Maintain a distinct PIIA template for each state where the corporation has employees, with the applicable state's carveout language embedded. This is administratively heavier but produces documents that read cleanly for each employee and each auditor.

The corporation's HR-operations team ([mod-104](../mod-104-hiring-onboarding-and-hr-operations/)) usually owns the choice of library vs. multi-state posture. The important thing is that *for every employee, the applicable state carveout is present in the PIIA they signed.* An employee based in California who signed a PIIA that does not include the § 2872 notice is entitled to argue that the assignment as applied to their own-time-and-resources inventions is unenforceable.

## The DTSA whistleblower-immunity notice — verbatim

The Defend Trade Secrets Act's whistleblower-immunity notice (18 U.S.C. § 1833(b)(3)) is a **verbatim inclusion** in every employee PIIA. Without it, the corporation's enhanced-damages remedy (exemplary damages up to 2× compensatory, plus attorneys' fees) under 18 U.S.C. § 1836(b)(3)(C)–(D) is unavailable in any trade-secret misappropriation action against that employee.

The notice is short. Standard-form language:

> **Notice of Immunity from Liability.** Pursuant to 18 U.S.C. § 1833(b), you are hereby notified that:
>
> (1) **Immunity.** An individual shall not be held criminally or civilly liable under any federal or state trade secret law for the disclosure of a trade secret that (A) is made in confidence to a federal, state, or local government official, either directly or indirectly, or to an attorney, and solely for the purpose of reporting or investigating a suspected violation of law; or (B) is made in a complaint or other document filed in a lawsuit or other proceeding, if such filing is made under seal.
>
> (2) **Use of Trade Secret Information in Anti-Retaliation Lawsuit.** An individual who files a lawsuit for retaliation by an employer for reporting a suspected violation of law may disclose the trade secret to the attorney of the individual and use the trade secret information in the court proceeding, if the individual (A) files any document containing the trade secret under seal; and (B) does not disclose the trade secret, except pursuant to court order.

The notice belongs in the PIIA's confidentiality section, adjacent to the definition of Confidential Information and the trade-secret protection language. Every corporation using a PIIA that lacks this notice is systematically leaving one of its main trade-secret remedies on the table. Fix it in the template.

[Mod-102 chapter 05](../mod-102-founding-team-legal-architecture/05-dtsa-whistleblower-and-trade-secret-baseline.md) covers the DTSA remedy stack and the "reasonable measures" program that supports a trade-secret claim in more depth.

## The confidentiality obligation and its exceptions

The confidentiality obligation runs during and after service. Standard structure:

- **Definition of Confidential Information.** Broad and specific. Includes (i) technical information — source code, algorithms, architecture, know-how, trade secrets, unpublished research; (ii) business information — customer lists, pricing strategy, sales pipelines, supplier relationships, financial forecasts, business plans; (iii) third-party confidential information the corporation has received under obligations of confidentiality; (iv) personnel information — compensation, HR data, medical / disability records.
- **Obligation.** The employee (i) will hold Confidential Information in strict confidence; (ii) will use it only for the corporation's business; (iii) will not disclose it to third parties without authorisation; (iv) will take reasonable measures to protect it (encryption, secure storage, credential hygiene, etc.).
- **Standard exceptions.** The obligation does not extend to information that: (a) was already in the employee's possession or already known to the employee free of any obligation of confidentiality before the disclosure; (b) is or becomes publicly known through no fault of the employee; (c) is independently developed by the employee without use of Confidential Information; (d) is disclosed pursuant to court order or legal process, subject to prior written notice to the corporation where legally permissible; or (e) is disclosed pursuant to the whistleblower protections above.
- **Duration.** Indefinite for trade secrets; a defined period (often 2–5 years) for non-trade-secret Confidential Information. Some jurisdictions read indefinite non-trade-secret confidentiality obligations narrowly; the defined-period pattern is safer.
- **Return of materials on termination.** The employee agrees to return all Confidential Information and property (documents, devices, media, electronic files) at termination or on request.

**A subtle but important point.** Overly broad confidentiality obligations that would prohibit disclosure of the employee's own wages, benefits, working conditions, or complaints about workplace conditions can violate Section 7 of the National Labor Relations Act (29 U.S.C. § 157) — the right to engage in "concerted activity for mutual aid or protection" — as interpreted by the NLRB in a series of decisions (culminating in *Stericycle, Inc.*, 372 NLRB No. 113 (2023)). <!-- needs-research: verify the current NLRB standard for workplace confidentiality rules after Stericycle and any subsequent Board or Circuit decisions before publishing a specific confidentiality-clause template. --> The confidentiality clause should carve out (or the corporation's overall workplace-rules policy should acknowledge) the right to discuss wages, working conditions, and to file complaints with government agencies. This carveout also matters for the SEC whistleblower rules (Dodd-Frank § 21F, 17 C.F.R. § 240.21F-17) which prohibit any action that "impedes" whistleblower reporting.

## The disclosure and cooperation clauses

Two obligations that most employees rarely think about but that matter operationally:

- **Ongoing invention disclosure.** The employee agrees to disclose to the corporation, promptly and in writing, all inventions made during service so that the corporation can determine whether the invention is subject to the PIIA's assignment. The disclosure obligation catches inventions the employee made "on their own time" that might or might not fall inside a state-law carveout — the corporation gets to make the coverage call rather than the employee.
- **Further-assurances / cooperation and power-of-attorney.** The employee agrees to execute, upon the corporation's request and at the corporation's expense, all documents reasonably necessary to perfect the corporation's ownership — patent filings, copyright registrations, assignments to foreign patent offices, litigation declarations. The power-of-attorney clause allows the corporation to sign such documents on the employee's behalf if the employee is unavailable, unreachable, or refuses. This is what allows the corporation to pursue patent perfection after the employee has left.

Both clauses are boilerplate — but they are boilerplate the corporation genuinely needs. Leave them out and you have to chase former employees at patent-application time.

## The post-termination surface

The PIIA's post-termination obligations are where the enforceability landscape gets state-specific. The general categories:

- **Continuing confidentiality.** Indefinite for trade secrets; defined period for other confidential information. Universally enforceable subject to the NLRB and SEC whistleblower carveouts above.
- **Return of property.** Unlimited in duration; universally enforceable.
- **Assignment of trailing inventions.** Post-termination inventions that use the corporation's confidential information, or that were substantially conceived during service, are assigned. Narrow drafting matters — a broad "any invention in any adjacent field for one year" is unenforceable in many states. The Cal. Lab. Code § 2870 carveout continues to constrain the corporation's reach.
- **Non-solicitation of employees.** Common in the PIIA. California generally does not enforce employee non-solicits against former California employees (*AMN Healthcare, Inc. v. Aya Healthcare Services, Inc.*, 28 Cal. App. 5th 923 (2018)) unless narrowly drawn as a trade-secret-protection measure. Other states enforce more readily. [Chapter 06](./06-non-compete-landscape-and-alternatives.md) covers the surviving-defaults landscape.
- **Non-solicitation of customers.** Similar state-dependence.
- **Non-compete.** Rare in modern employee PIIAs. Where present, drafted narrowly and typically confined to senior executives via a separate executive employment agreement. See [chapter 06](./06-non-compete-landscape-and-alternatives.md).

The trend across states is toward *narrower* post-termination restrictive covenants. Overreaching drafting invites judicial "blue-pencilling" (some states rewrite the clause narrower; others simply void the clause entirely) and increases the probability that the corporation will lose the whole surviving obligation set — including the confidentiality and trade-secret protections that would have held up on their own. Draft narrowly to preserve what the corporation genuinely needs.

## Signing pattern and record-keeping

The signed PIIA lives in the employee's personnel file, retained for the duration of employment plus the applicable retention period (federal FLSA record-retention is three years; some state-specific rules extend beyond that; corporations often retain personnel files for the longer of seven years post-termination or the state statute of limitations for the longest-running employment claim).

The Series-A diligence checklist will include a **personnel matrix** — a table listing every current and former employee, contractor, and advisor, with columns for: name, start date, end date (if applicable), state of employment, PIIA signed (Y/N and date), applicable state carveout schedule included (Y/N), Prior Inventions schedule completed (Y/N), NDA / arbitration / handbook acknowledgement signed (Y/N and date), file location. A blank cell is a defect. A "no" is a defect. The corporation should build and maintain this matrix from day one, not scramble to produce it at diligence.

## What happens if an employee did not sign the PIIA

The failure modes are analogous to the founder and contractor cases from [mod-102 chapter 04](../mod-102-founding-team-legal-architecture/04-piia-mutual-ip-assignment.md):

- **Employee-created work.** For W-2 employees, copyright work-for-hire under 17 U.S.C. § 101 attaches automatically to work made in the scope of employment. The corporation has a strong argument for copyright ownership even without a signed PIIA. For patents, the "hired to invent" doctrine or the "shop right" gives the corporation a nonexclusive license or ownership depending on the facts, but this is a weaker position than a signed present-assignment PIIA. Trade-secret protection is degraded without the confidentiality obligation.
- **Retroactive PIIA.** The corporation approaches the employee, explains the gap, and asks them to sign a PIIA now. Most current employees will sign. The retroactive PIIA typically includes explicit ratification language covering pre-signing work. The consideration question is state-specific; some states accept continued employment as sufficient consideration, others require additional consideration (a nominal bonus, a raise, an equity grant).
- **Departed employees.** Harder. The corporation contacts them, explains the ask, offers modest consideration (a small cash payment, an acknowledgement of continued equity vesting on a specific schedule) in exchange for signing the retroactive PIIA. If the departed employee refuses, the corporation is left with the implied-license / work-for-hire posture on the work the employee performed. Series-A diligence will note the gap.
- **Departed contractors** (see also [mod-102 chapter 04](../mod-102-founding-team-legal-architecture/04-piia-mutual-ip-assignment.md)). This is the sharpest exposure — copyright ownership does not automatically pass to the corporation for contractor-created work.

The prevention discipline is the day-one rule: no code access, no confidential-information access, no first-day work without a signed PIIA.

## Concrete example: the day-one PIIA for a new engineer

Ravi joins Acme Robotics as a full-stack engineer, San Francisco-based. On his start date, HR delivers a signed on-boarding packet:

- Executed offer letter ([chapter 03](./03-offer-letter-architecture-and-pay-transparency.md)).
- Signed PIIA, with the following contents:
  - Present-assignment language: "Employee hereby irrevocably assigns to the Company..."
  - Work-made-for-hire language for copyrightable works, with assignment backstop.
  - Confidentiality obligation with broad Confidential Information definition, defined-period non-trade-secret protection (3 years post-termination), indefinite trade-secret protection, and NLRA/SEC-whistleblower carveouts.
  - DTSA whistleblower-immunity notice (verbatim from 18 U.S.C. § 1833(b)(3)).
  - Ongoing invention-disclosure obligation.
  - Further-assurances / cooperation and power-of-attorney clause.
  - Cal. Lab. Code § 2870 carveout and § 2872 written notice.
  - Non-solicitation of employees for 12 months post-termination (California-narrowed, drafted as a trade-secret-protection measure).
  - No non-compete.
  - Prior Inventions Schedule (Schedule A): Ravi lists:
    - "goroutine-viz" — Ravi's open-source Go concurrency visualiser, developed pre-Acme, released under MIT, unrelated to Acme's business (robotics control software). Retained by Ravi; not assigned. Ravi will not use Acme equipment or trade secrets on continued work.
    - Ravi's personal blog at "ravi-writes.dev" — technical writing on general software topics, unrelated to Acme's business. Retained by Ravi.
    - No other inventions.
- Signed Mutual Arbitration Agreement ([chapter 09](./09-arbitration-and-class-action-waivers.md)), if the corporation uses one.
- Completed I-9 with document copies retained per USCIS rules.
- Signed employee handbook acknowledgement, with the acknowledgement re-stating at-will and confirming the handbook does not create a contract.

The signed PIIA is scanned and archived in Ravi's personnel file. HR marks the personnel-matrix row: Ravi Patel, start date, San Francisco, PIIA signed [date], Cal. § 2870 carveout Y, Prior Inventions completed Y, all standalone agreements Y. IT provisions Ravi's laptop and grants repository access.

At Series-A eighteen months later, Ravi's row on the personnel matrix reads clean.

## The exec-hire negotiation pattern

Senior engineering, product, or executive hires arriving from other technology companies frequently ask to negotiate the PIIA. Common asks:

- **Broader Prior Inventions listing.** Executive lists a broad category of pre-existing patents, open-source projects, or investments. Corporation reviews and can accept, narrow, or negotiate specific carve-in / carve-out language.
- **Personal-investment protection.** Executive is an angel investor and wants the PIIA to acknowledge that passive investing in non-competitive companies is not a conflict of interest. Corporation typically accepts subject to a defined scope (passive minority investments in non-competing businesses, with a size cap and a defined disclosure protocol).
- **Board-service protection.** Executive wants to continue serving on outside boards. Corporation typically requires disclosure and approval by the CEO or Board, and requires the outside board seat not to compete with the corporation. See also [mod-102 chapter 06](../mod-102-founding-team-legal-architecture/06-founder-conflict-of-interest.md) on the founder-side loyalty baseline.
- **Non-competition softening.** Executive resists a non-compete. In California this is moot — the non-compete is unenforceable anyway. In enforceable states, the negotiation is real and typically resolves via a narrow non-solicit or a garden-leave arrangement ([chapter 06](./06-non-compete-landscape-and-alternatives.md)).
- **Trailing-inventions narrowing.** Executive resists a broad "any invention within 12 months post-termination" clause. Corporation narrows to inventions that use the corporation's confidential information or were substantially conceived during service.
- **Confidentiality-period narrowing.** Executive resists indefinite confidentiality for non-trade-secret information. Corporation shortens the non-trade-secret period to 2–3 years.

Junior hires do not typically negotiate the PIIA. The corporation offers a standardised, no-negotiation-position document, and the recruiter and HR are trained to explain (i) that the PIIA is standard, (ii) that the Prior Inventions schedule is the employee's opportunity to preserve their own pre-existing work, and (iii) that the corporation is happy to answer specific questions but does not change the boilerplate for junior roles.

## Summary

- The employee PIIA is the direct extension of the founder PIIA ([mod-102 chapter 04](../mod-102-founding-team-legal-architecture/04-piia-mutual-ip-assignment.md)) — present-assignment language, work-for-hire plus backstop, Prior Inventions schedule, state-law carveouts, DTSA whistleblower notice, confidentiality, disclosure, cooperation, and narrow post-termination obligations.
- Every employee signs on or before the start date, before access to code or confidential information is granted. Signing at start avoids the additional-consideration question for restrictive covenants that would arise if the PIIA were signed later.
- The Prior Inventions schedule is where the employee lists side projects, open-source contributions, and personal writing they want to keep as their own. Drafting pattern: list the project specifically, confirm it does not relate to the corporation's business, confirm no use of corporation equipment or trade secrets, get corporation acknowledgement on the schedule.
- For a remote-first multi-state workforce, include the applicable state-law invention-assignment carveouts (Cal. Lab. Code § 2870 with § 2872 written notice, plus Delaware, Illinois, Kansas, Minnesota, North Carolina, Utah, Washington equivalents) keyed to the employee's state of residence.
- Include the DTSA whistleblower-immunity notice verbatim (18 U.S.C. § 1833(b)(3)) — without it, the enhanced-damages remedy is unavailable.
- Confidentiality obligations must carve out the employee's right to discuss wages, working conditions, and to report to government agencies (NLRA § 7 as interpreted by *Stericycle*, and SEC / Dodd-Frank § 21F whistleblower rules).
- Post-termination restrictive covenants (non-solicits, non-competes, trailing-invention assignments) are state-specific and increasingly narrow. See [chapter 06](./06-non-compete-landscape-and-alternatives.md) for the current landscape.
- The signed PIIA is archived in the personnel file and appears on the Series-A personnel matrix. No blank cells; no "no" answers. The prevention discipline is day-one enforcement of the "no PIIA, no access" rule.
