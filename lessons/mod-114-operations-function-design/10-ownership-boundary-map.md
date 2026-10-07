# 10. Ownership boundary map

> Operations is a boundary function. Every topic the COO / CoS touches is also touched by another function — People, Finance, Legal, IT, Product. The failure mode of operations is scope creep (ops owning everything no one else wants) and scope leakage (ops failing to own what only ops can own). This chapter is the written boundary.

## Motivation

A COO landing in a scale-up at Series C inherits a question-of-the-day that the previous regime answered inconsistently: "whose is this?" The HRIS migration — is it the CPO's call or the COO's? The board portal — the CoS or the corporate secretary? The sanctions screening on new vendors — procurement, GC, or the risk function in [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/)? The month-end close — CFO or operations? Each answer is defensible on its own; the problem is that *different* people in the organisation answer them differently, and the resulting handoff gaps are where things fall through.

This chapter is the reference. It names:

- **What this module owns end-to-end** — the operations function's exclusive territory.
- **What this module shares with a sibling module** — the handoff lines.
- **What this module defers to another module entirely** — the "not ours" calls.
- **What this module defers to specialist advisors** — the external-expertise edge.

Six worked examples at the end apply the boundary to concrete, often-contested questions.

## What mod-114 owns end-to-end

The operations function (as framed in this module) owns:

### Operations-function organisation and seating

- The **four-seat architecture** of operations: Chief of Staff, COO, Head of BizOps, Head of Workplace. The role definitions, hire triggers, reporting lines, and comp bands. See [chapter 01](./01-coo-vs-cos-and-bizops-org-design.md), [chapter 02](./02-first-ten-ops-hires-and-comp-benchmarks.md).
- The **first-ten-ops-hires sequencing** against stage triggers. See [chapter 02](./02-first-ten-ops-hires-and-comp-benchmarks.md).
- The **CoS-to-COO graduation path** and the operating relationship with the CEO. See [chapter 01](./01-coo-vs-cos-and-bizops-org-design.md), [chapter 08](./08-ceo-cos-or-coo-operating-relationship.md).

### Systems-selection meta-framework

- The **buying-criteria matrix** (build-or-buy, integration, security, scale, TCO, exit) applied to any material systems purchase. See [chapter 03](./03-systems-selection-meta-framework.md).
- The **graduation-trigger discipline** across system categories (HRIS, ATS, comp tool, CLM, privacy platform, GRC, board portal, spend management, procurement, IT-and-endpoint management).
- The **change-management pattern** for a system migration — the standard migration phases, the executive-sponsor pattern, the parallel-run and rollback discipline.
- The **Head of Business Systems seat** as the owner of the SaaS-architecture-and-integration layer.

The individual *system decisions* (which HRIS, which ATS, which CLM, which spend-management tool) are owned by the function the system primarily serves (CPO for HRIS/ATS, GC for CLM, CFO for spend/expense, Head of Business Systems for identity/MDM, corporate secretary for board portal). mod-114 owns the *framework* those decisions run against.

### Workplace and real estate

- The **workplace progression** from remote-first to coworking to direct lease to hub-and-spoke. See [chapter 04](./04-workplace-and-real-estate-progression.md).
- The **tenant-representation firm engagement** and lease-negotiation discipline (CBRE, JLL, Cushman & Wakefield, Newmark, Colliers, Savills, Cresa).
- The **TI negotiation**, the **sublease exit option**, and the **lease-document commercial terms**.
- The **physical workplace operations** — facilities, reception, mail, meeting-room A/V, security, janitorial, food service.
- The **Head of Workplace seat** and the workplace team.
- The **workplace-experience programme** — the physical expression of the hybrid / RTO policy owned by People.

The *hybrid / RTO policy itself* is owned by People ([mod-108](../mod-108-culture-employee-experience-and-dei/)). The *lease document legal review* is owned by GC ([mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/)) via retained real-estate counsel. mod-114 owns the operations.

### Procurement and vendor management

- The **spend taxonomy**, the **approval-authority matrix**, the **vendor-diligence checklist**. See [chapter 05](./05-procurement-operating-model.md).
- The **annual vendor review cadence**, the **renewal calendar**, the **vendor-consolidation playbook**.
- The **Head of Procurement seat** and the procurement team.
- The **procurement tooling stack** (Ramp / Brex / Spendesk / Airbase / Coupa and the SaaS-specific tools).
- The **commercial motion** in vendor negotiation and consolidation.

