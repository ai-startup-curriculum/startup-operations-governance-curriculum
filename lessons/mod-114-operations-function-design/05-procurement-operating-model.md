# 5. Procurement operating model and tooling

> Every scale-up quietly builds a shadow procurement function — some engineer buying a SaaS tool on their corporate card, some department head signing an MSA without legal review, some CFO writing a check to a vendor nobody else knows about. The choice is between running procurement as a real function or continuing to run it as an accident.

## Motivation

A scale-up at 200 employees typically has 75+ SaaS vendors, another 25+ non-SaaS third-party services (professional services, workplace, travel, contractors), and an annualised third-party spend of US$5–15M. At 500 employees the numbers are 150+ vendors and US$20–50M. Left unmanaged, this spend is:

- **Fragmented** — the same tool is bought three times by three different teams under different accounts.
- **Under-negotiated** — nobody has ever pushed back on a renewal quote.
- **Over-authorised** — spend commitments happen without anyone but the buyer knowing.
- **Under-diligence-d** — vendors are onboarded with no security, privacy, or IP review.
- **Un-tracked** — renewal dates are on individual buyers' calendars, and auto-renew clauses fire silently.
- **Un-consolidated** — three overlapping analytics tools sit in three departments.

The procurement operating model is the antidote. A well-run procurement function typically **saves 8–15% of controllable third-party spend** through consolidation, negotiation, and renewal discipline — a meaningful multiple of the fully-loaded cost of the Head of Procurement seat ([chapter 02](./02-first-ten-ops-hires-and-comp-benchmarks.md)). <!-- needs-research: verify the 8–15% controllable-spend savings benchmark from Gartner / Forrester / Vendr / Sastrify studies of SaaS procurement engagements — the figure is widely cited in vendor collateral and specific studies should be located and cited. -->

This chapter authors the operating model: spend taxonomy, approval-authority matrix, annual vendor review, consolidation playbook, tooling stack (Ramp / Brex / Spendesk / Airbase / Coupa and the SaaS-specific tools around them), and the coordination with the CFO's finance-ops function owned by the finance-fundraising curriculum.

## The spend taxonomy

Procurement's first act on the job is to publish a **spend taxonomy** — a canonical categorisation of third-party spend that every stakeholder agrees to use. Finance uses it in the GL. Procurement uses it to organise the vendor list. The COO uses it in the operating cadence. Without a shared taxonomy, every spend conversation restarts from zero.

A workable seven-category taxonomy for a venture-backed scale-up:

1. **SaaS software.** Subscription software the company runs its business on. Sub-categorised by function: engineering & infrastructure; sales & marketing; people & HR; finance & accounting; legal & compliance; security; internal / employee productivity. The largest single category by vendor count and often the fastest-growing by spend.
2. **Professional services.** Legal (outside counsel), accounting (auditor, tax), management consulting, executive search, PR / IR, specialised advisors (comp advisor, tax advisor, real-estate counsel). Typically 20–40 vendors, high per-vendor spend.
3. **Workplace.** Rent, utilities, common-area maintenance (CAM), janitorial, food service, security, mail, furniture, on-site A/V, workplace-experience programme (see [chapter 04](./04-workplace-and-real-estate-progression.md)). Dominated by rent as the single largest line.
4. **IT and equipment.** Laptops (Apple, Dell, Lenovo), monitors, peripherals, MDM subscriptions, endpoint security, network equipment, colocation or cloud infrastructure (a large category on its own that often gets its own sub-taxonomy). Coordinated with the Head of Business Systems ([chapter 03](./03-systems-selection-meta-framework.md)).
5. **Travel and expense.** Air, hotel, ground transport, corporate cards, per-diems, entertainment. Typically routed through a corporate-travel platform (Navan / TripActions, TravelPerk, Ramp Travel, or a traditional TMC like BCD / American Express Global Business Travel / CWT) with policy enforced at booking. <!-- needs-research: verify current corporate-travel-platform positioning and the T&E-spend benchmark distributions for venture-backed scale-ups in 2026. -->
6. **Marketing.** Media (digital, out-of-home, PR), events (booths, sponsorships, hosted events), agencies (creative, PR, growth), swag and merchandise, gifting programmes.
7. **R&D infrastructure.** Cloud (AWS, GCP, Azure, Oracle, specialised clouds), data (Snowflake, Databricks, BigQuery), observability (Datadog, New Relic, Splunk, Honeycomb, Grafana Cloud), CI/CD (GitHub Enterprise, CircleCI, Buildkite), specialised infra (Kubernetes-adjacent, ML-training compute, GPU capacity). Often the fastest-growing spend line at an AI-infrastructure or data-intensive company; often has its own dedicated FinOps / cloud-cost-optimisation seat separate from generalist procurement.

