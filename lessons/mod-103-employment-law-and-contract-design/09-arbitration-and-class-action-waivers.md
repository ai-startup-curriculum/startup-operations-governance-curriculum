# 9. Arbitration and class-action waivers

> Mandatory-arbitration-with-class-waiver is enforceable under federal law after *Epic Systems* (2018). The Ending Forced Arbitration Act (2022) carved out sexual-harassment and sexual-assault claims. PAGA carved itself into individual-plus-representative pieces after *Viking River* and *Adolph*. Draft with the carve-outs, not against them.

## Motivation

An arbitration clause with a class-action waiver in every employee agreement was, until recently, the default posture for US startups on the theory that (a) arbitration is faster and cheaper than court, (b) class-action exposure is materially larger than the sum of individual claims, and (c) *Epic Systems Corp. v. Lewis*, 584 U.S. 497 (2018), settled the enforceability question in the employer's favor.

The 2018 settlement has not held. The Ending Forced Arbitration of Sexual Assault and Sexual Harassment Act of 2021 (Pub. L. No. 117-90, effective March 3, 2022, "EFAA") carved out sexual-harassment and sexual-assault claims from mandatory arbitration at the employee's election. California's PAGA is now a bifurcated animal after *Viking River Cruises, Inc. v. Moriana*, 596 U.S. 639 (2022) and *Adolph v. Uber Technologies, Inc.*, 14 Cal. 5th 1104 (2023). The NLRB in *McLaren Macomb*, 372 NLRB No. 58 (Feb. 21, 2023), invalidated broad confidentiality and non-disparagement clauses in separation agreements and by extension in arbitration provisions. State legislatures in New York, New Jersey, Washington, Illinois, and California have moved to restrict mandatory arbitration for specific claim types. And the practical case for arbitration has softened as arbitration fees have risen materially and as plaintiffs have discovered mass-arbitration campaigns that impose thousands of individual filing fees on the employer at once.

A well-drafted 2026-era arbitration clause looks materially different from a 2018-era clause. This chapter maps the current enforceability landscape, the federal and state carve-outs, the drafting patterns that survive current law, and the practical trade-off between per-claim arbitration cost and class-action exposure.

## The Federal Arbitration Act and *Epic Systems*

The Federal Arbitration Act (9 U.S.C. §§ 1–16) makes written arbitration agreements involving interstate commerce "valid, irrevocable, and enforceable, save upon such grounds as exist at law or in equity for the revocation of any contract." The FAA's § 2 preempts state-law rules that single out arbitration agreements for special disfavor.

The FAA's § 1 carves out "contracts of employment of seamen, railroad employees, or any other class of workers engaged in foreign or interstate commerce." The Supreme Court in *Circuit City Stores, Inc. v. Adams*, 532 U.S. 105 (2001), narrowly construed the § 1 exemption to reach only *transportation* workers actually engaged in interstate commerce. The Court has since further clarified the transportation-worker carve-out in *Southwest Airlines Co. v. Saxon*, 596 U.S. 450 (2022) (baggage handlers who load cargo onto interstate flights are exempt), and in *Bissonnette v. LePage Bakeries Park St., LLC*, 601 U.S. 246 (2024) (transportation-worker exemption does not require that the worker's employer be in the transportation industry). For a technology startup with employees other than delivery drivers or interstate transportation crews, § 1 does not apply and the FAA governs.

In *Epic Systems Corp. v. Lewis*, 584 U.S. 497 (2018), the Supreme Court held that mandatory arbitration agreements with class-action waivers are enforceable under the FAA and do not conflict with the National Labor Relations Act's § 7 protection of concerted activity. Three cases were consolidated (*Epic Systems*, *Ernst & Young v. Morris*, *NLRB v. Murphy Oil*); the Court's 5-4 majority resolved the circuit split against the NLRB's position.

The doctrinal upshot after *Epic Systems*: employers can require employees to sign arbitration agreements as a condition of employment, and those agreements can bar the employee from participating in class or collective actions. The FAA preempts contrary state-law rules and contrary NLRA interpretations.

