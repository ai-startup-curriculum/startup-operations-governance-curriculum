# 8. Executive severance and release architecture

> Executive severance is not a goodbye gift. It is the back-half of the compensation package the corporation wrote on day one — the piece that compensates the executive for being personally on the hook for board-visible, investor-visible, and public-facing outcomes the executive cannot fully control.

## Motivation

The individual-contributor severance conversation is small. US employment is at-will by default; most IC separations in a venture-backed startup carry 0–4 weeks of severance per year of service (if any), capped in the 12–16 week range, with a basic release of claims. The executive-severance conversation is categorically different, and it is a comp-committee artifact — not an HR artifact.

The reason executive severance is bigger is not generosity. It is risk-sharing. A CEO, CFO, COO, CPO, or General Counsel sits in a seat where (a) the board can terminate the executive at will under the officer-service default (chapter in [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/)), (b) the executive's own equity vests over four years and front-ends very little in cash, (c) the executive's reputational outcome is tied to a board-and-investor-visible narrative the executive cannot fully author, and (d) a mid-cycle involuntary termination without severance would be career-defining in a way an IC separation would not. The severance package is the risk premium that makes an executive willing to accept a cash-light compensation structure anchored on equity and board-driven employment terms (see [./04-executive-compensation-packages.md](./04-executive-compensation-packages.md)).

The architecture of that severance package has moving parts the comp committee, the GC, outside employment counsel, and outside tax counsel each own a piece of. This chapter organises them.

## Why executive severance differs structurally from IC severance

### IC severance — the baseline

- At-will default; no statutory severance obligation in the US absent a WARN Act group-RIF trigger or a plant-closing statute.
- Market practice in venture-backed startups: 2–4 weeks of base per year of service, often capped at 12–16 weeks, with COBRA subsidy for the severance period and a general release of claims. <!-- needs-research: confirm current-market IC severance band across venture-backed startups; the numbers above are commonly cited practitioner defaults but should be checked against a recent survey. -->
- No equity acceleration. Unvested options and RSUs are forfeited on the termination date.
- Released claims scope: standard general release of statutory and common-law claims, with OWBPA 21/7-day formalities only for age-40+ separations.

### Executive severance — the premium

- 6–12 months of base plus some fraction of target bonus plus 6–12 months of COBRA / benefits continuation. CEO packages sometimes stretch to 18 months. <!-- needs-research: confirm current-market C-suite severance multiples by role (CEO vs. CFO vs. COO vs. CPO vs. GC) across Series B through pre-IPO; Equilar / Compensia / Pearl Meyer surveys are the usual sources. -->
- Equity acceleration — single-trigger on involuntary termination without cause for some packages; double-trigger (CoC + termination) is the near-universal CoC construct (see [./07-change-of-control-equity-policy.md](./07-change-of-control-equity-policy.md)).
- Good-reason resignation as a severance trigger — recognises that a materially-degraded role (reduced duties, reduced comp, forced relocation, change in reporting line) is a constructive termination.
- Payment timing driven by IRC § 409A — not by payroll convenience.
- 280G safe-harbor engineering in CoC scenarios.
- A release-and-non-disparagement agreement with mutual non-disparagement, continuing-cooperation covenant, and specific statutory carve-outs.

The structural point is that the IC severance program is a notice-and-hardship program; the executive severance program is a *risk-shifting* program. The design levers are different, and the review cadence is different (comp committee, not just HR).

## The executive severance agreement

The agreement is either (a) a standalone contract signed at hire, (b) a section embedded in the executive's offer letter, or (c) coverage under a formal "Executive Severance Plan" (see below). Whichever form, the eight recurring provisions are:

### (a) Triggering events

Two triggers are standard:

- **Involuntary termination without cause.** "Cause" is specifically defined — commonly includes (i) material breach of a written policy or agreement after notice and cure, (ii) wilful misconduct or gross negligence, (iii) commission of a felony or crime involving moral turpitude, (iv) material failure to perform duties after notice. Narrow drafting of "cause" is the executive's biggest leverage point — a loose cause definition can be used to terminate without triggering severance.
- **Good-reason resignation.** A resignation that follows one of a specified set of materially-adverse events — reduction in base, reduction in target bonus or target-incentive-opportunity, material reduction in duties / authority / reporting line, relocation of principal workplace by more than a specified distance, material breach by the corporation of the executive's agreement — with a notice-and-cure period (commonly 30 days' notice from the executive and 30 days' cure for the corporation) and a time limit on resignation after the triggering event (commonly 90 days).

