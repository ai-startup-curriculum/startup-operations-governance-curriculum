# Exercise 01 — MSA / SLA / DPA customer-contract-suite authoring

> Estimated time: **~10 hours** · Related chapter: [01 — The customer contract suite: MSA, SLA, DPA, Security Addendum, AUP](../01-customer-contract-suite-msa-sla-dpa-security-aup.md)

## Problem statement

Lumenbridge Observability is a Series-B B2B SaaS corporation selling an observability-and-data-governance platform into large enterprise data and platform teams. The corporation is 180 employees, Delaware C-corp, closed a $45M Series B thirteen months ago, and is headquartered in a hybrid-cadence office with engineering concentrated in two US metros. Lumenbridge's existing paper is a 7-page click-through MSA inherited from Series-A that was authored before the corporation had an enterprise motion — it has no DPA, no standalone SLA, no Security Addendum, and references an AUP that has never been maintained. The reliability team completed its first SOC 2 Type II six months ago and has an annual third-party pen-test letter dated eight months ago; the corporation has never produced a Shared Assessments SIG-lite response and does not have a sub-processor list published anywhere a customer can find it. The general counsel is three months in-seat, inherited the Series-A paper, and has been given eight weeks by the CEO to publish the six-document bundle and defend it through the first-round redline cycle on the corporation's first Fortune-500 deal.

The deal is in-flight. The counterparty is a Fortune-500 industrials conglomerate; its commercial-counsel office has demanded the "standard contract package" on first ask and has routed the request to procurement, the privacy office, infosec, and the business sponsor in parallel. The deal is $420k ACV in year one with a 15% annual ramp, a 3-year initial term, Enterprise-tier SKU with 500 seats across production and non-production environments, annual prepay. The CFO has heard three specific friction points from the account team's early conversations: counterparty-side commercial counsel has signalled it will push for (i) **unlimited liability for data-breach events**, (ii) **a 30-day termination-for-convenience right** running to the customer, and (iii) **a most-favoured-nation pricing clause** against Lumenbridge's book of enterprise accounts. The general counsel has to publish the six-document bundle, calibrate the Order Form to this specific deal, run the first-round redline response on the three named asks, and audit the cross-references across all six documents so that precedence, Annex II, the sub-processor list, and the AUP incorporation are internally consistent. Author the full package.

## Requirements

### Part A — Master Services Agreement

Draft the full MSA as operative text, not a summary. Cover the chapter-01 clause list:

1. **Order of precedence.** State the ordering explicitly (Order Form > DPA > MSA > SLA > Security Addendum > AUP, or a deliberate departure) with the reasoning carried in a short recital.
2. **Term, termination for cause, termination for convenience.** 3-year initial term with named auto-renewal mechanic, named notice-of-non-renewal window, named cure period on material breach, named payment-breach-shortened-cure posture, and the deliberate **no customer-side termination for convenience** stance (Part G defends this against the counterparty ask).
3. **Payment terms and taxes.** Net 30 from invoice date, late-payment interest, suspension right for extended non-payment, taxes-exclusive stance, cross-border withholding gross-up or evidence-of-withholding requirement.
4. **Warranties.** Limited functionality warranty (Service materially conforms to then-current documentation), workmanlike-performance warranty for any professional services, and the **UCC § 2-316-compliant disclaimer of implied warranties** in bold or all-caps mentioning "merchantability" by name.
5. **Limitation of liability (three-tier).** General cap at 12 months of fees; consequential-damages waiver; super-caps for the named carve-outs (confidentiality, IP indemnification, data breach, gross negligence / wilful misconduct, payment obligations) at specified multiples. Cross-reference the insurance-stack interaction and defer the policy-limit mechanics to [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/).
6. **IP ownership.** Customer owns Customer Data (with the limited aggregated / de-identified improvement licence stated); corporation owns the Service and all underlying IP; perpetual royalty-free feedback licence; residuals posture declared explicitly (adopt or decline).
7. **IP indemnification.** Mutual indemnity with the standard carve-outs (use outside licence, customer modification, combination with non-corporation products, continued use after non-infringing alternative) and the **procure / modify / refund remedy procedure** as the sole-and-exclusive remedy.
8. **Confidentiality, insurance, force majeure, governing law.** Confidentiality section with the NDA interaction stated (supersede or incorporate — do not leave silent coexistence); named insurance minimums across CGL / E&O / cyber-liability / workers' comp / umbrella (do not invent dollar figures beyond chapter 01 — flag figures the policy stack has to confirm with `<!-- needs-research: ... -->`); force majeure with pandemic called out; Delaware governing law with exclusive Delaware venue.

