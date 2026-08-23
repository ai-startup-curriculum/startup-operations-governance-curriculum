# 3. The vendor contract suite and vendor-onboarding workflow

> The sell-side ([chapter 01](./01-customer-contract-suite.md)) is the corporation as counterparty defending its own paper; the buy-side is the corporation as counterparty *accepting* someone else's paper and redlining the handful of clauses that actually matter. Same clause taxonomy, mirror-image posture, different operational choreography — because a vendor contract is not just a legal document but the trigger for a security, procurement, and access-provisioning workflow.

## Motivation

Every operating corporation buys more contracts than it sells. A Series-B startup with 60 employees is comfortably party to 80–200 active vendor agreements — the SaaS stack alone (identity, HRIS, payroll, CRM, marketing automation, analytics, observability, error tracking, data warehouse, BI, ticketing, source control, CI, cloud infrastructure, endpoint management, email, calendar, collaboration, e-signature, expense management, corporate cards, banking, legal-hold, contract management, board portal) is 25–40 agreements, and that is before professional-services engagements, contractors, freelancers, agencies, resellers, and one-off licenses. The unit cost of a mistake on the buy side is smaller than on the sell side (one auto-renewal missed vs. one master customer contract with an uncapped liability), but the *aggregate* cost is comparable because there are so many buy-side agreements and because a single Tier-1 vendor breach can pierce the corporation's own customer-facing security and privacy obligations.

The failure mode this chapter is written against is the "sales rep hands the CFO an order form on the last day of the quarter" pattern — where a business-unit owner has already committed to a vendor, procurement and legal and security are told about it after the fact, and the corporation ends up signing vendor paper without redlines, without a DPA, without a SOC 2 review, without an SSO integration, and with a three-year auto-renewing term that quietly rolls over ninety days before anyone remembers it exists. The remedy is not a heavier process; it is a *tiered* process that scales the amount of scrutiny to the actual risk of the vendor.

This chapter is the buy-side companion to [chapter 01](./01-customer-contract-suite.md) (customer contract suite) and [chapter 02](./02-contract-playbook.md) (redline playbook). The redlines here mirror the sell-side matrix, but the corporation now argues for the *opposite* posture — auto-renewal opt-out instead of auto-renewal-with-notice, price caps instead of uncapped escalators, liability *floor* instead of ceiling, data ownership on the corporation's side instead of the vendor's. The onboarding workflow below is the operational glue that turns a legal contract into an approved, provisioned, tracked, and reviewable relationship.

## The vendor contract suite

Five documents make up the corporation's buy-side contract stack. Not every vendor sees all five; the tier framework below determines which apply.

### Vendor MSA / subscription-service agreement

The vendor's master subscription agreement (or MSA, or terms of service, or SaaS agreement — the taxonomy is unstable) is the standing contract that governs the corporation's use of the vendor's product. It is the mirror image of the corporation's own customer MSA ([chapter 01](./01-customer-contract-suite.md)).

**The accept-vendor-paper default.** The common startup pattern below a spend threshold (typically $25K–$50K/year in annual contract value, but the threshold is a policy choice) is to *accept vendor paper without a full redline*. The rationale is asymmetric negotiation leverage — a $12K/year seat license to a category-leading SaaS product is not a contract the vendor will meaningfully negotiate for a Series-B customer, and the transaction cost of a full redline (2–6 hours of counsel time) exceeds the risk-adjusted benefit. Above the threshold, or for any Tier-1 vendor regardless of spend, the corporation negotiates specific clauses from the redline matrix below.

**The clauses to redline even on vendor paper below the threshold.** Even when the corporation is accepting vendor paper without a full markup, a short list of clauses is worth pushing on:

- Auto-renewal opt-out with a workable notice window (see the dedicated section below).
- Data ownership and data portability at termination.
- Vendor's DPA is executed alongside the MSA.
- Security addendum or reference to the vendor's SOC 2 report.

Everything else on vendor paper below the threshold is typically accepted on the vendor's form, with an internal note in the CLM ([chapter 07](./07-clm-and-obligation-tracking.md)) flagging the non-standard provisions the corporation has agreed to.

### Professional-services / Statement of Work (SOW) agreement

Professional-services engagements — vendor implementation, custom integration work, migration services, training engagements, agency deliverables — are typically structured as an MSA plus a series of SOWs. The MSA sets the standing terms; each SOW invokes the MSA and adds deal-specific scope, price, and deliverables.

The SOW itself specifies:

- **Fixed-fee vs. time-and-materials (T&M).** Fixed-fee shifts scope risk to the vendor and works when the deliverable is well-defined (e.g., "migrate the corporation's data from vendor A to vendor B"). T&M shifts scope risk to the corporation and works when the deliverable is exploratory (e.g., "implement custom integrations to be scoped during discovery"). Hybrid structures (fixed-fee discovery phase, T&M implementation) are common.
- **Deliverables list.** Enumerated, specific, testable. "A working integration between system A and system B" is not a deliverable; "an integration that produces a matching record in system B within five minutes for every event of type X in system A, tested against the corporation's staging environment, with documentation covering setup, error handling, and monitoring" is.
- **Acceptance criteria.** Objective tests the deliverable must pass for the corporation to accept it and for payment to be triggered. A deliverable is "accepted" either affirmatively (the corporation signs an acceptance certificate) or by lapse (the corporation does not object within N business days). The lapse-based model is common but requires the corporation to *actually test* within the window, which is an operational discipline.
- **Change-order process.** How the parties agree to modify scope, price, or timeline mid-engagement. A change order is a mini-amendment to the SOW, signed by both parties before the changed work begins.
- **IP assignment, work-for-hire, license-back for pre-existing tools.** The heart of the SOW. See below.
- **Warranty of services.** Vendor warrants the services will be performed in a professional and workmanlike manner, consistent with industry standards. Not a warranty of a specific outcome unless separately negotiated.
- **Insurance requirements.** Vendor carries commercial general liability, professional liability (E&O), workers' compensation, and (for engagements touching data or systems) cyber liability — see the insurance certificate discussion below and cross-reference [mod-112](../mod-112-security-compliance-and-vendor-review/README.md).

**IP in an SOW: the three layers.** A well-drafted SOW distinguishes three layers of intellectual property:

1. **Pre-existing IP of the vendor (background IP).** Tools, frameworks, libraries, code, methodologies the vendor already owned before the engagement. The vendor keeps ownership; the vendor grants the corporation a perpetual, royalty-free license to use the pre-existing IP *as embedded in the deliverables* for the corporation's internal business purposes.
2. **Pre-existing IP of the corporation.** The corporation's data, systems, code, brand assets, and confidential information that the vendor accesses to perform the services. The corporation keeps ownership; the vendor gets a limited license *only* for the purpose of performing the services.
3. **Newly created deliverables.** Work product created specifically for the corporation under the SOW. The vendor assigns all right, title, and interest in the deliverables to the corporation, with "hereby assigns" present-tense language (see the contractor discussion below on why this matters), and with a work-for-hire designation as a backstop for copyright.

Cross-reference [chapter 04](./04-ip-protection-strategy.md) on the corporation's IP strategy generally.

### Contractor / consultant agreement

The contractor / consultant agreement (sometimes called an independent contractor agreement, or ICA, or master consulting agreement) governs the corporation's engagement of individuals or small firms performing work as non-employees. It is structurally similar to the SOW pattern (MSA + SOWs, or a single integrated agreement for one-off engagements) but is written for an *individual counterparty* and therefore inherits some of the individual-facing drafting patterns from the employment side.

**Worker classification is out of scope for this chapter.** Whether the individual is properly classified as a 1099 contractor or should have been a W-2 employee is a distinct legal question governed by the IRS common-law test, the DOL economic-reality test, the ABC test (California AB5, codified at Cal. Lab. Code § 2775 et seq., and other adopting states), and various state-law analogues. That analysis lives in [mod-103 chapter 07](../mod-103-employment-law-and-contract-design/README.md) on worker classification. This chapter assumes classification has already been decided and authors the contract that documents the engagement.

**The essential clauses.**