### (b) Severance payment

Lump-sum vs. salary-continuation installments. Installments are the §409A-friendly default (short-term deferral and separation-pay exceptions below). Lump-sum post-tax is cleaner for the executive but more constrained by §409A.

Composition:

- Base pay for the severance period (6, 12, or 18 months).
- Target bonus — the full target amount, pro-rata through termination, or the full target annualised and multiplied by the severance-period fraction. Each produces materially different dollars.
- Earned-but-unpaid prior-year bonus if the fiscal year closed before termination.

### (c) Benefits continuation

COBRA premium subsidy for the severance period. Taxability of employer-paid COBRA after the ACA § 105(h) non-discrimination rules is a drafting consideration — a common fix is to pay the executive a taxable cash amount equal to the COBRA premium rather than directly subsidising the premium.

### (d) Equity acceleration

Cross-reference [./07-change-of-control-equity-policy.md](./07-change-of-control-equity-policy.md) for the double-trigger CoC structure. Standalone (non-CoC) acceleration is less common for pre-IPO; where present, it is usually 6–12 months of additional vesting on involuntary termination without cause.

### (e) Release-and-non-disparagement execution requirement

Severance is conditioned on execution — and non-revocation — of a general release of claims. The release-timing mechanics are a §409A compliance item (below).

### (f) 280G modified-economic-cutback