### Part B — Order Form

Author the Order Form template calibrated to this specific deal. Not a generic placeholder — the deal-specific economics:

1. **Effective date, initial term, auto-renewal.** 3-year initial term, named effective date placeholder, renewal mechanic cross-referencing the MSA.
2. **SKU and seats.** Enterprise-tier SKU, 500 seats, production and non-production environments.
3. **Pricing and ramp.** $420k Year 1 ACV, 15% annual ramp, Year 2 and Year 3 ACV computed, annual prepay, invoicing schedule, overage definition and per-unit overage pricing.
4. **Signers.** Authorised-signatory placeholders on both sides with title discipline.
5. **Deal-specific commercial terms carried on the Order Form.** Any pilot carve-in, named-feature commitment, or deal-specific SLA tier modification lands here, not in the MSA.

### Part C — Service Level Agreement

Author the SLA as operative text. Cover:

1. **Uptime tier.** 99.9% monthly availability mapped to the 43.2-minute monthly downtime budget against a 30-day month. Do not commit a higher tier without the underlying architecture backing it — note the chapter-01 warning if the student is tempted to upsell.
2. **Downtime definition.** The measurable health-check-based definition and the standard carve-outs (scheduled maintenance with named notice window, emergency maintenance, force majeure, customer-caused unavailability, third-party dependencies outside the corporation's control — with the chapter-01 note that the third-party carve-out will be contested).
3. **Credit remedy.** Three-tier escalating credit formula (10% / 25% / 50% of monthly fee at defined availability thresholds) with explicit **"sole and exclusive remedy"** language.
4. **Termination for cause on repeated breach.** Named 3-consecutive-months-or-3-in-6-rolling-months termination-for-cause right conceded to the customer.
5. **Support tiers.** P1 through P4 with named initial-response commitments (not resolution times — the SLA must state this distinction) and the executive-escalation path on P1.

### Part D — Data Processing Addendum

Author the DPA as operative text, with annexes. Defer the GDPR Art. 28 regulatory depth and the CCPA / CPRA substantive requirements to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/) — this exercise authors the **structural anatomy** chapter 01 defines. Cover:

1. **Controller / processor characterisation.** Customer-as-controller / corporation-as-processor under GDPR Art. 4(7)–(8); call out any processing (security monitoring, product-improvement analytics) that is genuinely controller-controller rather than processor-only.
2. **Annex I — scope of processing.** Categories of data subjects, categories of personal data, nature and purpose of processing, duration, special-category treatment.
3. **Annex II — TOMs.** Mirror or cross-reference the Part E Security Addendum; the two documents must not contradict (Part H audits this).
4. **Sub-processor list and change notification.** 30-day change-notification mechanic, named published-URL location for the live sub-processor list, customer objection and affected-service termination path.
5. **International transfers.** EU Standard Contractual Clauses incorporated under [Commission Implementing Decision (EU) 2021/914](https://eur-lex.europa.eu/eli/dec_impl/2021/914/oj) (all four modules), UK IDTA (or UK Addendum to the EU SCCs), Swiss addendum for FADP transfers, DPF schedule for the US importer where applicable. Carry all applicable mechanisms so a change in data-flow topology does not force re-signing.
6. **CCPA service-provider addendum.** Structural placeholder referencing Cal. Civ. Code § 1798.140(ag) — defer the substantive US-state-privacy drafting to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/).
7. **Breach notification, audit rights, deletion / return.** 72-hour processor-to-controller breach-notification commitment with named information-scope; **SOC 2 Type II report in lieu of on-site audit** with the specific-incident-triggered on-site-audit carve-back; deletion-or-return-at-customer-option on termination with the legally-required-retention and IT-backup carve-outs.

