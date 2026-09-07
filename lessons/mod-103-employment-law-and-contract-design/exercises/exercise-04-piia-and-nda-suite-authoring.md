# Exercise 04 — PIIA and NDA suite authoring

> Estimated time: **~5 hours** · Related chapters: [04 — The employee PIIA](../04-employee-piia.md), [05 — NDAs and MNDAs](../05-nda-and-mnda-layer.md)

## Problem statement

The offer letters from exercise 03 reference two standalone documents that must be executed on or before start date: (a) the **employee PIIA** and (b) the **arbitration agreement** (exercise 08). This exercise authors the employee PIIA package, plus the NDA / MNDA suite the corporation uses in its customer, vendor, candidate / recruit, and investor conversations. Both the PIIA (which is signed by every employee) and the NDAs (which are signed transactionally) are the corporation's day-to-day confidentiality and IP-protection paper.

You are the incoming COO / GC and you have four hires signing offer letters this week, plus a pipeline of customer POCs, vendor engagements, candidate interviews, and investor conversations. You are producing (a) an employee PIIA suite covering the four hires and the corporation's broader workforce, (b) a mutual NDA (MNDA) for two-way commercial conversations, (c) a one-way inbound NDA for the corporation's information disclosed to counter-parties, (d) a candidate / recruit NDA for late-stage interviews where confidential information may be shared, and (e) an investor-facing NDA (with an honest assessment of whether investors will sign one, per chapter 05).

## Facts

- **Corporation.** Acme Robotics, Delaware C-corp, principal place of business San Francisco. Employs in CA, NY, WA, CO, IL, MA, TX.
- **Four hires from exercise 03** — SWE in SF, Head of Marketing in LA, EA to CEO in SF, Enterprise SDR in Seattle. Each needs the employee PIIA per their state.
- **Broader workforce.** ~25 additional W-2 employees across the listed states. The corporation's current PIIA is a "founder-era" copy of a template found on a public forms site; it has "agrees to assign" language (not "hereby assigns"), no DTSA notice, no state-specific carveouts, and a broad non-compete that is void in California.
- **Q4 customer POCs.** Three enterprise POCs with prospects — one Fortune-500 healthcare-adjacent buyer, one bank, one consumer-tech company. The bank is likely to demand mutual NDA with strong dispute-resolution provisions.
- **Q4 vendor engagements.** New CRM vendor, new payroll vendor, new HRIS vendor. Each will share information both ways.
- **Candidate pipeline.** ~15 senior-role candidates in-flight (SWEs, engineering-leadership candidates, VP-level product and marketing candidates). The corporation shares confidential product / go-to-market information in the late stages of interviews.
- **Investor conversations.** The corporation is in early Series-A conversations with three VC firms.

## Requirements

### Part A — Employee PIIA (national template + state riders)

Author the corporation's employee PIIA. The chapter 04 baseline (which extends the mod-102 founder PIIA) is the standard. The PIIA must include:

1. **Recital, effective date, definitions.** Corporation, employee, effective date, definitions of Confidential Information, Prior Inventions, Assigned Inventions, Company Materials.
2. **Present-assignment language** — "hereby assigns" (not "agrees to assign") for all Assigned Inventions per *Stanford v. Roche Molecular Systems, Inc.*, 583 F.3d 832 (Fed. Cir. 2009), aff'd, 563 U.S. 776 (2011).
3. **Work-made-for-hire language** for copyrightable subject matter that qualifies under 17 U.S.C. § 101, *plus an assignment backstop* for anything that does not qualify.
4. **Confidential-information definition** — technical, business, financial, third-party, personnel information; the employee's obligation to use only for the corporation's benefit; the obligation to protect; the obligation to return on termination.
5. **Ongoing duty to disclose inventions.**
6. **Further-assurances and power-of-attorney clause** for patent and copyright perfection.
7. **Moral-rights waiver** to the extent permitted; note in the design memo that this is largely a non-issue for US-only employees but becomes material for international-workforce PIIA templates (mod-113).
8. **Post-termination confidentiality** — indefinite for trade secrets; a defined period (typically 3–5 years) for other Confidential Information.
9. **DTSA whistleblower-immunity notice** — 18 U.S.C. § 1833(b)(3), with the specific statutory language from the chapter 04 baseline. Also address § 1833(b)(1) and (b)(2) mechanics. Include the express carve-out that the DTSA notice does not impair any employee's right to (i) file a charge with the EEOC, NLRB, SEC, or other agency, (ii) engage in NLRA-protected concerted activity, or (iii) participate in a government investigation.
10. **Prior Inventions schedule** — with the "fill-in-or-forfeit" framing per chapter 04.
11. **State-law invention-assignment carveout schedule** — see Part B.
12. **Non-solicitation covenants** — see Part C.
13. **Non-compete language** — see Part D. (Spoiler: for most of these employees, none.)
14. **Trailing-inventions assignment** — a narrow post-termination window (e.g., 6 months) limited to inventions using Confidential Information or substantially conceived during service. Justify the window against chapter 04's guidance.
15. **Return of property on termination.**
16. **Cooperation clause** — post-termination cooperation on IP / trade-secret matters (subject to reasonable expense reimbursement).
17. **Assignment / successor clause.**
18. **Severability.**
19. **Signature block.**