See [separate section below](#the-280g-modified-economic-cutback). The agreement specifies the cutback formula and the responsible-party for the gross-up / cutback calculation.

### (g) 409A compliance representations

Specific drafting that structures all payments as either (i) short-term deferrals, (ii) separation-pay-exception payments, or (iii) §409A-compliant deferred compensation. The agreement typically includes a §409A savings-clause.

### (h) Non-compete / non-solicit survivors

Post-separation restrictive covenants that survive termination — cross-reference [../mod-103-employment-law-and-contract-design/06-non-compete-landscape-and-alternatives.md](../mod-103-employment-law-and-contract-design/06-non-compete-landscape-and-alternatives.md). California-based executives cannot be bound by post-employment non-competes; non-solicits of customers and employees are the practical alternative. For non-California executives, the non-compete duration should align with the severance period — asking an executive to sit out for 12 months while paying only 6 months of severance is both unfair and (in most jurisdictions requiring consideration-and-proportionality analysis) unenforceable.

## IRC § 409A compliance for severance

Section 409A of the Internal Revenue Code governs non-qualified deferred compensation. Severance is deferred compensation unless it fits an exception, and §409A violations trigger a 20% additional income tax on the executive (plus interest) — a cost the corporation often has to indemnify in practice.

### Payment-timing exceptions

- **Short-term deferral exception** — payment made within 2.5 months after the end of the calendar year (or fiscal year, if later) in which the right to the payment is no longer subject to a substantial risk of forfeiture. A severance payment made within 2.5 months of year-end following termination is outside §409A. Treas. Reg. § 1.409A-1(b)(4).
- **Separation-pay exception** — severance paid on involuntary termination that (i) does not exceed 2× the lesser of the executive's annualised comp or the IRC § 401(a)(17) compensation limit, and (ii) is paid in full by the end of the second calendar year following termination. Treas. Reg. § 1.409A-1(b)(9). <!-- needs-research: confirm current-year IRC § 401(a)(17) comp limit used in the separation-pay-exception cap; the cap is indexed annually. --> For most C-suite packages, the cap binds — the executive's annualised comp easily exceeds the § 401(a)(17) limit — and the exception operates up to 2× that capped amount.

### Specified-employee six-month-delay rule — IRC § 409A(a)(2)(B)(i)

For a "specified employee" of a corporation whose stock is publicly traded on an established securities market, any payment of deferred compensation on account of separation from service must be delayed by at least six months after separation. A "specified employee" is generally one of the top 50 officers by compensation (subject to specific identification rules — Treas. Reg. § 1.409A-1(i)).

Practically: a privately-held corporation is not subject to the six-month delay until it has an initial public offering of its stock (or stock otherwise becomes publicly tradable on an established securities market). The IPO-adjacency implication is that an executive-severance agreement written pre-IPO must be re-papered — or at minimum reviewed — before an S-1 is filed, to add the specified-employee delay for payments that would otherwise commence within six months of separation. A §409A-savings-clause typically handles this automatically, but a bespoke review before the public-offering transition is the responsible-practitioner default.

### Release-of-claims timing — the standard §409A fix

A severance package conditioned on execution of a release raises a §409A timing problem: if the executive can delay signing (and therefore delay the start of severance payments) across two tax years, the executive is effectively exercising a prohibited election over the payment year. The standard §409A-compliant fix is a **60-day release-execution-and-non-revocation window**:

- The release must be delivered to the executive within a specified number of days after separation (commonly 5–7 days).
- The executive has a specified window to execute (21 days for an individual separation if OWBPA applies — see below — or 45 days for a group termination program), followed by a 7-day OWBPA revocation window if the executive is age 40+.
- The combined 60-day window ends on a date certain, and severance payments commence on the first regular payroll date *after* the end of the 60-day window regardless of when within the window the executive actually signed. This structure prevents the executive from exercising a tax-year election by timing the signature.

Severance drafting that pays on signature-plus-X-days is a §409A trap; the release-execution-window-plus-payment-on-first-payroll-after-window-end pattern is the fix.

## The release-and-non-disparagement agreement

The release is a separate instrument — executed at separation, not at hire — that converts the severance commitment into a bilateral release of claims. The eight recurring provisions:

### General release of claims

A general release of all claims against the corporation, its officers, directors, subsidiaries, affiliates, and insurers, through the effective date. Specific statutes called out — Title VII, ADA, ADEA, FLSA, ERISA, state analogues (FEHA, NY HRL, Illinois HRA, etc.). Common-law tort and contract claims released.

### Carve-outs

The release must expressly carve out non-waivable rights:

- **Unemployment insurance** — cannot be waived by private contract.
- **Workers' compensation** — cannot be waived.
- **Vested retirement benefits** — ERISA-protected.
- **Indemnification rights** under the corporation's charter, bylaws, indemnification agreement, and D&O insurance — see [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).
- **D&O insurance coverage** for pre-separation acts.
- **Claims arising after signing.**
- **Right to file a charge with — or participate in an investigation by — the EEOC, NLRB, SEC, OSHA, or state analogues** (the executive can file but typically waives the right to individual monetary recovery, with limited exceptions for SEC whistleblower bounties under *Dodd-Frank § 21F*).

### Non-disparagement — mutual

A mutual non-disparagement provision binds both the executive and the corporation (specifically, the corporation's officers and directors in their official capacity, with a defined speaker-set). Scope covers the corporation, its officers, directors, affiliates, and products. One-sided non-disparagement — binding only the executive — is a market-weakness signal and increasingly unenforceable or disfavored in jurisdictions that have moved on gag-clause reform.

### Post-Speak-Out-Act carve-outs — Pub. L. No. 117-224 (December 7, 2022)

The **Speak Out Act** renders pre-dispute non-disclosure and non-disparagement clauses judicially unenforceable with respect to a sexual-harassment dispute or a sexual-assault dispute. A broad pre-dispute gag — signed at hire or signed as part of a general release before any dispute has arisen — cannot be enforced to silence a sexual-harassment or sexual-assault claimant. **Post-dispute** confidentiality — a settlement NDA signed after a specific sexual-harassment or sexual-assault dispute has arisen — remains possible but requires careful drafting. The release should include an express carve-out acknowledging the Speak Out Act and preserving the executive's right to speak about sexual-harassment and sexual-assault matters.

### EFAA cross-reference — Pub. L. No. 117-90 (March 3, 2022)

The **Ending Forced Arbitration of Sexual Assault and Sexual Harassment Act of 2021** renders pre-dispute arbitration agreements and pre-dispute joint-action waivers unenforceable at the claimant's election for sexual-harassment and sexual-assault disputes. The release should cross-reference EFAA where the executive's arbitration agreement survives separation, confirming that EFAA-covered claims are not swept into mandatory arbitration. See [../mod-103-employment-law-and-contract-design/09-arbitration-and-class-action-waivers.md](../mod-103-employment-law-and-contract-design/09-arbitration-and-class-action-waivers.md).

### Continuing cooperation covenant

The executive agrees to cooperate with the corporation on pending or future litigation, government investigations, regulatory inquiries, and transition matters for a defined period (6–12 months is typical). The corporation reimburses reasonable expenses (travel, counsel if separately-represented). Cooperation obligations beyond reasonable expense reimbursement — e.g., a per-hour compensation rate — are negotiated in packages for executives with substantial pending-litigation exposure.

### Return of corporate property and transition deliverables

Specific list — devices, documents, access credentials, keys, equity-plan-related documentation. Confirmation that no corporate information retained.

### Reaffirmation of surviving covenants

Confidentiality (PIIA / NDA — see [../mod-103-employment-law-and-contract-design/04-employee-piia.md](../mod-103-employment-law-and-contract-design/04-employee-piia.md)), non-solicitation of employees and customers, and any applicable post-employment non-compete. The executive reaffirms that these covenants survive separation per their original terms.

## OWBPA-compliant release for age-40+ separations

The **Older Workers Benefit Protection Act — 29 U.S.C. § 626(f)** sets formalities for a release of ADEA claims by an employee age 40 or older. Non-compliance invalidates the ADEA release even if the release is otherwise properly executed.

The specific requirements:

- **§ 626(f)(1)(E)** — the release must advise the employee in writing to consult with an attorney before signing.
- **§ 626(f)(1)(F)(i)** — the employee must be given **at least 21 days** to consider the release. For a group termination program (two or more employees terminated as part of an exit incentive or other employment-termination program), **at least 45 days**.
- **§ 626(f)(1)(G)** — the employee has **7 days after signing to revoke**. Severance payments cannot commence until the 7-day revocation period expires.
- **§ 626(f)(1)(H)** — for a group termination program, the employer must provide a list of (i) the job titles and ages of all employees eligible or selected for the program, and (ii) the ages of all employees in the same job classification or organisational unit not eligible or selected. **Even a two-person RIF structured as a program counts** — the group disclosure is not reserved for large RIFs.

The practical implication for an age-40+ executive separation: the release and severance timing have to accommodate the 21-day consideration + 7-day revocation = 28-day minimum (or 45 + 7 = 52 days for a group), and the 60-day §409A release-window is a comfortable envelope that absorbs this. For age-under-40 executives, OWBPA does not apply, but the 60-day §409A window is still the drafting default for consistency.

## SEC Reg S-K Item 402(j) disclosure — the pre-IPO flag

Once the corporation files an S-1, **Reg S-K Item 402(j)** requires narrative and tabular disclosure of potential payments upon termination or change-in-control for each named executive officer. The executive severance structure drives the Item 402(j) table — a specified-dollar-amount estimate at year-end of what each NEO would receive under each termination scenario (voluntary resignation, involuntary termination without cause, good-reason resignation, change-in-control with termination, death, disability). The mechanics of the disclosure are deferred to [./09-sec-reg-sk-item-402-disclosure.md](./09-sec-reg-sk-item-402-disclosure.md); the flag here is that the severance architecture written years before IPO ends up as a public-filing line item, and the comp committee should design it with that eventual disclosure visibility in mind.

## The severance-tier design

A sensible pre-IPO corporation has a tiered severance architecture with explicit role-based bands rather than individually-negotiated packages at every hire. The archetypal tiers:

### C-suite tier

- **CEO** — 12 months base + target bonus + 12 months COBRA + double-trigger CoC acceleration of 100% of unvested equity. Some corporations extend to 18 months on involuntary termination without cause. <!-- needs-research: confirm current-market CEO severance multiples pre-IPO; Compensia and Pearl Meyer survey data is the usual source. -->
- **CFO, COO, CPO, GC** — 12 months base + target bonus + 12 months COBRA + double-trigger CoC acceleration of 100% of unvested equity on CoC.

### VP tier

- 6–9 months base + pro-rata target bonus + 6–9 months COBRA + double-trigger CoC acceleration of 50–100% of unvested equity. <!-- needs-research: confirm current-market VP severance multiples pre-IPO. -->

### IC tier

- 2–4 weeks of base per year of service, capped at 12–16 weeks. COBRA subsidy for the severance period. No equity acceleration. <!-- needs-research: confirm current-market IC severance band. -->

The tier architecture should be adopted as a comp-committee policy — not negotiated separately for each hire — so that comp decisions are consistent across the executive team and so that the Item 402(j) disclosure, when it eventually lands, shows a coherent policy rather than an ad-hoc patchwork.

## Severance plan vs. individual agreement

Two architectures:

### Individual severance agreements

Each executive has a standalone severance agreement (or embedded offer-letter terms). The corporation negotiates variances individually. **Advantages** — flexibility, bespoke terms per executive, no ERISA plan administration overhead. **Disadvantages** — inconsistency, drift over time, difficult comp-committee oversight, Item 402(j) disclosure complexity.

### Formal Executive Severance Plan

The corporation adopts a written plan — a Severance Plan or an Executive Severance Benefits Plan — that specifies tiers, triggers, payment formulas, and governance. The plan is typically an **ERISA welfare-benefit plan** subject to ERISA's reporting (Form 5500 if 100+ participants), disclosure (SPD), and claims-procedure requirements. **Advantages** — consistency, cleaner comp-committee oversight, ERISA claims-procedure governs disputes (preempting state-law breach-of-contract claims and often favoring the plan sponsor), simpler Item 402(j) disclosure. **Disadvantages** — ERISA administration, less flexibility for bespoke terms, plan-amendment process required for changes.

Most pre-IPO corporations end up with a hybrid — a Severance Plan covering the C-suite and VP tiers with standard terms, plus individual amendments for the CEO and sometimes the CFO.

## The 280G modified-economic-cutback

**IRC § 280G** disallows the corporate deduction for — and imposes a 20% excise tax on the executive under IRC § 4999 for — "parachute payments" that are contingent on a change in control and that exceed three times the executive's base-amount (five-year average W-2 compensation). The excise-tax trigger is a cliff: if parachute payments equal 2.99× base-amount, no excise tax; if they equal 3.00× base-amount, excise tax applies to everything above 1.00× base-amount.

Pre-public-company corporations have a specific 280G shareholder-approval cleansing procedure (IRC § 280G(b)(5)) that private corporations use to eliminate 280G exposure before CoC closing. See [./07-change-of-control-equity-policy.md](./07-change-of-control-equity-policy.md) for depth.

The **modified-economic-cutback** is the severance-agreement clause that handles 280G exposure when the shareholder-approval cleanse is unavailable. The clause reduces the parachute payments to the maximum amount that does not trigger the 280G cliff — but only if the net-of-tax amount to the executive after the reduction is greater than the net-of-tax amount with no reduction (where the executive bears the 20% excise tax). The executive gets whichever outcome is actually better on an after-tax basis.

The two alternatives the modified-cutback is contrasted with:

- **Full gross-up** — the corporation grosses up the executive for the excise tax so that the executive is held economically harmless. **ISS flags gross-ups as a problematic pay practice** and the pre-IPO market has largely abandoned them.
- **Hard cutback** — mandatory reduction to the safe-harbor amount regardless of whether the cutback is actually better for the executive on an after-tax basis. Executive-unfriendly and uncommon.

The modified-economic-cutback is the modern pre-IPO market default — it protects the corporation from the deduction-loss issue in the common case and protects the executive from being worse off than a hard-cutback alternative in the uncommon case.

## A worked example — Alloygraph Systems, Inc. (Series C) hires a CFO

Alloygraph Systems, Inc. is a Series-C AI-infrastructure corporation. The board approves a CFO hire. The term sheet includes a severance architecture; the standalone severance agreement is executed on the start date alongside the offer letter and equity-grant documents.

**Severance architecture:**

- **Base severance** — 12 months of base salary payable in equal installments over the 12-month severance period.
- **Bonus severance** — 100% of target annual bonus, paid as a lump sum within the 60-day release-execution window following release effectiveness.
- **Benefits continuation** — 12 months of COBRA premium subsidy, structured as a monthly taxable cash payment equal to the COBRA premium to avoid ACA § 105(h) issues.
- **Equity acceleration** — on involuntary termination without cause not in connection with a CoC, 12 additional months of time-based vesting on all outstanding unvested equity. On a double-trigger CoC termination (involuntary termination without cause or good-reason resignation within 12 months after CoC), 100% acceleration of all unvested equity.
- **Triggers** — involuntary termination without cause or good-reason resignation. Cause narrowly defined — material breach of policy after notice-and-cure, wilful misconduct, felony conviction, material failure to perform duties after written notice. Good reason — reduction in base, reduction in target bonus opportunity, material diminution in duties / authority / title / reporting line, relocation of principal workplace by more than 35 miles, material breach by Alloygraph, each with 30-day CFO-notice and 30-day Alloygraph-cure, exercised within 90 days.
- **Release-of-claims condition** — severance commences on the first regular payroll date following the end of a 60-day release-execution-and-non-revocation window.
- **OWBPA** — if the CFO is age 40 or older at separation, the release provides for a 21-day consideration period and a 7-day revocation period, which fit comfortably inside the 60-day §409A window.
- **Speak Out Act carve-out** — the release expressly preserves the CFO's right to speak about sexual-harassment or sexual-assault matters, and the mutual non-disparagement provision is drafted around that preservation.
- **EFAA cross-reference** — the arbitration agreement signed at hire carves out EFAA-covered claims.
- **§ 409A compliance** — base and bonus severance structured as separation-pay-exception payments; §409A savings-clause included; specified-employee six-month-delay language included for post-IPO applicability.
- **§ 280G** — a modified-economic-cutback clause reducing parachute payments to 2.99× base-amount only if the net-of-tax outcome to the CFO is better after reduction. No gross-up.
- **Non-compete / non-solicit** — the CFO is based outside California. A 12-month post-separation customer-and-employee non-solicit survives separation. No post-separation non-compete.

**Cost sketch (pre-IPO modeling).** Assume CFO base of $425,000, target bonus of 50% of base ($212,500), equity grant with ~$9M fair value over four years. In an involuntary-termination-without-cause scenario in year two, the severance payout is approximately $637,500 cash ($425k base + $212.5k target bonus) plus 12 months of COBRA (~$30k) plus 12 additional months of time-based vesting on roughly 25% of the outstanding equity grant. The CoC-plus-termination scenario drives the Item 402(j) number materially higher once 100% equity acceleration lands.

## Summary

- Executive severance is a comp-committee risk-shifting instrument, not an HR hardship program. ICs typically receive 2–4 weeks per year of service capped at 12–16 weeks; execs typically receive 6–12 months of base plus target bonus plus benefits continuation plus equity acceleration — the risk premium that compensates execs for being personally exposed to board-and-investor-visible outcomes.
- The executive severance agreement has eight recurring provisions — triggers (involuntary without cause, good-reason resignation), payment, benefits, equity acceleration (cross-ref [./07-change-of-control-equity-policy.md](./07-change-of-control-equity-policy.md)), release-execution requirement, 280G modified-economic-cutback, 409A compliance, and surviving restrictive covenants (cross-ref [../mod-103-employment-law-and-contract-design/06-non-compete-landscape-and-alternatives.md](../mod-103-employment-law-and-contract-design/06-non-compete-landscape-and-alternatives.md)).
- IRC § 409A drives the payment-timing architecture: short-term deferral exception, separation-pay exception, specified-employee six-month-delay rule under IRC § 409A(a)(2)(B)(i) (post-IPO only), and the 60-day release-execution-and-non-revocation window that fixes the release-timing tax-year problem.
- The release-and-non-disparagement agreement includes a general release of claims with mandatory carve-outs (UI, workers' comp, vested benefits, indemnification, D&O, agency charges), mutual non-disparagement, and post-Speak-Out-Act and post-EFAA carve-outs for sexual-harassment and sexual-assault matters (Pub. L. No. 117-224 and Pub. L. No. 117-90).
- OWBPA — 29 U.S.C. § 626(f) — governs releases of ADEA claims by employees age 40+: 21-day consideration (45 for group), 7-day revocation, written counsel-advice notice, and group RIF disclosures under § 626(f)(1)(H) that apply even to small two-person programs.
- A tiered severance architecture (CEO/C-suite/VP/IC) adopted as formal comp-committee policy — ideally through an ERISA-covered Executive Severance Plan supplemented by individual amendments for the CEO — produces the cleaner Item 402(j) disclosure (deferred to [./09-sec-reg-sk-item-402-disclosure.md](./09-sec-reg-sk-item-402-disclosure.md)) and the more defensible governance narrative at IPO.
