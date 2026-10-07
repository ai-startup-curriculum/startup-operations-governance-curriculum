# Exercise 01 — EOR vs. PEO vs. direct-entity decision drill

> Estimated time: **~8 hours** · Related chapter: [01 — EOR vs. PEO vs. direct-entity decision framework](../01-eor-vs-peo-vs-direct-entity-decision-framework.md)

## Problem statement

Fathom Compute is a US Delaware C-corp 14 months past a $42M Series B. The company sells an AI-infrastructure product (model-serving + fine-tuning tooling) into mid-market enterprise. US headcount sits at 72 FTE. The incoming COO (seven weeks in-seat, inherited from the departed co-founder who had been nominally running operations) has an inbox full of international-hire requests that the previous regime handled ad-hoc through a single EOR platform the finance team never fully evaluated.

Five hire scenarios are open simultaneously. Each is a different country, a different trajectory, and a different combination of regulatory, IP, and operational pressure. The CFO has asked for a per-scenario door decision — EOR, direct entity, or "do not hire this person in this configuration" — with a one-page decision memo per scenario and a consolidated 12-month plan the executive team can sign off on at next week's business review.

The five scenarios:

- **Scenario A — Toronto.** The CTO has routed two senior ML engineers from a prior employer. Both are Canadian citizens, Ontario-resident. The CTO wants to open a Toronto satellite "within a quarter" and has indicated to the two candidates that they should expect "4–6 more roles" to join them inside 12 months. The CTO is unaware of SR&ED; the Head of Finance has heard of it but has never run a claim.
- **Scenario B — London.** The VP Sales has an enterprise-sales lead based in London — closed €450k ARR at her last employer in nine months of enterprise selling in the UK and EU. She is a UK national, UK-resident, and wants to be hired as a contractor through her existing personal-service company Ltd (which she already uses to invoice two prior employers). She has indicated she "does not care" how she is engaged as long as the compensation structure works for her.
- **Scenario C — Berlin.** A former university colleague of the Chief Scientist, a tenured ML researcher, is willing to leave academia and join Fathom. He is a German national, Berlin-resident. The Chief Scientist expects the Berlin presence to grow to 6–8 researchers in 18 months. The researcher's work will primarily be invention-generating; his first project would be an in-house pretraining optimisation that the Chief Scientist expects to drive a published paper and potentially a patent filing.
- **Scenario D — Bengaluru.** The VP Engineering wants to open a six-person offshore engineering team — four senior engineers and two staff-level — reporting to a tech lead in San Francisco. The team's work is production infrastructure and data pipelines; no customer-facing authority. The Head of Finance has heard of STPI / SEZ structuring but has not evaluated it.
- **Scenario E — Lisbon.** A single senior engineer, Portuguese national resident in Lisbon, referred by an existing US engineer. No near-term plan for additional Portugal hires. The engineer has asked about the Portuguese NHR (Non-Habitual Resident) tax regime; the Head of Finance has heard that it was narrowed in 2024 but has not confirmed the current state of the successor regime.

Alongside the five scenarios, two cross-cutting issues:

- The existing EOR platform (contracted via Deel on a per-employee monthly fee basis) was engaged in haste 18 months ago when the company's first UK contractor (now a UK employee under Deel) was hired. The platform agreement has not been reviewed by legal; no one has looked at the IP-assignment language; the equity-plan interface has not been confirmed. The platform is used today for four employees (UK: 2, Netherlands: 1, Spain: 1).
- The CEO has started referring to the company as "international from day one" in investor conversations and would like the executive team to adopt a global-hiring posture that matches that narrative. The COO's judgement is that this should not mean "replace every US hire with an international hire" — rather, that the group should have a defensible, replicable framework for routing every international-candidate scenario to the right door.

Author the per-scenario decision memo (five of them), the EOR platform audit (one artefact), the consolidated 12-month plan, and the Series-B diligence-ready country decision register. Each decision must be defensible on the chapter-01 four-question framework; the fallback positions must be named explicitly; the EOR / direct-entity cost comparison must be run at the operator level.

