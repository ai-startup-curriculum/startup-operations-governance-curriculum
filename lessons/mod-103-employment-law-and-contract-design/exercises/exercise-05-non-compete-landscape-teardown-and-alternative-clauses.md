# Exercise 05 — Non-compete landscape teardown and alternative clauses

> Estimated time: **~5 hours** · Related chapters: [06 — The non-compete landscape and its alternatives](../06-non-compete-landscape-and-alternatives.md), [04 — The employee PIIA](../04-employee-piia.md)

## Problem statement

Acme Robotics is cleaning up its restrictive-covenant stack. The founder-era employment agreements include a one-size-fits-all 24-month post-employment non-compete that forbids working for "any competitor, anywhere in the world, in any capacity." It was pulled off a public forms site in 2019 and signed by every employee the corporation has ever hired. It has never been tested.

The incoming COO / GC (you) has three overlapping deliverables:

1. A **landscape teardown** of why the existing clause is defective in every state the corporation operates in, with the specific statutes and cases that control.
2. A **replacement restrictive-covenant pack** built from the surviving practitioner defaults (confidentiality, trade-secret protection, non-solicits, garden leave, notice-of-resignation, equity claw-back) — scoped per state and per role — that goes into the chapter 04 PIIA plus the senior-executive employment agreement.
3. A **remediation plan** to migrate the existing workforce to the new pack, including the California AB 1076 / § 16600.1 notice-of-void obligation for California employees under the prior non-compete, and a defense-posture memo for the (unlikely, but possible) scenario where a departing employee or acquirer asks the corporation to attempt enforcement of a legacy non-compete.

You are not drafting the FTC rule, state statutes, or case law — you are applying them.

## Facts

- **Corporation.** Acme Robotics, Delaware C-corp, headquartered in San Francisco.
- **Current headcount: 60.** California (28), New York State and NYC (10), Washington (6), Colorado (5), Massachusetts (5), Illinois (4), Texas (2).
- **Current non-compete.** 24-month post-employment, "any competitor anywhere in the world in any capacity," no garden-leave pay, no state-specific carveouts, no notice beyond the offer letter, no severability. In every employee's "Employment Agreement" (which also contains the PIIA — a drafting choice chapter 04 would correct).
- **Four senior executives.** CFO (Boston, MA), VP Engineering (San Francisco), VP Sales (Seattle), Chief Product Officer (Chicago). All have genuine trade-secret access, customer-relationship responsibility, and competitive-market exposure.
- **One acquisition in flight.** Acme is in late-stage conversations to acquire a six-person computer-vision startup in San Diego. The target's founders (two) will be rolled into Acme as employees post-close; the acquisition agreement will separately include seller-side non-competes under Cal. Bus. & Prof. Code § 16601.
- **Two recent departures.** A senior SWE in San Francisco joined a direct competitor three months ago. A product manager in Chicago joined a non-competitor in the aerospace sector two months ago. Neither has been contacted by Acme about the legacy non-compete.
- **Series-A diligence is 90 days out.** Lead investor's counsel will review the restrictive-covenant stack as part of IP / people diligence.

## Requirements

### Part A — Landscape teardown of the existing clause

For each of the seven jurisdictions where Acme employs anyone (California, New York State / NYC, Washington, Colorado, Massachusetts, Illinois, Texas), produce a one-paragraph-per-state analysis of why the existing 24-month "any competitor anywhere" non-compete is defective. For each state, identify:

1. **The controlling statute** — e.g., Cal. Bus. & Prof. Code § 16600 (and its 2023–2024 amendments at § 16600.1 and § 16600.5), G.L. c. 149 § 24L (Massachusetts), RCW 49.62 (Washington), C.R.S. § 8-2-113 (Colorado), 820 ILCS 90 (Illinois), the pending-legislation posture in New York (chapter 06), and the reasonableness-test case law in Texas.
2. **The specific defect(s)** — categorical void (CA, MN, OK, ND), earnings threshold not met, duration excessive, geography unreasonable, consideration (garden-leave pay) absent, notice period not observed, no advice-of-counsel language, no severability, scope-of-prohibited-activities overbroad.
3. **The enforcement risk to the corporation** — in California, SB 699 fee-shifting plus § 16600.1 private right of action and civil penalty; elsewhere, fee-shifting under state statute (Massachusetts under § 24L(d); Washington under RCW 49.62.080) or reputational cost of attempted enforcement.
4. **Blue-pencil posture** — states that will blue-pencil a defective clause to make it enforceable (Illinois, Massachusetts, Texas under the Covenants Not to Compete Act, others), states that will void the entire clause (California, Virginia, Oklahoma under some lines of case law), and the practical implication for the corporation's drafting choice. The teardown should state that blue-pencil doctrine is not a drafting license — a clause overbroad on purpose is still a reputational and litigation cost.

