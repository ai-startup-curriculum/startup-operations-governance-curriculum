# 4. The mutual IP assignment (PIIA)

> Every founder, every employee, every contractor signs one. Without it, the corporation does not actually own its own product.

## Motivation

The Proprietary Information and Inventions Assignment (PIIA) — sometimes called the Confidential Information and Invention Assignment Agreement (CIIAA), the Employee Invention Assignment and Confidentiality Agreement (EIACA), or an "IP assignment" — is the contract that makes the corporation the owner of the IP its people create. Without a signed PIIA from every contributor who has touched the corporation's code, product, or trade secrets, the corporation has, at best, an implied license to use the work; it does not *own* it. That is fatal at Series-A: no institutional lead investor will fund a company that cannot demonstrate clear title to its own product.

The PIIA is a mutual instrument in the sense that it is a *two-way* set of obligations — the individual assigns work to the corporation, and the corporation acknowledges the individual's prior work and the statutorily-required carveouts. This chapter authors the founder-side PIIA and lays out the anatomy that mod-103 will extend to employees and mod-104 will extend to contractors. The DTSA whistleblower-immunity notice and the trade-secret baseline get their own chapter ([chapter 05](./05-dtsa-whistleblower-and-trade-secret-baseline.md)) because they are their own topic and their own failure mode.

## What the PIIA does

A defensible PIIA does six things:

1. **Assigns IP to the corporation.** Present-assignment language ("hereby assigns," not "will assign") that transfers all right, title, and interest in inventions, works, and know-how created in the course of the individual's work for the corporation.
2. **Confirms copyright work-made-for-hire.** For copyrightable subject matter that qualifies as a "work made for hire" under 17 U.S.C. § 101, confirms that the work vests in the corporation as author; for anything else, assigns the copyright.
3. **Carves out pre-existing inventions.** A schedule of prior work the individual claims is *not* being assigned. This is where the state-law carveouts (Cal. Lab. Code § 2870 and equivalents) attach.
4. **Imposes a confidentiality obligation.** Definition of "confidential information," obligation to use only for the corporation's business, obligation to protect, obligation to return on termination.
5. **Requires disclosure of inventions.** Ongoing obligation to disclose to the corporation any inventions created during service so that the corporation can assess whether they fall under the assignment.
6. **Provides post-termination obligations.** Confidentiality that survives termination; assignment of inventions created within a narrow post-termination window that use corporation confidential information; a covenant not to solicit employees (increasingly narrow due to state law); the DTSA whistleblower notice ([chapter 05](./05-dtsa-whistleblower-and-trade-secret-baseline.md)).

Every founder signs one. Every employee signs one. Every contractor signs one — with contractor-specific work-for-hire language because contractors are not statutory "employees" under the Copyright Act. Every third party who touches the code or trade secrets signs a related NDA or IP assignment.

## Present-assignment language: "hereby assigns," not "will assign"

The one clause that most often breaks a PIIA is the tense of the assignment. Courts have distinguished between:

- **"Employee hereby assigns to the Company"** — a present, automatic assignment that transfers title as inventions are created, without further action.
- **"Employee agrees to assign to the Company"** — a promise to assign in the future, which requires a separate assignment document to actually transfer title.

The Federal Circuit's decision in **Stanford v. Roche**, 583 F.3d 832 (Fed. Cir. 2009), *aff'd on other grounds*, 563 U.S. 776 (2011), held that "agree to assign" language did not automatically transfer patent rights, while a subsequent "hereby assign" agreement with a third party did — with the result that Stanford lost patent rights it thought it owned. The lesson is one word: **use "hereby assigns."** Any drafter who is unfamiliar with the Stanford v. Roche holding is not a drafter who should be authoring PIIA language.

## Copyright work-made-for-hire and the assignment backstop

**17 U.S.C. § 101** defines a "work made for hire" as either:

1. A work prepared by an *employee* within the scope of their employment; or
2. A work specially ordered or commissioned for use as one of nine enumerated categories (contribution to a collective work, part of a motion picture or audiovisual work, translation, supplementary work, compilation, instructional text, test, answer material for a test, atlas) *and* the parties expressly agree in a signed writing that the work is a work made for hire.

For copyright purposes, employee-authored code and content is generally a work made for hire and vests in the corporation as the "author" from the moment of creation. This is why the copyright work-for-hire language in the PIIA works cleanly for founder and employee grants.

