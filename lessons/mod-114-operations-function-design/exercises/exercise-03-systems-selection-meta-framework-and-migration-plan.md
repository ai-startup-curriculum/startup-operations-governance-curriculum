# Exercise 03 — Systems-selection meta-framework and migration plan

> Estimated time: **~10 hours** · Related chapter: [03 — Systems-selection meta-framework and migration](../03-systems-selection-meta-framework.md)

## Problem statement

Keelstone Health is a Series-C B2B SaaS company (900 employees, US + UK + Canada + India footprint, 18-month plan to grow to 1,500) building clinical workflow software for health systems. The company is on **Rippling** for HRIS, ATS, benefits, payroll (US + Canada), and IT (laptop provisioning + MDM). The combination has worked well through Series B but is reaching the end of its tier:

- Rippling's comp-management module cannot support the comp-committee-driven executive-comp architecture the new CPO wants to implement (see [mod-105](../../mod-105-equity-compensation-policy-and-comp-committee/) and [mod-106](../../mod-106-compensation-architecture-and-total-rewards/)).
- Multi-country payroll consolidation (US + Canada direct; UK + India through separate payroll partners) is becoming a reporting-cycle headache that the CFO cites in each MBR.
- The healthcare-vertical customer base (clinics, hospitals, health systems) is pushing security-questionnaire volume that Keelstone's Vanta posture is now barely keeping up with; the first customer has asked specifically whether Keelstone has formal "HR data residency" that Rippling does not clearly deliver.
- The 18-month plan to 1,500 employees — much of which is in R&D specialist roles with complex equity grants — tips the HRIS-tier decision into the Workday / UKG / SAP SuccessFactors / Oracle HCM enterprise bracket.

The incoming Head of Business Systems (3 weeks in-seat) has been asked by the COO to run the HRIS-migration decision end-to-end. The scope: pick the system; author the migration plan; produce the change-management artefacts; set the executive-sponsor structure. The CPO and CFO are the two line stakeholders; the COO is the executive sponsor; the GC and the Head of Security run the gates.

A parallel question has surfaced: the finance team's Head of Procurement (newly hired 2 months ago) has produced a sprawl-discovery report showing 128 SaaS vendors across the company, and a working group of VPs has asked whether the HRIS migration is the right moment to also look at the comp-tool, GRC, and board-portal categories — each of which may be approaching its own graduation trigger — or whether to run those as separate decisions.

Scope the HRIS decision end-to-end. Address the parallel-category question with a defensible call.

## Requirements

### Part A — The six-criterion buying matrix

Author the buying-criteria matrix for the HRIS decision against the four finalists (reasonable finalists for a Series-C 900-to-1,500-employee healthcare-vertical SaaS):

- **Workday HCM.**
- **UKG Pro.**
- **SAP SuccessFactors.**
- **Rippling Enterprise tier (incumbent, as the "stay-and-upgrade" option).**

For each candidate, score against the six criteria from chapter 03:

1. **Build or buy.** Not applicable for HRIS at this scale; buy is the answer. State so briefly.
2. **Integration to source-of-truth systems.** Keelstone's existing stack: Rippling as HRIS (incumbent); ADP for UK + India payroll; NetSuite for financials (hypothetical — if different, state); Okta as IAM; Salesforce as CRM; Ashby as ATS; Vanta as GRC; Diligent as board portal. For each HRIS candidate, enumerate the native-connector availability, the SCIM / SAML support, the ERP / GL integration, and the ATS integration.
3. **Security and compliance posture.** SOC 2 Type II; ISO 27001; data-residency options (US / EU-only / specific region); HIPAA / HITRUST posture (Keelstone's healthcare-vertical customer base makes this a hard requirement); DPA / SCCs / DPF / IDTA for UK and India transfers; sub-processor register.
4. **Scale trajectory.** The 1,500-employee 18-month target; the specialist / R&D workforce; the equity-grant complexity; the multi-country footprint; the comp-committee requirement.
5. **Total cost of ownership.** Year 1 / Year 3 / Year 5 TCO modelled with: license, implementation, integration, change-management, ongoing administration, overage. Numbers directional per chapter 03's "needs-research" discipline — do not invent specific per-employee-per-month pricing without flagging. The TCO exercise is to produce a defensible comparative structure, not a specific invoice.
6. **Exit / vendor lock-in.** Data-export terms; API completeness; contract term / renewal; vendor viability (public-company status of each candidate).

Produce a scored matrix (1–5 per criterion per candidate) with the scoring rationale documented alongside. Pick a winner with a 3-paragraph rationale.

### Part B — The HRIS migration plan

Author the end-to-end migration plan for the winning candidate from Part A. Follow chapter 03's seven standard phases:

1. **Scope and requirements.** 2–4 weeks. The scope document; the enumerated workflows; the integration surfaces; the sign-off.
2. **Vendor selection.** 2–4 weeks. The RFP structure; the demo scope; the reference-call list; the scoring matrix (from Part A).
3. **Implementation and configuration.** 4–16 weeks category-dependent — for Workday HCM at Keelstone's scale, estimate the window and name the partner / integrator model (Deloitte / Accenture / Alight / Collaborative Solutions / Kainos — pick one and justify).
4. **Data migration and reconciliation.** 2–8 weeks. The extract / transform / load design; the reconciliation gate (chapter 03 names the gate as the most-skipped and most-consequential — your plan must hold it).
5. **UAT and enablement.** 2–4 weeks. The pilot design; the training plan; the help-desk playbook.
6. **Cutover.** 1–2 weeks. The freeze; the final reconciliation; the hypercare war-room.
7. **Decommission and archive.** 4–8 weeks post-cutover. The data archive; the Rippling decommission date; the records-retention compliance (coordinated with mod-110).

For each phase, name:
- The phase lead (specific role: Head of Business Systems, Head of Payroll, Head of IT, CPO, CFO, GC, Head of Security, Head of Workplace where applicable).
- The gate for exiting the phase.
- The specific risks and the mitigation.

### Part C — The change-management artefacts

Produce the five change-management artefacts (chapter 03 names the structure):

1. **Executive sponsor charter.** One page. Who is the sponsor; what decisions does the sponsor own; what escalation path. Keelstone's sponsor is the COO; the charter authors the specific escalation and decision-rights model.
2. **Steering-committee design.** One page. Membership (COO sponsor, CPO as function lead, Head of Business Systems as technical lead, Head of Payroll as data lead, GC as contract / DPA lead, Head of IT as SSO / SCIM lead, CoS as comms lead); cadence (weekly during the migration); scope.
3. **Communications plan.** One page. The all-hands announcement; the monthly update cadence; the cutover communications; the post-cutover retrospective. Includes a sample all-hands announcement script (3–4 paragraphs).
4. **Training plan.** One page. Workday-provided admin training; a company-wide LMS module; live sessions for people managers; a help-desk playbook.
5. **Rollback plan.** One page. The state at cutover; the criteria that would trigger rollback; the mechanical steps to execute it; the retention of Rippling read access post-cutover.

### Part D — The parallel-category decision

Address the parallel question: should the HRIS migration be run concurrently with the comp-tool, GRC, and board-portal categories, or sequentially?

The answer must consider:
- **Change-management bandwidth.** The company can only absorb so much simultaneous system change. Chapter 03 names a mid-scope migration at 3–6 months and an enterprise HCM at 6–12 months. Running the three parallel categories against the HRIS timeline either breaks the organisation or produces visibly degraded migrations.
- **Category graduation triggers.** For each of comp-tool (currently Rippling / spreadsheets), GRC (currently Vanta), and board-portal (currently none / Diligent-adjacent): is the graduation trigger actually fired? Draw on chapter 03's graduation-trigger section.
- **Dependency ordering.** The comp-tool depends on the HRIS as source-of-truth for employee master data; it should land after the HRIS, not before. The GRC migration depends on the HRIS for the user / access-review feed; it should land after. The board portal is independent and could run in parallel if the corporate secretary wants to.
- **Executive-attention budget.** Keelstone's executive team can run one major migration at a time well, or two concurrent migrations badly. Which is right for this moment?

Produce a 24-month sequencing roadmap for the four categories, with the HRIS migration anchored in months 1–9 and the other three categories sequenced around it.

### Part E — The HRIS post-migration state

Author the one-page "post-migration state" artefact — the picture of the Keelstone systems architecture after the HRIS migration completes and the Rippling decommission is complete.

Must include:
- Source-of-truth system map (Workday HCM for employee master data; NetSuite / finance for financials; Okta for identity; Salesforce for customer master data; Ashby for ATS; Vanta for compliance; Diligent for board portal; the ADP relationship for international payroll where Workday Payroll does not cover; MDM retention from Rippling or a new vendor).
- Integration map (Workday ↔ ADP; Workday ↔ Okta; Workday ↔ NetSuite; Workday ↔ Ashby; Workday ↔ Vanta for the compliance evidence feed).
- The named administrator for each system (Head of Business Systems for Workday; VP People for the HR-process ownership; Head of Payroll for the payroll feed; CFO for the finance integration; Head of IT for the identity integration).
- The renewal calendar entry (Workday contract renewal date; the Rippling termination-notice date already executed).

## Starter guidance

- [Chapter 03](../03-systems-selection-meta-framework.md) is the primary reference. The six-criterion matrix, the graduation triggers, the migration phases, and the change-management artefacts are all there.
- [Chapter 05](../05-procurement-operating-model.md) is referenced for the procurement motion (RFP, MSA / DPA negotiation, vendor-diligence checklist).
- [Chapter 06](../06-operating-cadence-and-okrs-rhythm.md) is referenced for the executive-sponsor model inside the operating cadence.
- [Mod-104](../../mod-104-hiring-onboarding-and-hr-operations/) owns the specific HRIS decision; mod-114 provides the framework. Your Part A analysis is the mod-104-owned decision run through mod-114's framework.
- [Mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/) owns the privacy posture (DPA, SCCs, data residency) that Part A Criterion 3 depends on.
- [Mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/) owns the security review (SOC 2, ISO 27001, HIPAA) that Part A Criterion 3 depends on.
- Do not invent per-employee-per-month pricing. Where chapter 03 provides a directional range, use the range. Where it does not, flag with `<!-- needs-research: ... -->`.
- Do not invent partner / implementation-firm pricing. Chapter 03 states "US$0.5–1.5M for the full HCM + payroll + comp module scope" directionally for an HCM implementation at Series-C scale — you may use this range and flag any sharpening.
- The healthcare-vertical nature of Keelstone matters for Criterion 3 (HIPAA / HITRUST). Each HRIS candidate's HIPAA posture should be evaluated specifically; do not state HIPAA conformance without flagging `<!-- needs-research: ... -->` where the specific posture is not in the chapter.

## Deliverables

- `part-a-buying-matrix.md` — the scored six-criterion matrix across all four candidates with the winner and 3-paragraph rationale.
- `part-b-migration-plan.md` — the seven-phase migration plan for the winning candidate.
- `part-c-executive-sponsor-charter.md` — Part C artefact 1.
- `part-c-steering-committee-design.md` — Part C artefact 2.
- `part-c-communications-plan.md` — Part C artefact 3 (includes the all-hands announcement script).
- `part-c-training-plan.md` — Part C artefact 4.
- `part-c-rollback-plan.md` — Part C artefact 5.
- `part-d-parallel-category-roadmap.md` — the 24-month roadmap for the four categories.
- `part-e-post-migration-state.md` — the post-migration systems architecture.

## Acceptance criteria

The package is acceptable if:

1. Part A scores all four candidates on all six criteria with explicit rationale per cell; picks a winner with a 3-paragraph rationale; does not invent per-employee-per-month pricing beyond chapter 03's directional ranges.
2. Part A's Criterion 3 (security / compliance) addresses the healthcare-vertical HIPAA / HITRUST requirement explicitly for each candidate — flagged `<!-- needs-research: ... -->` where current-posture confirmation is required.
3. Part B's seven-phase migration plan is populated for every phase with lead role, exit gate, risks, and mitigations; the reconciliation gate (Phase 4) is held explicitly.
4. Part B names a specific partner / implementation-firm model for the Workday-or-equivalent implementation with a justification (why this partner, what the partner's role is, what Keelstone's internal team retains vs. hands off).
5. Part C produces all five change-management artefacts, each at least one page, with the Keelstone-specific leads named for each role.
6. Part C's communications-plan artefact includes a specific sample all-hands announcement script (3–4 paragraphs) — not a template placeholder.
7. Part D sequences the four categories (HRIS, comp-tool, GRC, board-portal) over 24 months with explicit dependency reasoning; the HRIS lands first with the other three sequenced around it; the roadmap is defensible against "but we need all of this at once" pressure.
8. Part D's reasoning explicitly addresses change-management bandwidth, category graduation triggers, dependency ordering, and executive-attention budget — each named and applied.
9. Part E produces the post-migration state as a source-of-truth map plus integration map plus named-administrator list; the artefact is diligence-ready.
10. Cross-references to chapters 03, 05, 06; to mod-104, mod-110, mod-112; are explicit where the reasoning draws from them.
11. No specific pricing figures or partner-cost figures are invented beyond chapter 03's directional ranges. No HIPAA / HITRUST claim about any vendor is stated without a `<!-- needs-research: ... -->` flag unless chapter 03 or chapter resources documents it.
12. Nothing is left as `[TBD]` or `[FILL IN]`. The rollback plan is a real plan, not a placeholder — the criteria that trigger rollback are specific, not "if there's a problem."
