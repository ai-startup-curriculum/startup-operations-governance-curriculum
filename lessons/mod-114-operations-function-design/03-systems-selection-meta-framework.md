# 3. Systems-selection meta-framework and migration

> Every scale-up buys forty to a hundred SaaS systems in its first five years. Most of them are bought badly — under-researched, over-integrated, wrongly-sized, and migrated with no plan — because the operations function that should have owned the meta-framework has never written one down. This chapter is the meta-framework.

## Motivation

An individual system decision — HRIS, ATS, comp tool, CLM, board portal, expense management, procurement, IT-and-endpoint management — is often authored by someone else. Payroll and expense management are the CFO's call. HRIS and ATS are the CPO's call. CLM is the GC's call. Endpoint management is the CTO / Head of IT's call. Board portal is the corporate secretary's call.

But there is a *pattern* to how every one of those decisions goes right or wrong, and that pattern is the operations function's product. The buying-criteria matrix, the graduation-trigger discipline, the vendor-diligence checklist, and the migration change-management pattern are all cross-cutting. Written once and enforced consistently, they turn systems selection from a series of one-off vendor pitches into a repeatable operating capability.

This chapter is the meta-framework. It does not choose the HRIS ([mod-104](../mod-104-hiring-onboarding-and-hr-operations/) does). It gives the ops function a reusable way to *run* the HRIS selection, and every other systems selection like it.

## The buying-criteria matrix

Every material systems purchase — meaning any purchase over some threshold ($25k / year is a common one; use whatever your approval-authority matrix in [chapter 05](./05-procurement-operating-model.md) says) — is evaluated against the same six criteria. Score each candidate on each; document the scoring; keep the artifact.

### Criterion 1 — Build or buy

Ask the build-or-buy question first, before any vendor pitch. For most operations systems the answer is "buy" — the market is deep, the systems are commoditised, and the total cost of ownership of an in-house build is enormous. But there are cases where "build" is the right answer:

- **The workflow is a differentiator.** If the system implements a workflow that is core to how the company competes (a pricing engine, a customer-onboarding orchestration, a data-labelling pipeline for an AI product), build it. Do not outsource competitive advantage to a vendor.
- **No vendor fits the requirement.** If the shortlist of candidates all fail the requirement, either the requirement is wrong (audit it) or the market is immature (build it, and revisit in 24 months).
- **The integration cost of a bought system exceeds the build cost.** Rare, but real for very specific niches (an internal-tooling framework that would need custom integration to every one of five legacy systems may be cheaper to build).

For operations systems specifically — HRIS, ATS, CLM, comp tool, board portal, expense management, procurement — buy is almost always right. The rare exception is a company at a scale (10,000+ employees) where the enterprise-tier vendor cost exceeds the amortised build cost of an in-house team of engineers; even then, buy is usually right and the build path is a warning sign.

### Criterion 2 — Integration to source-of-truth systems

Every operations system reads from and writes to at least one other operations system. The integration surface determines the operational cost of the vendor for the next 3–5 years.

- **Identify the source-of-truth systems** the company has committed to. Typically: **HRIS as the source of truth for employee master data**; **ERP / GL as the source of truth for financials**; **Salesforce (or comparable CRM) as the source of truth for customer master data**; **an IAM / identity provider (Okta, Microsoft Entra ID, JumpCloud, Google Workspace) as the source of truth for identity and access**; **an endpoint / MDM system as the source of truth for device inventory.**
- **Every new system must have a documented integration to the relevant source of truth.** Bidirectional, ideally; unidirectional (source-of-truth → new-system) at minimum for employee data flowing from HRIS to any HR-adjacent tool.
- **Prefer SCIM + SAML for identity.** Any system that provisions users should support **SCIM 2.0** (System for Cross-domain Identity Management) for user lifecycle and **SAML 2.0** (or OpenID Connect) for authentication. Systems that support neither fail the criterion; systems that support SAML but not SCIM require manual deprovisioning, which becomes a security-audit finding.
- **Prefer native connectors to iPaaS-only integration.** A vendor with a native Workday connector is cheaper to operate than one that only integrates via a middleware layer (Workato, Boomi, Zapier, Tray.io). iPaaS is a legitimate answer for the long tail; source-of-truth integrations should be native where possible.

### Criterion 3 — Security and compliance posture

