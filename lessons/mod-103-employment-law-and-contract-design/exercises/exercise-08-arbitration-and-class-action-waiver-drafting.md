# Exercise 08 — Arbitration and class-action waiver drafting

> Estimated time: **~4 hours** · Related chapters: [09 — Arbitration and class-action waivers](../09-arbitration-and-class-action-waivers.md), with cross-references to [03](../03-offer-letter-architecture-and-pay-transparency.md), [04](../04-employee-piia.md), [07](../07-eeoc-protected-category-framework.md), and [08](../08-state-law-variance.md)

## Problem statement

Acme Robotics is finalising its arbitration-and-dispute-resolution posture. The incoming COO / GC (you) is deciding whether the corporation (a) retains a mandatory employment arbitration agreement with a class-action waiver for its workforce, (b) runs a court-based dispute-resolution model with a jury-trial waiver and venue selection, or (c) adopts a hybrid — mandatory arbitration for a defined claim scope with court-based resolution for the rest.

Whichever model the corporation adopts, the drafting must survive the current federal-and-state-law landscape as of the chapter 09 publication horizon — the post-*Epic Systems* FAA framework, the Ending Forced Arbitration Act (EFAA) sexual-assault / sexual-harassment carve-out, the Speak Out Act's non-disclosure limit, the California PAGA bifurcation after *Viking River* and *Adolph*, the NLRB *McLaren Macomb* restriction on confidentiality and non-disparagement clauses, the EEOC / government-charge-filing right, the DTSA whistleblower immunity, state-specific statutes limiting mandatory arbitration (NY CPLR § 7515, Illinois Workplace Transparency Act, Washington RCW 49.44.210, California AB 51 — now largely preempted but still relevant for drafting), and the mass-arbitration-cost reality that materially shifts the economic calculus.

Your task is to produce the full arbitration-and-dispute-resolution package: the include-or-exclude decision memo, the arbitration agreement itself (with California-specific addendum), the standalone jury-trial-waiver-and-venue clause for the court-based alternative, the delivery-and-consideration protocol, the notice-and-training materials, and the maintenance discipline.

This is the chapter 09 counterpart to exercise 04 (PIIA / NDA suite) and exercise 05 (restrictive-covenant pack). The arbitration provision is a standalone agreement, delivered with the offer letter, signed by every W-2 employee as a condition of employment.

## Facts

- **Corporation.** Acme Robotics, Delaware C-corp. HQ San Francisco. Employs in CA (28), NY state and NYC (10), WA (6), CO (5), IL (4), MA (5), TX (2). Total 60 employees.
- **Current state of the arbitration provision.** The corporation's current offer-letter embeds a short arbitration provision that says: "Employee agrees that all disputes with the Corporation will be resolved by binding arbitration before a single arbitrator in San Francisco under the AAA Employment Arbitration Rules. Employee waives any right to a jury trial. Employee waives any right to participate in a class, collective, or representative action." No EFAA carve-out. No PAGA bifurcation. No fee-and-cost allocation. No notice period. No carve-out for charge-filing with government agencies. No DTSA whistleblower acknowledgment. No *McLaren Macomb* carve-outs. Delivered embedded in the offer letter with no separate signature, no advice-of-counsel language, no consideration period.
- **The two recent departures from exercise 05.** The SF SWE who joined a direct competitor three months ago; the Chicago PM who joined a non-competitor two months ago. Neither has initiated any claim. Hypothetically, if either filed, the current arbitration provision would be the governing document.
- **The pending acquisition from exercise 05.** The six-person San Diego computer-vision startup. The target has no arbitration agreement. Post-close, the two rolling-forward founder-employees and the four non-founder employees must execute Acme's arbitration provision.
- **The mass-arbitration consideration.** The CFO has flagged that a mass-arbitration campaign would require the corporation to pay AAA filing fees of ~$3,500 per claim plus the arbitrator's daily fee (commonly $5,000+/day) under the AAA Employment Arbitration Rules fee allocation; a 50-employee mass arbitration would represent $175,000+ in filing fees alone, before any merits analysis.
- **Series-A diligence is 90 days out.**

## Requirements

### Part A — Include-or-exclude decision memo

Produce a 2–3 page decision memo that:

