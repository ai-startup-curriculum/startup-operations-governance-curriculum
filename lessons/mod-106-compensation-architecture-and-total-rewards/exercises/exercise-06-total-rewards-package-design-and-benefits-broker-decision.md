# Exercise 06 — Total rewards package design and benefits broker decision

> Estimated time: **~5 hours** · Related chapter: [06 — Total-rewards package design](../06-total-rewards-package-design.md)

## Problem statement

Briarbend Analytics, Inc. is a Delaware C-corp building a vertical-SaaS analytics platform for regional financial-services providers. The corporation closed a $38M Series-B nine months ago at a $190M post-money and sits at **135 employees**: 56 engineering, 10 product / design, 32 GTM, 18 G&A, 19 operations / support. The footprint is CA (24), NY (18), MA (12), WA (9), CO (6), IL (6), TX (14), remote-US-tier-2 long tail (46).

Current state of the total-rewards package:

- **Medical, dental, vision are placed through a small regional PEO** (TotalPro Services) picked up at the corporation's seed stage. The PEO's PPO and HMO offerings are competitive at a 20-person size but have become materially under-market at 135; employees report 2026 open-enrollment premium increases of 18% on the PPO and a tightening of the in-network specialist list that has caused three families to switch to a spouse's plan. The Head of People believes the corporation has outgrown the PEO.
- **401(k) runs through Guideline**, the standalone 401(k) administrator the Head of People onboarded at Series-A. There is a **4% safe-harbor non-elective contribution** (no match, no vesting — standard for a safe-harbor non-elective design); the plan does not offer Roth, does not offer a backdoor-Roth, and has no auto-enrollment.
- **Commuter, FSA, HSA** are placed through the PEO's bundle. Enrollment is low (fewer than 20% of eligible employees enrolled in the commuter benefit, fewer than 15% in FSA, zero HDHP uptake because the PEO's HSA-eligible HDHP is not offered).
- **Parental leave** is 8 weeks of fully-paid birth-parent leave and 4 weeks of fully-paid non-birth-parent leave. The policy was authored in 2023 when the corporation was 30 employees and was flagged by the first joint People / Legal review nine months ago as under-market for the stage and under-researched against state-specific paid-family-leave statutes (CA PFL, NY PFL, WA PFML, MA PFML, CO FAMLI, IL in 2026 — flag `<!-- needs-research -->` for current effective dates and interaction rules).
- **Stipends** — a $1,200 / year WFH stipend, a $500 / year L&D stipend, no wellness stipend. Adoption is high (90%+ on WFH; 60% on L&D).
- **Exec-perk overlay** — no distinct exec-perk program; execs receive the same stipends and benefits as ICs. The Head of People believes a first-pass executive health benefit (annual executive physical, enhanced disability coverage) is overdue given the two C-suite hires (CRO and CFO) completed in the last six months.
- **Two live stressors.** First, a competitive-hiring environment — two Senior Engineer offers were declined in the last quarter with "benefits package" cited as a contributing reason. Second, the 2026 open-enrollment deadline is 90 days out; the comp committee has asked for a broker / PEO decision in time for 2026 plans to be in place.

Your role: you are the **Head of People** tasked with authoring the ratifiable total-rewards upgrade package and the broker / PEO graduation decision. Produce the current-state benchmark, the medical / dental / vision placement decision (broker vs. self-insured vs. staying with the PEO), the 401(k) upgrade, the parental-leave rewrite, the stipend architecture, the exec-perk overlay, and the comp-committee presentation memo.

## Requirements

### Part A — Current-state benchmark

Produce a written benchmark of the current total-rewards package against the market cuts chapter 06 recommends. Cover:

1. **Medical / dental / vision** — benchmark the current PEO PPO and HMO plans against a Series-B peer-set cut. The right benchmarks are Mercer's National Survey of Employer-Sponsored Health Plans, Aon Benefits Survey, or the Carta / Pave benefits-benchmarking module. Flag `<!-- needs-research -->` for the specific percentile and the premium-share-by-coverage-tier numbers.
2. **401(k)** — benchmark the current 4% safe-harbor non-elective against the market. The right benchmarks are PSCA (Plan Sponsor Council of America) Annual Survey, Vanguard's How America Saves report, Fidelity's plan-sponsor benchmarking. Flag `<!-- needs-research -->` for the specific percentile.
3. **Parental leave** — benchmark the 8-week birth-parent / 4-week non-birth-parent policy against the market. Note the state-paid-family-leave statutes (CA PFL, NY PFL, WA PFML, MA PFML, CO FAMLI, IL 2026) that *augment* an employer policy, and the interaction rule (employer policy typically runs concurrent with state PFL, with top-up to maintain full pay if the state benefit is below 100% wage replacement). Flag `<!-- needs-research -->` for state-specific wage-replacement percentages and the current corporate-market-median parental-leave weeks.
4. **Stipends** — benchmark the $1,200 WFH / $500 L&D stipends against the market. Flag `<!-- needs-research -->` for the specific percentile.
5. **Exec-perk** — benchmark the current "none" against the Series-B exec-perk norm. Note the chapter-06 default (annual executive physical, enhanced disability, financial-planning advisory, in some cases spouse travel for executive on-sites). Flag `<!-- needs-research -->`.
6. **The two declined offers.** For each, diagnose which benefits-package line item was the specific gap cited by the candidate and map the gap to the Part A benchmark.

### Part B — Medical / dental / vision placement decision

Produce the placement decision. Cover:

1. **The three options.** Chapter 06 names three placements at the 100–200-employee stage — stay with the current PEO, graduate to a broker-placed fully-insured plan (the usual answer at 100+), or graduate to a broker-placed self-insured plan (typically only at 300+ or with high-utilizers that make self-insurance economic). State Briarbend's chosen option with rationale.
2. **The broker RFP.** If the decision is to graduate to a broker-placed plan, state the broker RFP process:
    - The three-to-five brokers to invite (major examples: Lockton, OneDigital, Marsh McLennan Agency, Newfront, HUB International, Woodruff Sawyer — `<!-- needs-research -->` for Series-B tech specialisation). State the selection criteria (Series-B tech specialisation, plan-placement history with comparable corporations, in-house ERISA counsel or external ERISA panel, in-house DEI benchmarking, in-house pharmacy-benefit expertise, flat-fee vs. commission compensation).
    - The scope of the RFP (medical, dental, vision; the PEO-benefits-replacement scope; the carrier set the broker will recommend including the specific carriers — Aetna, Cigna, Blue Cross Blue Shield, UnitedHealthcare, Kaiser for CA — the broker will source).
    - The timeline — RFP issued, responses due, finalist interviews, selection, contract, carrier placement, open-enrollment-ready date relative to the 90-day window.
3. **The PEO-to-broker migration playbook.** The specific steps — PEO contract termination notice, COBRA treatment for employees mid-year, data-portability of the HRIS functions the PEO currently performs (payroll, time-off tracking, basic HR tasks), replacement HRIS selection (chapter 06 and [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md) cover the PEO-vs-HRIS graduation — Rippling, Gusto, Justworks, Sequoia One, TriNet — cross-reference the mod-104 treatment).
4. **The specific-carrier-plan selection.** Once the broker is retained, the broker returns a carrier-and-plan recommendation. State the carrier-and-plan-selection criteria Briarbend will apply — network breadth in the five primary states (CA, NY, MA, WA, CO) and the remote-US-tier-2 long tail, in-network specialist availability, HSA-eligible HDHP inclusion (addressing the current zero HDHP uptake), mental-health-coverage parity (MHPAEA compliance), and total employee-and-dependent cost. Flag specific premium numbers with `<!-- needs-research -->`.
5. **The broker-vs-benefits-consultant note.** State the distinction between a benefits broker (commissions-funded, plan-placement focused) and a benefits consultant (fee-for-service, strategy-and-benchmarking focused) and Briarbend's chosen posture — typically a broker at Series-B, a consultant added at Series-C / pre-IPO. Cross-reference [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md).

### Part C — 401(k) upgrade

Produce the 401(k) upgrade proposal. Cover:

1. **The contribution-design decision.** The three defensible designs — a safe-harbor non-elective (current), a safe-harbor match (e.g., 100% match on the first 3% + 50% match on the next 2%), or a discretionary match on top of the safe-harbor non-elective. State Briarbend's choice with rationale. Flag `<!-- needs-research -->` for current-market match formulas.
2. **The vesting schedule.** State the vesting schedule — safe-harbor contributions must be 100% vested on contribution; a discretionary match can carry a cliff or graded vesting schedule (typically 2-year cliff or 3-year graded for retention effect). Cross-reference IRC § 401(k)(12) and § 411(a)(2) for the vesting rules.
3. **Roth and backdoor-Roth.** State the plan-design upgrade — adding a Roth 401(k) option (allowing after-tax contributions) and a backdoor-Roth option (allowing after-tax contributions above the elective-deferral limit, with in-plan conversion to Roth). Flag the SECURE Act 2.0 provisions affecting Roth catch-up contributions `<!-- needs-research -->`.
4. **Auto-enrollment.** State the auto-enrollment design — Briarbend should adopt auto-enrollment at a 6% default rate with automatic annual escalation (e.g., 1% per year up to 10%). SECURE Act 2.0 § 101 mandates auto-enrollment for plans established after 2022-12-29 at a starting rate of 3%–10% with annual escalation to at least 10%; flag `<!-- needs-research -->` for whether Briarbend's plan vintage subjects it to the mandate or whether the adoption is voluntary.
5. **Investment-committee governance.** State the ERISA fiduciary posture — the Head of People and Head of Finance (or the CFO) constitute an investment committee that reviews the plan's fund lineup, the recordkeeper's fee disclosure (ERISA § 408(b)(2)), and the participant fee disclosure (ERISA § 404(a)(5)) annually. Flag `<!-- needs-research -->` for current ERISA fee-disclosure guidance.
6. **The recordkeeper decision.** State whether Guideline continues (adequate at 100–500 employees) or whether a graduation to a larger recordkeeper is on the roadmap (typically at 500+ or at IPO). Flag `<!-- needs-research -->` for Series-B / Series-C recordkeeper options.

### Part D — Parental leave rewrite

Produce the parental-leave rewrite. Cover:

1. **The new policy structure.** The upgraded policy — propose 16 weeks of fully-paid parental leave for all new parents (birth, adoption, foster) with no distinction between birth-parent and non-birth-parent primary caregivers, plus any birth-parent-specific pregnancy / recovery leave (a separate 6-week medical leave for birth parents, paid). Chapter 06 notes this is the Series-B-and-above market default; flag specific weeks `<!-- needs-research -->`.
2. **The state-PFL interaction.** For each state in-footprint (CA PFL, NY PFL, WA PFML, MA PFML, CO FAMLI, IL in 2026), state the specific interaction rule — the employer policy runs concurrent with the state benefit, with the employer topping up to 100% wage replacement where the state benefit is below 100%. Flag `<!-- needs-research -->` for state-specific wage-replacement percentages, weekly caps, and duration limits. Cross-reference [mod-103](../../mod-103-employment-law-and-contract-design/) for the state-law variance.
3. **The eligibility and documentation rule.** State the eligibility rule — all employees employed ≥90 days are eligible, no FLSA-exempt-only or tenure-based restriction. Cross-reference [mod-104 chapter 06](../../mod-104-hiring-onboarding-and-hr-operations/06-first-90-day-onboarding-and-new-hire-document-pack.md) for the 90-day onboarding anchor.
4. **The leave-administration mechanics.** State the administrator — self-administered via the HRIS (low complexity) or outsourced to a third-party administrator like Guardian, Unum, or a PFL-specialist like Parental Leave Consultants (`<!-- needs-research -->`). State the decision with rationale.
5. **The return-from-leave support.** Chapter 06 notes the ramp-back policy (e.g., 50% schedule for the first two weeks post-leave at 100% pay), the lactation / nursing-room accommodation (PUMP Act compliance; cross-reference [mod-103](../../mod-103-employment-law-and-contract-design/)), and the manager-training on parental-leave transition. State Briarbend's version.
6. **The retroactive-application decision.** State whether the new policy applies retroactively to employees currently on leave or who have taken leave in the last 12 months. Chapter 06 notes retroactive application is common at a stage-transition upgrade and signals a serious policy upgrade.

### Part E — Stipend architecture

Produce the stipend architecture. Cover:

1. **The new stipend suite.** Propose the upgraded stipend suite — $2,000 / year WFH (up from $1,200), $1,500 / year L&D (up from $500), $500 / year wellness (new), and an optional $1,000 one-time home-office setup stipend for new hires. Flag `<!-- needs-research -->` for Series-B / Series-C market cuts.
2. **The LSA (lifestyle spending account) alternative.** State the trade-off between a stipend-per-category approach and a consolidated LSA that gives employees a dollar pool to allocate across categories. Chapter 06 notes the LSA approach is operationally simpler (one taxable-wage-reporting path, one administrator) but a stipend-per-category approach has clearer behavioural-signalling value (the wellness stipend signals "we value wellness," which a generic LSA does not).
3. **The tax treatment.** State the tax treatment of each stipend — the WFH stipend is a taxable wage unless administered under an accountable plan (IRC § 62(c), Treas. Reg. § 1.62-2) with receipts; the L&D stipend is taxable unless the training qualifies as working-condition fringe (IRC § 132(d)); the wellness stipend is taxable unless placed in a qualified wellness program (which carries HIPAA / ADA / GINA compliance requirements). Flag `<!-- needs-research -->` for current-cut guidance.
4. **The administration mechanics.** State the administrator — reimbursement via the HRIS expense module vs. a card-based administrator like Fringe, Compt, or Forma (`<!-- needs-research -->`). State the choice with rationale.

### Part F — Exec-perk overlay

Produce the exec-perk overlay. Cover:

1. **The exec-perk inventory.** Propose the exec-perk suite for the C-suite and VP tier — annual executive physical (chapter 06 notes this is the market default), enhanced disability insurance (individual disability policy supplementing the group plan), financial-planning advisory (3–5 hours / year with a fiduciary advisor), spouse travel for executive on-sites. Flag `<!-- needs-research -->` for Series-B exec-perk market cuts.
2. **The IRC § 61 and § 132 tax treatment.** State the tax treatment — exec-perk benefits are generally taxable wages under IRC § 61 unless they qualify as working-condition fringe (§ 132(d)), de minimis fringe (§ 132(e)), or a qualified employee benefit (§ 132(h)-(n)). The executive physical is typically structured as either a taxable wage (gross-up) or as a reimbursable medical expense under IRC § 105(h) with the non-discrimination rule in mind (the physical cannot be offered only to highly-compensated employees without the § 105(h) excise exposure — the market practice is either to gross up or to offer the physical to all employees at an enhanced tier).
3. **The disclosure implication.** Note the SEC Reg S-K Item 402(c)(2)(ix) "All Other Compensation" footnote implication at IPO — exec perks totaling more than $10,000 per year are disclosed in the Summary Compensation Table. Cross-reference [mod-105 chapter 09](../../mod-105-equity-compensation-policy-and-comp-committee/09-sec-reg-sk-item-402-disclosure.md).
4. **The CRO and CFO two-hire test case.** Dispositions the two recently-hired C-suite roles — do they receive the exec-perk suite retroactively, is it part of their offer-letter addendum, and is the comp-committee resolution needed?

### Part G — Comp-committee presentation memo

Produce the **1-page memo** attaching the total-rewards upgrade. Cover:

- The current-state benchmark headline (Part A) and the specific lines where Briarbend is under-market.
- The five ratification asks: the broker / PEO graduation (Part B), the 401(k) upgrade (Part C), the parental-leave rewrite (Part D), the stipend architecture (Part E), the exec-perk overlay (Part F).
- The 2026 open-enrollment deadline and the specific timeline for the broker RFP and plan placement.
- The budget impact — the dollar delta per employee per year under the upgrade, the total annual incremental cost, and the retention-value expected return.
- The `<!-- needs-research -->` queue grouped by decision (benchmark percentiles, state-PFL interaction, SECURE Act 2.0 provisions, ERISA fee-disclosure guidance, exec-perk tax-treatment detail, broker shortlist specialisation).
- The forward-references to [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md) (PEO-vs-HRIS graduation), [mod-103](../../mod-103-employment-law-and-contract-design/) (state-PFL variance and NLRA / PUMP Act), and [mod-105 chapter 09](../../mod-105-equity-compensation-policy-and-comp-committee/09-sec-reg-sk-item-402-disclosure.md) (the exec-perk disclosure implication at IPO).