Every material systems purchase has a security-and-privacy review as a mandatory gate — no vendor signs without it. See [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) for the privacy side and the security-programme chapter of [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) for the security-review depth. The vendor-side checklist:

- **SOC 2 Type II report on file** — request under NDA, read the exception section, note the last audit date and the next.
- **ISO/IEC 27001 certification** where the vendor targets enterprise buyers.
- **Data-processing addendum (DPA) with SCCs / IDTA / DPF** as needed for cross-border data flows to non-adequate jurisdictions.
- **Sub-processor register** — the list of vendors the vendor uses (their cloud provider, their sub-tier tools). Any change should be notified to the customer per the DPA.
- **Encryption at rest and in transit** — table stakes, but verify the KMS integration and key-rotation posture.
- **SSO enforcement** and **SCIM provisioning** — see Criterion 2.
- **Data-residency options** where regulatory constraints (GDPR, sector-specific data-residency, national-security-sensitive data) apply. US-only, EU-only, or a specific-region hosting option may be a hard requirement.
- **Sector-specific certifications** — HIPAA / HITRUST for health data; PCI-DSS for payment data; FedRAMP for federal data; StateRAMP for state government; sector-specific attestations (SOX-relevant SaaS attestations, MAR / GDPR / SOX for public-company relevance).

The security-and-privacy review runs in parallel with the commercial evaluation. A vendor that fails the security bar is disqualified regardless of commercial fit. Do not sign a "we'll fix it in the next release" MSA on a security issue.

### Criterion 4 — Scale trajectory

Match the vendor's scale sweet spot to the company's 24-month trajectory, not to the current headcount. Systems bought for the current size often need to be replaced 12–24 months later at multiples of the switching cost.

- **HRIS example.** Rippling and Gusto are excellent below ~200 employees; Workday and UKG are excellent above ~1,000 employees; the 200–1,000 zone is the *hardest* market segment and includes BambooHR, ADP Workforce Now, Namely, Paylocity, Sage People, Justworks (via PEO tier), and Rippling's enterprise tier. Choose the system that fits the *end-of-24-months* headcount, not the *day-of-signing* headcount.
- **CRM example.** HubSpot is excellent early; Salesforce dominates enterprise; a mid-market company churning between the two at Series B is spending millions of dollars in replatforming for no incremental sales value.
- **ATS example.** Ashby, Greenhouse, and Lever are the modern venture-scale-up staples; Workday Recruiting is the enterprise standard. Below 500 headcount, the modern ATSs win; above 2,000 headcount, Workday's integration wins.

<!-- needs-research: verify current vendor positioning and scale bands for HRIS, CRM, and ATS in 2026 — the market consolidates and product tiers shift each year. -->

### Criterion 5 — Total cost of ownership (TCO)

TCO is not the sticker price. It includes:

- **License / subscription** — the annualised cost, at the projected 24-month headcount, at the projected per-seat or per-transaction rate. Watch for step-function pricing at seat-count thresholds and for annual price increases (a 5–8% annual escalator is common; some vendors quote 10–15%).
- **Implementation** — either self-serve, professional-services-led, or partner-led. Enterprise HCMs (Workday, UKG) and enterprise CRMs (Salesforce) typically require six-figure implementation projects with a system-integrator partner (Deloitte, Accenture, Alight, IBM, or a specialised boutique).
- **Integration cost** — engineering time to build and maintain integrations to the source-of-truth systems.
- **Change-management cost** — training, documentation, communication. A large system rollout can absorb weeks of internal-communications and enablement time.
- **Ongoing administration** — the FTE cost of the people who run the system inside the company (HRIS admin, Salesforce admin, ERP admin). At scale, a well-run system requires a dedicated administrator; the administrator's fully-loaded cost is part of TCO.
- **Data storage / API-call / transaction overages** — variable-cost components that can dominate at scale.

Model TCO at Year 1, Year 3, and Year 5. A vendor that is cheaper in Year 1 and more expensive in Year 3 is a bad buy unless the Year-1 savings are large enough to justify replatforming.

### Criterion 6 — Exit / vendor lock-in

Every systems purchase has an eventual exit. Design for the exit at the time of the purchase.