- **IP assignment with "hereby assigns" language.** Present-tense "The Contractor hereby assigns to the Corporation all right, title, and interest in and to the Work Product" — as opposed to future-tense "will assign" or "agrees to assign." The distinction matters because the Supreme Court in *Board of Trustees of the Leland Stanford Junior University v. Roche Molecular Systems, Inc.*, 583 U.S. 776 (2011), held that a future-tense "agrees to assign" clause did not operate as a present assignment and was defeated by a subsequent present-tense assignment to a different party. The remedy — universally adopted since — is present-tense "hereby assigns" language in every contractor and employee IP-assignment clause. Cross-reference [mod-103 chapter 04](../mod-103-employment-law-and-contract-design/04-employee-piia.md) on the same drafting pattern in the employee PIIA.
- **Work-for-hire backstop for copyright.** The Copyright Act at 17 U.S.C. § 101 defines "work made for hire" narrowly for non-employee-authored works — a work is work-for-hire only if (i) it falls within one of nine enumerated statutory categories and (ii) the parties expressly agree in a written instrument that the work is a work made for hire. The clause is drafted as a belt-and-suspenders: "The Work Product is a 'work made for hire' as defined in 17 U.S.C. § 101 to the fullest extent permitted by law; to the extent any Work Product does not qualify as work made for hire, the Contractor hereby assigns…"
- **DTSA whistleblower-immunity notice.** The Defend Trade Secrets Act at 18 U.S.C. § 1833(b) provides immunity to individuals who disclose trade secrets in specified circumstances (report of suspected illegal conduct to a government official, or in a court filing under seal). The statute requires the notice to be included in any contract governing the use of a trade secret entered with an employee or contractor; failure to include it forfeits the ability to recover exemplary damages and attorneys' fees in a subsequent DTSA action. Cross-reference [mod-103 chapter 04](../mod-103-employment-law-and-contract-design/04-employee-piia.md) and [chapter 05](../mod-103-employment-law-and-contract-design/05-nda-and-mnda-layer.md) for the same notice on the employee side.
- **Confidentiality.** A confidentiality obligation on the contractor with respect to the corporation's confidential information. The MNDA layer ([mod-103 chapter 05](../mod-103-employment-law-and-contract-design/05-nda-and-mnda-layer.md)) covers the mechanics; the contractor agreement typically incorporates confidentiality directly rather than requiring a separate NDA.
- **No-conflict warranty.** The contractor warrants that the engagement does not violate any obligation the contractor owes to any other party (e.g., an existing employer's non-compete, or an existing NDA that would prohibit the contractor from disclosing information relevant to the engagement).
- **Exhibit of pre-existing IP.** An exhibit listing the contractor's pre-existing intellectual property that the contractor intends to use in the engagement — typically tools, libraries, frameworks, or methodologies the contractor developed before the engagement. The exhibit is important because it (i) puts the corporation on notice of what the contractor is bringing in and (ii) defeats a later claim by the contractor that some component of the deliverables was actually pre-existing IP that was never assigned.
- **License-back for pre-existing IP embedded in deliverables.** For any pre-existing IP the contractor uses in the deliverables, the contractor grants the corporation a perpetual, worldwide, royalty-free license to use the pre-existing IP as embedded in the deliverables for the corporation's internal business purposes. Without this license, the corporation owns the deliverables but cannot use them without infringing on the contractor's pre-existing IP.

### Mutual NDA (MNDA) and unilateral NDA templates

The corporation maintains two NDA templates for the vendor-facing context:

- **Unilateral NDA, corporation as recipient.** Used when the corporation is evaluating a vendor's proprietary product and the vendor is doing all the substantive disclosing. The vendor shares product architecture, roadmap, security detail; the corporation shares little more than "we are evaluating vendors in this category."
- **Mutual NDA (MNDA).** Used when the corporation and vendor will exchange confidential information — typical of enterprise-vendor evaluations where the corporation is sharing usage details, integration scoping, or internal metrics for a joint discovery.

The anatomy of an NDA — direction, standard exceptions, confidential-information definition, purpose, ownership, dispute-resolution clauses, DTSA whistleblower carveout — is treated at length in [mod-103 chapter 05](../mod-103-employment-law-and-contract-design/05-nda-and-mnda-layer.md) and is not re-taught here. What matters for this chapter is that the NDA is executed *before* the vendor evaluation begins in earnest and is treated as a distinct step in the onboarding workflow below.

### Data Processing Agreement (DPA) from the vendor

When the vendor processes personal data on behalf of the corporation, the corporation is the *controller* (in EU GDPR terminology) or *business* (in California CCPA/CPRA terminology) and the vendor is the *processor* or *service provider*. GDPR Article 28 (for EU data subjects) and CCPA / CPRA at Cal. Civ. Code § 1798.140 et seq. (for California residents) require a written contract between controller and processor that specifies the subject matter, duration, nature and purpose of processing, categories of personal data, categories of data subjects, and the obligations of the processor. The DPA is that contract.

Vendors serving business customers typically maintain a standard DPA that they attach to or execute alongside the MSA. The vendor's DPA is what the corporation is agreeing to. The corporation reviews the DPA against a small checklist:

- Sub-processor list and change-notice mechanics (advance notice; right to object).
- Data-residency and cross-border transfer mechanism (Standard Contractual Clauses under Commission Implementing Decision (EU) 2021/914 for EU-to-US transfers; Data Privacy Framework certification for participating US vendors; UK IDTA for UK-to-US transfers).
- Data-return-and-destruction obligations on termination.
- Breach notification timeline (typically 24–72 hours from the vendor's knowledge of a breach affecting the corporation's data).
- Audit rights or, more commonly, the vendor's provision of an annual SOC 2 report in lieu of an on-site audit.
- Right to instruct the vendor on the processing.

The critical structural point: the vendor's DPA becomes the *corporation's* binding obligation to its own downstream data subjects and end customers. If the corporation has promised its customers (in its own customer DPA, per [chapter 01](./01-customer-contract-suite.md)) that sub-processors will provide at least the level of protection that the corporation itself provides, then the vendor's DPA must actually deliver that level. A gap between the corporation's customer-facing DPA commitments and the corporation's vendor-facing DPA acceptances is a compliance defect. Cross-reference [mod-110](../mod-110-data-privacy-regulatory/README.md) on the underlying privacy-regulatory framework.

## Clauses to redline on vendor paper (buy-side mirror of the sell-side matrix)

The redline matrix in [chapter 02](./02-contract-playbook.md) treats each clause from the corporation's *sell-side* posture. On the buy side, the corporation argues the mirror-image position. The clauses that matter most on vendor paper:

### Auto-renewal opt-out and notice windows

The default in enterprise SaaS vendor paper is auto-renewal for successive one-year terms unless the customer gives written notice of non-renewal at least *ninety days* prior to the end of the then-current term. The ninety-day window is notorious because it is (i) long enough that a customer who forgets about the contract for a quarter will miss it and (ii) drafted as a hard cutoff, not a rolling notice period.

The corporation's redline positions, in order of preference:

- **Best.** Term expires at the end of the initial term unless the parties affirmatively renew (opt-in renewal). Vendors rarely accept this.
- **Better.** Auto-renewal but with a *shorter notice window* — 30 days is a common negotiated outcome; 60 days is a fallback.
- **Fallback.** Auto-renewal with the vendor's default notice window (typically 90 days), *and* an obligation on the vendor to send a renewal notice to a specified email address at least 30 days before the notice deadline.

Every auto-renewing agreement, regardless of the negotiated window, is added to the obligation tracker ([chapter 07](./07-clm-and-obligation-tracking.md)) with a calendared reminder at least two weeks before the notice deadline.

### Price escalation caps

Vendor paper typically includes an annual price-escalator clause — "fees will increase by up to N% at each renewal." N is often left blank (uncapped) or set at a high default (10–15%). The corporation redlines to a hard cap — 5–7% for most categories, tied to an inflation index (CPI-U) for longer-term agreements — and pushes back on any "up to N% *or* the vendor's then-current list price, whichever is greater" formulation because the latter defeats the cap.

### Termination for convenience for the customer

Vendor paper generally does *not* grant the customer termination-for-convenience rights during the term (the vendor has bargained for the term commitment). The corporation asks for a customer-side termination-for-convenience right with a reasonable notice period (60–90 days) and, in exchange, may agree to a partial refund limitation or to a payment for the remainder of the term at a discount. This is typically only won on longer-term deals (2+ years) or when the corporation is a strategically-important customer.

### Most-favoured-nation (MFN) commitment from the vendor

The corporation asks the vendor to commit that the pricing, terms, and features offered under this agreement are at least as favourable as those the vendor offers to any similarly-situated customer of the vendor. MFN clauses are difficult to enforce in practice (the corporation has no visibility into other vendor customers), and vendors resist them for that reason, but even a weak MFN clause creates leverage in a subsequent renegotiation. Typically won only for large enterprise deals or when the corporation is genuinely a marquee customer.

### Data ownership and portability on termination

The corporation's data — including data the vendor generates about the corporation's use of the product (usage logs, analytics, derived data) — is owned by the corporation. The vendor's rights to use the data are limited to what is necessary to provide the service, generate aggregate benchmarks (with an opt-out if desired), and comply with the vendor's own legal obligations. On termination, the vendor provides the corporation's data in a documented, machine-readable format for a defined return window (30–90 days), after which the vendor destroys the data (with a carveout for backups and legal retention obligations).

The failure mode is a vendor MSA that grants the vendor a broad license to the corporation's data ("Customer Data may be used by Vendor for any purpose consistent with the service and Vendor's business") — this defeats downstream customer commitments and should be redlined out.

### Sub-processor change notice

The DPA (above) sets the sub-processor-change-notice mechanic. The corporation's redline position: at least 30 days' advance notice of any new sub-processor, with the corporation's right to object; if the corporation objects and the vendor cannot accommodate, the corporation has a termination right and a pro-rata refund. Vendors resist the termination right; the negotiated outcome is often notice + right to object without termination for smaller customers, and notice + right to object + termination for larger customers.

### Warranty and remedies

Vendor paper typically warrants the service will substantially perform in accordance with the documentation, with a limited remedy (fix or credit) as the sole and exclusive remedy for breach. The corporation redlines the remedy language to preserve *all* remedies at law and in equity, not just the vendor's chosen sole remedy — otherwise the warranty is functionally unenforceable if the vendor fails to fix. Alternatively, the corporation negotiates a termination-for-material-breach right that survives the sole-remedy limitation.

### Limitation of liability FLOOR

The mirror image of the sell-side limitation-of-liability *ceiling* discussion in [chapter 02](./02-contract-playbook.md): on the buy side, the corporation is *arguing that the vendor's cap is not so low that it doesn't cover the corporation's actual exposure*. Vendor paper typically caps the vendor's liability at fees paid in the trailing 12 months. For a $50K/year vendor that processes the corporation's regulated data, a $50K cap is inadequate for a data breach — the corporation's own breach-notification and remediation costs will vastly exceed the cap.

The corporation's redline positions:

- **Super-cap for data-breach and confidentiality claims.** A separate, higher cap (2×–5× fees, or a dollar amount like $1M–$5M) specifically for claims arising from the vendor's breach of data-security or confidentiality obligations.
- **Uncapped liability for confidentiality, IP infringement, data-security breach, and gross-negligence / wilful-misconduct claims.** The corporation carves specified categories *out* of the cap entirely — mirror-image of the sell-side carve-outs the corporation is defending against as a vendor.

### Uncapped liability carveouts

The categories the corporation attempts to carve out of the vendor's liability cap:

- Vendor's indemnification obligations (particularly IP indemnity — see below).
- Vendor's breach of confidentiality.
- Vendor's breach of data-security or privacy obligations.
- Vendor's gross negligence or wilful misconduct.
- Vendor's payment obligations (refunds owed to the corporation).

These carveouts are the exact mirror image of the sell-side "uncapped-liability carve-outs to defend against" in [chapter 02](./02-contract-playbook.md).

### Insurance certificate requirements

For Tier-1 and Tier-2 vendors (see below), the corporation requires the vendor to maintain — and to provide an annual certificate of insurance for — the following coverages, with the corporation named as an additional insured on the general-liability and (where applicable) cyber-liability policies:

- **Commercial General Liability (CGL).** $1M per occurrence / $2M aggregate is a common floor for a Tier-2 vendor; $2M / $5M for Tier-1.
- **Professional Liability / Errors & Omissions (E&O).** $1M–$5M depending on the engagement's risk profile. Required for professional-services vendors and for SaaS vendors whose product failure could cause the corporation direct financial loss.
- **Cyber Liability.** $1M–$10M depending on the sensitivity of the data the vendor processes. Non-negotiable for any vendor that processes regulated data classes (PHI, PCI, employee PII).
- **Workers' Compensation.** Statutory minimums per the vendor's home state. Required for any vendor whose workers will be on the corporation's premises.

Cross-reference [mod-112](../mod-112-security-compliance-and-vendor-review/README.md) for the insurance and vendor-review framework in more detail.

## The vendor-onboarding workflow

The workflow below is the operational choreography that turns a business-unit "we want to use vendor X" into a legally, security, and procurement-approved, provisioned vendor relationship. The steps are not always strictly sequential (security and legal review often run in parallel), but the milestones are.

1. **Business unit identifies need and short-lists vendors.** The requesting business unit (marketing, engineering, sales, finance, people) identifies a category need, evaluates 2–4 candidate vendors on functionality and cost, and short-lists a preferred vendor. Deliverable: a brief business case (why this vendor, why now, expected spend, budget line).

2. **Vendor evaluation and NDA (MNDA typical).** The business unit engages the vendor for a discovery or trial. Before any substantive information exchange, an NDA is executed — unilateral if the vendor is doing all the substantive disclosing, mutual if the corporation will be sharing internal information or integration detail. In practice, mutual NDAs are the more common outcome. Cross-reference [mod-103 chapter 05](../mod-103-employment-law-and-contract-design/05-nda-and-mnda-layer.md).

3. **Contract submission and legal review.** The vendor delivers its MSA (and DPA, and any SOW if professional services are involved). Legal reviews against the redline matrix above, applying the tier framework below to determine depth of review. For accept-vendor-paper cases, review is limited to the short list of "clauses to redline even below the threshold." For full-redline cases, counsel produces a redline against the vendor's paper and negotiates.

4. **Security review by the security team.** For Tier-1 and Tier-2 vendors, the security team requests and reviews the vendor's SOC 2 Type II report (or equivalent — ISO 27001 certification, HITRUST for healthcare vendors), a summary of the vendor's most recent penetration test, the vendor's DPA and sub-processor list, and any relevant compliance certifications (PCI DSS AOC for payment vendors, HIPAA BAA readiness for healthcare vendors). Deliverable: a security review record that either approves, approves with conditions, or rejects the vendor. Cross-reference [mod-112](../mod-112-security-compliance-and-vendor-review/README.md) for SecReview mechanics.

5. **Procurement / finance approval.** Finance verifies the spend is within the requesting business unit's budget, that the appropriate spend-authority approvals have been obtained (per the corporation's delegation of authority matrix — a Series-B corporation typically has thresholds like "manager can approve up to $5K, director up to $25K, VP up to $100K, CFO up to $500K, CEO or board above"), and that a purchase order is issued if required by the vendor. Deliverable: an issued PO or an approved spend request.