Each vendor is tagged to exactly one primary category. Multi-purpose vendors (Rippling, for example, which spans HRIS + IT + spend) get a primary category tag and secondary tags for the auxiliary functions.

## The approval-authority matrix

The approval-authority matrix is the corporation's answer to "who can commit the company to spend, up to what amount, without whose sign-off?" It is a **board-approved policy** at some level (typically an entry in the board-approved delegation-of-authority policy — see [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/)) and it is enforced through the procurement and spend-management tools.

### A representative approval-authority matrix

Illustrative for a Series-B–C venture-backed scale-up. Specifics vary by stage, industry, and the CFO's / COO's / board's risk posture.

| Spend commitment (annualised) | Approval required | Additional gates |
|---|---|---|
| Up to US$1,000 | Individual, on corporate card | None (per corporate-card policy) |
| US$1,000 – US$5,000 | Manager | None |
| US$5,000 – US$25,000 | Department head (VP-level) | None |
| US$25,000 – US$100,000 | Department head + Procurement + Finance | Vendor security + privacy review; GC review of MSA / DPA |
| US$100,000 – US$500,000 | + CFO or COO | + Board notification via monthly report |
| US$500,000 – US$2,500,000 | + CEO | + Board notification |
| Above US$2,500,000 | + Board approval (or specific committee) | Delegation-of-authority policy specifies which decisions are board-reserved |

**Multi-year commitments** apply the matrix against the **total contract value (TCV)**, not the annualised amount — a US$60k / year for 3 years contract lands in the US$100k–500k bracket, not the US$25k–100k one.

**Renewals** run through the same matrix — a renewal is a new commitment, even if the vendor is incumbent. The failure mode is treating renewals as invisible and letting them auto-renew without a decision.

### Where the matrix breaks

- **The "single-user seat" workaround.** Someone buys a $99/month tool on their card. Two years later 40 engineers are on it, spending US$50k/year, and nobody ran the security review. Fix: SaaS-discovery tooling (below) catches the unmanaged sprawl; a policy that any tool with more than N seats or any tool storing customer / employee / financial data goes through procurement regardless of monthly spend closes the loophole.
- **Circumventing procurement through professional-services POs.** A vendor is dressed up as "consulting" to route around SaaS procurement discipline. Fix: professional-services POs run through the same MSA / DPA gates, and the taxonomy category is set by procurement based on the substance of the deliverable, not the invoice label.
- **CEO / COO carve-outs.** The CEO signs a $150k tool they personally like without procurement review. Fix: the CEO and COO are subject to the matrix; the corporate-secretary function ([mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/)) tracks the delegation-of-authority policy and reports out-of-policy commitments to the board / audit committee.

## The annual vendor review cadence

Procurement runs an **annual vendor review** on the top N vendors by spend and on every vendor with a renewal in the following 12 months. The review answers:

1. **Do we still need it?** Utilisation data from the tool itself (seat activity, workflow completion, API call volume) is the truth here. A tool that shows sub-25% seat activity is a candidate for consolidation, downgrade, or elimination.
2. **Is there a better alternative?** Category re-scan — new entrants, consolidated offerings, incumbent competitors. This is where the systems-selection meta-framework from [chapter 03](./03-systems-selection-meta-framework.md) re-runs.
3. **Is the price right?** Benchmark against category peers (Vendr / Sastrify / Zip / Zluri publish or provide benchmarks); against the company's own prior renewal cycles; against comparable-size peer companies (via network exchange or via the procurement-tool marketplaces).
4. **Is the contract right?** Term length, payment terms, auto-renewal notice, data-export terms, security addendum currency (SOC 2 report refresh), DPA currency (privacy-regulation updates), MSA currency (indemnification, LoL, IP).
5. **Is the vendor healthy?** For smaller vendors, funding runway; for larger vendors, product roadmap and roadmap fit; for public-company vendors, financial disclosure.

### The renewal calendar as an operating artifact

The single most-leveraged procurement artifact is a **renewal calendar** — a single canonical list of every vendor's next renewal date, the required termination-notice deadline (typically 60–90 days before renewal), and the owner of the renewal decision.

Every renewal that arrives with a 60-day notice window and no prep landed with a diminished negotiating position — the incumbent knows you cannot easily switch. Every renewal that arrives with 6 months of prep, a benchmark, and a credible alternative on the shortlist lands 10–25% under the incumbent's opening quote. The difference is entirely the renewal calendar.