- **Data-export terms in the MSA.** The customer's data is the customer's data; the contract must say so. Enterprise vendors typically agree without pushback; some SaaS vendors need to be pushed. Insist on: right to export all data on demand and on termination, in a structured format (CSV, JSON, or a vendor-supported open format), for a defined window post-termination (30–90 days).
- **API completeness.** A system whose UI shows data its API cannot export is a lock-in trap. Confirm during the evaluation that every data element you will need to migrate has a corresponding API endpoint.
- **Contract term and renewal terms.** Multi-year deals earn a discount and add lock-in. Auto-renewal clauses need explicit termination-notice discipline (a diarised termination-notice date, 60–90 days before renewal, owned by procurement — see [chapter 05](./05-procurement-operating-model.md)).
- **Data-residency / re-hosting flexibility.** For systems that store material customer or employee data, understand whether the data can be re-hosted (region change, tenancy change) or whether re-hosting requires a full re-implementation.
- **Vendor viability.** A small vendor may be acquired by a larger vendor or may go out of business. Prefer vendors with clear enterprise-scale customers, funded runway (for private vendors — check funding history), or public-market ownership. Include a "material-adverse-change" out in the MSA where the leverage allows.

## Graduation triggers by system category

Every operations system has a **graduation trigger** — the moment the current tool stops working and the company needs to move to a bigger one. The trigger is category-specific. This section lists the common categories and their triggers.

### HRIS (Human Resources Information System)

- **Starter tier — ~1–50 employees.** Gusto, Rippling starter tier, or a PEO's bundled HRIS (Justworks, TriNet, Sequoia One). Payroll, benefits, basic employee master data.
- **Growth tier — ~50–200 employees.** Rippling, BambooHR, HiBob, Namely. Adds performance-management modules, ATS integration, org-chart, expanded reporting.
- **Scale tier — ~200–1,000 employees.** HiBob, Rippling, Paylocity, ADP Workforce Now, BambooHR at the high end. Adds workflow automation, deeper reporting, multi-country payroll integration.
- **Enterprise tier — ~1,000+ employees.** Workday HCM, UKG Pro, SAP SuccessFactors, Oracle HCM. Adds compensation modules, talent-management modules, complex org-structure modelling, deep integration with ERP/GL.

**Graduation trigger — starter → growth.** ~50 employees, or the first material multi-state / international payroll complexity, or the first performance-management cycle that exceeds spreadsheet capacity.

**Graduation trigger — growth → scale.** ~200 employees, or the emergence of multiple business units / geographies needing distinct reporting.

**Graduation trigger — scale → enterprise.** ~1,000 employees, or the emergence of a compensation-committee-driven executive-comp architecture, or the emergence of complex org modelling (matrix reporting, cost-centre hierarchies, multi-entity payroll).

<!-- needs-research: verify current HRIS vendor positioning and the specific tiers — the HRIS market is one of the most-consolidating segments in the systems landscape and product tiers shift with each vendor's annual release. -->

### ATS (Applicant Tracking System)

- **Starter — up to ~50 hires/year.** Ashby's starter tier; Greenhouse's starter tier; Workable; Lever's starter tier; Rippling ATS.
- **Growth — 50–500 hires/year.** Ashby, Greenhouse, Lever full-tier.
- **Enterprise — 500+ hires/year.** Ashby, Greenhouse (enterprise), Workday Recruiting, iCIMS, SmartRecruiters, Eightfold, Beamery for talent-CRM.

**Graduation trigger.** Hire volume, source-of-hire diversity (agency, sourcing, referral, employer brand), and the reporting depth the recruiting team needs.

### Compensation tool

- **Starter — spreadsheets.** Real, and adequate up to a couple of comp cycles.
- **Growth — Pave, Compa, Assemble, Barley, Ravio, Figures, Ledgy (comp module).**
- **Enterprise — Workday Compensation, PayScale MarketPay, Radford's tools, PeopleFluent.**

**Graduation trigger.** Comp-cycle complexity (multiple bands, geo-differentials, equity refresh); comp-committee cadence (executive comp needs a real tool once the committee exists); benchmarking-source integration.

### CLM (Contract Lifecycle Management)

- **Starter — a signed-PDF folder in Google Drive or a light e-signature product (DocuSign, HelloSign / Dropbox Sign, Adobe Sign).**
- **Growth — Ironclad, Juro, LinkSquares, ContractPodAi, DocuSign CLM, Concord.**
- **Enterprise — Icertis, Agiloft, SAP Ariba Contracts.**