The *GL coding and month-end close* is owned by the CFO. The *vendor contract documents (MSA, DPA, security addendum)* are owned by the GC. The *security review of vendor products* is owned by the security function in [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/). mod-114 owns the commercial and operational layer.

### Operating cadence

- The **four-layer cadence** — weekly ops review, monthly business review, quarterly OKRs cycle, annual planning. See [chapter 06](./06-operating-cadence-and-okrs-rhythm.md).
- The **operating-metrics dashboard** and the **BizOps analytical function** that populates it.
- The **E-team weekly meeting** choreography and the **executive-team rhythm**. See [chapter 09](./09-executive-team-operating-rhythm.md).
- The **CEO's calendar and prioritisation discipline** (CoS-owned). See [chapter 08](./08-ceo-cos-or-coo-operating-relationship.md).
- The **cross-functional programme management** function — the PMO work owned by BizOps.

The *monthly close* is owned by the CFO. The *annual budget and financial plan* is owned by the CFO. The *board pack content* is owned by the CFO; the *board pack choreography* is co-owned by the CoS and corporate secretary. mod-114 owns the rhythm that produces the raw material.

### Executive-team operating substrate

- The **E-team weekly meeting**, the **CEO-executive 1:1 cadence**, the **quarterly executive-team offsite**, the **annual 360**, the **executive-onboarding programme**. See [chapter 09](./09-executive-team-operating-rhythm.md).
- The **executive-conflict-management** pattern (Lencioni / Horowitz canon).
- The **CoS's role in the operating relationship** with the CEO. See [chapter 08](./08-ceo-cos-or-coo-operating-relationship.md).

The *comp-committee annual review* of executives is owned by the comp committee ([mod-105](../mod-105-equity-compensation-policy-and-comp-committee/)). The *CEO succession plan* is owned by the board ([mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/)). mod-114 owns the week-to-week executive-team mechanics.

### Organisational-evolution framing

- The **stage-model framing** of operating decisions — Greiner, Adizes, Scaling Up / Rockefeller Habits, OKRs canon. See [chapter 07](./07-scaling-up-greiner-adizes-org-evolution.md).
- The **adjustment of the operating rhythm to the stage** of the company.

## What mod-114 hands off to sibling modules

### To mod-101 — Legal Entity Formation & Corporate Structure

- **Delaware C-corp substrate, officer-authority framework, board resolutions.** The corporate basis under which mod-114's operating decisions are taken.
- **Officer appointments.** The COO is a corporate officer; the appointment is a mod-101 artifact.

### To mod-102 — Founding Team Legal Architecture

- **Founder-side legal architecture** — founder vesting, co-founder agreements, founder-level IP assignment. Pre-dates the operations-function design.

### To mod-103 — Employment Law & Contract Design

- **The US employment-contract substrate** — at-will, arbitration, PIIA, DTSA notice, non-compete / non-solicit state variance. The legal substrate for every mod-114 hire.
- **Employment-contract templates** for the ten ops hires in [chapter 02](./02-first-ten-ops-hires-and-comp-benchmarks.md).

### To mod-104 — Hiring, Onboarding & HR Operations

- **The hiring machinery and HRIS / ATS stack.** The infrastructure the ops hires run through.
- **The onboarding workflow** for every new hire. The 100-day executive-onboarding programme ([chapter 09](./09-executive-team-operating-rhythm.md)) sits on top of this baseline.
- **The I-9 / E-Verify operational substance.**
- **The specific HRIS and ATS systems-selection decisions.** mod-114 provides the meta-framework ([chapter 03](./03-systems-selection-meta-framework.md)); mod-104 makes the specific call.

### To mod-105 — Equity Compensation Policy & Comp Committee

- **The US equity-incentive plan and the comp-committee cadence.** Executive-comp decisions and the compensation-committee interaction.
- **The annual executive-performance review** led by the comp committee. mod-114's 360 feeds into it ([chapter 09](./09-executive-team-operating-rhythm.md)).
- **The CEO's own compensation decisions and the CEO succession planning.**

### To mod-106 — Compensation Architecture & Total Rewards