1. States the four coherent dispute-resolution postures: (i) mandatory arbitration with class-action waiver for all claim types (minus the EFAA and other statutory carve-outs); (ii) mandatory arbitration for a narrow scope (wage-and-hour, general employment) with court-based resolution for discrimination / harassment / retaliation and other sensitive claim types; (iii) voluntary arbitration (opt-in post-dispute) with court-based default; (iv) no arbitration, court-based dispute resolution with jury-trial waiver and venue selection.
2. Analyses the trade-offs per chapter 09 — the *Epic Systems* enforceability baseline, the EFAA sexual-assault / sexual-harassment carve-out, the PAGA bifurcation, the mass-arbitration cost realities, the reputational and recruiting dimensions, the diligence posture, the state-by-state preemption analysis.
3. Produces a specific recommendation. The chapter 09 drafting posture (chapter 09 § "Acme Robotics in a sentence") is **(ii) — mandatory arbitration for a defined scope with carve-outs for EFAA-covered claims, PAGA bifurcation for California employees, and NLRA / EEOC / government-cooperation and DTSA carve-outs preserved**. Your memo may recommend differently if you justify it, but should start from the chapter's recommendation.
4. Addresses the mass-arbitration cost pattern explicitly — including the AAA filing-fee allocation, the FairClaims-and-other-platform batched-arbitration protocols, and the corporation's economic exposure at the 60-employee and projected 120-employee scales.
5. Addresses the recruiting-friction dimension — what does the corporation tell senior candidates about the arbitration posture, and does the posture cost offers.

### Part B — The arbitration agreement (national base)

Draft the full arbitration agreement as a standalone document (not embedded in the offer letter). The agreement should include:

1. **Recital, effective date, consideration.** Recital identifies the agreement as a standalone document; effective date; recital of consideration (continued or new employment, or additional consideration where state law requires).
2. **Scope of covered claims.** The specific claim types that are subject to arbitration — wage-and-hour, general employment contract claims, confidentiality / IP / PIIA-related claims, benefit-plan claims, and other defined claim types.
3. **Scope of excluded / carved-out claims.** The specific claim types that are excluded — (i) EFAA-covered sexual-assault and sexual-harassment claims (9 U.S.C. §§ 401–402) at the employee's election; (ii) representative PAGA claims (California employees); (iii) workers'-compensation claims (statutory agency-based process); (iv) unemployment-insurance claims (statutory agency-based process); (v) claims that cannot be arbitrated under federal or state law; (vi) claims for injunctive relief to protect confidential information or trade secrets (preserved for both parties for either arbitration or court); (vii) charge-filing with the EEOC, NLRB, SEC, DOL, DOJ, state FEPAs, or any other government agency (NLRA § 7 and chapter 07 preserve this right).
4. **Class-action, collective-action, and representative-action waiver.** The waiver applies to the claim types subject to arbitration, with the explicit carve-out that non-individual PAGA claims (California employees post-*Viking River* / *Adolph*) are not waived.
5. **The arbitration forum and rules.** AAA Employment Arbitration Rules (or JAMS Employment Arbitration Minimum Standards) explicitly referenced, including the fee-allocation structure.
6. **The arbitrator selection process.** Single arbitrator, selected from the AAA / JAMS panel; selection method; disqualification standards; replacement process.
7. **Discovery.** Reasonable discovery subject to arbitrator discretion; the Armendariz / California-side mutuality requirement for California employees must be preserved.
8. **Hearing procedure.** Written statement of claim, written answer, hearing procedure, written award with findings of fact and conclusions of law; standard of review.
9. **Fees and costs.** The corporation pays all arbitration fees and administrative costs beyond what the employee would pay in court (filing fee, forum fee, arbitrator's compensation). The California-side *Armendariz* / Cal. Lab. Code analysis is addressed in the California addendum (Part C). Attorneys' fees per the applicable claim-specific fee-shifting statute.
10. **The confidentiality of the arbitration.** Narrowly scoped — the arbitration itself is confidential as to the arbitrator's deliberations and the proceeding, but the carve-outs preserve the employee's right to communicate about wages and working conditions, to file government-agency charges, to pursue coworker protected concerted activity under the NLRA, and to disclose required by law.
11. **The *McLaren Macomb* and Speak Out Act carve-outs.** Explicit statement that the arbitration agreement does not and cannot restrict (i) communication with coworkers about wages, working conditions, or workplace rules; (ii) filing charges with the EEOC, NLRB, SEC, DOJ, or any government agency; (iii) participating in a government investigation; (iv) exercising DTSA whistleblower immunity under 18 U.S.C. § 1833(b); (v) disclosing sexual-harassment or sexual-assault experiences under the Speak Out Act (Pub. L. No. 117-224).
12. **The DTSA whistleblower-immunity acknowledgment.** The arbitration agreement acknowledges the 18 U.S.C. § 1833(b)(3) notice (which also appears in the PIIA per chapter 04).
13. **Severability.** If any provision is unenforceable, the remainder stays in effect. **Explicit** that the class-action waiver, if unenforceable, severs *without* taking the arbitration agreement with it (consistent with chapter 09 "class-waiver-severed-not-agreement-severed" formulation).
14. **Governing law.** Governing law per chapter 09 (Delaware or California; the choice-of-law analysis matters especially for cross-state employees).
15. **Venue for court actions.** For any claim or motion that proceeds in court (e.g., motion to compel arbitration, EFAA-election cases), the venue — typically the county of the employee's work location.
16. **Signature block.** Specific signature of the employee acknowledging (a) receipt of the agreement, (b) consultation with counsel if desired, (c) opportunity to review and ask questions, (d) voluntary execution.
17. **Notice.** Explicit statement of the delivery-and-consideration-period protocol — chapter 09 "the 14-day Illinois Freedom to Work baseline" adopted nationally.

### Part C — The California addendum

For California employees, draft a California-specific addendum to the national arbitration agreement that addresses:

1. **The *Armendariz v. Foundation Health Psychcare Services, Inc.*, 24 Cal. 4th 83 (2000) requirements.** Mutual obligation (both parties bound to arbitrate); neutral arbitrator; adequate discovery; written award; limits on arbitration fees to not exceed court filing fees for the employee; no restriction on remedies available in court.
2. **The PAGA bifurcation under *Viking River Cruises, Inc. v. Moriana*, 596 U.S. 639 (2022) and *Adolph v. Uber Technologies, Inc.*, 14 Cal. 5th 1104 (2023).** The individual PAGA claim is compelled to arbitration; the non-individual (representative) PAGA claim is not waived. The employee retains standing to pursue non-individual PAGA claims after the individual arbitration concludes. Address the stay-pending-arbitration mechanics.
3. **The California AB 51 analysis.** Cal. Lab. Code § 432.6 attempted to prohibit mandatory arbitration as a condition of employment; the Ninth Circuit's *Chamber of Commerce v. Bonta*, 62 F.4th 473 (9th Cir. 2023), held AB 51 is preempted by the FAA. Address this in the addendum to confirm the agreement's compliance posture; even though preempted, do not take the position that voluntary / knowing / written assent is unnecessary.
4. **The California-specific fee allocation.** The corporation pays all arbitration costs and fees that exceed what the employee would pay to file and litigate in court. Explicit per *Armendariz*.
5. **The California-specific confidentiality and non-disparagement carve-outs.** Cal. Code Civ. Proc. § 1001 (STAND Act) and Cal. Gov. Code § 12964.5 (Silenced No More Act) require specific carve-outs for discrimination, harassment, and retaliation disclosures. Draft the explicit carve-out language.
6. **The California-specific forum-selection and choice-of-law.** Cal. Lab. Code § 925 prohibits forcing a California employee into a non-California forum or non-California governing law for claims arising in California. Address the venue and choice-of-law accordingly.

### Part D — The court-based alternative (for the hybrid or no-arbitration decision)

For the subset of claim types that proceed in court (EFAA-covered claims, non-individual PAGA, and any other carved-out claim type), produce a jury-trial-waiver and venue-selection clause. Address:

1. **Jury-trial waiver.** For non-EFAA claims that may proceed in court, a knowing-and-voluntary jury-trial waiver with the specific advisement language courts look for.
2. **Venue selection.** Specific state and federal courts for different claim types.
3. **Choice of law.** Delaware or California base; state-specific overrides where § 925 or analogous statutes require.
4. **Attorneys' fees.** Per the applicable claim-specific fee-shifting statute (Title VII, FLSA, EPA, state wage-and-hour, FEHA, NYCHRL, etc.). No general two-way fee shifting that would chill employee claims under *Christiansburg Garment Co. v. EEOC*, 434 U.S. 412 (1978).
5. **Statute of limitations.** No shortening — attempts to contract a shorter statute of limitations are void under FLSA and often void under state law.
6. **Non-waiver of agency charge filing.** Explicit — court-based resolution does not waive the EEOC / state FEPA / NLRB / government charge-filing right.

### Part E — Delivery, consideration, and training protocol

Author the delivery protocol — the operational workflow for the arbitration agreement:

1. **Timing.** The agreement is delivered with the offer letter, at least 14 calendar days before signing (chapter 09's national baseline). The offer letter references the arbitration agreement; the arbitration agreement is executed on or before start date (the chapter 03 contingent-condition structure).
2. **Consideration.** For new hires, employment is adequate consideration in most states; for existing employees being asked to sign, document the consideration under chapter 06 / chapter 09 state-specific analysis. Illinois and Massachusetts require additional consideration; California requires knowing-and-voluntary assent.
3. **Advice of counsel.** The agreement includes an explicit "employee may consult with counsel" advisement.
4. **FAQ for recruiters, hiring managers, and HR.** A standard set of questions the corporation prepares answers for — "do I have to sign?", "what if I refuse?", "what claims does this cover?", "what claims does this not cover?", "what if I'm a California employee?", "what if I have a sexual-harassment claim?", "what if I want to file a charge with the EEOC?" — with scripted, legally-reviewed answers. Chapter 09 is the reference.
5. **Record-keeping.** The corporation retains the signed agreement and the delivery timestamps in the HRIS; the executed agreement is a diligence artifact for Series-A and later rounds.
6. **The post-signing training.** The corporation does not train employees on how to initiate arbitration (that is the employee's choice if a dispute arises), but the Head of People should know the AAA / JAMS intake process in case an employee asks.

### Part F — The retroactive-cleanup plan for the existing workforce

The existing 60-employee workforce has signed the current defective arbitration provision (embedded in the offer letter, no EFAA carve-out, no PAGA bifurcation, no *McLaren Macomb* carve-outs, no DTSA acknowledgment, no notice period, no fee-and-cost allocation, no California addendum). Produce the retroactive-cleanup plan:

1. **Validity analysis.** For each state the corporation employs in, assess whether the current provision is enforceable at all. California — likely subject to *Armendariz* substantive-unconscionability challenges on mutuality, fee allocation, and PAGA. New York — EFAA preemption and NY CPLR § 7515 analysis. Washington — RCW 49.44.210 analysis for harassment claims. Illinois — Workplace Transparency Act analysis. Produce a per-state validity summary.
2. **The remediation sequence.** Execute the new arbitration agreement with each existing employee, as part of the broader PIIA / NDA / restrictive-covenant remediation campaign from exercise 05. Order of operations (chapter 03 and chapter 06 inform the sequencing).
3. **The two-departure analysis.** For the SF SWE and the Chicago PM (exercise 05), if either initiated an arbitration or filed a claim today, which arbitration provision governs — the one in effect at the time of hire, or the current defective one? Produce a one-paragraph analysis per departure addressing the enforceability of the then-current provision in each departing employee's state.
4. **The communication posture.** How you communicate the new arbitration agreement to existing employees. The communication must be neutral, informational, and advise consultation with counsel. The communication cannot threaten adverse action for refusal to sign (that would support a wrongful-termination or retaliation claim, especially under California AB 51 — even though preempted, the state's enforcement posture is active).
5. **The refuse-to-sign protocol.** For existing employees who refuse to sign the new agreement, the corporation's response — chapter 09 flags this as a design choice. Options: (a) accept the refusal, maintain the then-current provision at that employee's hire date (likely weakest), (b) require signature as a condition of continued employment (strongest; but each state has preemption / public-policy issues), (c) negotiate specific terms with the refusing employee (uneven). Document the decision.

### Part G — Series-A diligence response package

Produce the diligence-response package for the arbitration posture:

1. The include-or-exclude decision memo from Part A.
2. The clean national arbitration agreement from Part B.
3. The California addendum from Part C.
4. The court-based clause from Part D (for the subset of claims that proceed in court).
5. The delivery protocol from Part E.
6. The retroactive-cleanup plan from Part F, with status.
7. A short legal-opinion-style summary stating that the corporation's arbitration posture is compliant with the FAA, the EFAA, the Speak Out Act, the PAGA statutory framework, *McLaren Macomb*, and applicable state statutes.

### Part H — Design-choices memo

A 2–3 page memo covering:

- The include-or-exclude decision rationale (chapter 09's framework; the mass-arbitration cost analysis; the recruiting-friction dimension).
- The three drafting choices you found hardest and how you resolved them (likely: the scope of claims subject to arbitration; the California PAGA bifurcation mechanics; the retroactive-cleanup validity question for the two recent departures).
- The relationship between the arbitration agreement and the chapter 04 PIIA (both reference DTSA and *McLaren Macomb*; both are standalone documents; both are executed at the offer-letter stage).
- The relationship between the arbitration agreement and the chapter 06 restrictive-covenant pack (both include confidentiality carve-outs; both are state-specific where state law requires).
- The maintenance discipline — annual refresh plus post-material-event refresh (any Supreme Court decision; NLRB decision; federal or state statutory change; AAA / JAMS rule change).
- Any `<!-- needs-research -->` items you flagged — current AAA Employment Arbitration Rules fee structure, current JAMS Employment Arbitration Minimum Standards, current status of state-level mandatory-arbitration limitations (NY, IL, WA, CA, NJ, MD) post-EFAA, current status of mass-arbitration platforms and batched-arbitration protocols.

## Starter guidance

- Chapter 09 is the primary reference. Chapter 07 (EEOC) and chapter 04 (PIIA) provide the DTSA and *McLaren Macomb* carve-out language. Chapter 08 provides state-variance context for the delivery protocol and the retroactive cleanup.
- The EFAA is categorical. 9 U.S.C. §§ 401–402 invalidate pre-dispute mandatory arbitration for any case that "relates to the sexual assault dispute or the sexual harassment dispute," at the plaintiff-employee's election, regardless of what the agreement says. The carve-out operates at the case level — if an EFAA-covered claim is bundled with non-covered claims in the same case, the entire case can proceed in court at the employee's election under the Second Circuit's reading in *Olivieri v. Stifel, Nicolaus & Co., Inc.*, No. 23-2168, 2024 WL 3870447 (2d Cir. Aug. 20, 2024) and similar authority; address this in the drafting.
- The PAGA bifurcation is well-established post-*Viking River* and *Adolph*. The individual PAGA claim can be compelled; the non-individual PAGA claim cannot be waived and the employee retains standing. The California addendum must address this mechanic specifically; the national base document must have the California addendum reference and the explicit non-waiver of representative PAGA claims.
- The *McLaren Macomb* carve-outs are non-negotiable. Any confidentiality or non-disparagement language that could be read as prohibiting (i) coworker communication about wages or working conditions, (ii) filing agency charges, (iii) participating in government investigations, (iv) engaging in NLRA § 7 protected concerted activity, or (v) exercising DTSA whistleblower immunity is unenforceable and exposes the corporation to NLRB unfair-labor-practice charges.
- The Speak Out Act (Pub. L. No. 117-224) invalidates pre-dispute non-disclosure clauses relating to sexual-harassment or sexual-assault disputes. The arbitration agreement's confidentiality clause must carve this out explicitly.
- Cal. Lab. Code § 925 is a sharp constraint on choice-of-law and forum-selection for California-based employees. Even if the corporation uses a Delaware governing-law baseline, the California addendum must preserve California-choice-of-law for claims that arise in California.
- The mass-arbitration cost pattern is real and should factor into the include-or-exclude decision. The AAA fee allocation under its Employment Arbitration Rules structure assigns the corporation most of the forum and arbitrator fees; a coordinated mass filing of 50 or 100 claims produces $200,000–$500,000+ in filing-fee exposure before any substantive arbitration. Address this with specific economics.
- The California AB 51 / § 432.6 preemption is settled by *Chamber of Commerce v. Bonta*, but the California enforcement posture is active. Draft knowing-and-voluntary assent language.
- Do NOT draft a two-way general fee-shifting provision that would chill plaintiff claims; chapter 09 and the chapter 07 "retaliation" discussion both warn about this.
- Where current AAA / JAMS fee schedules or state-indexed thresholds matter, flag with `<!-- needs-research -->`.

## Deliverables

- `arbitration-include-or-exclude-decision-memo.md` — Part A.
- `arbitration-agreement-national-base.md` — Part B.
- `arbitration-agreement-california-addendum.md` — Part C.
- `court-based-alternative-and-jury-waiver.md` — Part D.
- `arbitration-delivery-protocol.md` — Part E, including the recruiter / HR FAQ.
- `arbitration-retroactive-cleanup-plan.md` — Part F, including the two-departure analysis.
- `arbitration-series-a-diligence-package.md` — Part G.
- `arbitration-design-choices-memo.md` — Part H.

## Acceptance criteria

The package is acceptable if:

1. The decision memo recommends a specific posture and justifies it under chapter 09's framework, including the mass-arbitration cost analysis.
2. The national arbitration agreement has: (a) scope of covered claims; (b) scope of excluded claims including EFAA carve-out, PAGA non-waiver (for California employees), workers'-comp and UI claims, government agency charge-filing, injunctive relief for trade-secret protection; (c) class/collective/representative waiver with the explicit non-waiver of representative PAGA claims; (d) AAA or JAMS forum reference with fee allocation to the corporation beyond what the employee would pay in court; (e) *McLaren Macomb* carve-outs for coworker communication, government agency charge filing, government investigation participation, NLRA § 7 activity, DTSA whistleblower immunity; (f) Speak Out Act carve-out for sexual-harassment / sexual-assault disclosure; (g) severability with class-waiver-severs-not-agreement-severs formulation; (h) governing-law and venue clauses; (i) signature-block with knowing-and-voluntary acknowledgment and advice-of-counsel notice; (j) 14-calendar-day pre-signing delivery.
3. The California addendum addresses *Armendariz* mutuality and fee allocation; PAGA bifurcation per *Viking River* and *Adolph*; AB 51 posture per *Chamber of Commerce v. Bonta*; Cal. Lab. Code § 925 forum and choice-of-law; Silenced No More Act and STAND Act carve-outs.
4. The court-based alternative clause has a knowing-and-voluntary jury-trial waiver, venue selection, choice-of-law, statute-of-limitations non-shortening, and non-waiver of agency charge filing. It avoids chilling fee-shifting.
5. The delivery protocol specifies the 14-day pre-signing delivery, standalone agreement (not embedded in offer letter), explicit advice-of-counsel notice, consideration analysis per state, FAQ for recruiters / HR, and record-keeping.
6. The retroactive-cleanup plan addresses per-state validity of the current defective provision; the remediation sequence; the two-departure analysis for the SF SWE and Chicago PM; the communication posture; the refuse-to-sign protocol.
7. The two-departure analysis cites the specific statute that would govern enforceability in California (and *Armendariz* for substantive-unconscionability) and in Illinois (and the Workplace Transparency Act and Freedom to Work Act interactions).
8. No clause purports to prohibit the counter-party's employees from (i) filing agency charges, (ii) engaging in NLRA § 7 activity, (iii) communicating with coworkers about wages or working conditions, (iv) exercising DTSA whistleblower immunity, or (v) disclosing sexual-harassment / sexual-assault experiences under the Speak Out Act.
9. The agreement is standalone — not embedded in the offer letter — and has its own signature block.
10. Statutory and case citations (9 U.S.C. §§ 1–16 (FAA); 9 U.S.C. §§ 401–402 (EFAA); 18 U.S.C. § 1833(b) (DTSA whistleblower immunity); Pub. L. No. 117-224 (Speak Out Act); Pub. L. No. 117-90 (EFAA); 42 U.S.C. § 2000e-5(k); Cal. Lab. Code §§ 925, 2698 et seq. (PAGA), 432.6; Cal. Code Civ. Proc. § 1001; Cal. Gov. Code § 12964.5; *Epic Systems Corp. v. Lewis*, 584 U.S. 497 (2018); *Viking River Cruises, Inc. v. Moriana*, 596 U.S. 639 (2022); *Adolph v. Uber Technologies, Inc.*, 14 Cal. 5th 1104 (2023); *McLaren Macomb*, 372 NLRB No. 58 (2023); *Armendariz v. Foundation Health Psychcare Services, Inc.*, 24 Cal. 4th 83 (2000); *Chamber of Commerce v. Bonta*, 62 F.4th 473 (9th Cir. 2023); *Circuit City Stores, Inc. v. Adams*, 532 U.S. 105 (2001); *Southwest Airlines Co. v. Saxon*, 596 U.S. 450 (2022); *Bissonnette v. LePage Bakeries Park St., LLC*, 601 U.S. 246 (2024); *Christiansburg Garment Co. v. EEOC*, 434 U.S. 412 (1978)) are correct.
11. Nothing left as `[FILL IN]` or `[TBD]` — every field populated or explicitly flagged with a `<!-- needs-research -->` marker.