## Requirements

### Part A — Per-scenario decision memo (Scenarios A–E)

For each of the five scenarios, author a one-page decision memo. Each memo must address:

1. **The four framework questions from chapter 01.**
   - **Headcount trajectory.** 12-month and 24-month expected headcount in-country; evidence basis (CTO / VP Sales / Chief Scientist stated intent; pipeline analysis; strategic plan). Flag where the stated trajectory is thin.
   - **Country regulatory regime.** The specific country tilts the chapter frames — Germany AÜG and Betriebsrat trigger, France CDI/CDD and portage, UK IR35, Canada provincial variance, India director-residency, Singapore nominee-director, Israel § 102 pre-grant-filing — named explicitly for each scenario and either in-scope or out-of-scope.
   - **IP / tax / regulatory posture.** The chapter's three triggers — IP ownership (worker's role in invention generation), local R&D-tax-credit generation (UK, Canadian SR&ED, French CIR, Irish R&D credit), local customer contracting (not applicable in these scenarios), regulated activity (not applicable) — applied to each scenario.
   - **Exit cost.** Weeks-to-months (EOR unwind) vs. months-to-years (direct-entity liquidation). Scenario-specific framing — e.g., a direct Indian Pvt Ltd is a multi-year commitment, so the headcount trajectory must justify the irreversibility.
2. **Door decision.** EOR, direct entity, or "do not hire in this configuration." No "it depends." If direct-entity is chosen, state the entity form; if EOR is chosen, state which platform (reusing the current Deel platform or evaluating alternatives); if "do not hire," explain the alternative structure (US-parent direct employment with relocation, convert to full-time employee on a different jurisdiction, defer the hire).
3. **Rationale.** Three to five sentences tying the decision to the four questions.
4. **Specific actions.** The next 2–4 operational steps per scenario — e.g., for Scenario A, the SR&ED programme engagement with a Canadian accountant; for Scenario B, the IR35 status determination before any contract is drafted; for Scenario C, the German counsel engagement for GmbH formation; for Scenario D, the Pvt Ltd formation with STPI evaluation; for Scenario E, the Portuguese NHR / IFICI confirmation with Portuguese counsel.
5. **Flag the risks you are accepting.** Each decision has a residual risk — EOR carries the IP-chain-of-custody risk, direct-entity carries the exit-cost risk, "do not hire" carries the hiring-loss risk. Name them explicitly.

For Scenario B, the IR35 analysis must be specific — the CEST tool, the HMRC off-payroll working rules, the "inside IR35" / "outside IR35" determination with reasoning, and the employer / client PAYE / NIC withholding exposure if the contractor is inside IR35 for a medium-sized or large client under Chapter 10, Part 2, ITEPA 2003 (as amended).

For Scenario E, the Portuguese NHR analysis must flag the regime's narrowing since 2024 and the successor IFICI / RNH 2.0 regime with explicit `<!-- needs-research: ... -->` where the current state is not grounded in the chapter or the problem statement.

### Part B — EOR / direct-entity cost comparison (Scenario C and Scenario D)

For the two scenarios with the strongest direct-entity case (C and D), produce an EOR-vs-direct-entity cost comparison at operating-year-one and operating-year-two.

For each scenario, the comparison must cover:

1. **EOR cost side.** Base salary + employer-side statutory contributions (country-specific, per chapter 06; e.g., Germany ~20%, India ~12% EPF + 15-days-per-year gratuity accrual) + EOR platform fee at a specified per-employee-per-month rate (grounded in the chapter 01 range, or `<!-- needs-research: ... -->` if a specific current rate is used) + any one-time setup / platform-onboarding fee.
2. **Direct-entity cost side.** Base salary + employer-side statutory contributions + local formation cost (notarial deed where applicable, local counsel fees, Companies House / commercial-register fees — defer specific fees to `<!-- needs-research: ... -->`) + ongoing local accountant / payroll provider fees + local counsel retainer + local statutory audit (where triggered by size) + any transfer-pricing documentation lift.
3. **Timing.** Year-one direct-entity costs are inflated by the formation lift; year-two costs smooth. The EOR cost is level per-year.
4. **Non-cost factors.** R&D-credit value (Scenario A SR&ED cash recovery; Scenario D STPI structuring; Scenario C CIR not applicable since Germany does not have a comparable regime), IP-chain cleanliness, exit-cost asymmetry.

