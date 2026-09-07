# 9. Ownership boundary map

> The commercial-contracts / IP / legal-ops function is the busiest desk in the corporation. This chapter is the reference map that decides — for any contract, IP, or legal-ops question — whether it belongs to mod-109, to a sibling module, or to a non-role track.

## Motivation

The general counsel's inbox is not neat. In any given quarter it receives an AI-indemnity redline from a sales director, an AGPL question from a staff engineer, a departing-engineer trade-secret concern from the head of people, a federal-agency SBOM demand from a channel partner, a CLM procurement request from finance, a customer audit-rights redline from a Fortune-500 privacy officer, a Series-C data-room request for contract inventory, and an employee subject-access request routed via a downstream vendor. Each of these looks like a "legal" question. Each of them touches at least one — and usually two or three — sibling functions. Without an explicit ownership map, mod-109 either overreaches into corporate-governance work, privacy regulatory analysis, or M&A transaction drafting it is not competent to produce, or under-reaches while sales, procurement, security, engineering, HR, or finance quietly write conflicting policies of their own.

The problem is structural. Commercial contracts, IP, and legal ops sit at the intersection of legal, sales, procurement, security, privacy, and finance. Every one of those functions has its own operating cadence, its own vocabulary, and its own view of "who owns this." An MSA touches sales (the revenue), finance (the billing terms), security (the security addendum), privacy (the DPA), engineering (the AUP and the API-scope), and product (the SLA). A vendor contract touches procurement (the spend), security (the SecReview), privacy (the vendor DPA), and finance (the P&L line). An IP-protection question touches R&D (the invention disclosure), HR (the PIIA enforcement), and outside counsel (the filings). Without a written map, the corporation ends up with three DPAs, two AUPs, and a shadow deal desk operated out of the sales operations team.

This chapter is the operating map — the tie-breaker used when a question arrives without a clear home. It states what mod-109 owns end-to-end, what mod-109 hands off to a specific sibling module, and what mod-109 explicitly defers to a non-role curriculum track. It is written to be quoted back at the person who wants to route work incorrectly. When someone insists that the AI-usage policy is "obviously a legal question, so it lives with you," this chapter is the citation that returns it to mod-108. When someone insists that the vendor DPA question is "obviously a privacy question, so it lives with the DPO," this chapter is the citation that keeps it in mod-109.

## What mod-109 owns

The eight substantive chapters of mod-109 own the following, end-to-end:

- **Customer contract suite (MSA / SLA / DPA structure / Security Addendum / AUP / Order Form)** — [chapter 01](./01-customer-contract-suite-msa-sla-dpa-security-aup.md). The architecture of the six-document bundle the corporation offers to every enterprise customer, the interaction between the documents, and the order-of-precedence clause that resolves conflicts among them. Every enterprise sale starts here.
- **Contract playbook / fallback-position matrix / deal desk / internal-legal-turn SLA / escalation-to-outside-counsel triggers** — [chapter 02](./02-contract-playbook-and-fallback-position-matrix.md). The redline manual, the deal-desk workflow, the acceptable / walk-away positions on each clause, the internal SLA for legal review, and the trigger list that sends a deal to outside counsel.
- **Vendor contract suite / vendor-onboarding workflow / vendor-tier framework** — [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md). The mirror-image of the customer suite, from the buyer's side: the vendor MSA / DPA / security addendum template pack, the tiered vendor-onboarding workflow, and the intake form procurement uses to route new vendor requests.
- **IP protection strategy: patents, trademarks, copyright, trade-secret programme** — [chapter 04](./04-ip-protection-strategy.md). The invention-disclosure programme, the patent-portfolio strategy, the trademark clearance / registration cadence, the copyright registration posture, and the trade-secret protection programme (marking, access controls, exit interviews).
- **Open-source hygiene / SBOM programme / outbound-contribution policy** — [chapter 05](./05-open-source-hygiene-and-sbom-programme.md). The OSS licence taxonomy, the approval tiers, the SBOM production workflow, and the outbound-contribution / corporate-open-source-release policy.
- **AI-vendor / AI-DPA / AI-transparency contracts / AI-indemnification pattern** — [chapter 06](./06-ai-vendor-contracts-and-ai-dpa-pattern.md). The customer-facing AI addendum, the AI-model-training carve-out, the hallucination-and-output-accuracy warranty position, the AI-DPA specifics, and the AI-indemnity structure — the *contract* side of AI risk allocation, distinct from the *policy* and *governance* sides that live elsewhere.
- **CLM stack / legal-ops build-out / CLM-vs-in-house-legal-hire graduation** — [chapter 07](./07-clm-stack-and-legal-ops-graduation.md). The CLM selection and implementation, the metadata / clause-library architecture, the legal-ops team build-out, and the graduation curve that maps stage of company to CLM investment versus in-house-counsel hiring.
- **In-house vs. outside-counsel decision framework / outside-counsel management** — [chapter 08](./08-in-house-vs-outside-counsel-decision-framework.md). The decision framework for what is done in-house versus routed to outside counsel, the panel-firm selection, the fee-arrangement structure, and the outside-counsel management cadence.