- **The US compensation architecture — job architecture, levelling, pay bands, geographic differentials.**
- **The specific comp-benchmark offer placement.** mod-114 ([chapter 02](./02-first-ten-ops-hires-and-comp-benchmarks.md)) names the market bands for the ten ops seats; mod-106 translates those into company offers through the comp architecture.

### To mod-107 — Performance, Promotion & Offboarding

- **The US performance-management calendar, the promotion cycle, the offboarding playbook.** The infrastructure mod-114's executive-team rhythm interlocks with.
- **Executive offboarding** (an executive departure, including the comms, the severance, the transition). Comp architecture is mod-105/106; the specific exit playbook is mod-107.

### To mod-108 — Culture, Employee Experience & DEI

- **The employee handbook, the hybrid / RTO policy, the internal-communications architecture, the AI-usage policy, the acceptable-use policy, the engagement-survey programme, the DEI programme.**
- **The workplace *policy* layer.** mod-114 owns the workplace operations ([chapter 04](./04-workplace-and-real-estate-progression.md)); mod-108 owns the policy that drives the demand pattern.

### To mod-109 — Commercial Contracts, IP & Legal Ops

- **The customer and vendor contract suite** — MSA, DPA, SLA, IP protection strategy, OSS / SBOM programme, CLM stack.
- **The commercial-contract templates** that run through the mod-114 procurement motion.
- **The CLM systems-selection decision.** mod-114 provides the meta-framework; mod-109 makes the specific call.
- **The GC's legal review** of every mod-114 vendor purchase, lease, and system contract.

### To mod-110 — Privacy, Data Governance & Sector Compliance

- **The US-side privacy programme and the substantive GDPR regulatory analysis.** The DPA templates, the sub-processor register, the Record of Processing Activities (RoPA), the DSAR workflow.
- **The privacy-platform systems-selection decision** (OneTrust / Transcend / DataGrail / Osano). mod-114 provides the meta-framework; mod-110 makes the specific call.
- **The privacy review of every mod-114 vendor purchase** touching customer / employee personal data.

### To mod-111 — Corporate Governance, Board Operations & Officer Duties

- **The board composition, D&O indemnification agreements, officer-authority framework, NVCA financing suite.** The governance substrate.
- **The board cadence, the board pack, the board resolutions, the board minutes.** mod-114's CoS partners with the corporate secretary on the choreography ([chapter 08](./08-ceo-cos-or-coo-operating-relationship.md)); the content and the corporate record are mod-111.
- **The board portal systems-selection decision.** mod-114 provides the meta-framework; mod-111 makes the specific call.
- **The delegation-of-authority policy** that frames mod-114's approval-authority matrix ([chapter 05](./05-procurement-operating-model.md)).

### To mod-112 — Enterprise Risk, Insurance & Compliance

- **The US-parent insurance programme (cyber, tech-E&O, D&O, EPLI, general liability).**
- **The FCPA / sanctions / export-controls programme substance.** The screening checks that run on new vendors are coordinated with mod-112.
- **The security programme substance** — SOC 2, ISO 27001, security review of vendors. mod-114's procurement engages mod-112's security function for the review.
- **The GRC platform systems-selection decision.** mod-114 provides the meta-framework; mod-112 makes the specific call.

### To mod-113 — International Expansion & Global Workforce

- **The international-expansion overlay** — EOR / direct-entity decision, the first-entity setup, intercompany and transfer pricing, the US immigration programme, international employment-law variance, international benefits / equity, international privacy, international workforce reduction.
- **The international ops lead seat** ([chapter 02 Seat 9](./02-first-ten-ops-hires-and-comp-benchmarks.md)) runs the international operations against mod-113's framework.
- **International workplace decisions** (opening a spoke office in London, Berlin, Toronto). The mod-114 workplace progression applies locally; mod-113 provides the entity and employment-law substrate.

### To startup-finance-fundraising-curriculum (adjacent track)

- **The CFO function substance** — accounting, controllership, FP&A, treasury, tax, financial systems, month-end close, audit, fundraising execution.
- **The ERP, GL, AP, expense-management systems-selection decisions.** mod-114 provides the meta-framework; the finance curriculum makes the specific call.
- **The monthly close cycle** that gates the MBR in [chapter 06](./06-operating-cadence-and-okrs-rhythm.md).
- **The board pack financial content** that the CFO authors and the CoS choreographs around.
- **The strategic finance function** (if housed in Finance rather than BizOps) — mod-114 names the placement question in [chapter 01](./01-coo-vs-cos-and-bizops-org-design.md); the finance curriculum authors the function. <!-- needs-research: verify the exact chapter paths in startup-finance-fundraising-curriculum mod-111 for the monthly close cycle, FP&A function, and strategic finance chapters that this module cross-references. -->