Produce a numeric table with scenarios A/C/D at headcount levels 1 / 3 / 6 / 10 showing EOR-cost and direct-entity-cost per year. Numeric figures tied to the problem statement (salary ranges, country-average statutory loadings per chapter 06) can be named; any specific fee or platform-pricing number not grounded in the chapter is flagged with `<!-- needs-research: ... -->`.

The comparison must reach a break-even headcount for each scenario and explain how that break-even informs the Part A door decision.

### Part C — EOR platform audit

The existing Deel engagement needs a legal / operational audit. Author the audit memo.

1. **Contract review scope.** Named provisions to confirm in the Deel client-services agreement — IP-assignment language (worker → EOR → client), confidentiality, non-solicit / non-compete pass-through, equity-plan handling (whether Deel supports grants to EOR-employed workers on the US parent's stock plan), executive / officer handling (if any Deel-employed worker is in a role where they could be deemed an officer under the client's internal authority matrix), termination and transition rights.
2. **Country-coverage review.** Deel's operating-licence approach per country for the current four EOR workers (UK, Netherlands, Spain, Spain — reconfirm). Address the chapter 01 concerns: UK IR35 posture, Dutch employment-contract compliance, Spanish ETT regulated-staffing rules.
3. **Operational review.** HRIS integration status, payroll-cadence confirmation, benefits-package equivalence to the Fathom US baseline, security review of Deel's handling of worker PII, incident-history inventory (if any).
4. **Alternative-platform benchmark.** A side-by-side evaluation of Deel against two to three alternative EOR platforms named in chapter 01 (Remote, Oyster, Rippling EOR, Papaya Global, Velocity Global, Multiplier, G-P). Score on country coverage for Fathom's targeted jurisdictions, IP-assignment language, equity-plan handling, HRIS integration, pricing (defer specific-pricing to `<!-- needs-research: ... -->`), customer-service reputation (based on chapter 01's named vendor profiles, not invented facts).
5. **Decision.** Continue with Deel, migrate to an alternative, or multi-platform (one platform per region). Named rationale.
6. **Migration plan if migration is chosen.** The sequence of events — new platform contracted, new local employment contracts drafted and offered to current EOR workers, worker transfer-and-consent process, old platform termination, residual tax / payroll close-out.

### Part D — Consolidated 12-month plan

Produce the consolidated 12-month country-and-structure plan the COO presents at the next executive business review.

1. **Country-sequencing timeline.** A month-indexed Gantt-style sketch of the country rollouts — Scenario A Toronto / direct entity by month 6; Scenario B London / EOR immediately; Scenario C Berlin / GmbH planned by month 9 with EOR bridge months 1–9; Scenario D Bengaluru / Pvt Ltd by month 4; Scenario E Lisbon / EOR immediately with annual review.
2. **Dependencies.** The specialist-advisor engagements that precede each direct-entity formation — Canadian local counsel + accountant for Scenario A; German local counsel + notary + accountant + works-council planning for Scenario C; Indian local counsel + CA for Scenario D. Named at the operator-review level, not at the specialist-engagement-letter level.
3. **Budget envelope.** Formation costs, year-one operating costs for direct entities, EOR platform spend. Numeric figures per chapter and problem-statement where grounded; `<!-- needs-research: ... -->` elsewhere.
4. **Milestones.** First direct hire per scenario, R&D-credit programme stand-up (Scenario A SR&ED, Scenario D STPI if applicable), executed intercompany services agreement per direct entity (deferring the mechanics to [chapter 03](../03-intercompany-and-transfer-pricing-structure.md)).
5. **Cross-functional ownership.** Who owns each workstream — COO as overall sponsor; GC for all legal matters; CFO for tax structuring and local accountant engagements; Head of People for HRIS and employment-contract execution; CTO / VP Sales / Chief Scientist as scenario sponsors.
6. **Executive-review decision asks.** The two or three decisions the COO is explicitly asking the executive team to ratify — e.g., commit the capex for direct-entity formation in Scenario C, approve the Deel-vs-alternative EOR decision, approve the hire of a dedicated People Ops / Global Mobility hire if one is required by headcount.