**Graduation trigger.** Contract volume past ~50–100 per quarter; renewal-tracking becomes a real problem; the GC's team is spending measurable time on contract-management overhead. See [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/).

### Privacy platform

- **Starter — spreadsheet-based Record of Processing Activities (RoPA), manual DSAR handling.**
- **Growth — OneTrust, TrustArc, Osano, Ketch, Transcend, DataGrail.**
- **Enterprise — OneTrust (enterprise), BigID, Securiti.**

**Graduation trigger.** GDPR RoPA becomes unmaintainable in a spreadsheet; DSAR volume passes a handful per quarter; the company adopts a sector-specific privacy regulation (CCPA/CPRA, HIPAA, sector-specific) with automated-compliance requirements. See [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).

### Security-compliance platform (GRC)

- **Starter — spreadsheets, ad-hoc auditor engagement.**
- **Growth — Vanta, Drata, Secureframe, Sprinto, Tugboat Logic (acquired by OneTrust).**
- **Enterprise — AuditBoard, LogicGate, ServiceNow GRC, Archer.**

**Graduation trigger.** First SOC 2 Type II audit; first ISO 27001 audit; first customer requirement for a security questionnaire response volume that exceeds manual capacity.

### Board portal

- **Starter — email + a shared drive.** (Not actually adequate — see [mod-111 chapter 02](../mod-111-corporate-governance-board-operations-and-officer-duties/02-board-cadence-and-materials.md).)
- **Growth — Diligent Boards, Nasdaq Boardvantage, OnBoard (Passageways), BoardEffect, Boardable, Board Intelligence.**

**Graduation trigger.** Preparing for a formal board (Series-A board formation onward); adding standing committees; adding independent directors; approaching an IPO.

### Spend management / expense management

- **Starter — corporate card (Amex, Brex, Ramp) + expense-report tool (Expensify, Concur).**
- **Growth — Ramp, Brex, Spendesk, Airbase, Rippling Spend, Divvy (BILL Spend & Expense).**
- **Enterprise — SAP Concur, Coupa Expenses, Oracle Fusion Expenses.**

**Graduation trigger.** Spend volume; multi-entity or multi-country consolidation needs; the CFO's cash-management discipline needing real-time visibility.

### Procurement platform

- **Starter — spreadsheet vendor list, distributed purchasing.**
- **Growth — Ramp Procurement, Airbase Procurement, Vendr, Sastrify, Zip, Zluri, Torii (SaaS-specific discovery).**
- **Enterprise — Coupa, SAP Ariba, Oracle Procurement Cloud, Ivalua, Jaggaer.**

**Graduation trigger.** SaaS vendor count past ~50–75; procurement-team formalisation (see [chapter 05](./05-procurement-operating-model.md)); the finance-audit trail requirement (SOX or SOX-adjacent) that requires purchase-order and three-way-match discipline.

### IT and endpoint management

- **Starter — a small MSP or a fractional IT lead; a laptop-provisioning workflow.**
- **Growth — Jamf Pro (macOS), Kandji, Fleetsmith (Apple, deprecated / merged), Microsoft Intune (mixed fleet), JumpCloud (identity + MDM), NinjaOne, Rippling IT.**
- **Enterprise — Jamf Enterprise, Microsoft Intune Suite, VMware Workspace ONE (Omnissa), IBM MaaS360, ServiceNow ITSM as the ticketing layer.**

**Graduation trigger.** Fleet size (~50 devices); security-programme requirement for MDM enforcement, disk encryption enforcement, and device-inventory reconciliation; the first security audit requiring MDM evidence.

<!-- needs-research: verify current vendor positioning across HRIS, ATS, compensation, CLM, privacy, GRC, board portal, spend, procurement, and IT-and-endpoint categories — the market is dynamic and multiple categories are consolidating rapidly. -->

## The change-management pattern for a system migration

Every material system migration follows the same pattern. The specific technical steps differ by system; the change-management skeleton does not.

### Migration length by category

- **Point tool (single-function, single-integration).** 4–8 weeks end to end.
- **Mid-scope system (HRIS, ATS, CLM, spend management).** 3–6 months end to end.
- **Enterprise-scale HCM or ERP.** 6–12 months for a full replatform; some Workday HCM or NetSuite implementations run 12–18 months at scale-up size, longer at enterprise size.

### Standard migration phases