### Part B — State-law invention-assignment carveout schedule

Include the applicable state-law carveout language for each state the corporation employs in. Per chapter 04's state list, at minimum:

- **California** — Cal. Lab. Code § 2870 carveout plus § 2872 written notification. Include the specific statutory text or a compliant summary.
- **Illinois** — 765 ILCS 1060/2 (Illinois Employee Patent Act).
- **Washington** — RCW 49.44.140.
- **Delaware, Minnesota, Kansas, North Carolina, Utah** — include as applicable if the corporation employs in any of these states now or in the near-term hiring plan. Cite the statute for each.

Note in the design memo that Colorado, Nevada, New Jersey, and Nevada have been active on invention-assignment reform (or adjacent restrictive-covenant reform); flag the current-state list as a `<!-- needs-research -->` item and describe the compliance posture for those states (default to state carveout language equivalent to the § 2870-Washington-Illinois template pending statutory clarity).

### Part C — Non-solicitation covenants

Include the chapter 06 non-solicitation architecture in the PIIA:

- **Employee non-solicit** — 12 months post-termination, limited to employees the departing employee worked with in the last 12 months of employment. Not enforceable in California (per *AMN Healthcare*); state the California carve-out or omit the covenant for California employees entirely.
- **Customer non-solicit** — 12 months post-termination, limited to customers the departing employee worked with in the last 12 months of employment. Narrow trade-secret framing for California employees.
- **Illinois Freedom to Work Act** — non-solicit void for employees earning under $45,000/year. For any Illinois employee in the roster whose compensation is below this threshold, the covenant must be omitted.

### Part D — Non-compete decision

Author the corporation's decision on whether to include a non-compete in the standard employee PIIA. Chapter 06 recommends "no non-compete for rank-and-file employees; narrow non-compete for senior executives in states that enforce them." Apply that recommendation to the four Q4 hires and the broader workforce.

For any senior executive (VP-and-above) who receives a non-compete in the executive employment agreement:

- **Not in California** (§ 16600 voids; SB 699 voids across state lines).
- **Massachusetts** requires notice ≥10 business days before start, garden-leave pay per G.L. c. 149 § 24L, and other formalities.
- **Washington** requires disclosure at time of offer and RCW 49.62 earnings-threshold compliance.
- **Illinois** requires 14 calendar days before start and earnings-threshold compliance per 820 ILCS 90.
- **Colorado** requires C.R.S. § 8-2-113 formalities and earnings-threshold compliance.
- **New York** — check current status per chapter 06.

You do not need to draft the executive-agreement non-compete text (it is a separate document); you need to state the corporation's decision on which roles receive one and under what conditions.

### Part E — Retroactive-cleanup plan for existing workforce

The corporation's current PIIA is defective (see Facts). Produce a plan to migrate the existing ~25-employee workforce to the new PIIA suite:

1. **Notice and consideration.** The existing employees are being asked to sign a new PIIA. In most states, "continued employment" is sufficient consideration for existing employees; some states (Illinois, Massachusetts) require additional consideration. Address per state.
2. **Communication.** How you communicate the change — the reasons (Series-A diligence readiness, DTSA notice compliance, present-assignment language, state-law carveout correctness), the process (review, questions to HR / counsel, signing window).
3. **The California employees' non-compete cleanup.** Cal. Bus. & Prof. Code § 16600.1 (AB 1076) requires the corporation to notify California employees in writing that any prior non-compete clause is void. The corporation missed the February 14, 2024 deadline; the remediation posture is late compliance. Draft the notice.
4. **The existing PIIA's "agrees to assign" defect.** Because the corporation has been operating on "agrees to assign" language, its ownership of specific inventions authored under the defective PIIA is contestable per *Stanford v. Roche*. Address whether re-execution retroactively fixes the assignment, whether a separate express assignment is required for each Assigned Invention, and what the diligence posture is at Series-A.