### Part E — Country decision register (diligence artefact)

Author the Series-B / Series-C diligence-ready **country decision register**. This is the single artefact the diligence team sees. One row per country in which Fathom has any worker.

Columns:

- **Country / jurisdiction.**
- **Current headcount** (direct-employed + EOR-employed broken out).
- **Entity form** (direct-entity type and formation date, or EOR platform name).
- **Lawful-work-structure confirmation** (local-counsel-review date; IR35 determination date for UK contractors; Deel client-services-agreement review date for EOR workers).
- **Immigration posture** (any sponsored foreign nationals — not expected to be yes at this stage, but the field is here for completeness; cross-reference to [chapter 04](../04-us-immigration-programme.md)).
- **R&D-credit programme status** (not applicable / planned / in-flight / claiming).
- **Permanent-establishment analysis status** (US-parent-only / country-sub established / PE-risk flagged for tax-advisor review).
- **12-month-plan trajectory** (hold / grow / wind down).
- **Specialist-advisor contact** (local counsel / accountant / global-mobility if any).
- **Last review date.**

Populate with all countries currently touched (US baseline; UK, Netherlands, Spain for current EOR workers; new countries per the five scenarios).

The register must be structured so that a Series-C diligence lead can open it and understand the Fathom international footprint in five minutes without further explanation.

## Starter guidance

- Chapter 01 is the primary reference. The four-question framework in chapter 01's "The decision framework" section is the operating lens; every per-scenario memo is a worked application of that framework.
- Chapter 02 ([02 — First international entity setup](../02-first-international-entity-setup.md)) carries the entity-form and formation-timeline material referenced in direct-entity decisions.
- Chapter 03 is referenced for the intercompany-services agreement that follows direct-entity formation; the mechanics are not re-authored here.
- Chapter 06 is referenced for country-specific statutory-contribution rates; the Part B cost comparison uses chapter 06's rates (or `<!-- needs-research: ... -->` where chapter 06 flags them).
- Chapter 08 is cross-referenced where exit-cost analysis is in play.
- No real-company names should be invented as "the firm we retained." Chapter 01 and chapter 09 name specialist firms as examples of advisor-type presence; the exercise narrative names the *type* of advisor (Canadian local counsel; German notary; Indian CA) but not a specific name as the retained advisor.
- Any specific fee, platform-price, benchmark, or threshold figure not grounded in the chapters or problem statement is flagged with `<!-- needs-research: ... -->`. Do not invent dollar amounts.
- The IR35 analysis in Scenario B is specific; the practitioner-canon default for an enterprise-sales role is "inside IR35" unless the engagement has demonstrable substitution rights, no mutuality of obligation, no personal-service test — which an enterprise-sales role typically does not.
- The Scenario C German analysis must address the AÜG limit, the Betriebsrat trigger (6+ permanent employees), the GmbH formation mechanics ([chapter 02](../02-first-international-entity-setup.md)), and the ArbnErfG employee-invention regime ([chapter 06](../06-international-benefits-and-equity-comp.md)) since the hire is invention-generating.
- The Scenario D Indian analysis must address the two-director requirement (one Indian-resident) and the direct-entity-day-one case given the headcount.
- Flag the counsel sign-off step throughout. No operator-level decision in this exercise is a legal opinion.

## Deliverables