**Phase 1 — Scope and requirements (2–4 weeks).** Confirm the six criteria above are satisfied by the incoming vendor. Enumerate the specific workflows the outgoing system supports and the ones the incoming system must support. Identify integration surfaces. Publish a scope document that the CoS / COO signs off on.

**Phase 2 — Vendor selection (2–4 weeks).** Two to four candidates on the shortlist; each gets a demo scoped to the specific workflows; each answers a security-and-privacy questionnaire; each provides references (call at least two per finalist); a scoring matrix aligned to the buying-criteria matrix produces the finalist. Contract negotiation runs in parallel — pricing, term, data-export terms, security addendum, DPA, MSA. GC / procurement review is a hard gate.

**Phase 3 — Implementation and configuration (4–16 weeks, category-dependent).** Vendor implementation team, internal admin, and integration engineering work in parallel. Data model design; workflow configuration; integrations built and tested; permissions and access model defined and provisioned via SSO / SCIM.

**Phase 4 — Data migration and reconciliation (2–8 weeks, overlapping Phase 3).** Extract from the outgoing system; transform to the incoming system's schema; load; reconcile record-by-record. Reconciliation is the phase that most often blows the timeline — plan for it, and hold a "no go-live without clean reconciliation" gate.

**Phase 5 — User acceptance testing and enablement (2–4 weeks).** A pilot group of users runs the incoming system on live workflows in parallel with the outgoing system. Bugs and configuration issues surface. Training materials, help-desk documentation, and communications plan are finalised.

**Phase 6 — Cutover (1–2 weeks).** Freeze the outgoing system for writes; run the final reconciliation; cut users over to the incoming system; monitor the first cycle (first payroll on the new HRIS, first month-end on the new ERP, first hire on the new ATS) closely. A dedicated post-cutover war-room for the first 5–10 business days.

**Phase 7 — Decommission and archive (4–8 weeks post-cutover).** Extract full data archive from the outgoing system; store per records-retention policy; terminate the outgoing contract on the last-day-of-service date documented in the termination-notice ([chapter 05](./05-procurement-operating-model.md)).

### Change-management side of the migration

The technical migration is only half the work. The other half is the workforce transition:

- **Executive sponsor.** The COO / CoS or a peer executive is the accountable sponsor. All escalations go there. All go/no-go decisions are made there. Without a sponsor, the migration drifts.
- **Steering committee.** Weekly steering meeting for the duration of the migration. Attendees: sponsor, incoming-system admin owner, integration owner, security / privacy owner, communications owner, function-lead owner (e.g., Head of People for an HRIS migration).
- **Comms plan.** Announcement, mid-migration update, cutover comms, post-cutover retro. All-hands touchpoints for a company-wide system (HRIS, expense, spend). Manager-cascade for a function-specific system.
- **Training plan.** Vendor-provided training for admins; internally-produced enablement for end users; a help-desk playbook for the first month post-cutover.
- **Parallel-run window.** For high-risk migrations (payroll, financial GL, sales CRM), run the incoming and outgoing systems in parallel for one full cycle. The cost is real; the risk reduction is worth it.
- **Rollback plan.** Every migration has a rollback plan, even if it is never used. Document the state at cutover, the criteria that would trigger rollback, and the mechanical steps to execute it.

## Concrete example — HRIS migration from Rippling to Workday HCM

A representative growth-stage migration:

**Company:** Series-C SaaS, 900 employees, US + UK + Canada + India. Rippling as HRIS, ATS, and IT management. Growing to 1,500 employees over the next 18 months; comp-committee-driven executive-comp architecture becoming a hard requirement; multi-country consolidation reporting straining Rippling's mid-market feature set.

**Trigger.** Scale-tier graduation. Rippling's tier is a fit through ~1,000 employees; the pressure of the next 18-month plan tips the buy call to Workday HCM.

**Migration length.** 9 months end to end, of which 4 months implementation, 2 months data migration, 1 month UAT, 1 month cutover / hypercare, 1 month decommission.

**Change-management footprint.**
- Executive sponsor: COO.
- Steering committee: COO (sponsor), VP People (function lead), Head of Business Systems (technical lead), Head of Payroll (data lead), GC (contract / DPA lead), Head of IT (SSO / SCIM lead), CoS (comms lead).
- Comms: all-hands announcement at the start; a monthly update; a company-wide "Workday goes live on X date" communication one month before cutover; a post-cutover survey.
- Training: Workday-provided admin training for 8 admins; a company-wide LMS module for end users; live sessions for people managers on the new workflows.
- Parallel run: one payroll cycle on both systems, with a formal reconciliation gate.
- Rollback plan: retain Rippling read access for 90 days post-cutover; the trigger for rollback is a defined payroll-error rate or a data-integrity failure that cannot be resolved in-flight.

