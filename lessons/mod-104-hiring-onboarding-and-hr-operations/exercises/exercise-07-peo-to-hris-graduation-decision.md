# Exercise 07 — PEO-to-HRIS graduation decision

> Estimated time: **~6 hours** · Related chapter: [07 — The HRIS / PEO / payroll stack and the graduation path](../07-hris-peo-payroll-stack.md)

## Problem statement

Sierra Vector is a Delaware C-corp that just closed a $60M Series-B. Sierra has 92 employees today (target 210 in 18 months), on Justworks (PEO) since seed. Employees are in 11 states: California, Oregon, Washington, Colorado, Texas, Illinois, New York, Massachusetts, Georgia, Florida, and North Carolina. Sierra has just hired a Payroll Operations lead (starting in 4 weeks) and is finalising the hire of a Head of People (starting in 2 weeks).

The Series-B has changed the operating economics:

- **PEO cost.** Justworks's PEO fee on Sierra's current payroll is materially larger in absolute terms than at seed and grows as the corporation grows. The CFO's initial back-of-envelope shows the PEO fee crossing an internal threshold within 6 months.
- **Benefits design.** The Head of People coming in has explicit customer-referenceable experience with a specific health carrier network and a specific 401(k) safe-harbour design that Justworks's plan on offer does not support. The board's compensation committee (formed at Series-B) is going to ask about total-rewards design in the next 90 days.
- **International.** Sierra plans its first international hire — a research engineer in London — within 6 months, and 2–4 additional international hires in the following 6 months.
- **Diligence.** Series-C is a plausible 18–24 month horizon. Diligence is easier as the direct employer of record.
- **SOC 2.** Sierra is pursuing SOC 2 Type II attestation to close two enterprise deals; the HRIS choice is part of the SOC 2 vendor-management boundary and the corporation's own controls over HR data are in scope.

You are the incoming Head of People. Produce (a) the graduation decision memo, (b) the HRIS / broker / 401(k) vendor selection, (c) the full 3–6 month migration project plan, (d) the multi-state payroll-registration plan, and (e) the SOC 2 boundary and the international-hire handoff analysis.

## Requirements

### Part A — Graduation decision memo

Produce a decision memo for the CEO and board covering:

1. **The graduation-trigger analysis** — walk each of the chapter's triggers (cost, benefits design, operating maturity, feature gap, diligence) and determine whether it has fired at Sierra today.
2. **The recommendation** — a specific decision (graduate now / graduate in 6 months / stay on PEO through Series-C). Justify.
3. **The cost model** — a projected 12-month and 24-month total-cost-of-ownership comparison for two scenarios:
   - Scenario A: Stay on Justworks PEO.
   - Scenario B: Migrate to HRIS + broker + 401(k) stack.
   Include: PEO fee (% of payroll) vs. HRIS subscription + payroll ops FTE + benefits-broker fees + 401(k) provider fees + workers'-comp broker fees. Do not manufacture Justworks or Rippling pricing — flag it as `<!-- needs-research -->` and show the model with placeholder ranges. What matters is the model structure.