- `scenario-a-toronto-decision-memo.md` — Part A, Scenario A.
- `scenario-b-london-decision-memo.md` — Part A, Scenario B (with IR35 analysis).
- `scenario-c-berlin-decision-memo.md` — Part A, Scenario C.
- `scenario-d-bengaluru-decision-memo.md` — Part A, Scenario D.
- `scenario-e-lisbon-decision-memo.md` — Part A, Scenario E.
- `cost-comparison-c-d.md` — Part B (cost comparison for Scenarios C and D at headcount levels 1 / 3 / 6 / 10).
- `eor-platform-audit.md` — Part C.
- `twelve-month-plan.md` — Part D.
- `country-decision-register.md` — Part E.

## Acceptance criteria

The package is acceptable if:

1. Each per-scenario decision memo (Part A) answers the four framework questions explicitly — headcount trajectory with evidence basis, country regulatory regime with the specific chapter-01 tilts named, IP / tax / regulatory posture, exit cost — and reaches a specific door decision ("EOR," "direct entity + form," or "do not hire in this configuration"). "It depends" is unacceptable.
2. Scenario B's IR35 analysis names the CEST tool, the HMRC off-payroll working rules under Chapter 10, Part 2, ITEPA 2003, and reaches an "inside IR35" or "outside IR35" determination with reasoning. The analysis explicitly addresses the end-client PAYE / NIC withholding obligation for a medium or large client under the status-determination-statement mechanism.
3. Scenario C's analysis names the AÜG limit, the 6+-employee Betriebsrat trigger, the ArbnErfG employee-invention regime relevant to the researcher's invention-generating role, and reaches a GmbH-formation decision with an EOR bridge during formation.
4. Scenario D's analysis names the two-director rule with Indian-resident-director requirement under Companies Act 2013 s. 149(3), the Pvt Ltd formation mechanics, and reaches a direct-entity-day-one decision.
5. Scenario E's analysis acknowledges the Portuguese NHR regime narrowing since 2024, flags the IFICI / RNH 2.0 successor regime with `<!-- needs-research: ... -->`, and reaches an EOR-with-annual-review decision given the single-hire trajectory.
6. Part B produces a cost-comparison table for Scenarios C and D at headcount levels 1 / 3 / 6 / 10 with EOR cost and direct-entity cost per year, identifies a break-even headcount, and ties that break-even to the Part A door decision.
7. Part B's numeric figures are grounded in chapter 01, chapter 02, or chapter 06 content; any additional specific fee or platform-price is flagged with `<!-- needs-research: ... -->`.
8. Part C's EOR platform audit covers the chapter-01-named provisions (IP-assignment, equity handling, executive handling, termination), produces a side-by-side alternative-platform benchmark, reaches a continue-with-Deel / migrate / multi-platform decision with rationale, and includes a migration plan if migration is chosen.
9. Part D's 12-month plan is month-indexed, named per scenario, with dependencies, budget-envelope sketch, milestones, cross-functional ownership, and two-to-three explicit executive-review decision asks.
10. Part E's country decision register is populated with every country Fathom currently touches (US + UK + Netherlands + Spain for current workers + new countries per scenarios), has every column populated per the specified structure, and is formatted for diligence-team readability.
11. Deferrals to sibling modules and chapters are explicit: [chapter 02](../02-first-international-entity-setup.md) for entity-form mechanics; [chapter 03](../03-intercompany-and-transfer-pricing-structure.md) for the ICSA; [chapter 06](../06-international-benefits-and-equity-comp.md) for benefits / statutory loadings; [chapter 08](../08-international-workforce-reduction-playbook.md) for exit-cost mechanics; [mod-104](../../mod-104-hiring-onboarding-and-hr-operations/) for the HRIS integration; [mod-112 chapter 04](../../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md) for sanctions-screening on new hires.
12. Any specific fee, platform-pricing, or benchmark figure not grounded in chapter 01, chapter 06, or the problem statement is flagged with `<!-- needs-research: ... -->`. No real-company names are invented as "retained advisor." Nothing is left as `[TBD]` or `[FILL IN]`.