**Contractor-created work is not a work made for hire by default** — none of the nine enumerated categories in § 101 includes "software" or "computer code." A commissioned software work by a non-employee contractor is *not* automatically a work made for hire, even if the contract labels it so. This is the origin of the standard belt-and-suspenders drafting: the contractor PIIA (or the equivalent independent-contractor agreement) says (i) the work is a work made for hire *to the extent it qualifies as one under § 101*, and (ii) *to the extent it does not qualify*, the contractor hereby assigns all right, title, and interest in the work to the corporation. This assignment backstop is what actually transfers copyright ownership from the contractor to the corporation.

Founder PIIAs use the same two-step language for the same reason — a founder who works on the product before their formal employment relationship begins (as a paid employee) is arguably not creating "employee" works in the copyright sense until the employment begins, and the assignment backstop covers the pre-employment work.

## The pre-existing invention carveout schedule

Every PIIA has a schedule — variously named "Schedule A," "Exhibit A," "Prior Inventions" — where the individual lists inventions, patents, works of authorship, and trade secrets they claim are *not* being assigned to the corporation. This carveout serves two purposes:

- **It protects the individual's prior work** from being swept into the assignment.
- **It puts the corporation on notice** of what the individual claims to own personally, so that a future dispute over ownership is resolved by reference to the schedule.

The schedule is *fill-in-or-forfeit*. If the individual signs the PIIA without listing prior work, the default position is that no prior work is excluded from the assignment — everything the individual creates during service belongs to the corporation, and any pre-existing work the individual later claims to have brought in is difficult to prove.

For a founder who has been working on the prototype for six months before formation, the schedule is where the pre-formation code, designs, and documentation get identified as prior work. But at the same time, the founder is contributing that pre-formation IP as consideration for their shares (see [chapter 02](./02-founders-restricted-stock-and-repurchase.md)); the schedule and the SPA's consideration language must be *consistent*. The typical structure:

- The founder lists the pre-formation IP on the PIIA carveout schedule (Prior Inventions).
- The founder then executes a separate, express assignment of that same pre-formation IP to the corporation (either inside the PIIA or in a parallel IP assignment agreement) as consideration for the founder's shares.
- Net effect: the founder has both *identified* the pre-existing work (fulfilling the PIIA disclosure discipline) and *assigned* it to the corporation (making the corporation the owner). Nothing is lost in the carveout; the assignment is explicit and traceable.

Documentation matters. If the founder later claims that some code was "their prior work" and was not assigned, the SPA + PIIA + Prior Inventions schedule need to tell a coherent story. Series-A diligence will read all three.

## The state-law invention-assignment carveouts

Several US states have statutes that *require* PIIAs to carve out from any assignment inventions the employee developed entirely on their own time, without using the employer's equipment, supplies, facilities, or trade secrets, unless the invention relates to the employer's business or the employee's work for the employer. These statutes vary in scope but share the same spine.

The most-cited is **California Labor Code § 2870**:

> Any provision in an employment agreement which provides that an employee shall assign, or offer to assign, any of his or her rights in an invention to his or her employer shall not apply to an invention that the employee developed entirely on his or her own time without using the employer's equipment, supplies, facilities, or trade secret information except for those inventions that either: (1) Relate at the time of conception or reduction to practice of the invention to the employer's business, or actual or demonstrably anticipated research or development of the employer; or (2) Result from any work performed by the employee for the employer.

And **§ 2872** requires that the employer provide the employee with a written notification of § 2870 whenever the employer requires the employee to sign an invention-assignment agreement.

Substantially similar carveouts exist in:

- **Delaware** — 19 Del. C. § 805.
- **Illinois** — 765 ILCS 1060/2 (Illinois Employee Patent Act).
- **Kansas** — K.S.A. § 44-130.
- **Minnesota** — Minn. Stat. § 181.78.
- **North Carolina** — N.C. Gen. Stat. § 66-57.1.
- **Utah** — Utah Code § 34-39-3 (Employment Inventions Act).
- **Washington** — RCW 49.44.140.

The Nevada and New Jersey statutes take somewhat different approaches; other states have no invention-assignment carveout statute. <!-- needs-research: Colorado, New York, and other states have moved on invention-assignment carveouts in recent legislative sessions — verify the current state list and citations before publishing a comprehensive multi-state carveout schedule. -->

The standard PIIA drafting response is to include the applicable carveout language and the notification required by § 2872 (for California-based individuals) as an exhibit or schedule to the PIIA. The best practice for a multi-state workforce is to include *all* applicable state-law carveouts on the same schedule, keyed to the individual's state of employment.

Failure to include the required notice does not invalidate the assignment of *inventions that fall inside* the corporation's carveout — it invalidates the assignment as applied to inventions that the statute already excludes. The practical risk is that the individual claims an invention was developed on their own time and does not fall inside the statutory carveout; the required notice being included is what puts the corporation on strong footing to argue that the individual was on notice of exactly what they were assigning and what they were not.