6. **Data classification and DPA assessment.** The privacy or data-governance function classifies the data the vendor will process (public, internal, confidential, regulated — see [mod-110](../mod-110-data-privacy-regulatory/README.md) on the corporation's data classification schema). For vendors processing personal data, confidential business data, or regulated data classes (PHI, PCI, employee PII), the vendor's DPA is executed and any required regulatory addenda (BAA for HIPAA, PCI DSS attestation for payment card data) are attached. Deliverable: executed DPA (and any addenda), plus a data-flow record documenting what data the vendor receives.

7. **SSO / access provisioning through IT.** IT provisions access — ideally through the corporation's identity provider (Okta, Google Workspace, Microsoft Entra) via SAML or OIDC single sign-on, so that access can be centrally managed and centrally revoked. Direct-provisioned accounts (username + password managed by the vendor) are permitted only for vendors that do not support SSO, and even then are managed through the corporation's password manager rather than left with individual users. Deliverable: SSO integration configured, initial user accounts provisioned, offboarding process in place.

8. **Contract centrally filed and obligations added to the tracker.** The signed contract (including the MSA, DPA, order form, and any addenda) is uploaded to the CLM ([chapter 07](./07-clm-and-obligation-tracking.md)) with metadata (vendor name, effective date, term end date, auto-renewal window, notice deadline, tier, primary business owner, security approver, data classification, spend). Calendared reminders are set for the notice deadline, the renewal date, and any annual-review milestone (SOC 2 renewal, insurance certificate renewal, DPA re-execution). Deliverable: contract filed, obligations tracked.

The workflow is not linear in the sense that steps must strictly complete before the next begins. Steps 3, 4, and 6 (legal, security, DPA) commonly run in parallel; steps 5 and 7 (finance, IT) typically wait for legal and security approval before executing. The critical gate is that *no step is skipped* for vendors above the tier-3 threshold.

## Vendor-tier framework

Not every vendor deserves the full workflow. The tier framework calibrates scrutiny to risk.

**Tier 1 — mission-critical or regulated-data-processing vendors.** Vendors whose failure would materially impair the corporation's ability to serve its customers, *or* whose access includes regulated data classes (PHI, PCI, employee PII, cardholder data, sensitive customer data covered by industry regulation). Examples: primary cloud provider, identity provider, payroll processor, HRIS, primary payment processor, EHR integration vendor for a health-tech corporation. Treatment: full legal redline, full security review including SOC 2 Type II, DPA plus regulatory addenda (BAA / PCI attestation as applicable), insurance certificate with corporation as additional insured, executed contract with negotiated liability terms, annual re-review of security posture and contract obligations.

**Tier 2 — business-important vendors without regulated data.** Vendors that support important business functions but do not process regulated data and whose failure is disruptive but not existential. Examples: CRM, marketing automation, analytics, observability, ticketing, source control, CI/CD, collaboration tools, expense management. Treatment: abbreviated legal review focusing on the short list of clauses above, security review with SOC 2 Type II accepted, DPA executed if the vendor processes personal data, insurance certificate collected, biennial re-review.

**Tier 3 — low-risk personal-productivity vendors.** Small-spend, low-risk, individual-productivity tools that touch minimal corporate data. Examples: individual seat licenses to design tools, note-taking apps, browser extensions, small utilities. Treatment: self-serve provisioning against an allow-list maintained by IT and security. No formal legal review; standard vendor paper accepted; no DPA unless the vendor happens to process personal data; no insurance requirement.

The tier assignment is made at the outset of the onboarding workflow (during step 3 or step 4) by the security or legal function, based on the data classification and the criticality of the vendor. The tier assignment is recorded in the CLM and drives the depth of ongoing review.

## SOW vs. MSA relationship and order of precedence

The MSA is the standing contract; each SOW is a work order that invokes the MSA. The MSA supplies the standing terms (limitation of liability, warranties, indemnities, IP framework, confidentiality, dispute resolution, insurance requirements); each SOW supplies the deal-specific scope (deliverables, timeline, price, acceptance criteria, personnel).

**Order of precedence.** A well-drafted SOW explicitly states the order of precedence between the SOW and the MSA. The conventional order is:

**SOW > MSA** — the SOW controls to the extent of any conflict with the MSA. The rationale is that the SOW is the more recent and more specific document; the parties presumably intended the SOW's specifics to modify the MSA's generalities for the particular engagement.

Two footnotes:

- The convention is not universal. Some vendors' paper reverses the order (MSA > SOW), arguing that the MSA is the negotiated framework and the SOW should not silently modify it. The order of precedence is negotiable; what matters is that the agreement states it explicitly.
- The order of precedence typically excludes the "core commercial terms" of the SOW (scope, price, deliverables) from the potential-conflict analysis — the SOW's commercial terms are additive to, not in conflict with, the MSA. The order-of-precedence rule matters for genuinely conflicting terms (e.g., an SOW that purports to increase the vendor's liability cap or extend an IP indemnity beyond the MSA's terms).

The failure mode is an unspecified order of precedence combined with an SOW that quietly modifies MSA terms — the corporation ends up in a dispute over which document controls, and courts default to interpretation principles that may not align with either party's expectations.

## Concrete example: a vendor-onboarding kanban for a Series-B startup

Acme Robotics (Delaware C-Corp, San Francisco, 80 employees, Series-B) receives 8–12 new-vendor requests per month across engineering, marketing, sales, people, and finance. The vendor-onboarding process is run out of the "Legal Ops / Procurement" workstream (a shared responsibility of the general counsel and the CFO's office) with a Kanban board in the corporation's project-management tool.

The board has columns:

- **Intake.** Business-unit owner submits a request via a short form: vendor name, category, business case, expected spend, category of data the vendor will process, urgency. The intake form drives an initial tier assignment (auto-assigned Tier 3 if spend < $5K and no personal data; auto-assigned Tier 2 if $5K–$50K and no regulated data; auto-assigned Tier 1 otherwise, subject to review).
- **NDA.** MNDA sent to the vendor via e-signature. Column dwell time: 3–5 business days.
- **Legal review.** Vendor MSA / DPA / SOW submitted to counsel. For Tier 3, this column is skipped. For Tier 2, review dwell time is 3–5 business days. For Tier 1, dwell time is 1–3 weeks including negotiation.
- **Security review.** SOC 2 requested, DPA reviewed, sub-processor list evaluated. Runs in parallel with legal review. Dwell time: 5–10 business days.
- **Data-classification / DPA.** Vendor's DPA executed; regulatory addenda attached if applicable; data-flow record created. Dwell time: 2–5 business days.
- **Finance / procurement.** Spend approval, PO issued if required. Dwell time: 2–5 business days.
- **IT provisioning.** SSO configured, users provisioned. Dwell time: 3–7 business days.
- **Filed and tracked.** Contract uploaded to CLM, obligations calendared. Dwell time: 1 business day.

Total onboarding time end-to-end: 1–2 weeks for a Tier 3 vendor (mostly a rubber-stamp path), 2–4 weeks for a Tier 2 vendor, 4–8 weeks for a Tier 1 vendor.

The corporation also runs a monthly review meeting (legal, security, finance, IT) to (i) triage any stalled onboarding cards, (ii) review the previous month's newly-onboarded vendors for any pattern issues, (iii) surface upcoming renewal deadlines from the CLM, and (iv) audit a random sample of tier-3 self-serve provisions to confirm they were correctly classified as Tier 3. The monthly cadence keeps the onboarding process from becoming invisible bureaucracy and creates a forcing function for the business units to plan vendor requests with lead time rather than emergency purchases.

<!-- needs-research: whether industry benchmarks exist for vendor-onboarding cycle time at Series-B stage; the 1-2 / 2-4 / 4-8 week ranges above are typical from practitioner discussion but not from a citable study. -->

## Common failure modes

- **Accepting vendor paper without reading the DPA.** The MSA gets a review, the DPA gets rubber-stamped, and the corporation inherits a downstream compliance gap.
- **Skipping the NDA step.** The vendor and the business unit have already exchanged confidential information on a discovery call before an NDA is in place.
- **Auto-renewals rolling silently.** The 90-day notice window expires, the contract renews for another year, the corporation is on the hook for another term at the escalated price.
- **Sub-processor lists not tracked.** The vendor adds a sub-processor via a notice email that nobody opens; the corporation is now inheriting a downstream processor it never approved.
- **Insurance certificates not collected or not renewed.** The certificate expires; the vendor is out of compliance with the MSA; the corporation is exposed without recourse in the event of a claim.
- **SSO not enforced.** The vendor is provisioned with individual-account credentials; departing employees retain access; access is not centrally revocable.
- **Tier misassignment.** A vendor that processes employee PII is treated as Tier 3 because the spend is small; the SOC 2 is never requested; the DPA is never executed.
- **SOW-MSA order of precedence unstated.** A conflict between the SOW and the MSA becomes a dispute the corporation cannot cleanly resolve.
- **Contractor IP-assignment clause using "will assign" or "agrees to assign" language.** The clause is defeated by a subsequent present-tense assignment to a different party, per *Stanford v. Roche*, 583 U.S. 776 (2011).
- **Missing DTSA whistleblower notice in the contractor agreement.** The corporation forfeits exemplary damages and attorneys' fees in a subsequent DTSA action, per 18 U.S.C. § 1833(b).

## Summary

- The buy-side contract stack is five documents: vendor MSA / subscription agreement, professional-services SOW under a services MSA, contractor / consultant agreement, MNDA / unilateral NDA, and the vendor's DPA. Not every vendor sees all five; the tier framework calibrates which apply.
- Accepting vendor paper below a spend threshold is the common startup default; even then, redline the short list of clauses that matter — auto-renewal opt-out, data ownership, DPA execution, security-addendum reference.
- Above the threshold or for Tier-1 vendors, redline the mirror-image of the sell-side matrix: auto-renewal opt-out with a workable notice window, price-escalation caps, customer termination-for-convenience where obtainable, MFN, data ownership and portability, sub-processor change notice, warranty preserving all remedies, liability *floor* adequate to cover data-breach exposure, uncapped-liability carveouts for confidentiality / IP / data-security / gross negligence, and insurance certificate requirements with the corporation named as additional insured.
- The contractor agreement includes present-tense "hereby assigns" IP language per *Stanford v. Roche*, 583 U.S. 776 (2011), work-for-hire backstop for copyright per 17 U.S.C. § 101, DTSA whistleblower notice per 18 U.S.C. § 1833(b), confidentiality, no-conflict warranty, pre-existing-IP exhibit, and license-back for pre-existing IP embedded in deliverables. Worker classification is a separate analysis in [mod-103](../mod-103-employment-law-and-contract-design/README.md).
- The vendor's DPA becomes the corporation's binding obligation to its own downstream customers and data subjects — review the sub-processor mechanics, cross-border transfer basis, breach-notification timeline, and audit or SOC 2 provisions against the corporation's own customer-facing commitments.
- The vendor-onboarding workflow has eight steps: business-unit intake, NDA, legal review, security review, finance / procurement approval, data-classification and DPA execution, SSO / access provisioning, and central filing with obligation tracking. Steps 3, 4, and 6 commonly run in parallel; steps 5 and 7 gate on legal / security approval.
- The vendor tier framework — Tier 1 mission-critical or regulated data, Tier 2 business-important without regulated data, Tier 3 low-risk personal-productivity — calibrates the depth of review and the ongoing re-review cadence.
- The SOW invokes the MSA and supplies deal-specific scope, price, deliverables, and acceptance criteria; the order of precedence (typically SOW > MSA) should be stated explicitly to avoid conflict-of-terms disputes.
- Central filing in the CLM ([chapter 07](./07-clm-and-obligation-tracking.md)) with calendared obligation reminders is the bridge from "contract signed" to "obligations actually tracked" — without it, auto-renewals roll silently, insurance certificates expire, and sub-processor notices go unread.