If a question maps to one of the above, mod-109 owns it. If it maps to one of the below, mod-109 explicitly hands off.

## What mod-109 hands off

Each sibling module owns a specific slice of adjacent work. The pattern to keep in mind: mod-109 owns the *commercial-contract / IP / legal-ops layer*; sibling modules own the *corporate, employment, privacy, security, governance, or international layer* underneath.

### mod-101 — legal entity formation and corporate structure

- The entity-level corporate work — charter, bylaws, subsidiary structure, corporate record, qualification to do business in each state.
- Board authorisation resolutions for contract execution over the officer-authority threshold.
- The corporate-record side of contract signing (secretary's certificates, incumbency certificates, delegation-of-authority resolutions).

mod-109 drafts and signs the commercial contract; mod-101 is where the entity that signs it, and the corporate authority to sign, actually live. See [mod-101](../mod-101-legal-entity-formation-and-corporate-structure/).

### mod-102 — founding team legal architecture

- Founder-side legal architecture — founder PIIAs, restricted-stock and 83(b) elections, founder side letters, pre-formation IP-assignment.
- The clean-up of any founder-era IP that has to be scrubbed into the corporation before enterprise diligence.
- The founder-side non-compete / non-solicit posture where it deviates from the standard employee pack.

The IP-protection strategy in [chapter 04](./04-ip-protection-strategy.md) assumes that founder IP has already been assigned into the corporation via mod-102's mechanics; if it has not, that is a mod-102 problem, not a mod-109 problem. See [mod-102](../mod-102-founding-team-legal-architecture/).

### mod-103 — employment law and contract design

- The employment-facing contract layer: at-will language, arbitration, non-compete / non-solicit enforceability, employee PIIA, offer-letter and employee-agreement drafting.
- State-law variance analysis for employment terms (California Business & Professions Code § 16600, the New York non-compete landscape, the FTC final rule and its litigation posture).
- The employment-side of trade-secret enforcement — PIIA breach, garden-leave mechanics, employee-side injunction practice.

mod-109 owns *commercial* contracts; mod-103 owns *employment* contracts. When a departing employee is threatening to misappropriate trade secrets, mod-109 chapter 04 owns the trade-secret protection programme; mod-103 owns the PIIA enforcement mechanics. See [mod-103](../mod-103-employment-law-and-contract-design/).

### mod-104 — hiring, onboarding, and HR operations

- HRIS / PEO configuration and the hiring-loop mechanics that touch employment-adjacent contracts (contractor onboarding, background-check consents, I-9 workflow).
- The onboarding-day IP-assignment execution — the actual signing ceremony that makes the employee PIIA effective.
- Recruiter operations that route contractor-versus-employee determinations to legal.

mod-109 drafts the contractor template; mod-104 is where the contractor is actually onboarded and where the contractor-versus-employee determination is operationalised. See [mod-104](../mod-104-hiring-onboarding-and-hr-operations/).

### mod-105 — equity compensation policy and comp committee

- Equity-plan documents (the equity incentive plan itself, the sub-plan for non-US grantees), grant-agreement templates (ISO, NSO, RSU, restricted stock), and the comp-committee governance around them.
- 409A valuation cadence and the strike-price mechanics.
- Repricing / exchange programmes and the shareholder-approval mechanics.

Equity documents are legal documents but they are not commercial contracts; they are governed by the comp-committee cadence in mod-105, not by the deal-desk cadence in mod-109 [chapter 02](./02-contract-playbook-and-fallback-position-matrix.md). See [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/).

### mod-107 — performance, promotion, and offboarding

- Separation-and-release agreements — the OWBPA-compliant release, the ADEA-specific 21/45-day and 7-day revocation windows, the age-band disclosure schedule.
- Severance policy and the mechanics that trigger a release.
- The offboarding-side of trade-secret protection (exit interview, return-of-property, reminder-of-continuing-obligations letter).

mod-109 owns the trade-secret programme structurally ([chapter 04](./04-ip-protection-strategy.md)); mod-107 owns the individual offboarding execution. See [mod-107](../mod-107-performance-promotion-and-offboarding/).

### mod-108 — culture, employee experience, and DEI

- The internal AI-usage / acceptable-use policy for employees — the tier framework for approved tools, the red-line data classes, the discipline path when an employee misuses a tool.
- The employee handbook, into which the internal AUP is bound.
- The values-based operationalisation of confidentiality and IP-protection expectations.

mod-108 owns the *internal-behaviour* AUP; mod-109 owns the *customer-facing* AI contract terms. Two documents, two audiences, two owners. The [chapter 06](./06-ai-vendor-contracts-and-ai-dpa-pattern.md) AI-addendum states what the corporation promises its *customers* about AI; the mod-108 AI-usage policy states what the corporation requires of its *employees*. See [mod-108](../mod-108-culture-employee-experience-and-dei/).

### mod-110 — privacy, data governance, and sector compliance

- GDPR / CCPA / HIPAA / SOC 2 / sector-specific privacy regulatory depth.
- The data-classification scheme, the data-inventory / RoPA, and the Article 30 record.
- The privacy-impact / DPIA methodology, the transfer-impact assessment (TIA), and the sub-processor-approval workflow on the substantive side.
- Data-subject-request (DSAR / subject-access-request) operational programme.

mod-109 owns the DPA as *one document in the customer contract stack* and the vendor DPA as *one document in the vendor stack*. mod-110 owns the regulatory analysis that determines what has to be in that document, the data-inventory that makes the DPA truthful, and the substantive privacy analysis that answers subject-request and cross-border-transfer questions. When a customer redlines the DPA, the redline goes to mod-109; the question of whether the redline is compatible with GDPR Article 28 goes to mod-110. See [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).

### mod-111 — corporate governance, board operations, and officer duties

- Corporate-governance and board-level contracts: the NVCA financing suite (stock purchase agreement, amended and restated certificate of incorporation, investors' rights agreement, right-of-first-refusal-and-co-sale agreement, voting agreement), D&O indemnification agreements, the insider-trading policy, related-party transaction approval mechanics.
- Board authorisation of contracts over the officer-authority threshold.
- Section 220 books-and-records demand practice and the responsive-production workflow.

Financing documents are legal documents, but they are governance documents, not commercial contracts. They live under the general counsel's remit but are governed by the board cadence in mod-111, not by the deal-desk cadence in mod-109. See [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).

### mod-112 — enterprise risk, insurance, and compliance

- The insurance programme — cyber, E&O / tech-E&O, D&O, EPLI, general liability, umbrella — including tower construction and policy-language review.
- The risk-register / enterprise-risk-management cadence.
- The SecReview / VendorReview process on the substantive-security side.
- The SOC 2 / ISO 27001 audit programme and the compliance-controls owner map.

mod-109 owns *contractual* insurance clauses — the counterparty's insurance requirements in the MSA, the certificate-of-insurance workflow, the additional-insured / waiver-of-subrogation mechanics. mod-112 owns the *actual* insurance programme — what policies the corporation carries, at what limits, on what forms, with what exclusions. When a customer contract requires $10M of cyber-liability coverage, mod-109 owns the contract clause; mod-112 owns the question of whether the corporation actually has that coverage. See [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/).

### mod-113 — international expansion and global workforce

- Cross-border commercial contract work — governing-law and forum-selection strategy against a non-US counterparty, foreign-language contract execution, choice-of-law analysis under Rome I.
- International contractor arrangements and the permanent-establishment / EOR analysis that surrounds them.
- International-expansion legal structuring — foreign-subsidiary formation, branch-versus-subsidiary election, transfer-pricing setup.
- Country-specific consumer-law and B2B-contract overlays.

The MSA is drafted in mod-109; whether it can be used in Germany without a country-specific supplement is a mod-113 question. See [mod-113](../mod-113-international-expansion-and-global-workforce/).

### mod-114 — operations function design

- General operations function design — the weekly / quarterly business-review cadence, OKR mechanics, the programme-management office.
- The cross-functional reporting rhythm that surfaces legal-ops metrics to the executive team.

The legal-ops team has its own cadence ([chapter 07](./07-clm-stack-and-legal-ops-graduation.md)); the ops-function has the corporation-wide cadence. They are choreographed but not merged. See [mod-114](../mod-114-operations-function-design/).

## What mod-109 defers to non-role tracks

Some questions look like commercial-contract or IP questions but are actually technical, GTM, engineering, or transactional questions that belong to a different curriculum track altogether. mod-109 does not attempt them.

- **`chief-ai-officer-learning` / `head-of-ai-governance-learning` / `ai-risk-engineer-learning`** — AI-model-risk methodology, red-team programme design, evaluation-suite construction, model-risk register, AI-incident-response methodology. The AI-vendor / AI-DPA chapter ([chapter 06](./06-ai-vendor-contracts-and-ai-dpa-pattern.md)) covers *contract terms* for AI; it explicitly does not cover model-risk engineering, red-teaming, or evaluation infrastructure. Those are AI-governance-role artefacts.
- **`startup-product-gtm-curriculum`** — sales-contract negotiation as a *sales-management* discipline. The deal-desk workflow in [chapter 02](./02-contract-playbook-and-fallback-position-matrix.md) is the legal-side of deal desk; the sales-side (quota structure, deal-review committee, forecasting-discipline, deal-slippage analysis) is a GTM-curriculum artefact. The two intersect at the deal desk but they have different owners.
- **`cto-curriculum`** — engineering-side implementation of OSS scanning (CI wiring for FOSSA / Snyk / Black Duck), engineering-side SBOM generation, the developer workflow of license-approval enforcement, the architectural response to a copyleft-contamination finding. mod-109 [chapter 05](./05-open-source-hygiene-and-sbom-programme.md) sets the licence-approval policy and the SBOM requirement; the `cto-curriculum` owns the engineering-side implementation.
- **`startup-exit-curriculum`** — M&A transaction documents (merger agreement, stock purchase agreement, asset purchase agreement, definitive-agreement drafting, disclosure schedules, earn-outs, escrow), IPO transaction documents (S-1 / F-1, underwriting agreement, comfort letters, lock-up agreements), change-of-control-triggered contract flowdown, transaction-side representations-and-warranties insurance. mod-109 owns the *standing* commercial-contract programme; exit-transaction contract work is a distinct curriculum.

## Boundary worked examples

Eight vignettes. Each one arrives on the general counsel's desk in a normal quarter. Each requires routing.

**1. The sales team wants to sign a $500k enterprise deal that includes a customer-requested "AI hallucination indemnification" clause.**
Question: who authors the clause and who approves the exposure? Answer: mod-109 [chapter 06](./06-ai-vendor-contracts-and-ai-dpa-pattern.md) owns the AI-indemnification pattern — the standard structure of what the corporation is willing to indemnify against, the carve-outs (customer misuse, prompt injection, model-output used contrary to documentation), the super-cap position, and the interaction with the standard IP-indemnification. [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) owns the question of whether the insurance tower — cyber, tech-E&O, and any AI-specific rider — actually supports the cap the corporation is being asked to accept. `startup-product-gtm-curriculum` owns the sales-side commercial trade-off analysis: is the deal worth the concession, does it set a precedent for the next ten deals, does it move the fallback matrix. Three owners, one deal.

**2. The engineering team wants to bundle an AGPL v3 library into the SaaS backend.**
Question: who says yes or no? Answer: mod-109 [chapter 05](./05-open-source-hygiene-and-sbom-programme.md) owns the approval decision. AGPL v3 § 13 extends copyleft to network use; the default policy for a proprietary SaaS product is *disapproved*. If engineering wants an exception, the request flows through the OSS-approval workflow in chapter 05, and the answer is almost always "no, use an Apache-2.0 or MIT alternative." `cto-curriculum` owns the engineering-side remediation — the architectural alternatives, the effort to swap the library, the interim quarantine if the library is already in the codebase. mod-109 gates; cto-curriculum implements.

**3. A departing engineer is threatening to take proprietary code to a competitor.**
Question: who runs the response? Answer: mod-109 [chapter 04](./04-ip-protection-strategy.md) owns the trade-secret protection programme — the marking, the access-log posture, the DTSA / state-UTSA cause-of-action architecture, the preservation letter template. mod-103 owns the employment-side PIIA-enforcement analysis — whether the PIIA is enforceable in the departing employee's state, whether the non-solicit / non-compete surface has any hope of adding value, and the choice-of-law question. mod-107 owns the offboarding-side execution — the exit interview, the return-of-property demand, the reminder-of-continuing-obligations letter. Outside counsel is looped in for the litigation posture per the [chapter 08](./08-in-house-vs-outside-counsel-decision-framework.md) trigger list. Four owners, one incident.

**4. A federal-agency prime contractor asks for the corporation's SBOM and CISA SSDF attestation.**
Question: who produces which artefact? Answer: mod-109 [chapter 05](./05-open-source-hygiene-and-sbom-programme.md) owns the SBOM programme end-to-end — the SPDX / CycloneDX format decision, the production cadence, the customer-facing delivery mechanic, and the accompanying license-and-vulnerability disclosure posture. mod-112 owns the security-attestation infrastructure — the SOC 2 evidence, the SSDF self-attestation letter, the CISA-form-repository submission. `cto-curriculum` owns the engineering-side SBOM tooling — the CI wiring, the artefact-signing / provenance step, the vulnerability-triage workflow when Dependabot / Snyk raises a critical.

**5. The finance team wants to sign a $200k / year enterprise CLM subscription.**
Question: who owns the buy? Answer: mod-109 [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md) owns the vendor-onboarding workflow that the CLM vendor has to pass through — the tiered SecReview / privacy review, the vendor MSA / DPA / security-addendum papering. mod-109 [chapter 07](./07-clm-stack-and-legal-ops-graduation.md) owns the *selection* decision itself — which CLM, at what stage of company, with what feature set, and whether the corporation is at the CLM-graduation point or still on a lighter stack. mod-112 owns the SecReview substance for a Tier-1 vendor holding contract data. Finance / procurement owns the spend-authorisation approval under the corporation's spend-policy matrix.

**6. A customer redlines the DPA to demand real-time on-site audit rights.**
Question: how far does the fallback matrix let us go? Answer: mod-109 [chapter 01](./01-customer-contract-suite-msa-sla-dpa-security-aup.md) and [chapter 02](./02-contract-playbook-and-fallback-position-matrix.md) own the fallback position on audit rights — the standard walk-away being that audits are (i) once annually, (ii) on 30-days' written notice, (iii) at the requesting party's expense, (iv) subject to a customary NDA, (v) satisfied by an unredacted SOC 2 Type II where the customer is not a regulated financial-services or healthcare entity, and (vi) not entitling the customer to inspect other customers' data or infrastructure. mod-110 owns the GDPR Article 28(3)(h) regulatory floor — the DPA must at minimum permit the controller "to conduct audits, including inspections" — which is the reason the audit right cannot simply be zeroed out. mod-112 owns the security-programme readiness question — could the corporation actually pass an on-site audit if one were exercised.

**7. The board asks for the current contract-obligation exposure map ahead of a Series-C lead's diligence request.**
Question: where does the answer come from? Answer: mod-109 [chapter 07](./07-clm-stack-and-legal-ops-graduation.md) owns the CLM as the source of truth on contract inventory — the metadata model, the clause library, the query surface that produces "all MSAs with a most-favoured-nation clause," "all deals with an uncapped indemnity," "all contracts with a change-of-control consent right." Producing the exposure map is a mod-109 exercise against the CLM. `startup-exit-curriculum` owns the transaction-side disclosure-schedule mechanics — how the exposure map is translated into the definitive-agreement disclosure schedules if the round converts into a transaction, what representations are qualified by the schedules, and how the schedules are updated between signing and closing.

**8. An employee filed a GDPR Article 15 request for their data held in a Salesforce CRM the corporation is a customer of.**
Question: who fulfils the request? Answer: mod-110 owns the substantive privacy analysis — is the requester a data subject, is the corporation the controller, what is the response window under Article 12, what is the response format, and what redactions / third-party carve-outs apply. mod-109 [chapter 03](./03-vendor-contract-suite-and-onboarding-workflow.md) owns the vendor DPA as *the mechanism* through which the corporation exercises the request against Salesforce — the sub-processor-assistance obligation in the vendor DPA (Article 28(3)(e)), the operational ticket to the vendor's DSR portal, the audit trail. mod-110 answers the question of what has to be done; mod-109 provides the contractual lever that makes the vendor do its part.

## Using this map

- When a new question arrives, look first at "what mod-109 owns." If it maps to one of the eight chapters, mod-109 owns it end-to-end. Do not sub-contract it out reflexively.
- If it does not map cleanly, look at "what mod-109 hands off." Find the sibling module that owns the underlying corporate, employment, privacy, security, governance, or international layer. Route the substantive work there and keep only the contractual instrument in mod-109.
- If the question is transactional (M&A / IPO), technical (AI-model risk, engineering-side OSS tooling), or GTM-cultural (sales-management), look at "what mod-109 defers to non-role tracks." Route it out of the curriculum entirely and coordinate at the seam.
- When two modules could plausibly own the question, apply the pattern: **mod-109 owns the commercial-contract / IP / legal-ops layer; the sibling module owns the substrate underneath.** The customer AI addendum is mod-109; the internal AI-usage policy is mod-108. The DPA-as-document is mod-109; the privacy-regulatory analysis is mod-110. The insurance clause is mod-109; the insurance policy is mod-112. The commercial contract is mod-109; the entity that signs it is mod-101.

The point of the map is not to shrink mod-109's scope. Commercial contracts, IP, and legal ops is a large-surface function that touches every part of the corporation, and mod-109 has to be assertive about what it owns or the vacuum will be filled by well-meaning sales, procurement, and security teams writing their own inconsistent policies. The point of the map is to keep mod-109 *competent within its scope*: focused on the commercial-contract instrument, the IP instrument, and the legal-ops infrastructure, rather than dispersed across corporate governance, privacy regulation, insurance construction, and M&A transaction work it is not competent to lead.

## Summary

- mod-109 owns eight substantive areas end-to-end: the customer contract suite, the contract playbook / deal desk, the vendor contract suite, IP protection strategy, OSS hygiene and the SBOM programme, AI-vendor contracts and the AI-DPA pattern, the CLM stack and legal-ops build-out, and the in-house-versus-outside-counsel decision framework.
- mod-109 hands off to sibling modules along a consistent seam: entity and board work to mod-101 and mod-111; founder legal architecture to mod-102; employment contracts and PIIA enforcement to mod-103; hiring operations to mod-104; equity documents to mod-105; separation agreements and offboarding-side trade-secret execution to mod-107; the internal AI-usage policy to mod-108; privacy-regulatory analysis to mod-110; the insurance programme and security-review substance to mod-112; cross-border overlay to mod-113; corporation-wide cadence to mod-114.
- mod-109 defers AI-model-risk methodology, engineering-side OSS tooling, GTM-side sales-management practice, and M&A / IPO transaction drafting to non-role curriculum tracks.
- The controlling pattern when ownership is disputed: mod-109 owns the *commercial-contract / IP / legal-ops layer*; the sibling module or non-role track owns the *substrate underneath*.
- Two documents are frequently confused and are worth stating twice: (i) mod-108 owns the *internal-employee* AI-usage policy; mod-109 owns the *customer-facing* AI contract terms. (ii) mod-109 owns the DPA-as-document; mod-110 owns the privacy-regulatory analysis that makes the DPA legally correct.
- The eight vignettes are the reference cases. When a new question arrives, find the vignette it most closely resembles and route accordingly.
- The map exists so that mod-109 stays assertive about its scope without overreaching. Legal is the default residual owner of ambiguous work in most corporations, and the map is the tool for pushing back when the residual is not actually mod-109's.