The teardown is primary-source-grounded. Cite the statute or case for each state. Flag any statutory thresholds (Washington earnings threshold under RCW 49.62.020, Colorado "highly-compensated worker" threshold under C.R.S. § 8-2-113(2)(b), Illinois earnings thresholds under 820 ILCS 90/10 and 90/15) with a `<!-- needs-research -->` marker if you cannot verify the current-year indexed figure.

### Part B — FTC rule status memo

A one-page memo covering:

- The procedural history of 16 C.F.R. Part 910 — the April 23, 2024 final rule, the Ryan LLC v. FTC (N.D. Tex. 2024) nationwide-vacatur ruling, the Properties of Villages Inc. v. FTC (M.D. Fla. 2024) preliminary-injunction ruling, and the ATS Tree Services v. FTC (E.D. Pa. 2024) decision denying the injunction. Cite the dockets.
- The current operative status of the rule and any appellate activity.
- The FTC's non-rule enforcement posture under FTC Act § 5 (individual-enforcement actions against specific non-competes the FTC views as anti-competitive).
- The practical implication for Acme's drafting — the rule is not currently enforceable, so state law governs, but the drafting posture should not assume broad non-compete enforceability over a multi-year horizon.
- Flag the current status of the FTC appeal, parallel rulemaking, and congressional action (e.g., Workforce Mobility Act proposals) as a `<!-- needs-research -->` item that must be refreshed before any client-facing memo is issued.

### Part C — Replacement restrictive-covenant pack

Design the replacement restrictive-covenant pack as *layers*, each with a specific population, state scope, and chapter 06 reference:

#### Layer 1 — All employees, all states, embedded in the chapter 04 PIIA

- **Confidentiality obligations** — indefinite for trade secrets as defined by 18 U.S.C. § 1839(3) and the applicable state UTSA; defined period (3–5 years) for other Confidential Information. Chapter 04 is the drafting reference.
- **DTSA whistleblower notice** — 18 U.S.C. § 1833(b)(3).
- **Return of property on termination.**
- **Cooperation and further-assurances clause.**
- **Trailing-inventions assignment** — 6-month post-termination window, narrow to inventions using Confidential Information or substantially conceived during service. Chapter 04 trade-off.
- **No post-employment non-compete** in the general PIIA. Explicit — do not leave a dormant non-compete section with a "[reserved]" placeholder; a reviewer should see that the corporation has intentionally omitted the covenant.

#### Layer 2 — Non-California, non-threshold-exempt employees, in the chapter 04 PIIA

- **Employee non-solicit** — 12 months post-termination, narrow to employees the departing employee worked with directly in the last 12 months of employment. Address the Illinois 820 ILCS 90/10 earnings threshold ($45,000 indexed) — for any Illinois employee under the threshold, the non-solicit is void and must be omitted; design the PIIA to omit the covenant for those employees rather than include a void clause.
- **Customer non-solicit** — 12 months post-termination, narrow to customers the departing employee worked with directly in the last 12 months of employment. For California employees, replace the general covenant with a narrow trade-secret-based customer-list covenant per the chapter 06 drafting posture (and the Ninth Circuit case-by-case treatment).
- **No general employee non-solicit for California employees** per *AMN Healthcare Inc. v. Aya Healthcare Services, Inc.*, 28 Cal. App. 5th 923 (2018).

#### Layer 3 — Senior executives, in a separate executive employment agreement (not the PIIA)

For each of the four current senior executives (CFO, VP Eng, VP Sales, CPO), design the executive-level restrictive-covenant pack:

- **60-day notice-of-resignation obligation** with continued-compensation garden-leave for the notice period.
- **Post-termination non-compete** — 12 months, competitor-specific (defined by reference to a named-competitor list or an industry-and-product-scope formulation), geographic scope limited to markets where the corporation does business and the executive had responsibility, supported by **garden-leave pay** covering the restricted period. State-by-state:
  - **CFO (Boston, MA)** — compliant with G.L. c. 149 § 24L (10-business-day pre-start notice, right-to-consult-counsel advisement, duration ≤ 12 months, garden-leave pay at ≥ 50% of highest base salary over the preceding two years or other mutually-agreed consideration, geographic reasonableness, not void against non-exempt employees, not void if termination was with cause).
  - **VP Engineering (SF, CA)** — **no post-employment non-compete** per § 16600; SB 699 voids any non-compete signed anywhere and enforced against California employees. The executive agreement for the VP Eng omits the non-compete entirely and relies on the chapter 06 alternatives.
  - **VP Sales (Seattle, WA)** — compliant with RCW 49.62: disclosure at time of offer (and prior to acceptance), 18-month duration cap (rebuttable presumption), earnings threshold compliance, garden-leave for the restricted period if the executive is terminated without cause.
  - **CPO (Chicago, IL)** — compliant with 820 ILCS 90: 14-calendar-day pre-execution notice, advice-of-counsel advisement, earnings threshold compliance, adequate consideration (two years of continued employment or additional signing consideration), reasonable duration / geography / scope.
- **Executive-level customer non-solicit** — 12–18 months post-termination, defined customers (customers the executive had direct responsibility for during the last 24 months of employment).
- **Executive-level employee non-solicit** — 12 months post-termination, employees the executive had reporting responsibility for or recruited.
- **Board-service and outside-activity disclosure and approval framework** — the executive must disclose and obtain board approval before serving on any outside board or engaging in any outside advisory activity in a related industry.
- **Equity claw-back for competitive activity** — forfeiture of unvested options and claw-back of exercised-but-held shares if the executive breaches the post-termination non-compete, non-solicit, or confidentiality covenants. Chapter 06 flags the California-side enforceability doubt (SB 699, AB 1076); document the design and address the California posture (no claw-back for the VP Eng).

Do NOT draft the executive employment agreement in full; produce the restrictive-covenant section plus a one-page summary per executive stating the design choices.

#### Layer 4 — Acquisition-related (sale-of-business non-competes)

For the pending San Diego acquisition, author the seller-side non-compete framework under Cal. Bus. & Prof. Code § 16601:

- Non-compete tied to the sale of the business (the acquired corporation's stock or substantially-all-assets sale), with the departing founders bound to a duration and geographic scope that courts have found reasonable in the acqui-hire / M&A context.
- The non-compete is enforceable against California-resident sellers under § 16601 even post-SB 699; cite the statutory exception. Address whether the two founders will become Acme employees post-close and whether the employee-side California § 16600 bar would nonetheless void a parallel employee non-compete; the sale-of-business carveout controls the enforcement posture.
- Note that this clause lives in the acquisition agreement (which is in mod-109 and beyond mod-103's drafting scope) — produce only the design memo stating the structure and the citations, not the clause text.

### Part D — Garden-leave structure for executives

For the three senior executives who are receiving a post-termination non-compete (CFO, VP Sales, CPO), design the garden-leave structure:

1. **Trigger.** Which separation events trigger garden leave — resignation, termination without cause, termination for cause (typically forfeited), termination for performance (consider carefully).
2. **Duration.** The garden-leave period matches the non-compete restricted period (12 months).
3. **Compensation.** Base salary, benefits continuation, equity treatment (continued vesting vs. frozen), bonus / commission eligibility.
4. **Non-work obligation.** The executive is on garden leave and does not perform work for the corporation. The corporation may contact the executive for transition cooperation under reasonable terms.
5. **Breach consequences.** Breach of the garden-leave obligations (performing work for a competitor during the period) terminates garden-leave payments and triggers the equity claw-back.
6. **Interaction with severance.** If severance is separately negotiated, define the interaction with garden-leave (whether severance is on top of, in lieu of, or offset against garden-leave pay).
7. **State-specific calibration.** Massachusetts G.L. c. 149 § 24L requires garden-leave pay at ≥ 50% of highest base salary over the preceding two years or other mutually-agreed consideration — explain the design choice for the Boston CFO; Washington and Illinois do not mandate specific garden-leave compensation levels but require consideration.

### Part E — Remediation plan for existing workforce

The current 60-employee workforce is operating under a defective 24-month non-compete. Produce a remediation plan:

1. **Communication and consideration.** How you communicate the new restrictive-covenant pack and the retirement of the old non-compete. In most states, continued employment is sufficient consideration for existing employees signing a new PIIA with narrower restrictive covenants; some states (Illinois, Massachusetts) require additional consideration. Address per state.
2. **The California AB 1076 / § 16600.1 notice-of-void obligation.** For the 28 California employees, author the specific written notice that Cal. Bus. & Prof. Code § 16600.1 requires. The February 14, 2024 statutory deadline is past; produce the late-compliance notice with a brief preface explaining the late-compliance posture, and document the private-right-of-action and § 17200 exposure the corporation is carrying for the missed deadline.
3. **The two recent departures.** For the SF SWE who joined a direct competitor and the Chicago PM who joined a non-competitor, produce a one-paragraph decision memo per departure stating whether the corporation would attempt enforcement of the legacy non-compete. Chapter 06's framework should drive these to "no" in both cases (California § 16600 voids the SF SWE's clause; the Chicago PM's new role is not competitive and the clause is overbroad under 820 ILCS 90 blue-pencil analysis), but each decision must be documented with the specific reasons.
4. **The order of operations.** New PIIA execution sequence — senior executives first (with their executive employment agreement; signatures front-run the AB 1076 notice to avoid negotiation friction), then the California workforce (combined PIIA execution + AB 1076 notice), then the balance of the workforce. State the rationale.
5. **The IP-assignment interaction.** The old agreement contains "agrees to assign" IP language, not "hereby assigns" (chapter 04 defect per *Stanford v. Roche*). Re-execution of a corrected PIIA is both a non-compete-replacement and an IP-assignment-perfection step. Address whether re-execution retroactively perfects the assignment of pre-execution inventions or whether a separate express assignment is required for each pre-execution invention. Flag the Series-A diligence posture.

### Part F — Series-A diligence response package

Produce the diligence-response package the corporation will provide to lead investor's counsel:

1. The replacement restrictive-covenant pack (clean copy of the new PIIA plus the four executive employment agreement restrictive-covenant sections).
2. The remediation plan from Part E, with status (number of employees signed on the new PIIA by category, outstanding counts, projected completion date).
3. The California AB 1076 notice package — the notice itself, delivery proof per employee, and the late-compliance memo.
4. A short memo addressing the FTC rule status and the corporation's forward-looking drafting posture.
5. A sale-of-business non-compete framework memo for the pending acquisition.
6. The two-departure decision memos.
7. A legal-opinion-style summary stating that the corporation's current restrictive-covenant stack is compliant with the applicable state laws in each of the seven jurisdictions where it employs anyone.

### Part G — Design-choices memo

A 2–3 page memo covering:

- Why Acme is retiring the general non-compete (chapter 06's practitioner-default framework).
- The three design choices you found hardest and how you resolved them — e.g., whether to extend the executive non-compete to the VP Engineering under some tortured theory (the answer is no, § 16600 governs), whether to blue-pencil Texas (likely yes but with narrower scope than historical draft), whether to apply the strictest state's requirements as a national baseline for notice-of-resignation and garden-leave (optional under chapter 08's highest-common-denominator framework).
- The equity claw-back decision for competitive activity post-separation — whether to include, whether to apply nationally, how to address the California-side enforceability doubt.
- The maintenance discipline — chapter 06's recommendation to refresh non-compete / non-solicit drafting annually and after any material state statutory change (and after any FTC rulemaking or appellate ruling).
- Any `<!-- needs-research -->` items you flagged — current Washington RCW 49.62 earnings threshold, current Colorado C.R.S. § 8-2-113 "highly-compensated worker" threshold, current Illinois 820 ILCS 90 thresholds, current FTC rule and Ryan LLC appellate status, current status of New York non-compete legislation after any 2025–2026 action.

## Starter guidance

- Chapter 06 is the primary reference. Chapter 04 is the reference for how the restrictive-covenant pack fits inside the PIIA structure. Chapter 08 is the reference for state variance beyond non-compete alone (interaction with pay-transparency and salary-history).
- The California posture is categorical — § 16600 as extended by SB 699 and AB 1076 voids non-competes "regardless of whether the contract or provision was signed in California." This governs the VP Engineering, the SF SWE departure, and the 28 California employees.
- The Massachusetts posture under G.L. c. 149 § 24L is a procedural checklist — timing of notice, advice-of-counsel language, garden-leave consideration, duration, and the categorical void for non-exempt / student / minor / terminated-without-cause employees. Build the CFO's clause as a checklist.
- The FTC rule is not currently enforceable (Ryan LLC v. FTC, 3:24-cv-00986, N.D. Tex., Aug. 20, 2024). Do not design the pack as if the rule applied; do not design it as if the rule could never apply. The corporation's forward-looking posture is to use the pack even if some future rule would mandate it.
- Do NOT include a "general catch-all restraint" clause — courts read these as attempted non-competes and void them. Each clause must be scoped specifically.
- Do NOT include a confidentiality or non-disparagement clause that would run afoul of *McLaren Macomb*, 372 NLRB No. 58 (2023), or the Speak Out Act of 2022 (Pub. L. No. 117-224). The chapter 09 drafting carve-outs apply.
- The sale-of-business non-compete under § 16601 is a legitimate, enforceable mechanism in California; do not confuse the acquisition-side framework with the employee-side § 16600 bar.
- Where current-year indexed thresholds matter (Washington, Colorado, Illinois earnings thresholds), do not invent numbers — flag with `<!-- needs-research -->`.
- The remediation-plan sequencing is a judgment call; justify your choice.

## Deliverables

- `non-compete-landscape-teardown.md` — Part A.
- `ftc-rule-status-memo.md` — Part B.
- `replacement-restrictive-covenant-pack.md` — Part C (with executive-level sub-documents per executive).
- `garden-leave-structure-memo.md` — Part D.
- `workforce-remediation-plan.md` — Part E, including the AB 1076 late-compliance notice draft.
- `series-a-diligence-response-package.md` — Part F (table-of-contents with references to the other deliverables).
- `restrictive-covenant-design-choices-memo.md` — Part G.

## Acceptance criteria

The package is acceptable if:

1. The teardown identifies the controlling statute and the specific defect for each of the seven jurisdictions. California cites § 16600 as extended by SB 699 (§ 16600.5) and AB 1076 (§ 16600.1); Massachusetts cites G.L. c. 149 § 24L; Washington cites RCW 49.62; Colorado cites C.R.S. § 8-2-113; Illinois cites 820 ILCS 90. New York addresses the pending-legislation status and the current-common-law reasonableness posture. Texas addresses the common-law reasonableness test and the blue-pencil posture under the Covenants Not to Compete Act.
2. The teardown correctly identifies California as a categorical void and does not attempt to argue partial enforceability.
3. The FTC-rule memo correctly states that the rule is not currently enforceable, cites Ryan LLC v. FTC (3:24-cv-00986, N.D. Tex., Aug. 20, 2024), and flags the appellate status as a research item.
4. The replacement pack has no post-employment non-compete in the rank-and-file PIIA for any employee in any state.
5. The replacement pack has a narrow employee non-solicit (12 months, direct-work-relationship scope) and customer non-solicit (12 months, direct-customer-relationship scope) for non-California employees, with the Illinois earnings-threshold carve-out applied.
6. No general employee non-solicit is included for California employees; the customer non-solicit for California employees is narrowly framed as trade-secret protection per the chapter 06 posture.
7. The executive-level restrictive-covenant pack has state-specific compliance for the CFO (MA § 24L), VP Sales (WA RCW 49.62), and CPO (IL 820 ILCS 90). The VP Engineering (CA) has no post-employment non-compete.
8. Garden-leave structures are designed per the chapter 06 framework and comply with Massachusetts § 24L for the CFO.
9. The sale-of-business non-compete framework for the San Diego acquisition cites Cal. Bus. & Prof. Code § 16601 correctly and addresses the post-close employee-side § 16600 bar.
10. The California AB 1076 / § 16600.1 late-compliance notice is drafted and the compliance posture is documented.
11. The two-departure decision memos recommend non-enforcement with specific reasons cited to the applicable state law.
12. The IP-assignment interaction (chapter 04 "agrees to assign" defect, *Stanford v. Roche*) is addressed as part of the remediation plan.
13. Statutory and case citations (Cal. Bus. & Prof. Code §§ 16600, 16600.1, 16600.5, 16601; G.L. c. 149 § 24L; RCW 49.62; C.R.S. § 8-2-113; 820 ILCS 90; *AMN Healthcare Inc. v. Aya Healthcare Services, Inc.*, 28 Cal. App. 5th 923 (2018); *Stanford v. Roche Molecular Systems, Inc.*, 583 F.3d 832 (Fed. Cir. 2009), aff'd, 563 U.S. 776 (2011); *Ryan LLC v. FTC*, 3:24-cv-00986 (N.D. Tex. 2024); 16 C.F.R. Part 910; 18 U.S.C. § 1833(b)(3)) are correct.
14. No clause purports to prohibit the counter-party's employees from filing agency charges, engaging in NLRA-protected activity, or exercising DTSA whistleblower immunity.
15. Nothing left as `[FILL IN]` or `[TBD]` — every field populated or explicitly flagged with a `<!-- needs-research -->` marker.