The renewal calendar is owned by procurement, populated from every executed contract, and reviewed monthly at the procurement operating meeting.

## The vendor-consolidation playbook

Consolidation is the highest-leverage procurement work. The playbook:

1. **Discover the sprawl.** Use SaaS-discovery tooling (Zluri, Torii, Torii's category peers, or the spend-management tool's discovery module) to enumerate every SaaS subscription paid by any corporate card or invoice. Expected finding: 30–50% more SaaS than the leadership team thought existed.
2. **Categorise against the taxonomy.** Every discovered tool gets tagged to a primary category and sub-category.
3. **Identify overlap.** Two or more tools in the same sub-category serving overlapping workflows. Common patterns: three project-management tools (Asana / Notion / Linear); two documentation tools (Confluence / Notion); two design tools (Figma / Sketch); two customer-support tools (Zendesk / Intercom); two BI tools (Looker / Tableau / Mode). Overlap is not always bad — different teams may legitimately need different tools — but every overlap should be an explicit choice, not an accident.
4. **Author the consolidation proposal.** For each overlap, propose the consolidation target (which tool stays), the transition plan (migration timeline, data movement, retraining), and the projected savings.
5. **Get the department head to own it.** Consolidation is unpopular with the team that has to switch tools. It has to be sponsored by the department head, not imposed by procurement. Procurement provides the data and the plan; the department head owns the decision and the change.
6. **Track the savings.** The savings number goes into the procurement quarterly report. It is a real metric with a real target; treat it as such.

## The tooling stack — corporate card, invoice, and PO split

Procurement's tooling stack has three primary payment / control patterns, each with its own tooling:

### Corporate card

For low-value, high-frequency spend. Every employee (or every department) has a corporate card with a limit set by policy. Modern corporate-card platforms — **Ramp, Brex, Rho, Mercury Cards** — layer spend controls (per-card limits, per-vendor limits, category restrictions), receipt capture, GL coding, and reconciliation on top of the card itself. Older-generation options (Amex Business Platinum, Bank of America commercial cards) exist but have weaker software.

Corporate-card platforms have consolidated toward integrated spend-management platforms (Ramp, Brex, and Rho all now offer corporate card + expense + bill pay + procurement); the choice is often between an integrated stack (one vendor for everything) or a best-of-breed stack (card from one, expense from another, procurement from a third).

<!-- needs-research: verify current market positioning for Ramp, Brex, Rho, Mercury, and the traditional corporate-card providers in 2026, including their integrated-platform vs. point-product evolution. -->

### Invoice (bill pay)

For mid-value, mid-frequency spend where the vendor issues an invoice. Vendors invoice the company; the AP team codes the invoice, matches it against the approval, and pays via ACH / wire / check. Tooling: **Bill (formerly Bill.com), Ramp Bill Pay, Brex Bill Pay, Airbase Bill Pay, Tipalti (multi-currency, larger scale), Melio, Rho Bill Pay.** Enterprise AP platforms (Coupa Pay, SAP Ariba Payables, Oracle Fusion Payables) apply at enterprise scale.

Invoice-based spend often carries a **payment-terms** conversation — 30-day / 45-day / 60-day terms are the standard levers; early-payment discounts (2/10 net 30 — 2% discount if paid within 10 days) are worth taking at scale.

### Purchase order (PO)

For high-value, high-formality spend where the company issues a purchase order **before** the vendor delivers. The PO is a commitment; the vendor invoices against the PO; AP performs a **three-way match** (PO + goods receipt + invoice) before paying. Tooling: **Spendesk, Airbase, Ramp Procurement, Zip, Approve, ProcurementFlow, Vendr, Sastrify**; enterprise tools (Coupa, SAP Ariba, Oracle Procurement Cloud, Ivalua) for larger organisations.

PO discipline is often required for **SOX-adjacent** or pre-IPO financial controls, for audited financial-statement environments, and for large regulated-customer-facing companies. Below that threshold, many venture-backed scale-ups operate on a card-and-invoice basis with a "PO-if-over-$X" rule.

### The split — what pays for what

A representative split by spend category:

| Category | Primary payment method | Tooling example |
|---|---|---|
| SaaS software (< $10k / year, low risk) | Card | Ramp / Brex card |
| SaaS software (mid- to high-value) | Invoice, PO for high-value | Bill / Ramp Bill Pay + Vendr / Zip for negotiation |
| Professional services | Invoice, PO for defined-scope engagements | Bill / Airbase |
| Workplace (rent) | Invoice / ACH | Bill or direct-bank ACH |
| Workplace (services) | Mix — card and invoice | Ramp / Bill |
| IT and equipment | PO for equipment, invoice for MDM subscriptions | PO tool + Bill |
| Travel and expense | Card, corporate-travel-platform booking | Navan / TripActions + Ramp / Brex |
| Marketing | Card for tactical, invoice / PO for agency retainers | Ramp / Brex + Bill |
| R&D infrastructure | Invoice, monthly usage billing | Bill / Ramp; direct vendor billing for AWS / GCP |

## Coordination with the CFO / finance-ops team

Procurement is a **shared** function between the operations org (this module) and the finance function (owned by the `startup-finance-fundraising-curriculum`). The exact reporting line varies by company — Head of Procurement reports to COO in some orgs, CFO in others — but the coordination surface is the same.

### What operations owns

- **Vendor management and negotiation** — the commercial motion with the vendor, the RFP, the LOI, the negotiation.
- **Consolidation strategy** — the vendor-consolidation playbook (above).
- **Approval workflow design** — the approval-authority matrix (above), enforced through the tooling.
- **Renewal calendar** — the operational discipline of never letting a renewal auto-fire without a decision.
- **Category leadership** — a category lead (SaaS, Professional Services, Workplace) inside procurement responsible for that category's cost and quality.

### What finance owns

- **General ledger coding** — every spend commitment is coded to the GL against the spend taxonomy.
- **Month-end close** — the close cycle owned by the CFO (see the finance-curriculum monthly-close chapter). <!-- needs-research: confirm the exact chapter path in startup-finance-fundraising-curriculum mod-111 for the monthly close cycle chapter. -->
- **Accounts payable execution** — cutting the payment, running the ACH batches, managing bank relationships.
- **Financial reporting** — spend by category in the monthly / quarterly financial reports.
- **Cash management** — the CFO's cash-runway discipline sets the outer bound on committable spend.
- **Compliance** — SOX / SOX-adjacent controls, three-way-match discipline, segregation of duties in the AP workflow.

### The RACI

For a specific vendor purchase over the approval-authority threshold:

| Activity | Requester | Procurement | Finance | GC | Security | Approver |
|---|---|---|---|---|---|---|
| Need identified | R | C | I | I | I | I |
| Vendor shortlist | C | R | I | I | I | I |
| RFP and evaluation | C | R | C | C | C | I |
| Security / privacy review | I | C | I | I | R | I |
| MSA / DPA negotiation | I | C | I | R | C | I |
| Commercial negotiation | I | R | C | C | I | I |
| Approval | I | C | C | I | I | R |
| Invoice / payment | I | C | R | I | I | I |
| Renewal review | C | R | C | C | C | I |

## The vendor-diligence checklist

For any vendor over the approval-authority threshold, procurement runs a diligence checklist before contract execution:

- **Corporate identity** — legal entity name, jurisdiction of formation, D&B / Duns number, business address.
- **Financial viability** — for larger commitments to smaller vendors, evidence of funding runway or profitability.
- **References** — 2–3 customer references, called by procurement or the requester.
- **Security posture** — SOC 2 Type II report, ISO 27001 if applicable, penetration-test summary, data-encryption posture.
- **Privacy posture** — DPA, sub-processor list, cross-border transfer mechanism (SCCs / IDTA / DPF), data-residency options if needed.
- **IP posture** — the vendor's assignments-of-IP language in the MSA; the customer-IP protection language; the vendor's own IP-warranty language.
- **Sanctions / export-controls screening** — OFAC / SDN / consolidated screening list check against the vendor entity and ultimate beneficial owner. Coordinated with [mod-112 chapter 04](../mod-112-enterprise-risk-insurance-and-compliance/04-sanctions-and-export-controls-compliance-programme.md).
- **Insurance** — the vendor's cyber insurance, errors-and-omissions insurance, and general liability insurance where relevant.
- **Certificate of insurance** — where the vendor accesses the company's premises or systems, request a certificate of insurance naming the company as additional insured.

## Concrete example — Series-B SaaS procurement build-out

**Company:** Series-B B2B SaaS, 180 employees, ~US$8M annualised third-party spend across 90+ SaaS vendors, 25+ professional-services vendors, workplace + IT + travel + marketing.

**State at the start:** No dedicated procurement seat. CFO's controller handles AP; department heads sign their own contracts; the GC reviews MSAs when asked; auto-renewals fire silently; SaaS-tool sprawl is visible but unmeasured.