The practical upshot: the enforceability question no longer drives the design of an arbitration clause. The design questions are (a) which claim types the clause reaches, (b) how the corporation pays for arbitration and manages mass-arbitration risk, and (c) how the clause interacts with the federal and state carve-outs.

## The Ending Forced Arbitration Act (EFAA)

**Ending Forced Arbitration of Sexual Assault and Sexual Harassment Act of 2021** (Pub. L. No. 117-90, codified at 9 U.S.C. §§ 401–402), effective March 3, 2022, invalidates pre-dispute mandatory-arbitration and pre-dispute class/collective-action waivers with respect to any case that "relates to the sexual assault dispute or the sexual harassment dispute." At the plaintiff-employee's election, the case (or the covered portion of the case) proceeds in court rather than in arbitration, regardless of any pre-dispute agreement to the contrary.

Key mechanics:

- **The election belongs to the plaintiff, not the defendant.** The employee decides whether to enforce the arbitration agreement or invoke the EFAA carve-out. The employer cannot force arbitration once the EFAA is invoked.
- **"Relates to" is broadly construed.** Post-EFAA case law suggests that a hostile-work-environment claim with a sexual-harassment component brings the entire case within the EFAA carve-out, not just the specific harassment claim. Some courts have taken a narrower view. <!-- needs-research: verify the current circuit consensus on the scope of "relates to" for EFAA purposes; a hostile-work-environment case that combines sexual harassment with other Title VII theories is a common fact pattern where the scope question is decided. -->
- **Post-dispute arbitration is still enforceable.** The EFAA prohibits *pre-dispute* mandatory arbitration; the parties can voluntarily agree to arbitrate after a dispute arises.
- **Federal law preempts state law to the extent inconsistent.** The EFAA sets the federal floor; state statutes (like NY CPLR § 7515, California AB 51) that predated EFAA or extended further remain relevant to non-covered claims and to belt-and-suspenders analysis.

The corollary in **section 4 of the EFAA** — the Speak Out Act (Pub. L. No. 117-224, effective December 7, 2022) — additionally invalidates pre-dispute non-disclosure and non-disparagement clauses with respect to sexual-harassment and sexual-assault disputes. Any clause in an offer letter, employment agreement, or standalone NDA that would prohibit the employee from disclosing a sexual-harassment or sexual-assault dispute is unenforceable to that extent as against the employee.

Drafting implication: every arbitration provision must contain an explicit EFAA carve-out language, and every confidentiality / non-disparagement provision must contain an explicit Speak Out Act carve-out.

## PAGA — *Viking River*, *Adolph*, and the bifurcated animal

California's **Private Attorneys General Act** (Cal. Lab. Code § 2698 et seq.) authorises aggrieved employees to bring civil-penalty claims on behalf of the state for Labor Code violations. Because PAGA claims are technically brought as an agent of the state (the "aggrieved employee" is deputised to act for the state), they are not "individual" claims that a private arbitration agreement can bind — that was the California Supreme Court's holding in *Iskanian v. CLS Transportation Los Angeles, LLC*, 59 Cal. 4th 348 (2014).

**Viking River Cruises, Inc. v. Moriana**, 596 U.S. 639 (2022), partially overrode *Iskanian*. The Supreme Court held that:

- **Individual PAGA claims** — the employee's own PAGA claim seeking penalties for violations the employee personally suffered — *can* be compelled to arbitration under the FAA. *Iskanian*'s rule to the contrary was preempted.
- **Non-individual (representative) PAGA claims** — PAGA claims seeking penalties for violations suffered by other aggrieved employees — cannot be compelled to arbitration, but the plaintiff *loses standing* to pursue them once the individual PAGA claim is separated out and sent to arbitration.

The California Supreme Court in **Adolph v. Uber Technologies, Inc.**, 14 Cal. 5th 1104 (2023), rejected the standing conclusion. The California court held as a matter of California standing law that an employee who is compelled to arbitrate the individual PAGA claim *retains standing* to pursue the non-individual PAGA claims in court. The federal court's *Viking River* reading of California standing law was, per *Adolph*, incorrect.