**Cost.** Software: Workday license at Year 1 approximately US$25–40 per employee per month at Series-C scale <!-- needs-research: verify Workday HCM per-employee-per-month pricing at ~1,000-employee scale in 2026, as vendor pricing varies by module set and geographic scope. -->. Implementation: partner-led (Deloitte, Accenture, Alight, or a Workday-specialised boutique) at US$0.5–1.5M for the full HCM + payroll + comp module scope. Internal cost: 2 FTE-years of Business Systems + 1 FTE-year of Payroll + 0.5 FTE-year of the CoS's time. Total 3-year TCO in the low-to-mid single-digit millions.

**Post-migration state.** Workday HCM as source-of-truth for employee master data; Ashby (ATS) integrated bidirectionally; Ramp (expense) integrated for expense-to-payroll; ADP (multi-country payroll partner) integrated where Workday Payroll does not cover the country; Rippling IT retained as MDM (not migrated); Rippling HRIS decommissioned.

## Common failure modes

- **Sticker-price shopping.** The company picks the cheapest vendor on Year-1 quoted price and pays for it in Year-3 integration overages, migration cost, and admin overhead.
- **No integration owner.** The system is bought; nobody owns the SSO / SCIM setup; two years later the security audit surfaces provisioning gaps. Fix: the migration plan names an integration owner from Business Systems on day one.
- **Under-scoping the migration.** A 6-month HRIS migration is planned as a 3-month project; the timeline slips; the freeze-outgoing-system decision gets deferred; the two systems run in parallel for a year, doubling cost. Fix: use industry benchmarks for migration length by category and budget accordingly.
- **No reconciliation gate.** Cutover happens without a clean reconciliation because "we'll fix it in-flight"; the first cycle on the new system has systemic data errors that erode trust in the tool. Fix: hold the gate.
- **No decommission of the old system.** The old system stays subscribed "in case we need it" for 12+ months post-cutover, paying license fees for nothing. Fix: the migration plan includes a decommission date and a records-retention archive.
- **Vendor lock-in discovered at exit.** The company tries to leave a vendor and discovers the data-export process is undocumented, the API is incomplete, and the vendor is uncooperative. Fix: read the MSA exit terms at the *purchase* stage, not at the exit stage.
- **Security review skipped for "small" tools.** A specific team buys a $10k / year tool without security review; the tool has access to customer data; a breach at the vendor becomes the company's incident. Fix: security review is mandatory for any tool touching customer / employee / financial data, regardless of dollar threshold.

## Summary

- Every material systems purchase runs against the same **six-criterion buying matrix**: build-or-buy, integration to source-of-truth, security / compliance posture, scale trajectory, total cost of ownership, and exit / vendor lock-in.
- Every system category has **graduation triggers** — HRIS starter → growth → scale → enterprise; ATS starter → growth → enterprise; CLM, privacy, GRC, board portal, spend management, procurement, IT-and-endpoint each have their own tier ladders. Match the buy to the *24-month* trajectory, not the day-of-signing headcount.
- **Migration length benchmarks:** 4–8 weeks for a point tool; 3–6 months for a mid-scope system; 6–12 months for an enterprise HCM or ERP; longer for the largest deployments.
- The **standard migration phases** are Scope → Vendor selection → Implementation → Data migration → UAT → Cutover → Decommission. Each has a gate; the reconciliation gate is the most-skipped and most-consequential.
- The **change-management footprint** — executive sponsor, steering committee, comms plan, training plan, parallel-run window, rollback plan — is half the migration. Skipping it is why systems migrations blow their timelines.
- The ops function owns the **meta-framework**. The specific system decisions live in the owning function's module ([mod-104](../mod-104-hiring-onboarding-and-hr-operations/) for HRIS/ATS; [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/)/[mod-106](../mod-106-compensation-architecture-and-total-rewards/) for comp tools; [mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/) for CLM; [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) for privacy; [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/) for board portal; [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) for GRC; the finance-fundraising curriculum for ERP / spend / expense / procurement systems).