4. **The risk-and-mitigation** — the specific risks of migration (missed state registrations, benefits-transition gaps, W-2 reconciliation errors, project overrun) with a specific mitigation for each.
5. **The alternative** — the "stay on PEO but negotiate" alternative (renegotiate the fee; move to Justworks's non-PEO payroll product without a full migration). Analyse and reject (or accept) with reasons.

### Part B — HRIS / broker / 401(k) vendor selection

Produce a written vendor-selection package covering:

1. **HRIS selection** — one specific HRIS chosen from Rippling, Gusto, Deel HR, BambooHR, or Namely. Justify against Sierra's specific requirements (multi-state US payroll, international expansion in 6 months, IT provisioning integration, benefits administration, SOC 2 readiness). Address the international dimension explicitly — a US-only HRIS paired with a per-country international provider vs. an international-first HRIS (Rippling International, Deel).
2. **Benefits broker selection** — one broker chosen from Newfront, Sequoia Consulting Group, Woodruff Sawyer, Aon, One Digital, Marsh & McLennan Agency, or an HRIS-native brokerage. Justify against Sierra's specific requirements (book of business in the 11 states, startup-native service model, HRIS integration depth, executive-benefits capability for the growing exec team). Include the specific interview criteria and the reference-check plan for the shortlist of 2–3 brokers.
3. **401(k) provider selection** — one provider chosen from Guideline, Human Interest, ForUsAll, Betterment for Business, Fidelity, Vanguard, or Empower. Justify against plan-design requirements (safe-harbour vs. non-safe-harbour, match structure, vesting, eligibility, HRIS integration).
4. **Workers'-comp posture** — whether workers'-comp is placed through the same broker as health, a separate P&C broker, or through the HRIS-native workers'-comp product (Rippling, Gusto, and Deel each offer variants). Justify.
5. **Rejected options** — for each vendor category, the specific reason each rejected option was not chosen. Do not write "not as good"; write the specific constraint.
6. **Rippling-specific note** — if Rippling is your HRIS choice, note the specific value of the integrated IT (Okta-adjacent identity, MDM integration, SCIM into every SaaS system) and estimate the tools it replaces. Consider explicitly whether Sierra's current identity / MDM stack is displaced. If Rippling is *not* your HRIS choice, address the integration story between your chosen HRIS and Sierra's existing identity / MDM.

### Part C — Migration project plan

Produce a full 3–6 month migration project plan. Cover:

1. **Month 0 — decision and vendor selection.** Board / CEO decision. Vendor contracts executed. Payroll Ops lead onboarded (already scheduled). Head of People onboarded (already scheduled).
2. **Months 1–3 — state-tax registrations.** Registrations in each of Sierra's 11 states for state income-tax withholding, state unemployment insurance, and workers'-comp. Each registration has a target start date, an expected completion window (2–8 weeks per state), an owner, and a blocking-status flag for payroll cutover. Include the specific state agencies for each of the 11 states (California EDD, New York DTF, Texas TWC / Comptroller, etc.). Some states can be registered in parallel; some have sequencing dependencies.
3. **Months 1–3 — benefits plan design.** Broker quotes health / dental / vision / life / disability with Sierra's employee census. Plan-design decisions (HDHP + HSA vs. PPO tiers, employer contribution %, family-plan strategy, dependent-care FSA vs. HSA). Executive-benefits design if applicable.
4. **Months 1–3 — 401(k) plan setup.** Plan document. Safe-harbour vs. non-safe-harbour decision. Match design. Vesting. Eligibility. Entry dates.
5. **Months 2–4 — HRIS setup and data migration.** Employee data migration from Justworks. Historical payroll data reconciliation for W-2 continuity. Every employee's data validated by the employee (self-service review) and by the Payroll Ops lead.
6. **Months 3–4 — open enrollment window.** Employees enroll in the new benefits plans. 2–3 week enrollment window with clear communication, an employee-education session (or two), and a broker-led Q&A. Post-enrollment reconciliation with the broker.
7. **Month 4 — parallel run.** One or two payroll cycles run in parallel between Justworks and the HRIS to validate calculations before cutover.
8. **Month 4–5 — cutover.** Justworks's last payroll runs. The HRIS's first payroll runs. Employees experience continuity of benefits and pay.
9. **Months 5–6 — Justworks exit and W-2 reconciliation.** Justworks issues W-2s for the portion of the year under its EIN; Sierra issues W-2s for the portion under Sierra's EIN. Employee communication about receiving two W-2s.
10. **Project governance** — the specific project-management posture (dedicated project lead, written project plan with owners and deadlines, external counsel review on employment-law questions, weekly executive updates until cutover is confirmed successful).

### Part D — Multi-state payroll-registration plan

Produce a per-state registration plan for each of the 11 states. For each state, cover:

1. The specific state tax authority (name of the department, URL).
2. The specific registrations required — state income-tax withholding, state unemployment insurance, workers'-comp, any state-specific paid-leave programme (California CFRA / PDL / PSL, Oregon Paid Leave, Washington PFML, Colorado FAMLI, Massachusetts PFML, New York PFL, and any others in Sierra's footprint).
3. The specific documents / information required to register (EIN, formation documents, officer / registered-agent info).
4. The expected timeline (2–8 weeks; some states are faster).
5. The specific person owning that state's registration (Payroll Ops lead by default; external counsel or a payroll-consultancy overlay if needed).
6. The blocking status — which registrations are dependency-blocking for payroll cutover and which can be completed post-cutover.

Flag as `<!-- needs-research -->` any state where the specific agency, URL, or registration requirement cannot be confidently cited.

### Part E — SOC 2 boundary and international-hire handoff

1. **SOC 2 audit boundary** — the corporation's SOC 2 Type II audit boundary as it relates to the HRIS. Cover:
   - Which employee-data controls are in-scope (SSO, MFA, access review, data-classification handling, terminated-employee de-provisioning).
   - The HRIS's own SOC 2 report as a vendor-management artifact.
   - The role of the corporation's benefits broker and 401(k) provider in vendor-management scoping.