The current operative framework in California:

- The employer can compel the individual PAGA claim to arbitration.
- The non-individual (representative) PAGA claim proceeds in court, stayed pending the arbitration outcome.
- If the arbitrator finds the employee is an "aggrieved employee" who suffered a Labor Code violation, the court reopens the non-individual PAGA claim, which the employee retains standing to prosecute.
- If the arbitrator finds the employee did not suffer any Labor Code violation, the employee loses standing (having no basis to be "aggrieved") and the representative PAGA claim is dismissed.

**PAGA reform — SB 92 and AB 2288 (2024).** The California Legislature significantly revised PAGA in mid-2024, adjusting penalty caps, expanding cure and reform options for employers, adjusting the distribution of penalties (65% to state / 35% to employees, vs. the pre-reform 75/25), and strengthening the standing and notice requirements. <!-- needs-research: verify the current text and implementation status of PAGA reform after SB 92 and AB 2288, including the litigated scope of the amended cure provisions. -->

**Drafting implication.** A California-employee arbitration provision must (a) explicitly compel individual PAGA claims to arbitration, (b) explicitly acknowledge that non-individual PAGA claims are not compelled, (c) address the stay-pending-arbitration mechanics, and (d) not attempt to waive representative PAGA claims (which is unenforceable per *Iskanian* to the extent not overridden by *Viking River*). A generic "all claims to arbitration including class and representative actions" clause is a drafting defect that a plaintiff's attorney will exploit and that a California court will sever or strike.

## State-law layer beyond PAGA

Several states have enacted statutes restricting mandatory arbitration of specified claim types. Post-EFAA, the state statutes are often (a) redundant for sexual-harassment/assault claims (federal law now covers), (b) additive for other claim types (harassment, discrimination, retaliation, wage-and-hour), and (c) preempted by the FAA to the extent they single out arbitration.

- **California — Cal. Lab. Code § 432.6 (AB 51, 2019).** Prohibits an employer from requiring, as a condition of employment or the receipt of any employment-related benefit, that an applicant or employee waive any right, forum, or procedure for a violation of FEHA or the California Labor Code — targeting mandatory arbitration. In *Chamber of Commerce v. Bonta*, 62 F.4th 473 (9th Cir. 2023), the Ninth Circuit held AB 51 is preempted by the FAA to the extent it applies to arbitration agreements entered into after March 3, 2022. The residual scope is narrow.
- **New York — CPLR § 7515 (2018, amended 2019).** Prohibited mandatory arbitration of certain harassment and discrimination claims. Partially preempted by the FAA (federal courts have generally held so — see *Latif v. Morgan Stanley & Co.*, 2019 WL 2610985 (S.D.N.Y. June 26, 2019)); the state statute continues to matter in state-court venues and for non-FAA-covered contracts.
- **New Jersey — N.J.S.A. § 10:5-12.7 (2019).** Prohibits waiver of substantive or procedural rights or remedies under the New Jersey Law Against Discrimination. Same preemption analysis.
- **Washington — RCW 49.44.210.** Restricts mandatory arbitration of discrimination and harassment claims. Same preemption analysis.
- **Illinois — Workplace Transparency Act (820 ILCS 96).** Prohibits mandatory arbitration of certain claims. Same preemption analysis.

The pattern: state statutes have been substantially preempted by the FAA except in narrow contexts. Where the corporation is in a preempted state, the arbitration clause is enforceable; where the corporation is in the narrow non-preempted context (post-dispute arbitration, non-FAA contract, transportation worker), the state statute matters.

## The NLRB *McLaren Macomb* posture on confidentiality and non-disparagement

In **McLaren Macomb**, 372 NLRB No. 58 (Feb. 21, 2023), the National Labor Relations Board held that overly broad confidentiality and non-disparagement clauses in separation agreements violate NLRA § 8(a)(1) by "chilling" employees' § 7 rights to engage in concerted activity for mutual aid or protection. The decision voided the challenged separation-agreement clauses and, by implication, similar clauses in offer letters, employment agreements, and arbitration provisions.