## Starter guidance

- Chapter 06 is the primary reference. Re-read the "health / dental / vision," "401(k)," "parental leave," "stipends," and "exec-perk" sections before authoring.
- The broker-vs-PEO decision is the highest-stakes line in Part B. Do not re-author the PEO-vs-HRIS graduation here — defer to [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md).
- The parental-leave rewrite must interact precisely with the state-PFL regimes. The specific wage-replacement percentages, weekly caps, and duration limits are state-specific statutory numbers — flag with `<!-- needs-research -->`; do not invent them.
- **Do not manufacture benchmark numbers or statutory cuts.** Every percentile, every match formula, every state-PFL wage-replacement number, every SECURE Act 2.0 provision, every ERISA guidance citation must be flagged `<!-- needs-research -->`.
- The exec-perk overlay has a non-discrimination landmine — the IRC § 105(h) rule makes an executive-only physical taxable unless carefully structured. Reference the specific IRC sections; do not re-derive the tax treatment.
- The 2026 open-enrollment deadline is the hard forcing function. Part B's broker RFP and plan placement must fit inside the 90-day window.

## Deliverables

- `current-state-benchmark.md` — Part A.
- `medical-placement-decision.md` — Part B.
- `401k-upgrade-proposal.md` — Part C.
- `parental-leave-rewrite.md` — Part D.
- `stipend-architecture.md` — Part E.
- `exec-perk-overlay.md` — Part F.
- `comp-committee-memo.md` — Part G (1 page).

## Acceptance criteria

The package is acceptable if:

1. Part A benchmarks every current total-rewards line item against the market cuts chapter 06 recommends, flags every percentile claim `<!-- needs-research -->`, and diagnoses the two declined-offer benefits-package gaps.
2. Part B picks one of the three placements with rationale, specifies the broker RFP process (shortlist, scope, selection criteria, timeline), states the PEO-to-broker migration playbook with cross-reference to [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md), states the carrier-and-plan selection criteria, and notes the broker-vs-benefits-consultant distinction.
3. Part C states the contribution-design decision (safe-harbor non-elective, safe-harbor match, or discretionary match on top), the vesting schedule with IRC citation, the Roth / backdoor-Roth / SECURE Act 2.0 cut, the auto-enrollment design, the investment-committee governance with ERISA citation, and the recordkeeper continuation decision.
4. Part D proposes the new parental-leave structure (specific weeks for primary caregiver, pregnancy / recovery leave for birth parent), states the state-PFL interaction rule per state, states the eligibility and documentation rule, states the leave-administration mechanics, states the return-from-leave support with PUMP Act cross-reference, and states the retroactive-application decision.
5. Part E states the new stipend suite with amounts, discusses the LSA alternative, states the tax treatment of each stipend with IRC citation, and states the administration mechanics.
6. Part F states the exec-perk inventory, the IRC § 61 / § 132 tax treatment with the § 105(h) non-discrimination note, the SEC Reg S-K Item 402(c)(2)(ix) disclosure implication at IPO, and dispositions the two recently-hired C-suite roles.
7. The comp-committee memo is **one page**, names the current-state benchmark headline, the five ratification asks, the 2026 open-enrollment timeline, the budget impact, and the `<!-- needs-research -->` queue.
8. Every benchmark percentile, every match formula, every state-PFL wage-replacement number, every SECURE Act 2.0 provision, every exec-perk market-cut number, every broker shortlist specialisation claim is flagged `<!-- needs-research -->`. Every tax-treatment claim carries the specific IRC section.
9. Cross-references to [mod-103](../../mod-103-employment-law-and-contract-design/), [mod-104 chapter 06](../../mod-104-hiring-onboarding-and-hr-operations/06-first-90-day-onboarding-and-new-hire-document-pack.md), [mod-104 chapter 07](../../mod-104-hiring-onboarding-and-hr-operations/07-hris-peo-payroll-stack.md), and [mod-105 chapter 09](../../mod-105-equity-compensation-policy-and-comp-committee/09-sec-reg-sk-item-402-disclosure.md) are present.
10. Nothing left as `[TBD]` or `[FILL IN]`.