### To startup-product-gtm-curriculum (adjacent track)

- **The GTM organisation design** — CRO / VP Sales / VP Marketing / VP CS seats, sales operations, revenue operations, marketing operations.
- **The GTM-ops / rev-ops function design.** The analytical layer for the commercial engine, often adjacent to or integrated with BizOps.
- **The product-ops function design.** The analytical layer for the product organisation.

mod-114 owns the *corporate* operations function; the product-and-gtm curriculum owns the *commercial* operations functions. The two coordinate at the executive-team level and at the operating-cadence level.

## What mod-114 defers to specialist advisors

Operations is a boundary function; some of its decisions require specialist expertise.

### Executive-coaching and team-coaching firms

- **For the quarterly offsite** at growth stage — The Table Group (Lencioni's firm), ghSMART, independent executive-team coaches.
- **For the annual 360** at growth stage — specialist 360 vendors or coach-run programmes.
- **For the CEO's own coaching** — Reboot.io, independent CEO coaches, specialist firms.

<!-- needs-research: verify the current market positioning of The Table Group, ghSMART, Reboot.io and comparable firms in 2026 for executive-team coaching, 360 programmes, and CEO coaching. -->

### Tenant-representation firms

- **CBRE, JLL, Cushman & Wakefield, Newmark, Colliers, Savills, Cresa, Avison Young.** See [chapter 04](./04-workplace-and-real-estate-progression.md).

### Real-estate counsel

- Retained under GC oversight for lease-document negotiation. Common names in US markets: specialised commercial real-estate counsel at the AmLaw 100 firms, boutique real-estate practices.

### Procurement specialist firms

- **Vendr, Sastrify** and comparable SaaS-specific procurement firms. Can be retained for negotiation on specific vendor renewals, or as fractional procurement capacity before a full-time Head of Procurement.
- **Spend-management / FinOps consultancies** for cloud-cost optimisation (AWS, GCP, Azure) — a specialist adjacent to procurement.

### Business-systems implementation partners

- **Workday HCM implementation** — Deloitte, Accenture, Alight, IBM, Collaborative Solutions, Kainos, or Workday-specialised boutiques.
- **NetSuite / ERP implementation** — equivalent partner ecosystem.
- **Salesforce implementation** — equivalent partner ecosystem.
- **IT and MDM implementation** — Managed Service Providers (Electric, ExpressIT) and specialist consultancies.

### Executive-search firms

- For executive hires — Heidrick & Struggles, Spencer Stuart, Russell Reynolds, Egon Zehnder, Korn Ferry at the senior end; specialist startup-focused firms (True Search, Daversa, Riviera Partners, Thrive Partners for operating roles).

<!-- needs-research: verify the current executive-search landscape and specialist startup-focused firms in 2026. -->

### Fractional / interim executives

- **Fractional CoS, fractional COO, fractional Head of Workplace, fractional Head of Procurement** — bridge options before full-time hires per [chapter 02](./02-first-ten-ops-hires-and-comp-benchmarks.md). Multiple firms and independent practices offer fractional operators.

### Workplace-experience and facilities-vendor ecosystems

- **Food service, janitorial, security, A/V, mail services, reception.** Local or national vendors engaged under the Head of Workplace's management.

### Insurance brokers (via mod-112)

- **The insurance programme** is mod-112's territory; mod-114 coordinates with the broker on insurance implications of lease signings (property insurance), vendor contracts (certificates of insurance), and executive hires (D&O coverage changes).

## The six worked examples

The boundary becomes clearest in specific contested cases. Six representative examples:

### Worked example 1 — The HRIS migration

**Question.** The company is at 180 employees, outgrowing Rippling. A migration to Workday HCM is proposed. Who owns the decision?

**Answer.** The *CPO owns the decision* on which HRIS to adopt (mod-104). The *COO / CoS owns the migration meta-framework* — the systems-selection buying criteria ([chapter 03](./03-systems-selection-meta-framework.md)), the change-management pattern, the executive sponsor role for the migration programme. The *Head of Business Systems owns the technical implementation* — integration architecture, data migration, SSO/SCIM provisioning. The *CFO* is a stakeholder on TCO and on the finance-systems integration (HRIS ↔ payroll ↔ GL). The *GC* reviews the MSA, DPA, security addendum. The *security function* (mod-112) reviews the vendor security posture.

mod-114 does not pick Workday; mod-114 ensures the decision is picked through a defensible meta-framework.

### Worked example 2 — The hybrid / RTO policy change

**Question.** The company announces a shift from remote-first to hybrid-anchored (3 days in office). Who owns the decision and the operational cascade?

**Answer.** The *CPO owns the policy* (mod-108). The *COO / Head of Workplace owns the operational cascade* — the workplace footprint sized to the new peak-day attendance, the facilities services scaled up, the hybrid-day scheduling, the executive-team RTO modelling ([chapter 04](./04-workplace-and-real-estate-progression.md)). The *CoS owns the executive-team coordination* — the comms sequencing, the executive-team alignment on how to live the policy, the operating cadence that enforces it. The *GC* reviews the policy for employment-law compliance (mod-103). The *CPO + People's internal-communications team* run the workforce comms.

mod-114 does not author the policy; mod-114 operationalises it.

### Worked example 3 — The $300k vendor renewal

**Question.** A $300k/year CLM renewal is up. The GC's team wants to switch to a different vendor. Who decides and what are the gates?

**Answer.** The *GC owns the specific vendor decision* (mod-109) — which CLM best serves the legal operations. The *Head of Procurement* (mod-114 [chapter 05](./05-procurement-operating-model.md)) runs the commercial motion — the RFP, the negotiation, the renewal / termination mechanics against the renewal calendar. The *CFO* approves the spend commitment per the approval-authority matrix (the $300k lands in the CFO/COO approval bracket). The *security function* (mod-112) reviews the vendor security posture. The *GC's own team* reviews the MSA / DPA.

mod-114 provides the procurement discipline and the systems-selection meta-framework; mod-114 does not pick the CLM.

### Worked example 4 — The $12M direct lease signing

**Question.** The company is signing its first long-term hub lease — 25,000 sqft, 5-year term, $12M total obligation. Who decides and what are the gates?

**Answer.** The *CEO / COO owns the strategic decision* — commit to the city, commit to the term. The *Head of Workplace owns the operational selection* ([chapter 04](./04-workplace-and-real-estate-progression.md)) — the tenant-rep firm engagement, the submarket survey, the shortlist, the RFP, the TI negotiation. The *CFO* approves the capital commitment per the approval-authority matrix (the $12M lands in the board-approval bracket or near it) — and runs the balance-sheet (ASC 842 right-of-use asset / lease liability) treatment. The *GC + retained real-estate counsel* review and negotiate the lease document. The *Board* approves the commitment per the delegation-of-authority policy. The *CPO* coordinates on the RTO policy / peak-day attendance sizing.

mod-114 owns the operational selection; the final capital commitment runs through the full cross-functional / board apparatus.

### Worked example 5 — The new executive onboarding

**Question.** A new CRO is landing. Who owns the onboarding programme?

**Answer.** The *CEO owns the integration* — the first-day welcome, the 1:1 cadence, the executive-team integration, the explicit scope of the first 100 days. The *CoS owns the operational onboarding* ([chapter 09](./09-executive-team-operating-rhythm.md)) — the briefing packet (co-authored with the CPO), the listening-tour scheduling, the operating-cadence immersion, the 100-day review mechanics. The *CPO* owns the HR substance — HRIS onboarding, benefits enrollment, equity grant finalisation, compensation discussions. The *VP of Sales / VP of CS (CRO's directs)* are briefed and prepared for their new leader. The *GC* reviews any carryover restrictions (non-compete, non-solicit from prior employer).

mod-114 owns the executive-team integration; mod-104 / mod-106 own the HR substance.

### Worked example 6 — The sanctions screening on a new international vendor

**Question.** Procurement is about to engage a new vendor based in a jurisdiction that triggers an OFAC / sanctions concern. Who decides and what are the gates?

**Answer.** The *Head of Procurement* (mod-114 [chapter 05](./05-procurement-operating-model.md)) flags the issue as part of the vendor-diligence checklist. The *sanctions / export-controls function* (mod-112 chapter 04) runs the screening — OFAC / SDN / consolidated-list check, due diligence on ultimate beneficial ownership, review against any applicable export-control triggers. The *GC* reviews the legal exposure. The *CFO* ratifies the commitment or declines, informed by the sanctions review. The *Board* is notified if the vendor relationship implicates a material enterprise risk (mod-111).

mod-114 does not run the sanctions screening; mod-114 ensures the diligence checklist routes the question to the function that does.

## When the boundary is contested

Three patterns recur:

### Pattern 1 — Scope creep

**Shape.** Something nobody else wants (a cross-cutting administrative function, a one-off project, a legacy ownership of a long-forgotten system) accretes to operations because operations has the lightest "no." Over time operations' scope sprawls; nothing is owned deeply.

**Fix.** The CoS / COO treats scope creep as a strategic risk. New ownership asks get the "is this ops's work?" question explicitly. If the answer is "no one else will own it," the next question is "should it exist?" — not "can we add it to the ops backlog?"

### Pattern 2 — Scope leakage

**Shape.** Something that should be operations's (a cross-functional coordinating mechanism, an operating-cadence discipline, a vendor-management function) ends up in a sibling function because operations is not confident enough to claim it. Months later the sibling function hands it back half-baked.

**Fix.** The CoS / COO reclaims it explicitly. "We are now the owner of X. We will integrate it into the operating cadence by date Y."

### Pattern 3 — Interface failure

**Shape.** Operations and a sibling function (People, Finance, Legal, IT) both believe the other owns the specific decision. Decisions fall through the gap.

**Fix.** The CoS / COO authors an explicit RACI with the sibling function and ratifies it with the owning executive. The example-6-style worked examples above are a template.

## The boundary tested at diligence

A Series-C or growth-stage diligence package tests the boundary. The diligence lead asks:

- **"Who owns your operating cadence?"** The CoS / COO names it. The weekly ops review, the monthly business review, the quarterly OKRs cycle, the annual planning — all show up on a single operating calendar.
- **"Who owns your systems architecture?"** The Head of Business Systems names it. The HRIS, ATS, CLM, spend management, procurement, IT-and-endpoint systems are catalogued with their owners and renewal dates.
- **"Who owns your workplace footprint?"** The Head of Workplace names it. The leases and the renewal dates and the sublease rights are catalogued.
- **"Who owns your vendor list?"** The Head of Procurement names it. The spend taxonomy, the vendor count by category, the renewal calendar are all visible.
- **"Who owns your approval-authority matrix?"** The CoS / COO names it, and it reconciles with the delegation-of-authority policy at the board level (mod-111).

A diligence lead who gets consistent, named-owner answers across those questions concludes the ops function is real. A diligence lead who gets different answers from different people concludes the ops function is immature — regardless of how many ops hires are on the payroll.

## Summary

- mod-114 owns the **operations-function design, systems-selection meta-framework, workplace, procurement, operating cadence, executive-team rhythm**. It defers to sibling modules and specialist advisors for the specific function-level content.
- The **hand-off map** names what belongs where — mod-101 / 102 (corporate substrate), mod-103 (US employment-contract substrate), mod-104 (HR operations), mod-105 / 106 (comp and equity), mod-107 (performance / offboarding), mod-108 (culture / policy), mod-109 (contracts / IP), mod-110 (privacy), mod-111 (governance / board), mod-112 (risk / insurance / security / sanctions), mod-113 (international), and the finance-fundraising / product-gtm curricula for the adjacent-track handoffs.
- **Specialist advisors** carry the external edges — executive-coaching firms, tenant-rep firms, real-estate counsel, procurement firms, business-systems implementation partners, executive-search firms, fractional operators, workplace-vendor ecosystems.
- The **six worked examples** make the boundary concrete — HRIS migration, RTO policy change, CLM renewal, direct-lease signing, executive onboarding, sanctions screening.
- The three recurrent failure patterns are **scope creep, scope leakage, and interface failure.** Each is a known pathology with a known fix.
- The **diligence test** of the boundary is whether every operating function has a named owner, a single canonical calendar / register / taxonomy, and consistent cross-executive answers to the "who owns X?" question.