**Practical drafting implications:**

- Confidentiality and non-disparagement clauses must be narrowly tailored — cannot prohibit the employee from discussing wages, working conditions, or the terms of the agreement with coworkers, from filing a charge with the NLRB / EEOC / state FEPA, from cooperating with a government investigation, or from otherwise engaging in protected concerted activity.
- Broad "you shall not disclose any information about this agreement or your employment" language is void as against a covered employee.
- The clause should carry an express carve-out for NLRA § 7 rights, EEOC/state-agency charge-filing rights, and government-investigation cooperation.

The NLRB's General Counsel has issued follow-on guidance (Memorandum GC 23-05, March 22, 2023) clarifying the scope of *McLaren Macomb*, its retroactive effect, and the acceptable savings-clause language. <!-- needs-research: verify the current NLRB posture on McLaren Macomb after any 2025–2026 Board membership changes; the Board's position has historically shifted with administration transitions. -->

The interaction with arbitration: an arbitration clause frequently sits within a broader employment agreement or offer letter that has confidentiality and non-disparagement provisions elsewhere. The corporation's belt-and-suspenders drafting posture is to add the NLRA / EEOC / government-cooperation carve-out to the arbitration clause itself as well as to the confidentiality section, so that no reader can plausibly interpret the arbitration clause as barring protected communications.

## The FLSA collective-action question

The Fair Labor Standards Act permits "collective actions" under 29 U.S.C. § 216(b) — the FLSA's variant of a class action, using opt-in rather than opt-out procedure. Post-*Epic Systems*, class-action-waiver language enforceably bars FLSA collective actions if the arbitration agreement is otherwise enforceable. A well-drafted class-and-collective-action waiver reaches FLSA collective actions, state wage-and-hour class actions, ERISA class actions, and other aggregate procedures.

The drafting posture: enumerate the specific procedural mechanisms the waiver reaches, rather than relying on a generic "no class or collective action" formulation. Enumeration reduces the interpretive risk that a court sever-and-preserve analysis leaves a hole.

## The mass-arbitration problem

Class-action-waiver clauses were sold to employers on the theory that they eliminated aggregate exposure. In the last five years, plaintiffs' firms have discovered that they can weaponise the very individual-arbitration requirement the employer negotiated for — by filing thousands of individual arbitration demands at once, each triggering the employer's obligation under AAA / JAMS rules to pay the individual filing fee (commonly $2,000+ per case) up-front. Uber, DoorDash, Amazon, Chipotle, and many others have faced mass-arbitration campaigns with 5,000–100,000+ filings.

The result: an employer that pushed all disputes into individual arbitration and then received 30,000 individual arbitration demands owes $60M+ in filing fees before the underlying merits are addressed. Mass arbitration has arguably re-invented the aggregate-exposure risk that the class-action-waiver was designed to eliminate.

**Practitioner responses have included:**

- **Batched-arbitration protocols.** Contract terms that require plaintiffs to proceed in coordinated batches (e.g., 100 cases at a time, with the results of the batch informing settlement discussions on the remainder). AAA and JAMS have rolled out modified mass-arbitration rules that provide for administrative-fee reductions when large numbers of demands are filed together.
- **Fee-shifting mechanisms.** Arbitration clauses that require the losing party to bear filing fees, or that structure filing-fee payment through mediation and pre-arbitration conferring steps. Enforceability of employer-friendly fee-shifting is state-and-federal-law specific.
- **Small-claim court carve-outs.** Clauses that allow individual employees to pursue certain claims in small-claims court instead of arbitration, on the theory that most employees will not do so and that the option preserves an argument that the arbitration provision is not unconscionable.
- **Reverting to court.** Some employers, having done the mass-arbitration math, have simply removed the arbitration clause and preferred class-action exposure in court. This is a live and legitimate strategy for populations where mass-arbitration risk is meaningful (large hourly workforces, gig-economy classifications, alleged wage-hour violations).