2. **International-hire handoff to mod-113** — the specific operating questions the London research-engineer hire raises, cleanly split between:
   - Questions this module (mod-104) answers — the HRIS's international-payroll / EOR capability, the HRIS's I-9-equivalent workflow for the UK (right-to-work check), the HRIS's benefits-administration scope for UK employees.
   - Questions [mod-113](../../mod-113-international-expansion-and-global-workforce/) answers — per-country employment law and worker-classification, EOR vs. direct-hire, UK-specific benefits requirements, cross-border payroll tax, work-authorisation for the UK-based hire.
   Do not answer mod-113's questions; identify them and defer. If your HRIS choice (Part B) does not cover the UK well, name the fallback (a per-country provider — Deel EOR, Remote, Papaya Global — for the London hire specifically).

## Starter guidance

- Chapter 07 is the primary reference. The bundled-vs-unbundled framing, the three-stage graduation (PEO → HRIS → HCM), the migration checklist, and the multi-state payroll complexity are all covered.
- The chapter's worked example (Series-B PEO-to-HRIS graduation at 80 employees on Justworks) is a direct analogue. Sierra is slightly larger (92) and multi-state (11 vs. 8) with a nearer-term international hire.
- Do not manufacture PEO or HRIS pricing. Where you cite a per-employee-per-month fee or a percentage-of-payroll rate, flag it `<!-- needs-research -->` and show the model with placeholder ranges.
- The state-tax-registration plan (Part D) is the single most operationally consequential piece of the migration. Each state has its own agency portal and its own timeline; underestimating registration lead time is a common cause of payroll-cutover slippage.
- The migration is not casual. A defensible plan has a dedicated project lead, weekly executive updates, external counsel review on employment-law questions, and pre-defined criteria for "cutover successful."
- The international hire is a mod-113 problem in substance; this exercise is where the mod-104 / mod-113 handoff is authored. Identify the questions; do not answer them.
- The SOC 2 boundary analysis is deliberately narrow — the corporation's compliance and security team owns the deeper analysis. Identify the intersection points.
- The "stay on PEO but negotiate" alternative is worth taking seriously. Some corporations delay migration another 6–12 months while renegotiating the PEO fee; some corporations move to the PEO vendor's non-PEO payroll product (e.g., Justworks Payroll without PEO). Analyse and either accept or reject.

## Deliverables

- `graduation-decision-memo.md` — Part A.
- `hris-broker-401k-vendor-selection.md` — Part B.
- `migration-project-plan.md` (or `.xlsx`) — Part C.
- `multi-state-payroll-registration-plan.md` (or `.xlsx` / `.csv`) — Part D.
- `soc2-boundary-and-international-handoff.md` — Part E.
- `cost-model.xlsx` (or `.md` if you prefer a written model) — the 12-month and 24-month TCO comparison from Part A.

## Acceptance criteria

The package is acceptable if:

1. The decision memo (Part A) explicitly walks each of the chapter's five triggers and lands on a specific recommendation.
2. The cost model has line items for HRIS subscription, payroll ops FTE, benefits-broker fees, 401(k) fees, and workers'-comp broker fees (or the equivalent PEO fee). Every price is either cited or flagged as `<!-- needs-research -->`.
3. The vendor selection (Part B) picks one HRIS, one broker, one 401(k) provider, and one workers'-comp posture — with rejected options listed and rejected for specific reasons.
4. The vendor selection engages with the international dimension (US-only HRIS + per-country provider vs. international-first HRIS).
5. The migration project plan (Part C) covers all 9–10 phases of the chapter's checklist with target dates, owners, and definitions of "done."
6. The parallel-run phase is included and comes before cutover.
7. The state-registration plan (Part D) has an entry for each of the 11 states with agency, registrations required, timeline, and owner.
8. The state-specific paid-leave programmes are identified for each applicable state (California CFRA / PDL / PSL, Oregon Paid Leave, Washington PFML, Colorado FAMLI, Massachusetts PFML, New York PFL, and any others).
9. The SOC 2 boundary analysis identifies the in-scope employee-data controls and treats the HRIS's SOC 2 report as a vendor-management artifact.
10. The international-hire handoff clearly separates mod-104 questions from mod-113 questions and does not attempt to answer mod-113's questions.
11. The "stay on PEO but negotiate" alternative is analysed and either accepted or rejected with reasons.
12. Every market price / vendor claim is either cited to chapter 07 or flagged with `<!-- needs-research -->`.