### Part F — Mutual NDA (MNDA) for commercial conversations

Draft a mutual NDA for two-way commercial conversations. The template will be used with the bank prospect in Part I (below) and with vendor counter-parties. Include:

1. **Recital, definition of Confidential Information, definition of the Purpose.**
2. **Standard exceptions** per chapter 05 — already-known, publicly-available, independently-developed, third-party received without confidentiality obligation, compelled disclosure (with notice and cooperation obligations).
3. **Term.** Confidentiality obligations survive for a defined period (typically 3–5 years); trade-secret obligations survive as long as the information qualifies as a trade secret under DTSA and applicable state law.
4. **No-license clause.** Disclosure does not grant a license to intellectual property.
5. **Return / destruction of Confidential Information.**
6. **No-warranty clause.**
7. **Dispute-resolution provisions.** Governing law (Delaware or California per chapter 05's guidance), venue, injunctive-relief availability, attorneys' fees (mutual).
8. **Employee-facing carve-outs.** The counter-party's employees remain free to file agency charges, engage in NLRA-protected activity, and exercise DTSA whistleblower immunity.
9. **No non-solicit within the NDA.** Non-solicit obligations belong in the commercial contract, not the NDA. Note this in the design memo.
10. **Signature block.**

### Part G — One-way inbound NDA (Acme discloses to counter-party)

Draft a one-way NDA under which the counter-party is bound to protect Acme's Confidential Information. Include the same elements as the MNDA but structured as one-way. Include a specific "you shall not reverse-engineer" clause for any software or hardware Acme discloses.

### Part H — Candidate / recruit NDA

Draft a short, candidate-facing NDA for late-stage interviews where the corporation shares confidential product / go-to-market information. Include:

1. **Narrow scope** — only Confidential Information disclosed for the specific interview process. Do not extend to information the candidate obtains from other sources.
2. **Term.** Short (12 months from disclosure) — the information generally becomes stale.
3. **Career-mobility carve-out.** The candidate is free to continue their career, apply to competitors, and use their general knowledge and skills. This is critical to avoid the NDA being read as an unenforceable de facto restrictive covenant.
4. **The standard exceptions.**
5. **A specific non-use clause** — the candidate shall not use the disclosed Confidential Information in their current or future employment.
6. **Dispute-resolution.**
7. **Signature block.**

State in the design memo that candidate NDAs are often skipped in early-stage conversations because they add friction to the recruiting funnel; the corporation's posture is to require them only in specifically-identified late-stage interviews where genuinely sensitive information will be shared.

### Part I — Investor-facing NDA

Draft an investor-facing NDA (mutual), and produce an honest assessment memo (per chapter 05) that:

1. Names the reality — VC firms almost never sign NDAs at the pitch-deck / initial-conversation stage.
2. Recommends when the corporation would legitimately request one (e.g., data-room access for a late-stage deal, technical deep-dive with a strategic corporate investor, exchange of financial projections).
3. Identifies the specific paper the corporation would accept as an NDA substitute (the "no-shop" language in a term sheet, the definitive investment agreement's confidentiality clause, a shortened one-way NDA specifically for data-room access).
4. Assesses which of the three Series-A VC counter-parties are most likely to sign a form NDA (typically corporate-strategic investors will; institutional financial VCs will not).

### Part J — Design-choices memo

A 2–3 page memo covering:

- The PIIA architecture and the state-rider design (national base + per-state carveout schedule vs. per-state entire-document variants).
- The present-assignment language and *Stanford v. Roche* citation.
- The trailing-inventions window (why the window you chose).
- The DTSA notice placement and the interaction with the NLRA / EEOC / government-cooperation carve-outs.
- The non-solicit design (California carve-out, Illinois threshold, non-California baseline).
- The non-compete decision (no rank-and-file, executive-only in enforceable states, decision matrix per state).
- The retroactive-cleanup posture (consideration analysis per state, communication plan, § 16600.1 late-compliance notice, "agrees to assign" defect remediation).
- The NDA suite architecture (MNDA, one-way inbound, candidate, investor) and when each is used.
- Any `<!-- needs-research -->` items you flagged (current state-list for invention-assignment statutes, current state-list for non-solicit thresholds, current DTSA statutory citations, current state statutes for the Fair Chance / salary-history / pay-transparency workflow that flowed from exercise 03 and impacts the offer-letter-to-PIIA cross-reference).

## Starter guidance

- Chapter 04 is the primary reference for the employee PIIA structure. Chapter 05 is the primary reference for the NDA / MNDA suite. Chapter 06 is the reference for the non-compete and non-solicit design.
- The present-assignment "hereby assigns" language is non-negotiable per *Stanford v. Roche*. Any "agrees to assign" is a defect.
- The DTSA notice must be present; the § 1833(b)(3) statutory language should be quoted or closely paraphrased. Omission means the corporation cannot recover exemplary damages or attorneys' fees under § 1836(b)(3)(C)–(D).
- The California employee PIIA differs from the non-California PIIA in three material ways: (a) § 2870 carveout with § 2872 written notice, (b) no general employee non-solicit (per *AMN Healthcare*), (c) no non-compete under any conditions (per § 16600 as extended by SB 699 and AB 1076).
- The Illinois employee PIIA differs on the non-solicit / non-compete thresholds under 820 ILCS 90 and requires 14-calendar-day notice for restrictive-covenant provisions.
- The retroactive-cleanup for the existing workforce is *legally* straightforward (new PIIA execution) but *practically* delicate (employees will read the new document carefully and may push back on the non-solicit or the DTSA carve-outs). The design memo should address the communication.
- Do NOT include a "confidentiality of this NDA" clause that would run afoul of *McLaren Macomb*; the NDA can protect Confidential Information but cannot prohibit the counter-party's employees from filing agency charges or engaging in protected concerted activity.
- The investor NDA is an *honesty exercise* more than a drafting exercise. Do not pretend a top-tier VC will sign a form NDA at the pitch stage.
- Do NOT draft the arbitration provision — that is exercise 08.

## Deliverables

- `employee-piia-national-template.md` — Part A.
- `state-carveout-schedule.md` — Part B (referenced from the PIIA).
- `non-solicit-schedule.md` — Part C (embedded in or referenced from the PIIA).
- `non-compete-decision-memo.md` — Part D.
- `retroactive-cleanup-plan.md` — Part E, including the AB 1076 late-compliance notice draft.
- `mnda-template.md` — Part F.
- `one-way-nda-template.md` — Part G.
- `candidate-nda-template.md` — Part H.
- `investor-nda-and-assessment.md` — Part I.
- `piia-and-nda-design-choices-memo.md` — Part J.

## Acceptance criteria

The package is acceptable if:

1. The PIIA uses **"hereby assigns"** present-assignment language. Any "agrees to assign" is a fail.
2. The PIIA includes a work-made-for-hire clause paired with an assignment backstop.
3. The DTSA § 1833(b)(3) notice is present and cited.
4. The Prior Inventions schedule is present with "fill-in-or-forfeit" framing.
5. State carveouts are present and cited for California (§ 2870 / § 2872), Illinois (765 ILCS 1060/2), and Washington (RCW 49.44.140), at minimum.
6. Non-solicits are drafted per chapter 06's design: 12-month post-termination, direct-work-relationship scope; California employees get no general employee non-solicit; Illinois employees under the $45,000 threshold get no non-solicit.
7. No non-compete is included in the rank-and-file PIIA; the executive-employment-agreement non-compete decision is documented per state.
8. The retroactive-cleanup plan addresses consideration per state, the § 16600.1 late-compliance notice, and the "agrees to assign" defect remediation.
9. The MNDA includes the standard exceptions, term, no-license, return/destruction, no-warranty, dispute-resolution, employee-facing carve-outs, and correctly-scoped signature block.
10. The one-way inbound NDA includes a no-reverse-engineering clause.
11. The candidate NDA is narrowly scoped with a career-mobility carve-out and a 12-month term.
12. The investor NDA + assessment memo is honest about VC firms' non-signature posture and identifies the correct alternative-paper mechanisms.
13. No NDA or PIIA clause purports to prohibit the counter-party's employees from filing agency charges, engaging in NLRA-protected activity, or exercising DTSA whistleblower immunity.
14. Statutory / case citations (*Stanford v. Roche*, 583 F.3d 832 (Fed. Cir. 2009), aff'd, 563 U.S. 776 (2011); 17 U.S.C. § 101; 18 U.S.C. § 1833(b)(3); Cal. Lab. Code §§ 2870, 2872; 765 ILCS 1060/2; RCW 49.44.140; Cal. Bus. & Prof. Code § 16600 and § 16600.1; *AMN Healthcare, Inc. v. Aya Healthcare Services, Inc.*, 28 Cal. App. 5th 923 (2018); 820 ILCS 90) are correct.
15. Nothing left as `[FILL IN]` — every field populated or explicitly flagged with a `<!-- needs-research -->` marker.