For a startup with a 50-300-person exempt employee base, mass arbitration is a lower-probability event than for a 30,000-person hourly workforce. The mass-arbitration question is nonetheless part of the drafting discussion for any corporation that expects to grow into a larger workforce, particularly one with non-exempt or contractor populations.

## Practical drafting patterns

Below are the operating patterns for a modern arbitration provision in an offer letter or standalone arbitration agreement.

### Scope of covered claims

Enumerate the covered claims. A common pattern:

- All disputes arising out of or relating to the employee's employment, termination, or compensation, including but not limited to claims under Title VII, the ADA, the ADEA (subject to OWBPA), the FLSA, the FMLA, § 1981, ERISA, and the wage-and-hour and anti-discrimination statutes of any state where the employee performs work.
- Explicit exclusion of the EFAA-covered claims (sexual-assault and sexual-harassment disputes at the employee's election).
- Explicit exclusion of representative PAGA claims for California employees.
- Explicit exclusion of workers'-compensation claims (which under state law generally proceed through the state administrative agency).
- Explicit exclusion of unemployment-insurance claims.
- Explicit exclusion of NLRB charge-filing.
- Explicit exclusion of EEOC / state FEPA charge-filing (which is a statutory right the employee retains regardless of any private agreement) — while retaining the ability to compel to arbitration any subsequent private civil suit.

### Class and collective-action waiver

- Explicit waiver of the right to bring or participate in a class action, collective action, or representative action, except as to representative PAGA claims and any other claim types not lawfully waivable.
- Provision that any question of the arbitrator's authority to hear class or collective claims is a "question of arbitrability" for the court to decide, not the arbitrator (to avoid *Stolt-Nielsen* / *Lamps Plus* interpretive risk).
- Severability clause providing that if the class-waiver provision is held unenforceable, the class-related claims proceed in court and the individual claims remain in arbitration.

### Arbitration forum, procedure, and cost

- Designated arbitration forum (typically AAA or JAMS) and the applicable rules (AAA Employment Arbitration Rules, JAMS Employment Arbitration Rules and Procedures).
- Location — typically the county where the employee performed work.
- Employer pays arbitration fees and administrative costs beyond what the employee would pay in court (this is a *California enforceability requirement* per *Armendariz v. Foundation Health Psychcare Services, Inc.*, 24 Cal. 4th 83 (2000), and is broadly required in other states as well; failure to include this provision is a common enforceability defect).
- Employee retains right to counsel; each party bears its own attorneys' fees except to the extent that fee-shifting is available under the underlying substantive statute (Title VII, FLSA, § 1981, etc.).
- Right to full discovery consistent with the AAA / JAMS employment rules and consistent with *Armendariz* (which requires arbitration discovery to be adequate for the vindication of statutory rights).
- Written decision on the merits, including findings of fact and conclusions of law.
- Judicial review consistent with the FAA (limited grounds under 9 U.S.C. § 10).

### EFAA carve-out

- Explicit statement that, notwithstanding any other provision, the employee may elect at any time to have any dispute that constitutes or relates to a "sexual assault dispute" or "sexual harassment dispute" (as defined in 9 U.S.C. §§ 401–402) proceed in a court of competent jurisdiction rather than in arbitration.
- Companion clause in the confidentiality / non-disparagement section per the Speak Out Act.

### PAGA carve-out (California employees)

- Individual PAGA claims compelled to arbitration.
- Non-individual (representative) PAGA claims are not waived and are not compelled to arbitration.
- Stay-pending-arbitration mechanics per *Adolph*.

### NLRA / EEOC / government-investigation carve-out

- Nothing in the arbitration provision (or the associated confidentiality / non-disparagement provisions) prohibits the employee from (a) filing a charge with the NLRB, EEOC, state FEPA, DOL, SEC, or any other government agency; (b) participating in a government investigation; (c) reporting suspected violations of law; (d) engaging in NLRA-protected concerted activity, including discussing wages, working conditions, or the terms of the employment relationship with coworkers.
- Preservation of DTSA whistleblower immunity per 18 U.S.C. § 1833(b)(3) — see [chapter 04](./04-employee-piia.md) and [mod-102 chapter 05](../mod-102-founding-team-legal-architecture/05-dtsa-whistleblower-and-trade-secret-baseline.md).

### Notice and consideration

- The arbitration provision is provided to the employee with adequate opportunity to review — some states (Massachusetts, Illinois) require specific pre-employment notice periods; California case law (*Armendariz*) requires the arbitration agreement to be a bilateral, mutual agreement (both employer and employee bound), not employee-only.
- Consideration — the offer of employment (for new hires) or continued employment (for existing employees, where state law permits) is the consideration. Some state case law requires additional consideration for existing-employee arbitration agreements; check state law.

### Severability and reformation

- If any provision of the arbitration agreement is held invalid or unenforceable, the invalid provision is severed and the remainder enforced to the maximum extent permitted by law.
- A "poison pill" — some clauses provide that if the class-action waiver is held unenforceable, the entire arbitration agreement is unenforceable and all claims proceed in court. This is an anti-mass-arbitration protective structure that the corporation may or may not want, depending on its risk posture.

## The practical trade-off: when arbitration is worth it and when it isn't

Arbitration is not a free lunch. The trade-off has evolved:

**Reasons to include mandatory arbitration:**

- Individual-claim resolution is faster and cheaper than court (for most single-plaintiff cases).
- Class-action exposure in court is materially larger than the sum of individual arbitrations for a well-drafted waiver.
- Confidentiality of proceedings — arbitration awards are not typically part of the public record.
- Reduced discovery scope compared to federal court (though *Armendariz* limits this reduction for statutory-rights cases).

**Reasons to exclude mandatory arbitration:**

- Mass-arbitration exposure for populations that plaintiffs' firms coordinate against.
- Employer-friendly damages-cap and evidentiary rules in some jurisdictions may make court more favorable for certain claim types.
- Employee-recruiting friction — arbitration provisions are increasingly seen negatively by prospective employees, particularly in the post-*Bostock* / post-EFAA landscape, and many corporations have removed mandatory arbitration to signal a modern employment brand (Google, Microsoft, Facebook, Uber all publicly ended mandatory arbitration for at least some claim types in 2018–2019).
- Public-optics risk — a mandatory-arbitration provision that produces a plaintiff-alleged pattern of hidden harassment complaints creates its own reputational exposure.
- Reduced value post-*Viking River* / EFAA / *McLaren Macomb* — the most-consequential claims (sexual harassment, PAGA representative, whistleblower, NLRA charge) are increasingly outside the reach of the arbitration provision anyway.

**The middle path.** Some corporations retain arbitration for wage-and-hour and general-employment claims (where class-action exposure is meaningful) but exclude discrimination and harassment claims broadly (not just the EFAA-covered slice), on the theory that (a) the reputational optics are better and (b) discrimination and harassment claims lend themselves to individual-plaintiff resolution in court without material aggregate risk.

## Concrete example: the arbitration clause for a distributed 50-person workforce

Acme Robotics has 50 employees across California, Colorado, Illinois, New York, Washington, and Massachusetts, all salaried professionals, most in engineering and product roles. The arbitration provision in the standard offer letter (with a separate California-employee addendum):

- **Scope.** All disputes arising out of or relating to the employee's employment, termination, or compensation, including but not limited to claims under Title VII, the ADA, the ADEA (subject to OWBPA), the FLSA, the FMLA, § 1981, ERISA, and the wage-and-hour and anti-discrimination statutes of the state where the employee performs work.
- **EFAA carve-out.** Sexual-harassment and sexual-assault disputes are not covered at the employee's election.
- **Class and collective-action waiver.** Explicit; excluded representative PAGA per California addendum; carve-out for non-waivable claim types.
- **Forum.** AAA under AAA Employment Arbitration Rules; location in the county where the employee performed work; employer pays arbitration fees and administrative costs beyond what the employee would pay in court.
- **NLRA / EEOC / government carve-out.** Employee retains right to file charges with any government agency, participate in government investigations, engage in protected concerted activity, and disclose wages / working conditions to coworkers.
- **DTSA whistleblower immunity.** Explicit.
- **PAGA (California employees, addendum).** Individual PAGA claims compelled to arbitration; representative PAGA claims not waived; stay-pending-arbitration mechanics.
- **Severability.** Standard, with class-waiver-severed-not-agreement-severed formulation.
- **Notice.** Provided with the offer letter, at least 14 days before signing per Illinois Freedom to Work Act baseline (adopted nationally for simplicity), with express advice to consult counsel.

Sensitive drafting choices:

- **Confidentiality and non-disparagement** in the offer letter itself are drafted with *McLaren Macomb* carve-outs.
- **The Speak Out Act** requires the confidentiality clause to carve out sexual-harassment / sexual-assault disclosure explicitly.
- **The California addendum** also addresses the *Armendariz* mutuality requirements and pays specific attention to arbitration-cost allocation.

Acme's counsel refreshes the clause annually and after any material Supreme Court decision, NLRB decision, or federal / state statutory change touching arbitration or the class-waiver structure.

## The choice not to require arbitration

Some corporations decide that the reputational and mass-arbitration downsides outweigh the benefits, and go with court-based dispute resolution for all claim types. If the corporation makes this choice, the drafting move is not to *remove* the arbitration provision from an existing template — it is to *replace* it with a clear choice-of-forum, choice-of-law, venue-selection, jury-trial-waiver, and (where enforceable) fee-shifting structure that reflects an intentional court-based dispute-resolution posture. Silence in the offer letter defaults to whatever state law provides, which is unlikely to be what the corporation wants.

The class-action-waiver still has independent value in some contexts even without arbitration — some contracts include a class-action waiver enforceable through court proceedings, though state-law and unconscionability analysis is more skeptical of court-based class waivers than of arbitration-based ones (see *American Express Co. v. Italian Colors Restaurant*, 570 U.S. 228 (2013), and the state-law limits some courts apply outside the FAA context).

## Summary

- Under *Epic Systems* (2018) and the FAA, mandatory employment arbitration with class-action waiver is enforceable, subject to a growing list of federal and state carve-outs.
- The Ending Forced Arbitration Act (2022, 9 U.S.C. §§ 401–402) invalidates pre-dispute mandatory arbitration for sexual-assault and sexual-harassment disputes at the employee's election. The Speak Out Act (2022) invalidates pre-dispute non-disclosure and non-disparagement clauses covering the same claim types.
- California's PAGA is bifurcated after *Viking River* (2022) and *Adolph* (2023): individual PAGA claims can be compelled to arbitration; non-individual (representative) PAGA claims cannot, and the employee retains standing to pursue them after arbitration. PAGA reform (SB 92 / AB 2288, 2024) adjusted penalty caps and cure options but did not alter the bifurcation structure.
- The NLRB in *McLaren Macomb* (2023) voided overly broad confidentiality and non-disparagement clauses; arbitration provisions must carry NLRA § 7, EEOC / government charge-filing, and government-cooperation carve-outs.
- Mass-arbitration campaigns have created a new aggregate-exposure risk that class-waiver was meant to eliminate. Batched-arbitration protocols, filing-fee structures, and — increasingly — a decision not to require arbitration at all are the practitioner responses.
- A well-drafted 2026-era arbitration clause enumerates the covered claim types, carves out the EFAA and PAGA and NLRA and government-agency slices, addresses arbitration-forum and cost allocation, provides for severability, and is delivered with adequate notice and consideration under the applicable state law.
- The include-or-exclude decision is a real trade-off. Corporations increasingly exclude discrimination and harassment claims broadly, either through the EFAA carve-out or voluntarily beyond it, and reserve arbitration for wage-and-hour and general-employment claims where the mass-arbitration risk is manageable and the class-action-in-court exposure is meaningful.