### Part E — Security Addendum / SIG-lite-ready response

Author the Security Addendum as a standalone document that could also be delivered as a completed Shared Assessments SIG-lite response. Cover:

1. **Certifications and attestations.** SOC 2 Type II (named report date, named audit window, delivery under NDA within one business day); pen-test summary letter posture; posture on ISO 27001 / FedRAMP / HITRUST / PCI-DSS (adopt, roadmap, or decline — do not overstate).
2. **Encryption.** TLS 1.2+ in transit, AES-256 at rest, named key-management posture.
3. **Authentication.** MFA for all Lumenbridge personnel with production access; SSO / SAML support on the Enterprise SKU.
4. **Access control.** Least-privilege, RBAC, quarterly access-review cadence.
5. **Logging, monitoring, incident response.** 24×7 monitoring, defined IR process, breach-notification timelines aligned to the Part D DPA.
6. **Business continuity and disaster recovery.** Named RTO / RPO commitments, backup frequency, tested-failover posture (do not invent figures — flag with `<!-- needs-research: ... -->` where the reliability team must confirm).
7. **Personnel security.** Background checks, security training on hire and annually, offboarding process.
8. **Sub-processor / vendor management.** Alignment to the Part D DPA mechanic.

### Part F — Acceptable Use Policy

Author the AUP as a unilateral, publishable document, with the chapter-01 suspension-right mechanic. Cover:

1. **Prohibited uses.** Illegal use (CFAA, export-controls, sanctions, CSAM); harassment and abuse; malware and security threats (including DoS, port scanning, unauthorised access attempts); high-volume automation and rate-limit abuse without prior permission; benchmarking-and-publishing without permission; reverse engineering beyond what law permits notwithstanding contractual restriction; circumvention of access controls or usage limits.
2. **Suspension right.** Immediate suspension for critical violations; notice-and-opportunity-to-cure for lesser violations; explicit **suspension-does-not-entitle-customer-to-SLA-credit** and **does-not-toll-payment-obligation** carve-outs.
3. **Update mechanic.** 30-day notice posture with the MSA's notice-clause cross-reference.

### Part G — First-round-redline response memo

The counterparty's commercial counsel has returned the first redline with the three named asks. Author the written redline-response memo the general counsel will send back, grounded in chapter 01 and the fallback-position matrix carried in [chapter 02](../02-contract-playbook-and-fallback-position-matrix.md). Cover each ask:

1. **Unlimited liability for data-breach events.** Name Lumenbridge's acceptable position (super-cap at a named multiple of annual fees aligned to the cyber-liability policy stack), the walk-away position, and the written counter-language. Reference the chapter-01 note that the cap must never exceed insurance limits; defer the specific policy-limit confirmation to [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/).
2. **30-day customer-side termination for convenience.** Chapter-01 default is "no." Name the counter: either refuse outright with the initial-term-economics defence, or concede with a **cancellation fee equal to the remaining committed spend** that converts TfC into early payoff. Name the fallback and the walk-away.
3. **Pricing MFN against the enterprise book.** Name Lumenbridge's position (decline — MFN is operationally untenable at Series-B and causes revenue-leak across the book), the fallback (narrow MFN limited to like-for-like SKU, like-for-like volume, like-for-like term, with carve-outs for pilots, strategic design partners, and non-arm's-length deals), and the walk-away. Any specific win-rate or industry MFN-concession benchmark that is not in chapter 01, chapter 02, or `resources.md` gets `<!-- needs-research: ... -->`.

Carry the memo in the voice of the general counsel writing to the account team and the CFO, not to the counterparty — the counter-redline itself is a separate internal attachment.

### Part H — Cross-reference audit

Author the audit document the general counsel runs across the six-document bundle before sending the first draft. Cover:

1. **Order-of-precedence consistency.** Precedence stated in the MSA matches the incorporation-by-reference clauses in each attached document; no document silently claims superiority.
2. **DPA Annex II vs. Security Addendum.** The two documents cover the same controls and do not contradict on encryption posture, MFA, access-review cadence, RTO / RPO, or incident-response timelines.
3. **Sub-processor list synchronisation.** The DPA's named sub-processor list (and its published URL) matches the Security Addendum's vendor-management statement; both match the sub-processor inventory the reliability team actually maintains.
4. **AUP incorporation reference.** The MSA incorporates the then-current AUP by reference with a named notice mechanic; the AUP's suspension-does-not-entitle-SLA-credit carve-out is consistent with the SLA's credit-remedy clause.
5. **Governing-law and notice-clause consistency.** All six documents reference the same governing law, same notice address, and same notice mechanic — no stray older-template references.
6. **Internal-defined-terms audit.** "Service," "Customer Data," "Confidential Information," "Personal Data," and "AUP" are defined once (in the MSA) and used consistently across the bundle.

## Starter guidance

- Chapter 01 is the primary reference. Each named clause in Parts A through F maps directly to a chapter-01 section — reread the "MSA architecture," "SLA design," "DPA structure," "Security Addendum and SIG-lite response," and "Acceptable Use Policy" sections before drafting.
- The fallback-position matrix for the three named counterparty asks lives in [chapter 02](../02-contract-playbook-and-fallback-position-matrix.md). Part G is a chapter-02 output; reference it, do not re-derive the matrix.
- Defer the **GDPR Art. 28 processor-obligation depth**, the **CCPA / CPRA substantive language**, the **HIPAA BAA mechanics**, and the US-state-privacy map to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/). This exercise authors the structural anatomy chapter 01 defines, not the regulatory depth.
- Defer the **insurance policy-limit mechanics** (CGL / E&O / cyber-liability / umbrella layer design) to [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/). The MSA states insurance minimums; the policy stack confirms whether Lumenbridge can carry them.
- Defer the **CLM-stack publication, versioning, and clause-library mechanics** to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md). This exercise produces the paper; chapter 07 governs how it is managed and reused.
- Defer the **IP-protection posture** (trade-secret regime, patent strategy, copyright) that sits behind the IP-ownership and IP-indemnification clauses to [chapter 04](../04-ip-protection-strategy.md).
- Defer the **open-source hygiene posture** that sits behind the warranty, IP, and SBOM-expectations stance to [chapter 05](../05-open-source-hygiene-and-sbom-programme.md).
- Do not invent **real counterparty names, real law-firm engagement details, or real policy-limit figures**. Where chapter 01 and `resources.md` carry a figure, use it; where they do not, propagate `<!-- needs-research: ... -->` markers so the general counsel can refresh before publication. Do not leave `[TBD]` or `[FILL IN]` placeholders.
- Do not invent **real industry benchmarks** on cap multiples, super-cap multiples, breach-notification turnaround, or MFN-concession rates. If the figure is not in chapter 01, chapter 02, or `resources.md`, flag it.
- The redline-response memo in Part G is written to Lumenbridge's internal account team and CFO, not to the counterparty. The counter-redline language is a separate internal attachment the general counsel can lift from the memo.
- The cross-reference audit in Part H is not optional and is not a summary — it is the specific check-list the general counsel runs before sending the draft. Each named check must have a stated outcome, not just a question.

## Deliverables

- `msa.md` — Part A.
- `order-form.md` — Part B.
- `sla.md` — Part C.
- `dpa.md` — Part D (with Annex I and Annex II inline).
- `security-addendum.md` — Part E.
- `aup.md` — Part F.
- `redline-response-memo.md` — Part G.
- `cross-reference-audit.md` — Part H.

## Acceptance criteria

The package is acceptable if:

1. Part A's MSA is operative text (not a summary), covers all nine named clause areas (order of precedence; term and termination; payment and taxes; warranties with UCC § 2-316-compliant disclaimer; three-tier limitation of liability; IP ownership; IP indemnification with procure / modify / refund; confidentiality, insurance, force majeure, governing law), and states the no-customer-side-termination-for-convenience posture explicitly.
2. Part B's Order Form is calibrated to the specific $420k ACV / 15% annual ramp / 3-year / 500-seat Enterprise-tier deal, computes the Year 2 and Year 3 ACV, and names overage mechanics without re-opening MSA clauses.
3. Part C's SLA sets 99.9% availability mapped to the 43.2-minute monthly downtime budget, defines downtime measurably with the named carve-outs, carries the three-tier escalating credit remedy with explicit "sole and exclusive remedy" language, concedes termination-for-cause on repeated breach, and separates P1–P4 initial-response commitments from resolution-time commitments.
4. Part D's DPA covers controller / processor characterisation, Annex I scope, Annex II TOMs cross-referenced to Part E, sub-processor list with 30-day change notification, international-transfer schedule (EU SCCs per Commission Implementing Decision (EU) 2021/914, UK IDTA, Swiss addendum, DPF), CCPA service-provider addendum placeholder, 72-hour breach-notification, SOC 2 Type II in lieu of on-site audit, and deletion / return on termination — and defers GDPR Art. 28 and CCPA / CPRA substantive depth to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/).
5. Part E's Security Addendum covers certifications, pen-test summary, encryption at rest and in transit, MFA / SSO, access control, logging / monitoring / incident response, BC / DR with RTO / RPO, personnel security, and sub-processor management — and does not contradict the Part D DPA on any control.
6. Part F's AUP covers the chapter-01 prohibition list (illegal use, harassment, malware / attacks, high-volume automation, benchmarking without permission, reverse engineering, circumvention) with the suspension-right mechanic and the explicit SLA-credit and payment-obligation carve-outs.
7. Part G's redline-response memo answers each of the three named counterparty asks (unlimited data-breach liability, 30-day customer-side termination for convenience, pricing MFN) with a named acceptable position, a named fallback, a named walk-away, and counter-language — grounded in chapter 01 and the [chapter 02](../02-contract-playbook-and-fallback-position-matrix.md) fallback matrix.
8. Part H's cross-reference audit runs the six named checks (precedence consistency, DPA Annex II vs. Security Addendum, sub-processor list sync, AUP incorporation, governing-law and notice-clause consistency, defined-terms audit) and states an outcome for each, not just a question.
9. **The six-document bundle is internally consistent.** Order of precedence stated in the MSA matches the incorporation clauses in each attached document; the DPA Annex II and the Security Addendum do not contradict; the sub-processor list is referenced consistently; defined terms are defined once and used consistently.
10. Any figure not in chapter 01, chapter 02, or `resources.md` is flagged with `<!-- needs-research: ... -->` — specific insurance policy limits, specific sub-processor identities, cap-multiple benchmarks, MFN-concession rates, RTO / RPO figures the reliability team has not yet confirmed. No real counterparty names, real law-firm names, or real policy-limit figures are invented. Nothing is left as `[TBD]` or `[FILL IN]`.
11. Deferrals to sibling modules are named explicitly where the chapter-01 ownership boundary assigns the mechanic elsewhere — [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/) for GDPR Art. 28 and CCPA / CPRA substantive depth, [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/) for the insurance stack confirming the liability-cap ceiling, [chapter 02](../02-contract-playbook-and-fallback-position-matrix.md) for the fallback-position matrix behind Part G, [chapter 04](../04-ip-protection-strategy.md) for the IP-protection posture behind the IP clauses, [chapter 05](../05-open-source-hygiene-and-sbom-programme.md) for the open-source hygiene posture behind the warranty and IP stance, and [chapter 07](../07-clm-stack-and-legal-ops-graduation.md) for the CLM-stack publication and clause-library mechanics.
12. Lumenbridge Observability is used as the authored corporation throughout; no real company name is substituted. The $420k / 15% ramp / 3-year / Fortune-500 industrials-counterparty scenario is reflected in Part B's Order Form and Part G's redline-response memo — the paper is not written as a generic template divorced from the deal.
