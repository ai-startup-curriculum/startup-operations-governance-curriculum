# 1. The customer contract suite: MSA, SLA, DPA, Security Addendum, AUP

> A B2B SaaS deal is not one contract. It is a bundle of six documents that reference each other, each of which was separated from the others for a specific reason of reuse, redline surface, or regulatory drift.

## Motivation

An enterprise customer that signs a B2B SaaS deal is not signing "a contract." The customer is signing a stack — an MSA, one or more Order Forms, an SLA, a Data Processing Addendum, a Security Addendum (often responsive to a Shared Assessments SIG-lite), and an Acceptable Use Policy. The stack is what a Fortune-500 procurement team expects to receive on first ask, and the corporation that ships fewer documents than that will be sent a procurement template to sign instead — with worse terms and a longer redline cycle.

The bundle exists in six documents rather than one because each document serves a different reuse and redline pattern. The MSA is a long, heavily-negotiated document that both sides want to sign *once* and reuse across every subsequent deal. The Order Form is a short pricing-and-scope document that changes every renewal and every add-on purchase. The SLA is an operations document owned by the reliability team and updated when the platform's actual reliability posture changes. The DPA is the document that has to be re-papered whenever privacy law moves (new SCCs, new UK IDTA, new US state statute) and it needs to be able to change without re-opening the MSA. The Security Addendum tracks whatever the current security-questionnaire canon is. The AUP is a unilateral document the corporation can update on notice without a counter-signature.

Bundling all of this into one document would (i) force every renewal to re-open the whole thing, (ii) force every regulatory update to re-open the whole thing, (iii) give the counterparty a much larger redline surface on first sign, and (iv) prevent the corporation from reusing the MSA verbatim across deals. The six-document architecture is the practitioner canon for exactly these reasons.

This chapter covers the *architecture* of the bundle — what each document contains, why they are separate, and how they reference each other. [Chapter 02](./02-contract-playbook-and-fallback-position-matrix.md) covers the negotiation playbook — the acceptable / walk-away positions on each clause. [Chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md) covers the mirror-image suite the corporation signs *as a customer of vendors*. DPA regulatory depth (GDPR Art. 28, CCPA service-provider requirements, HIPAA BAA mechanics) is handled in [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/); this chapter treats the DPA structurally as one document in the stack.

## Why six documents instead of one

The three practical reasons the bundle is separated:

1. **Reuse across deals.** The MSA is drafted once by counsel, reviewed on first-sign by the counterparty, and then reused verbatim across every subsequent Order Form the same counterparty signs. A single-document architecture forces every add-on purchase to re-execute the whole contract; the MSA + Order Form split lets a renewal or seat expansion be a one-page Order Form against the existing MSA.
2. **Redline surface control.** A single 60-page contract invites a 60-page redline. Splitting the stack lets the corporation route different documents to different counterparty reviewers (procurement gets the MSA; the security team gets the Security Addendum; the privacy office gets the DPA) and reduces the probability that any one reviewer takes the whole document sideways.
3. **Regulatory and operational drift.** Privacy law and platform reliability posture both change on their own schedules. The DPA can be amended on notice (or under an "updated DPA" mechanic) when the European Commission issues new SCCs — see [Commission Implementing Decision (EU) 2021/914](https://eur-lex.europa.eu/eli/dec_impl/2021/914/oj) — without re-opening the MSA. The SLA can be updated when the platform's SLO posture changes. The AUP can be updated on notice. Bundling these into the MSA forces every regulatory update through a full contract amendment.

The corollary is that the documents need an **order of precedence** clause in the MSA so that the inevitable conflicts between them are resolved deterministically. See the ["Order of precedence"](#order-of-precedence) section below.

## MSA architecture

The Master Services Agreement is the long-form document that governs everything not specific to a particular purchase. The canonical section list:

### Order of precedence

The MSA states which document controls when documents conflict. The common ordering — Order Form > DPA > MSA > SLA > Security Addendum > AUP — reflects that (i) the Order Form is what the parties actually signed most recently and captures the deal-specific economics, (ii) the DPA carries statutory language that cannot be silently overridden by general MSA terms, (iii) the MSA is the general framework, and (iv) the SLA, Security Addendum, and AUP are operational documents. Any deviation from this ordering (some enterprise counterparties push for MSA > Order Form) should be a deliberate call, not an accident.

### Term, termination for cause, termination for convenience

Term is typically an initial term (1, 2, or 3 years) with auto-renewal for successive terms of the same length unless either party gives notice of non-renewal 30, 60, or 90 days before the current term ends. Startups generally prefer longer initial terms (revenue predictability) and auto-renewal (retention friction); enterprise procurement teams generally push for shorter terms and opt-in renewal.

**Termination for cause.** Standard: either party may terminate for the other's uncured material breach after a notice-and-cure period (typically 30 days). The cure period is the negotiation surface — the corporation wants a long cure period on its own breaches (to fix service issues before losing the customer) and no cure period on payment breaches (to accelerate collection). Enterprise counterparties will push for the reverse.

**Termination for convenience.** A right for either party to terminate on notice without a reason. Startups strongly resist customer-side termination for convenience because the deal's economics depend on the initial-term commitment; a customer who can walk out at any time is not really committed to the initial term. Enterprise procurement will frequently request 30- or 60-day convenience termination and the correct default startup position is "no." If the corporation concedes convenience termination, it should be paired with a **cancellation fee** equal to the remaining committed spend, which functionally converts "termination for convenience" into "early payoff."

### Payment terms and taxes

Payment terms — typically Net 30 from invoice date — with late-payment interest (often 1.5% per month or the maximum permitted by law) and suspension rights for extended non-payment. Enterprise counterparties will push for Net 60 or Net 90; the startup default is Net 30 with a discount for annual prepayment.

Taxes are the counterparty's responsibility (fees are stated exclusive of taxes; the counterparty pays sales, use, VAT, GST as applicable). The corporation is responsible for taxes on its own income. Withholding for cross-border payments should be spelled out — the counterparty must gross up so that the corporation receives the invoiced amount net of any required withholding, or the counterparty must provide the corporation with evidence of any tax withheld to support a foreign tax credit.

### Warranties

The warranties section is one of the most negotiated. The startup default has three parts:

- **Limited functionality warranty.** The Service will materially conform to the then-current documentation for a specified period (often 30 or 90 days after initial delivery, or throughout the term for a SaaS product). The remedy for breach is re-performance or, if re-performance fails within a defined window, refund of pre-paid unused fees.
- **Workmanlike-performance warranty for professional services.** Any professional services performed under a Statement of Work will be performed in a professional and workmanlike manner in accordance with generally-accepted industry practices.
- **Disclaimer of implied warranties.** All other warranties — merchantability, fitness for a particular purpose, non-infringement, accuracy — are disclaimed. Under UCC Article 2 § 2-316, disclaimers of merchantability must be conspicuous and must mention "merchantability" by name; disclaimers of fitness must be in writing and conspicuous. Whether Article 2 applies to a SaaS transaction is genuinely unsettled (Article 2 governs sales of goods, and SaaS is arguably a service, not a good) — the practical drafting response is to write the disclaimer to satisfy § 2-316 anyway, in all-caps or bold, so that if a court later applies Article 2 the disclaimer holds.

### Limitation of liability

The limitation of liability clause is the single largest financial risk allocation in the contract. The Series-A / Series-B default structure has three tiers:

- **General cap.** Neither party's aggregate liability under the agreement exceeds the fees paid or payable in the 12 months preceding the claim. Twelve months of fees is the practitioner-canon default; enterprise counterparties frequently push for 24 or 36 months, or for a fixed dollar multiple of annual fees.
- **Consequential-damages waiver.** Neither party is liable for lost profits, lost revenue, lost data (subject to carve-outs), or other indirect / incidental / consequential / special / punitive damages.
- **Super-caps for specific carve-outs.** Certain categories are excluded from the general cap and have their own higher cap (or are uncapped). The canonical carve-outs are (i) breach of confidentiality, (ii) IP indemnification, (iii) data-breach / privacy-law violations, (iv) gross negligence and wilful misconduct, and (v) payment obligations. Enterprise customers will insist on super-caps or uncapped exposure for data-breach; the negotiation is over the multiple (2x, 3x, 5x, or uncapped) and the trigger (any breach vs. breach caused by the corporation's negligence).

The interaction of the cap with the insurance stack ([mod-112](../mod-112-security-review-and-insurance/)) is important: the corporation should never accept a liability cap that exceeds its cyber-liability and E&O policy limits, because the delta between the cap and the insurance is uninsured balance-sheet exposure.

### IP ownership

The IP section is short and load-bearing:

- **Customer Data.** The customer owns its Customer Data — the data the customer or its users submit to the Service. The corporation gets a limited licence to use Customer Data solely to provide the Service and, in aggregated / de-identified form, to improve the Service. The de-identification and aggregation licence is negotiable — some enterprise customers refuse it outright.
- **The Service.** The corporation owns the Service, the underlying software, and all IP therein. The customer gets a limited, non-exclusive, non-transferable licence to use the Service during the term.
- **Feedback.** The corporation gets a perpetual, irrevocable, royalty-free licence to use any feedback or suggestions the customer provides about the Service. This is standard and should not be conceded.
- **Residuals.** Some enterprise MSAs include a "residuals" clause allowing the corporation to use information that becomes retained in the unaided memory of its employees. This is contentious and should be evaluated deal-by-deal; the startup default is not to insist on it.

### IP indemnification

The corporation indemnifies the customer against third-party claims that the Service infringes the third party's IP; the customer indemnifies the corporation against third-party claims that Customer Data infringes third-party IP. Both indemnities have standard carve-outs — no indemnity for (i) use of the Service outside the licence, (ii) modifications made by the customer, (iii) combination with third-party products not provided by the corporation, or (iv) continued use after the corporation has provided a non-infringing alternative.

The remedy procedure on an infringement claim: the corporation may, at its option, (i) procure a licence to allow continued use, (ii) modify or replace the Service so it is non-infringing, or (iii) if neither (i) nor (ii) is commercially reasonable, terminate the affected portion of the Service and refund pre-paid unused fees. This "procure / modify / refund" structure is the canonical clause.

### Confidentiality, insurance, force majeure, governing law

- **Confidentiality.** The MSA has its own confidentiality section covering information exchanged in the course of the engagement. If the parties previously signed an NDA (see [mod-103 chapter 05](../mod-103-employment-law-and-contract-design/05-nda-and-mnda-layer.md)), the MSA typically either supersedes it or explicitly incorporates it — the two documents should not silently coexist.
- **Insurance.** The corporation maintains stated minimum coverage across commercial general liability, professional liability / E&O, cyber liability, workers' comp, and umbrella policies. The minimums are negotiable ($1M / $2M / $5M / $10M layer combinations are typical). See [mod-112](../mod-112-security-review-and-insurance/).
- **Force majeure.** Neither party is liable for delays or failures caused by events beyond its reasonable control (natural disasters, war, government action, internet backbone failures). Post-COVID drafting typically calls out pandemics explicitly.
- **Governing law and venue.** The corporation's home-state law (typically Delaware or California), with exclusive venue in the corporation's home-state courts. Enterprise counterparties frequently push for their own home-state law; the compromise is often Delaware as a neutral commercial-law jurisdiction, or New York for financial-services counterparties.

## The Order Form pattern: one MSA, many Order Forms

The Order Form is a short document (often 1–2 pages) that captures the deal-specific economics against the framework the MSA established. What belongs on it:

- **Effective date and initial term.** When the Order Form takes effect and how long the initial term runs.
- **Products / SKUs purchased.** The specific Service editions, modules, or SKUs the customer is buying.
- **Pricing.** The per-unit price, the unit definition (per seat, per API call, per GB, per environment), the total contract value, and the payment schedule (annual prepay, monthly, quarterly).
- **Seat / usage counts.** The committed volume and the overage-pricing mechanics for usage above the commitment.
- **Contract signer.** The authorised signatory on each side.
- **Any deal-specific commercial terms.** A pilot discount, a most-favoured-customer clause, a specific SLA carve-in, a custom feature commitment.

Everything else — warranties, liability caps, IP ownership, indemnification, dispute resolution — lives in the MSA and is incorporated by reference. The Order Form should be short enough that a customer's procurement team can approve it in a single review; long Order Forms defeat the purpose of the MSA + Order Form split.

Renewals, seat expansions, and add-on module purchases each execute a new Order Form under the same MSA. Over the lifetime of a large enterprise account, the corporation may execute a dozen Order Forms against a single MSA.

## SLA design

The Service Level Agreement is the operations document that promises specific uptime and support-response commitments and specifies the credit remedy when the corporation falls short. It is a separate document because it is owned by the reliability team, is updated when the platform's SLO posture changes, and is often the subject of a customer-specific tier structure that would be awkward inside the MSA.

### Uptime percentages and their minutes-per-month implications

The industry-canon uptime tiers, expressed as monthly availability against a 30-day month (43,200 minutes):

- **99.5%** — 216 minutes / month of allowable downtime (~3.6 hours). Common for entry-tier or self-serve SKUs.
- **99.9%** ("three nines") — 43.2 minutes / month (~43 minutes). The mid-market default for enterprise-tier SKUs.
- **99.95%** — 21.6 minutes / month (~22 minutes). Common for higher-tier enterprise SKUs.
- **99.99%** ("four nines") — 4.32 minutes / month (~4 minutes). Reserved for premium tiers and typically requires the platform to have a multi-region active-active architecture. Startups should be extremely cautious about committing to four-nines without the underlying architecture to sustain it.

The uptime tier should map to the SKU. Committing four-nines on a self-serve SKU that runs on a single-region deployment is a credit-remedy exposure with no operational backing.

### What counts as downtime

The SLA's downtime definition is where most of the ambiguity lives. The standard carve-outs from "downtime" are:

- **Scheduled maintenance** during a defined maintenance window, on advance notice (typically 48 or 72 hours).
- **Emergency maintenance** required for security patching or critical stability fixes, on shorter notice.
- **Force majeure** — same events as the MSA's force majeure clause.
- **Customer-caused unavailability** — the customer's own network issues, misconfiguration, exceeding rate limits or documented capacity, or use of unsupported features.
- **Third-party dependencies outside the corporation's control** — this is contentious because the customer sees the Service as a single stack and does not care whether the root cause was the corporation's code or its cloud provider. Enterprise customers frequently push back on broad third-party carve-outs.

The definition of "downtime" itself should be measurable — the standard is a monitored HTTP or health-check endpoint that returns non-2xx responses for more than N consecutive minutes, aggregated over the month.

### Credit-remedy formula

The credit remedy is a percentage of the monthly fee (for the affected service) credited against a future invoice, escalating in tiers as availability drops:

- **Availability below the SLA but above a first threshold** (e.g., 99.5% target, actual 99.0%–99.5%): 10% monthly-fee credit.
- **Below the first threshold but above a second** (99.0%–99.5% actual against 99.9% target): 25% monthly-fee credit.
- **Below the second threshold** (below 95% actual): 50% monthly-fee credit, sometimes 100%.

The **"as sole and exclusive remedy" language** is essential — the SLA should state that the SLA credit is the customer's sole and exclusive remedy for availability failures. Without this language, the customer can claim SLA credit *and* pursue damages for the same event, which defeats the purpose of the cap-and-credit structure.

**Termination for repeated breach.** The one exception the customer will insist on is a right to terminate for cause if the corporation misses the SLA in some number of consecutive or rolling months (typically 3 consecutive months or 3 out of any 6 rolling months). This is a reasonable ask and should be conceded.

### Support tiers

The SLA also defines support-response commitments by severity:

- **P1 (critical / production down).** Response within 15 minutes to 1 hour; continuous engineering effort until resolution; executive escalation available.
- **P2 (major functionality impaired).** Response within 1–4 hours; business-hours engineering effort.
- **P3 (minor functionality impaired).** Response within 1 business day.
- **P4 (question / feature request).** Response within 2–3 business days.

Response times are for *initial response*, not resolution — the SLA should be explicit about the distinction. Enterprise customers on premium support tiers may negotiate resolution-time targets; the corporation should resist committing to resolution times because resolution depends on root-cause complexity that cannot be predicted.

## DPA structure

The Data Processing Addendum is the document that governs the corporation's processing of personal data on behalf of the customer. It is a separate document because privacy law moves independently of commercial law — new Standard Contractual Clauses, new US state privacy statutes, new international transfer mechanisms — and the DPA needs to be amendable on notice without re-opening the MSA.

The regulatory depth (GDPR Art. 28 processor obligations, CCPA / CPRA service-provider requirements, HIPAA BAA mechanics, sector rules) is treated in [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/). This chapter covers the structural anatomy.

### Controller / processor characterisation

The DPA identifies the customer as the **controller** and the corporation as the **processor** under GDPR Art. 4(7)–(8) (the controller determines purposes and means of processing; the processor processes on the controller's behalf). This characterisation drives most of the downstream obligations. Some processing (analytics, product-improvement, security-monitoring) may be genuinely controller-controller or joint-controller and needs to be called out explicitly rather than shoehorned into a processor characterisation that does not fit.

### Annex I: scope of processing

Annex I to the DPA specifies the *scope* of the processing — the categories of data subjects, categories of personal data, nature and purpose of the processing, duration, and any special categories of data (health, biometric, criminal-record). This is not boilerplate; it is the description of what the corporation is actually doing with the customer's data and what data-protection authorities will look at first in an audit.

### Annex II: security measures

Annex II specifies the **technical and organisational measures** (TOMs) the corporation implements to protect personal data — encryption at rest and in transit, access controls, MFA, network segmentation, logging and monitoring, incident response, business continuity, personnel security. Annex II typically mirrors or cross-references the Security Addendum (see below); duplication is fine as long as the two documents do not contradict.

### Sub-processor list and change notification

Under GDPR Art. 28(2), the processor must not engage sub-processors without the controller's prior specific or general written authorisation. The practical implementation is a **sub-processor list** attached to the DPA (or maintained on a public URL) and a **change-notification mechanic** — the corporation gives the customer notice (typically 30 days) before adding a new sub-processor, and the customer has a right to object. If the customer objects and the parties cannot reach a resolution, the customer typically has a termination right for the affected service.

### International transfers

Personal data transferred out of the EEA to a "third country" requires an approved transfer mechanism. The current stack:

- **EU Standard Contractual Clauses** under [Commission Implementing Decision (EU) 2021/914](https://eur-lex.europa.eu/eli/dec_impl/2021/914/oj), incorporated as a schedule to the DPA. Four modules cover controller-to-controller, controller-to-processor, processor-to-processor, and processor-to-controller flows.
- **UK International Data Transfer Addendum (UK IDTA)** or the UK Addendum to the EU SCCs, for transfers under UK GDPR.
- **Swiss addendum** to the SCCs for transfers under Swiss FADP.
- **EU–US Data Privacy Framework** for US importers that have self-certified adequacy under the framework (recognised by [Commission Implementing Decision (EU) 2023/1795](https://eur-lex.europa.eu/eli/dec_impl/2023/1795/oj)). A DPF-certified US importer can receive EU personal data without SCCs for the covered categories.

The DPA should include all applicable mechanisms so that a change in the customer's data-flow topology does not require re-signing.

### CCPA service-provider addendum

For US-state privacy law, the DPA includes a **CCPA service-provider addendum** with the specific language required by Cal. Civ. Code § 1798.140(ag) — the corporation certifies that it processes personal information solely for the business purposes specified, does not sell or share personal information, and does not combine the personal information received from the customer with personal information from other sources for unauthorised purposes. Analogous language covers Colorado, Virginia, Connecticut, and other US state statutes; mod-110 treats the full US state map.

### Breach notification, audit rights, deletion / return

- **Breach notification.** The processor notifies the controller of a personal-data breach without undue delay (GDPR Art. 33(2) — often operationalised as "within 72 hours"), with a defined scope of information to include.
- **Audit rights.** The customer has a right to audit the corporation's compliance with the DPA. On-site audits at the corporation's data centres or offices are operationally expensive; the standard compromise is that **the corporation provides its SOC 2 Type II report** (and typically a recent penetration-test summary) *in lieu of* on-site audit, with the customer retaining an on-site right if a specific incident triggers it or if the report is materially insufficient.
- **Deletion or return on termination.** On termination, the corporation deletes or returns personal data at the customer's option, subject to legally-required retention and IT-backup carve-outs (with continuing confidentiality on retained copies).

## Security Addendum and SIG-lite response

The Security Addendum is a document (sometimes standalone, sometimes a completed questionnaire) that specifies the corporation's security controls. Enterprise procurement teams almost always require it, either as a standalone document attached to the MSA or as a completed **Shared Assessments SIG-lite** — a standardised information-gathering questionnaire maintained by the Shared Assessments Program that has become the practitioner canon for third-party security assessments.

The Security Addendum / SIG-lite response typically covers:

- **Certifications and attestations.** SOC 2 Type II (the practitioner-canon proof for B2B SaaS), ISO 27001 (more common for European-facing corporations), FedRAMP (for US federal customers), HITRUST (for healthcare), PCI DSS (for payment processing). SOC 2 Type II covers a defined period (typically 12 months) and reports on the operating effectiveness of controls; a Type I report covers a point-in-time design and is materially weaker.
- **Penetration test summary.** An annual third-party pen-test summary letter (not the full report, which is confidential) — attestation of scope, date, methodology, and remediation status.
- **Encryption.** Data encrypted in transit (TLS 1.2 or later) and at rest (AES-256 or equivalent) with a stated key-management approach.
- **Authentication.** MFA required for all corporation personnel with production access; SSO / SAML support for customer users on enterprise SKUs.
- **Access control.** Least-privilege, role-based access control, quarterly access reviews.
- **Logging, monitoring, and incident response.** 24×7 monitoring, defined incident-response process, defined breach-notification timelines (aligned to the DPA).
- **Business continuity and disaster recovery.** RTO / RPO commitments, backup frequency, tested failover.
- **Personnel security.** Background checks, security training on hire and annually, offboarding process.
- **Vendor / sub-processor management.** Alignment to the DPA's sub-processor mechanic.

The **SOC 2 Type II report** is the single most important artefact — for many enterprise deals, providing the SOC 2 report alone will substitute for a SIG-lite response. The corporation should be able to deliver the current SOC 2 Type II report under NDA within one business day of an enterprise ask; not being able to is a signal to procurement that the corporation is not enterprise-ready.

## Acceptable Use Policy

The AUP is a unilateral document — the corporation publishes it and the customer's use of the Service is subject to it. Because it is unilateral, the AUP can be updated on notice (typically 30 days) without a counter-signature, which is why it lives outside the MSA.

The canonical AUP prohibits:

- **Illegal use.** Any use in violation of applicable law (CFAA violations, export-control violations, sanctions violations, child sexual abuse material, etc.).
- **Harassment and abuse.** Threats, harassment, defamation, hate speech targeted at individuals.
- **Malware and security threats.** Distributing malware, viruses, worms, ransomware; using the Service to attack third-party systems (including denial-of-service, port scanning, unauthorised access attempts).
- **High-volume automated attacks.** Load testing, scraping, or automated traffic beyond documented rate limits without prior written permission.
- **Benchmarking and public disclosure without permission.** Benchmarking the Service for public comparison, or publishing performance / capability data, without the corporation's prior written consent. This clause is standard but frequently redlined by enterprise customers (particularly research institutions and analyst firms).
- **Reverse engineering** beyond what applicable law permits notwithstanding contractual restrictions.
- **Circumvention of access controls or usage limits.**

The AUP reserves the corporation's right to **suspend** the Service (in whole or in part) for AUP violations, with a notice mechanic (immediate suspension for critical violations; notice-and-opportunity-to-cure for lesser violations). Suspension is distinct from termination — suspension pauses the Service; termination ends the contract. The AUP should be explicit that suspension for AUP violation does not entitle the customer to an SLA credit and does not toll the payment obligation.

## Order of precedence

The MSA states which document controls when documents conflict. The practitioner-canon ordering:

1. **Order Form** — most specific, most recently signed, captures deal economics.
2. **DPA** — carries statutory language that cannot be silently overridden.
3. **MSA** — the general framework.
4. **SLA** — operational service commitments.
5. **Security Addendum** — operational security commitments.
6. **AUP** — unilateral usage rules.

The reasoning: the Order Form is what the parties actually just agreed to for this deal; the DPA carries mandatory regulatory language; the MSA is the frame; the SLA, Security Addendum, and AUP are operational documents that inherit their gravity from the frame. Some enterprise counterparties will push for MSA > Order Form (reasoning: the MSA is the "master"). This inverts the intent of the MSA + Order Form architecture and should generally be resisted; the compromise is often "Order Form controls except for the sections of the MSA that expressly cannot be modified by an Order Form" (liability caps, IP ownership, dispute resolution).

## How the documents cross-reference

The six documents form a graph, not a tree. The important cross-references:

- The MSA incorporates each of the other five documents by reference and states the order of precedence.
- Each Order Form incorporates the MSA and any deal-specific SLA / DPA / Security-Addendum modifications.
- The DPA references the MSA's confidentiality, liability, and termination provisions (so a customer terminating the MSA also terminates the DPA).
- The DPA's Annex II (technical and organisational measures) either mirrors or cross-references the Security Addendum; the two should not contradict.
- The SLA's credit-remedy clause references the MSA's payment and billing terms (credits are applied against future invoices).
- The AUP is referenced from the MSA (customer's use of the Service is subject to the then-current AUP) and, where updated, notice is given per the MSA's notice clause.

Drafting these cross-references consistently is the ongoing job of legal ops and the CLM stack ([chapter 07](./07-clm-stack-and-legal-ops-graduation.md)).

## Concrete example: what a Series-B SaaS ships to Fortune-500 procurement on first ask

Acme Analytics, a Series-B B2B SaaS corporation selling to enterprise data teams, has been asked by a Fortune-500 procurement team for its "standard contract package." On first ask, Acme ships:

1. **Master Services Agreement** (12–15 pages). Standard Series-B MSA with mutual 12-months-fees general liability cap, super-caps for confidentiality (2x cap), IP indemnification (3x cap), and data breach (uncapped or a specified higher multiple aligned to Acme's cyber-liability policy). Termination for uncured material breach with a 30-day cure period; no customer-side termination for convenience. Delaware governing law; exclusive venue in Delaware. Mutual IP indemnification with the procure / modify / refund remedy. UCC § 2-316-compliant disclaimer of implied warranties in bold. Payment terms Net 30 with 1.5%-per-month late-payment interest. Insurance minimums aligned to Acme's actual policy limits.
2. **Order Form** (1–2 pages). Effective date; initial term (typically 12 months annual, or 24–36 months for a multi-year enterprise deal with a discount); SKU (Enterprise Edition, 500 seats, prod + non-prod environments); annual contract value; annual prepay; overage pricing at $X per seat per month; authorised signers on both sides.
3. **Service Level Agreement** (2–3 pages). 99.9% uptime target (Enterprise-tier SKU); 43.2-minute monthly downtime budget; carve-outs for scheduled maintenance (48-hour notice, defined maintenance window), force majeure, and customer-caused. Escalating credit tiers (10% / 25% / 50% of monthly fee). Sole-and-exclusive-remedy language. Termination for cause on 3 consecutive months of missed SLA. Support tiers P1 (1-hour response, 24×7) through P4 (2 business days).
4. **Data Processing Addendum** (8–12 pages including annexes). Controller / processor characterisation; Annex I scope of processing; Annex II TOMs (mirroring Security Addendum); sub-processor list at a public URL with 30-day change notification; EU SCCs (all four modules, per Commission Implementing Decision (EU) 2021/914); UK IDTA; Swiss addendum; DPF certification if applicable; CCPA service-provider addendum; 72-hour breach-notification commitment; SOC 2 Type II report in lieu of on-site audit; deletion / return on termination with IT-backup carve-out.
5. **Security Addendum / completed SIG-lite** (as a filled Shared Assessments SIG-lite spreadsheet plus a summary document). SOC 2 Type II report available under NDA; annual pen-test summary letter; TLS 1.2+ in transit; AES-256 at rest; MFA required for all Acme personnel with production access; SSO / SAML for customer users on Enterprise SKU; documented incident-response process; 24×7 monitoring; annual security training; documented BC / DR with stated RTO / RPO.
6. **Acceptable Use Policy** (2–3 pages, published on Acme's public website and referenced in the MSA). Prohibitions on illegal use, harassment, malware / attacks, high-volume automated abuse, benchmarking-and-publishing without permission, and reverse engineering beyond what law allows. Suspension right on notice; immediate suspension for critical violations.

The bundle is 30–40 pages total. Procurement routes the MSA to its commercial counsel, the DPA to its privacy office, the Security Addendum and SIG-lite to its infosec team, and the Order Form to the business sponsor. Each reviewer sees a document scoped to their concern, which cuts the first-round redline dramatically compared to sending a single 40-page contract to procurement to route internally.

Acme's contract playbook (see [chapter 02](./02-contract-playbook-and-fallback-position-matrix.md)) then governs the redline — what Acme accepts, what it counters, and what it walks from.

## Summary

- The customer contract suite is six documents (MSA, Order Form, SLA, DPA, Security Addendum, AUP), not one; the separation exists for reuse across deals, redline surface control, and regulatory drift.
- The MSA is the long-form framework: order of precedence, term / termination, payment, warranties (with a UCC § 2-316-compliant disclaimer of implied warranties), a mutual 12-months-fees liability cap with super-caps for confidentiality / IP / data-breach carve-outs, IP ownership (customer owns Customer Data; corporation owns the Service; feedback licence), mutual IP indemnification with the procure / modify / refund remedy, confidentiality, insurance, force majeure, and governing law.
- The Order Form is short — pricing, term, seat / usage counts, effective date, signer — and reuses the MSA across every renewal and add-on.
- The SLA sets uptime (99.5% / 99.9% / 99.95%, mapped to 216 / 43.2 / 21.6 monthly downtime minutes), defines what counts as downtime with the scheduled-maintenance / force-majeure / customer-caused carve-outs, sets an escalating credit remedy "as sole and exclusive remedy," and defines P1–P4 support tiers with response (not resolution) times. It concedes termination on repeated breach.
- The DPA is structurally separate from the MSA so privacy-law updates (new SCCs, new US state statutes) do not re-open the MSA. Its anatomy is controller / processor characterisation, Annex I (scope), Annex II (TOMs), sub-processor list with change notification, international-transfer mechanisms (EU SCCs per Commission Implementing Decision (EU) 2021/914, UK IDTA, Swiss addendum, DPF), CCPA service-provider addendum, breach-notification commitment, SOC 2 Type II in lieu of on-site audit, and deletion / return on termination. Regulatory depth belongs to [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).
- The Security Addendum (often a completed Shared Assessments SIG-lite) covers certifications (SOC 2 Type II is the canonical proof), pen-test summary, encryption at rest and in transit, MFA / SSO, incident response, BC / DR, and personnel security.
- The AUP is unilateral, updateable on notice, and covers illegal use, harassment, malware, high-volume automation, benchmarking without permission, and reverse engineering, with a suspension right.
- Order of precedence typically runs Order Form > DPA > MSA > SLA > Security Addendum > AUP; state it explicitly in the MSA.
- A Series-B SaaS should ship the full six-document bundle on first ask; not being able to signals "not enterprise-ready" to procurement and invites the counterparty's own worse-for-the-corporation template as a substitute.