## Confidentiality and the trade-secret hook

The PIIA imposes a confidentiality obligation on the individual with respect to the corporation's "Confidential Information," typically defined broadly to include:

- Technical information (algorithms, source code, architecture, know-how, trade secrets).
- Business information (customer lists, pricing, supplier relationships, financial forecasts, business plans).
- Third-party information the corporation has received under an obligation of confidentiality (customer data, partner data).
- Personnel information (compensation, HR data).

The obligation runs both during and after service. The obligation is what allows the corporation to argue trade-secret protection under the Defend Trade Secrets Act and state trade-secret statutes; without a confidentiality obligation on the individual, the corporation has not "taken reasonable measures" to keep the information secret, which is a required element of a trade-secret claim.

The DTSA-required whistleblower-immunity notice (18 U.S.C. § 1833(b)(3)) attaches at this point in the document. [Chapter 05](./05-dtsa-whistleblower-and-trade-secret-baseline.md) covers it in detail.

## Disclosure, cooperation, and moral rights

Two lower-visibility clauses that still matter:

- **Obligation to disclose inventions.** The individual agrees to disclose to the corporation, promptly and in writing, all inventions made during service so that the corporation can assess whether the invention falls under the assignment. Without this clause, the individual's silence about a potentially-assignable invention creates a downstream ownership dispute.
- **Further-assurances / cooperation clause.** The individual agrees to execute, upon the corporation's request and at the corporation's expense, all documents reasonably necessary to perfect the corporation's ownership (patent filings, copyright registrations, foreign filings, litigation declarations). Combined with a **power-of-attorney** clause that lets the corporation execute such documents on the individual's behalf if the individual is unavailable or refuses. This is what allows the corporation to pursue patents on assigned inventions after the individual has left.
- **Moral rights waiver.** For jurisdictions that recognise moral rights (attribution, integrity) in copyrightable works, the individual waives (or agrees not to assert) those rights to the extent permitted by law. Rarely material in a US-only startup context; becomes material in an international expansion (deferred to [mod-113](../mod-113-international-expansion-and-global-workforce/)).

## Post-termination obligations

The PIIA typically imposes several post-termination obligations, each of which needs to be drafted narrowly to survive as enforceable:

- **Continuing confidentiality.** Indefinite for trade secrets; a defined period (often 2–5 years) for other confidential information; carve-outs for information that becomes public through no fault of the individual.
- **Return of property.** Return of documents, devices, media, and all copies at termination or upon request.
- **Assignment of trailing inventions.** Inventions created within a defined post-termination window (often 6 months to 1 year) that use the corporation's confidential information or arise from work the individual performed for the corporation. This clause should be narrow (relates to the corporation's business, uses confidential information) rather than broad (any invention in any adjacent field).
- **Non-solicitation of employees / customers.** Traditionally a common clause; increasingly limited by state law. California generally does not enforce non-solicits of employees against former California employees ([mod-103](../mod-103-employment-law-and-contract-design/) has depth). Federal Trade Commission activity on non-competes and non-solicits has been significant. <!-- needs-research: verify current federal (FTC final rule on non-competes and its litigation status) and state (Cal. Bus. & Prof. Code § 16600 amendments in 2023–2024, Minnesota's 2023 non-compete ban, and other state changes) landscape before drafting founder-side non-solicit language. -->
- **Non-compete.** Rare in modern startup PIIAs. Enforceability is state-dependent and increasingly limited. Where used, drafted narrowly (specific competitors, defined geography, short duration) and often confined to the executive employment agreement rather than the general PIIA.

The DTSA whistleblower-immunity notice (chapter 05) is what preserves the corporation's ability to seek exemplary damages and attorneys' fees under 18 U.S.C. § 1836(b)(3) for trade-secret misappropriation by an individual who has signed the PIIA. Without the notice, the exemplary-damages remedy is not available. Include the notice.

## Who signs, when, and what happens if they don't

**Who signs:** every founder (on formation day, alongside the SPA); every employee (on the first day of employment, alongside the offer letter and I-9); every contractor (before starting work, as part of the independent-contractor agreement package); every advisor with access to confidential information or working on the product (as part of the advisor agreement).

**When they sign:** *before* they access confidential information or begin creating IP. A PIIA signed after work has begun is enforceable prospectively but the pre-signing work is arguably not covered (or, worse, is covered by state-law default rules that vary in what they mean for pre-agreement work).

**What happens if they don't:**

- If a *founder* has not signed a PIIA: the corporation does not own the founder's contributions. This is fatal at Series-A. The fix is a retroactive PIIA + explicit assignment of all pre-signing work + Prior Inventions schedule with the "prior" work now explicitly assigned.
- If an *employee* has not signed a PIIA: the corporation may still argue that the employee-created work is a work made for hire under 17 U.S.C. § 101 (for copyright) and that the "hired to invent" doctrine or "shop right" applies (for patents), but these are weaker positions than a signed PIIA. Fix: retroactive PIIA, with the same treatment.
- If a *contractor* has not signed a PIIA: the contractor almost certainly *owns* the copyright in what they created ([Community for Creative Non-Violence v. Reid](https://www.law.cornell.edu/supremecourt/text/490/730), 490 U.S. 730 (1989), reaffirmed the § 101 employee-vs-contractor distinction). The corporation may have an *implied license* to use the work for the purpose for which it was commissioned, but does not *own* it. Fix: contact the contractor, execute a retroactive PIIA (or an IP assignment agreement), pay a fee if necessary. If the contractor is unreachable or unwilling, the corporation may have to work around or replace the contractor's contributions. This is one of the sharpest fangs on the Series-A diligence list.

## Concrete example: the founder PIIA and Prior Inventions schedule

Founder A signs the PIIA on 2026-05-15, the same day as the SPA and the § 83(b) filing. The PIIA includes:

- Present-assignment language: "Founder hereby irrevocably assigns to the Corporation all right, title, and interest..."
- Work-made-for-hire language for copyrightable works, with an assignment backstop for anything that does not qualify.
- Confidentiality obligation with a broad definition of Confidential Information, running during and after service.
- DTSA whistleblower-immunity notice (chapter 05) in the confidentiality section.
- Cal. Lab. Code § 2870 carveout and § 2872 notice (Founder A is based in California).
- Prior Inventions schedule ("Schedule A") listing three items:
  - "pyfast-tokenizer" — an open-source Python library authored by Founder A pre-formation, released under Apache-2.0, unrelated to the corporation's business. Retained by Founder A; not assigned.
  - "Founder A blog and personal website (fictional-name.dev)" — personal writing, unrelated to the corporation's business. Retained by Founder A; not assigned.
  - "acme-prototype-v0" — pre-formation prototype code that is the direct basis for the corporation's product. **Assigned** to the corporation (referenced separately in the SPA's consideration section and in the parallel IP Assignment Agreement executed on the same day).
- Further-assurances / power-of-attorney clause covering patent and copyright perfection.
- Post-termination assignment of trailing inventions within 6 months that use corporation confidential information.

The corporation archives the executed PIIA in the corporate record. On the same day, the founder-employment relationship is documented ([chapter 07](./07-founder-employment-relationship-and-departure.md)) with a signed offer letter that references the PIIA. Every subsequent employee follows the same template on day one. Every contractor follows the contractor variant.

## Diligence reads the whole package

At Series-A, diligence will ask for a table (often called an "IP schedule" or "personnel matrix") listing every current and former founder, employee, and contractor, with a "PIIA signed?" column, the date signed, and the file location. Any "no" or blank entry is a defect. The retroactive-cleanup work — chasing signatures, negotiating with departed contractors, sometimes buying out prior work — is one of the more time-consuming pre-closing tasks.

The prevention discipline is the checklist: no access to code or confidential information without a signed PIIA. The corporate secretary owns the tracker. HR onboarding integrates the PIIA into the day-one paperwork ([mod-104](../mod-104-hiring-onboarding-and-hr-operations/) has depth). External counsel or the corporate secretary reviews the executed PIIA for completeness (Prior Inventions schedule filled in, DTSA notice present, present-assignment language, applicable state carveouts included).

## Summary

- The PIIA is the contract that makes the corporation the owner of the IP its people create. Without it, the corporation has, at best, an implied license — not ownership.
- Use **present-assignment** language ("hereby assigns"), not future-promise language ("agrees to assign"). See *Stanford v. Roche*, 583 F.3d 832 (Fed. Cir. 2009).
- Copyright work-made-for-hire under 17 U.S.C. § 101 covers employee works; use a work-for-hire + assignment-backstop belt-and-suspenders drafting for founder and contractor works.
- Every PIIA includes a **Prior Inventions schedule** — fill in or forfeit.
- Include the state-law invention-assignment carveouts (Cal. Lab. Code § 2870, Del. § 805, Ill. 765 ILCS 1060, and the analogous statutes in Kansas, Minnesota, North Carolina, Utah, Washington) — and the required § 2872 notice for California individuals.
- Include the DTSA whistleblower-immunity notice ([chapter 05](./05-dtsa-whistleblower-and-trade-secret-baseline.md)) so the exemplary-damages remedy stays on the table.
- Every founder, employee, and contractor signs before they touch code or confidential information. Retroactive PIIAs work but are more expensive and less clean than the day-one discipline.