**Ninety-day build-out plan:**

- **Days 1–15.** Hire the Head of Procurement. Publish the spend taxonomy. Deploy a SaaS-discovery tool (Zluri, Torii, or the spend-management platform's built-in discovery) and inventory every SaaS subscription. Expected finding: 30–40% more vendors than the leadership team knew about.
- **Days 15–30.** Publish the approval-authority matrix, ratified by the board (audit committee if one exists). Configure the spend-management platform (Ramp / Brex / Airbase) to enforce the matrix at card-issuance and bill-pay stages. Roll out the vendor-diligence checklist for any new vendor over $25k / year.
- **Days 30–60.** Build the renewal calendar. Every executed contract goes into the CLM ([mod-109](../mod-109-commercial-contracts-ip-and-legal-ops/)) with its renewal date and termination-notice deadline. Diarise every notice deadline in the procurement calendar.
- **Days 60–90.** Author the first vendor-consolidation proposal. Target: 3–5 overlaps with a combined US$300–500k annualised savings. Sponsor with the relevant department heads. Execute the first 2–3 consolidations in the next quarter.
- **First-year outcomes.** Procurement discipline in place. 5–10 renewals negotiated at 10–20% under incumbent quotes. 3–5 consolidations executed. Vendor diligence a routine, not an exception. Auto-renewal misses down to zero. Total cost of the Head of Procurement seat: US$250–350k fully loaded; realised savings in Year 1: US$800k–1.5M. Positive ROI in the first quarter.

## Common failure modes

- **No spend taxonomy.** Every spend conversation restarts because there is no shared vocabulary. Fix: publish the taxonomy first.
- **Approval matrix un-enforced.** The matrix exists on paper; the tools do not enforce it; department heads route around it. Fix: encode the matrix in the spend-management platform so it enforces at card-issuance and bill-pay.
- **Renewal calendar in a spreadsheet nobody reads.** The calendar exists but the deadlines slip. Fix: monthly renewal-review meeting; renewal-owner assignment for every vendor; notice-deadline alerts.
- **Consolidation imposed rather than sponsored.** Procurement announces a consolidation; the affected team ignores it; the tools stay. Fix: department head sponsors the consolidation; procurement provides data and plan.
- **Vendor-diligence checklist skipped for small vendors.** A $5k / year tool with access to customer data has no security review; a breach at the vendor is the company's incident. Fix: security review is a function of data sensitivity, not spend threshold.
- **Card-only spend with no controls.** Every employee has an unlimited corporate card; SaaS sprawl explodes. Fix: per-card limits, per-vendor limits, category restrictions, mandatory receipt capture.
- **PO discipline collapses at audit time.** SOX-adjacent controls exist on paper; three-way match is skipped in practice; the auditor writes a finding. Fix: PO tool integrated with AP; three-way match enforced at payment.

## Summary

- **Spend taxonomy** first — SaaS, Professional Services, Workplace, IT and Equipment, Travel and Expense, Marketing, R&D Infrastructure. Every vendor tagged. Every spend conversation uses it.
- **Approval-authority matrix** — board-approved, encoded in the tooling, applies to TCV not annualised, applies to renewals not just new contracts, applies to CEO / COO not just ICs.
- **Annual vendor review** — utilisation, alternative, price, contract, health. Renewal calendar is the single most-leveraged procurement artifact.
- **Vendor-consolidation playbook** — discover sprawl, categorise, identify overlap, propose target, sponsor with department head, track savings.
- **Tooling stack** splits into corporate card (Ramp, Brex, Rho for low-value high-frequency), invoice / bill pay (Bill, Ramp Bill Pay, Brex Bill Pay, Airbase, Tipalti for mid-value), and purchase order (Spendesk, Airbase, Zip, Vendr, Sastrify at scale-up; Coupa, Ariba, Oracle at enterprise).
- **Coordination with the CFO** — operations owns vendor management, consolidation, approval workflow, renewal calendar, category leadership; finance owns GL coding, month-end close, AP execution, financial reporting, cash management, compliance.
- **Vendor-diligence checklist** — identity, financial viability, references, security, privacy, IP, sanctions / export, insurance. Runs for every vendor over the approval threshold.
- The **Head of Procurement seat** ([chapter 02](./02-first-ten-ops-hires-and-comp-benchmarks.md)) typically earns 3–5× its fully-loaded cost in Year 1 through consolidation and renewal-negotiation discipline.
