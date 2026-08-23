# 2. The contract playbook and fallback-position matrix

> Every clause the corporation negotiates has three pre-decided answers: what it opens with, what it will accept, and what it will walk from. Write those answers down, publish them to sales and deal-desk, and the negotiation stops being a one-lawyer-per-deal cottage industry.

## Motivation

[Chapter 01](./01-customer-contract-suite-msa-sla-dpa-security-aup.md) defines the document architecture — MSA, SLA, DPA, security exhibit, AUP — and the substantive clauses the corporation publishes as its paper. This chapter is about the second-order artefact that turns those documents from a starting point into a repeatable negotiation: the **contract playbook**.

The failure mode without a playbook is familiar. Every deal is a bespoke exercise. Sales sends a redline over to counsel; counsel reads the whole contract from scratch; counsel makes a judgement about whether the counterparty's proposed language is acceptable; counsel sends a reply. The next deal arrives, and a different counsel — or the same counsel on a different day — makes a subtly different judgement on the same clause. The corporation cannot tell sales in advance what it will and won't accept, so sales cannot close cleanly, and the redline cycle stretches to weeks. When the corporation grows past ten or twenty deals per quarter, the model breaks.

A playbook is the fix. It is a per-clause reference document that captures, for every negotiable clause in the corporation's contract suite: the **ideal** position (what the corporation opens with — its published paper), the **acceptable** position (what the corporation will agree to without escalation), the **walk-away** position (the point past which the deal is not worth doing on those terms), the **pre-approved trade-offs** (what the corporation will give up on Clause X in exchange for holding on Clause Y), and the **negotiation moves** (specific language and rhetorical tactics that have historically closed the point). The playbook lets a trained deal-desk analyst or sales operations person triage 80% of counterparty markups without counsel's involvement and lets counsel intervene only where the markup actually crosses a boundary.

The playbook is not a legal document. It is an internal operations document, revised quarterly, owned by the general counsel or head of legal ops in collaboration with the head of sales.

## What a contract playbook actually is

A playbook is a clause-indexed table. Its rows are the negotiable clauses in the corporation's contract suite; its columns are (at minimum) ideal, acceptable, walk-away, trade-offs, and rationale. A mature playbook adds columns for market-precedent notes ("Salesforce accepts this in their standard paper"), deal-size gating ("acceptable position applies to deals ≤ $100k ARR; larger deals get the ideal only"), and links to the underlying template clause.

The playbook covers only the clauses that actually get negotiated. Boilerplate that never draws a redline — the choice of counterparts, the severability clause, the notice-address mechanics — is not playbook material. What draws redlines, and therefore what the playbook must cover, is roughly two dozen clauses across the MSA, SLA, DPA, and order form. The rest of this chapter walks the clause list.

The playbook has three audiences. **Deal-desk / legal-ops** uses it to triage counterparty redlines and route deals — most redlines can be answered directly from the playbook without escalation. **Sales** uses it to set expectations with the counterparty in real time ("we don't offer termination for convenience, but we can offer a mid-term termination right if you miss our SLA for three consecutive months"). **Counsel** uses it as the authoritative statement of what has been pre-approved so that counsel's time is spent on the genuinely novel or edge-case markup, not on re-litigating the same three clauses every deal.

## The clause-by-clause fallback matrix

The tables below present the corporation's default positions for the clauses that draw the most redlines. Each row states the ideal (what the corporation's paper says), the acceptable (what the corporation will agree to without escalation to counsel or executive), and the walk-away (the point at which the corporation should either escalate or decline the deal). Numbers and thresholds shown are illustrative of common startup-SaaS practice; the corporation should calibrate to its own risk tolerance, ARR, and insurance limits.

### Limitation of liability

| Position | Direct-damages cap | Excluded consequential damages | Enhanced-remedy carve-outs |
|---|---|---|---|
| Ideal | Fees paid in the 12 months preceding the claim | Full waiver of indirect, consequential, incidental, special, punitive, and lost-profits damages by both parties | Carve-outs limited to: (a) breach of confidentiality — 2x fees cap; (b) IP indemnification — 2x fees cap; (c) breach of DPA / data security — 2x fees cap; (d) gross negligence, wilful misconduct, and fraud — uncapped |
| Acceptable | 12 months' fees for standard deals; 24 months' fees for enterprise deals ≥ $250k ARR | Same as ideal | Super-cap of 3x fees for the enumerated carve-outs; uncapped only for gross negligence, wilful misconduct, and fraud |
| Walk-away | Any uncapped direct-damages liability on the corporation's ordinary performance | Removal of the mutual consequential-damages waiver (i.e., counterparty demands one-sided waiver in its favour) | Full uncapped liability for data breach, IP infringement, or confidentiality — insurance won't respond and the deal is not worth the tail risk |

Notes: The direct-damages cap is often the single most-negotiated clause. Enterprise counterparties routinely push for 2x or 3x fees on the direct cap and super-caps of 3x–5x on the enhanced-remedy items. The corporation's [insurance program](../mod-105-workplace-safety-and-insurance-program/) — tech E&O / cyber tower — sets the practical ceiling; do not agree to a cap that exceeds available insurance limits by an order of magnitude without underwriter conversation. See [chapter 01](./01-customer-contract-suite-msa-sla-dpa-security-aup.md) for the underlying clause language.

### Indemnification

| Position | IP indemnification | Customer content indemnification | Procedure and control |
|---|---|---|---|
| Ideal | Provider defends and indemnifies customer against third-party claims that the Service (as delivered by provider and used within scope) infringes a US patent, copyright, trademark, or trade secret; enhanced-remedy escape — modify, replace, or refund unused fees and terminate | Customer defends and indemnifies provider against third-party claims arising from Customer Data or customer's use in breach of the AUP | Sole control of defence and settlement by indemnifying party; indemnified party gives prompt written notice and reasonable cooperation; no settlement that admits liability or imposes non-monetary obligations on indemnified party without consent |
| Acceptable | Same as ideal, plus indemnification for wilful infringement and for combination claims where the Service itself would infringe standalone; drop the "US only" limitation for enterprise customers with international operations | Same as ideal | Joint control on high-stakes claims (defence by indemnifying party, but indemnified party may participate at its own expense with its own counsel) |
| Walk-away | Indemnification without the modify / replace / refund escape; indemnification of combination claims where the combination is with counterparty-supplied components; indemnification for open-source components counterparty selected | Removal of customer's reciprocal indemnification for its content and use | Loss of control of defence — the indemnifying party must control the defence or it cannot manage its exposure |

Notes: The IP indemnification is where AI-enabled products draw the sharpest redlines today. Enterprise counterparties are increasingly demanding uncapped IP indemnification for AI-generated output, and the corporation's position on this belongs in [chapter 06](./06-ai-and-model-contracts-inbound-and-outbound.md). The DPA-side indemnification for data-protection violations is treated separately in the DPA and cross-references [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/).

### IP ownership

| Position | Service and IP | Customer Data | Feedback and aggregated data |
|---|---|---|---|
| Ideal | Provider owns all right, title, and interest in the Service, the platform, and any improvements or derivatives thereof, including all IP created by provider personnel in the course of performance | Customer owns Customer Data; provider gets a limited licence to process Customer Data solely to provide the Service | Provider gets a perpetual, royalty-free licence to use feedback for any purpose without attribution; provider may generate and use aggregated / de-identified usage data for any lawful purpose |
| Acceptable | Same as ideal | Same as ideal | Feedback licence stays; aggregated / de-identified data licence narrowed to internal analytics, benchmarking, and product improvement; explicit prohibition on re-identification |
| Walk-away | Any customer claim to ownership of the Service, of provider improvements, or of provider-developed IP arising from customer's use | Provider ownership of Customer Data, or a provider licence to Customer Data broader than "solely to provide the Service" | Loss of the aggregated / de-identified data right entirely — this is often material to the corporation's product-improvement pipeline and its model-training pipeline; if lost, the deal economics must reflect the loss |

Notes: The aggregated / de-identified usage clause is contested in regulated verticals (healthcare, finance, education) and is often the primary reason a customer requires a bespoke DPA. See [chapter 06](./06-ai-and-model-contracts-inbound-and-outbound.md) for the model-training variant.

### Warranty

| Position | Functionality warranty | Performance warranty | Disclaimer |
|---|---|---|---|
| Ideal | Service will materially conform to its documentation | Service will be performed in a workmanlike manner consistent with generally-accepted industry standards | Explicit disclaimer of all implied warranties (merchantability, fitness for a particular purpose, non-infringement, and title beyond what is expressly warranted) |
| Acceptable | Same as ideal, plus a 30-day cure period; sole remedy is re-performance or, if re-performance fails, a pro-rata refund of prepaid fees for the non-conforming portion | Same as ideal | Disclaimer stays; may narrow to acknowledge that provider is not disclaiming warranties that cannot be disclaimed under applicable law |
| Walk-away | Uncapped functional warranty ("Service will perform without error"); acceptance-testing regime that lets counterparty reject the Service after go-live | Warranty tied to specific business outcomes for the customer that the corporation cannot control | Loss of the implied-warranty disclaimer entirely — this reopens exposure that no reasonable SaaS provider takes on |

### Termination for convenience

| Position | Provider termination for convenience | Customer termination for convenience |
|---|---|---|
| Ideal | Not permitted during the initial term or any renewal term | Not permitted during the initial term or any renewal term; termination only for material breach with cure period |
| Acceptable | Not permitted | 30-, 60-, or 90-day termination for convenience with pro-rata refund of prepaid but unused fees; no refund of fees for the period consumed |
| Walk-away | Any right for provider to terminate for convenience mid-term without cause | Termination for convenience without notice period, or termination for convenience with refund of already-consumed fees |

Notes: Termination for convenience is usually a hard "no" from the corporation because it destroys forecast reliability and the CAC-payback model. Enterprise customers occasionally have procurement policies that require it; the acceptable-position row is the fallback for those cases.

### SLA credits and enhanced remedy

| Position | Service credit | Enhanced remedy |
|---|---|---|
| Ideal | Tiered credits (5% / 10% / 25% of monthly fees) for defined uptime tiers below the SLA target; sole and exclusive remedy for missed SLA; customer must claim credits in writing within 30 days | None; SLA credits are the sole remedy |
| Acceptable | Same as ideal | Termination-for-cause right if the provider misses the SLA in 3 consecutive months or 3 out of any 6 months; on termination, pro-rata refund of prepaid fees for the terminated portion |
| Walk-away | Uncapped SLA damages beyond the credit; SLA credits calculated on ARR rather than monthly fees; per-incident damages liability | Termination-with-refund after a single missed month; automatic refund without customer claim |

See [chapter 01](./01-customer-contract-suite-msa-sla-dpa-security-aup.md) for the underlying SLA architecture.

### MFN (Most Favoured Nation)

| Position | MFN scope |
|---|---|
| Ideal | No MFN. The corporation does not offer pricing MFN, terms MFN, or feature MFN. |
| Acceptable | Pricing MFN narrowly scoped to: (a) same product SKU, (b) same tier of usage, (c) same contract length, (d) same customer segment (measured by ARR band); explicitly excludes promotional pricing, pilot pricing, strategic-account pricing, and pricing to affiliates of the counterparty; measurement window limited to net-new customers signed during the applicable period; enforceable only by contract audit at counterparty's expense |
| Walk-away | Feature MFN (any feature offered to any customer must be offered to this one); terms MFN (any terms accepted for any customer flow to this one); undefined-scope pricing MFN; MFN measured against every existing customer |

Notes: MFN clauses are a compounding drag on pricing strategy. Every MFN accepted narrows the future space of deals the corporation can do. Resist aggressively; where accepted, scope tightly and log the obligation in the CLM ([chapter 07](./07-clm-stack-signature-storage-obligation-tracking.md)).

### Audit rights

| Position | Compliance audit | Financial audit |
|---|---|---|
| Ideal | SOC 2 Type II report delivered annually in lieu of on-site audit; customer may request penetration-test summary letter; no on-site audit rights | Not permitted; the corporation is a licensor, not a licensee — there is nothing for the customer to audit financially |
| Acceptable | SOC 2 in lieu of on-site; if regulated customer (financial services, healthcare) has statutory audit rights, on-site audit once per calendar year with 30 days' written notice, at customer's expense, during business hours, subject to NDA and reasonable security requirements, limited to systems processing customer's data | Not permitted |
| Walk-away | On-demand on-site audit; audit at provider's expense; audit of source code, business records, or other customers' data; audit by a competitor of the provider | Any financial audit right |

### Renewal and auto-renewal

| Position | Renewal mechanism | Notice window |
|---|---|---|
| Ideal | Auto-renew for successive terms equal to the initial term unless either party gives written notice of non-renewal at least 60 days before the end of the then-current term; renewal at then-current list pricing (or with a specified uplift cap, e.g., CPI plus 5%) | 60 days |
| Acceptable | Auto-renew with 30-, 60-, or 90-day non-renewal window; uplift cap of CPI, CPI+3%, or a fixed percentage; some enterprise customers require affirmative (opt-in) renewal — accept for large deals if the customer commits to a renewal-decision milestone in the contract | 30 to 120 days |
| Walk-away | Auto-renewal with less than 30 days' notice window (many state auto-renewal statutes require clearer notice — see the California ARL, Cal. Bus. & Prof. Code § 17600 et seq., and the equivalents in NY, IL, and others, which apply to consumer contracts but have influenced enterprise practice); indefinite auto-renewal without a rate mechanism; auto-renewal without a corresponding provider non-renewal right |

Notes: The state auto-renewal statutes primarily target consumer contracts but the compliance discipline (clear disclosure, easy cancellation) is a good baseline. See [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) for state-consumer-law crosswalks.

### Assignment

| Position | Assignment scope |
|---|---|
| Ideal | Neither party may assign without the other's prior written consent, except that either party may assign without consent to (a) an affiliate under common control, or (b) a successor in interest by merger, acquisition, reorganisation, or sale of all or substantially all assets |
| Acceptable | Same as ideal, with the qualifier that consent will not be unreasonably withheld, conditioned, or delayed; carve-out for assignment to a direct competitor of the non-assigning party requires consent regardless |
| Walk-away | Free assignability by counterparty (loss of change-of-control control); prohibition on the corporation's assignment to a successor in a bona fide M&A transaction |

### Governing law and venue

| Position | Governing law | Venue |
|---|---|---|
| Ideal | Delaware (if Delaware C-Corp) or the corporation's home state, without regard to conflicts principles; UCC applies to the extent applicable | Exclusive jurisdiction in state and federal courts of the corporation's home county / state; mutual waiver of forum non conveniens |
| Acceptable | Neutral state (Delaware, New York) if counterparty resists home state; New York if counterparty is a New York financial institution; California if counterparty is California-based and refuses to leave state | Neutral venue in the chosen state; JAMS or AAA arbitration in the chosen state |
| Walk-away | Counterparty's home state where that state has plaintiff-friendly consumer-protection statutes that apply to the deal; foreign-law governance for a US-only deal; UN Convention on Contracts for the International Sale of Goods (should always be excluded) |

### Confidentiality term

| Position | Term |
|---|---|
| Ideal | Confidential Information: 5 years from disclosure; Trade Secrets: indefinite, as long as the information qualifies as a trade secret under applicable law (DTSA / state UTSA) |
| Acceptable | 3 to 7 years for Confidential Information; indefinite for trade secrets; alternatively, "for the term of the Agreement plus 5 years" for tied-to-relationship structure |
| Walk-away | Indefinite confidentiality for all Confidential Information without a trade-secret carve-out (unenforceable in some jurisdictions and impractical to operationalise); term of less than 2 years for Confidential Information |

See [mod-103 chapter 05](../mod-103-employment-law-and-contract-design/05-nda-and-mnda-layer.md) for the NDA-layer treatment of the same concepts.

### Data breach notification window

| Position | Notification timeline |
|---|---|
| Ideal | Without undue delay, and in any event within 72 hours of provider's confirmed determination that a Security Incident affecting Customer Data has occurred (aligns with GDPR Article 33 and general US practice) |
| Acceptable | 48 hours from confirmation; some financial-services customers require 24 hours from detection (not confirmation) — accept only where the customer will accept "detection of a suspected Security Incident" language rather than certainty of an actual incident |
| Walk-away | Notification obligation triggered on mere suspicion without an investigation window; notification measured in hours from the initial alert rather than from confirmed determination; notification obligations that override applicable law-enforcement or regulator instructions to delay notification |

Notes: Every US state has a breach-notification statute; the state statutes apply to notification to *individuals*, not to notification to the corporation's customers. The contract clause here governs the B2B provider-to-customer notification. HIPAA (45 C.F.R. § 164.410) requires business-associate notification without unreasonable delay and no later than 60 days. See [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/) for the state-and-sector detail.

### Publicity and logo rights

| Position | Marketing use |
|---|---|
| Ideal | Provider may use customer's name and logo on its website, marketing collateral, and investor materials; customer may reference the relationship in its own materials subject to trademark guidelines |
| Acceptable | Provider may use customer's name and logo with prior written consent, not to be unreasonably withheld, on customer-list pages and in generic marketing collateral; case studies and quotes require specific written approval; some enterprise customers grant a one-time press-release right at signing in lieu of an ongoing logo licence |
| Walk-away | No provision either way (silence tends to be read as no consent); prohibition on the corporation's naming the customer as a customer in confidential investor materials |

### Insurance

| Position | Coverage |
|---|---|
| Ideal | Commercial General Liability $1M/$2M; Professional Liability / Tech E&O $2M–$5M; Cyber Liability $2M–$5M; Workers' Compensation as required by law; Employer's Liability $1M; Umbrella at the corporation's discretion |
| Acceptable | Same base coverages; Tech E&O and Cyber may be pushed to $5M–$10M for enterprise deals or regulated verticals; Umbrella coverage $5M–$25M for the largest deals; customer named as additional insured on CGL only (not on E&O / Cyber, which do not accept AI endorsements) |
| Walk-away | Coverage limits that the corporation cannot procure at commercially reasonable premiums; naming the customer as additional insured on Cyber or Tech E&O (typically not available and would invalidate the policy); waivers of subrogation on all policies (some are acceptable, some invalidate coverage) |

See [mod-105](../mod-105-workplace-safety-and-insurance-program/) for the full insurance program design.

## Internal-legal-turn SLA by growth stage

The playbook is only half the operational discipline. The other half is a published internal service level for how quickly counsel or deal-desk turns a redline back to sales and to the counterparty. Without a published turnaround SLA, sales cannot forecast close dates and the counterparty cannot plan procurement.

Typical turnaround by stage:

- **Pre-seed / seed.** No in-house counsel. One part-time outside counsel or a fractional GC. Turnaround: 3 to 7 business days per redline round is realistic and typical. Sales must set expectations accordingly.
- **Series A.** A first-in-house GC or a full-time head of legal ops. Turnaround: 3 to 5 business days per redline round for non-standard deals; 1 to 2 business days for standard deals that hit the playbook cleanly.
- **Series B.** A legal-ops function with 2 to 4 people (GC, deal-desk analysts, contract-lifecycle-management operator). Turnaround: 24 to 48 hours for standard deals; 3 to 5 business days for non-standard; escalation path to outside counsel for bespoke.
- **Series C+.** A fully-staffed legal ops with deal desk, contract-lifecycle-management platform ([chapter 07](./07-clm-stack-signature-storage-obligation-tracking.md)), and integrated Salesforce workflow. Turnaround: same-day for standard bundles that pass playbook checks; 24 to 48 hours for non-standard; 3 to 5 business days for bespoke.

The published SLA is a commitment to the sales organisation. Missed SLA counts against the legal-ops team's metrics ([see below](#metrics-that-matter)) and drives capacity planning for outside-counsel augmentation and additional headcount.

## The deal-desk model

A deal desk is a lightweight intake-and-triage function that stands between sales and counsel. Its purpose is to make the routing decision — standard, non-standard, or bespoke — so that counsel's time is not consumed on redlines the playbook already answers.

**Intake.** The deal enters the queue through one of several channels: a Slack channel with a bot that opens a ticket, an Airtable or Notion form, a Google Form, or a purpose-built request form in the CLM. The intake captures deal size, customer segment, counterparty name (for existing-customer or existing-precedent lookup), counterparty's redline (as an attached document or as a link to a working document), and the salesperson's summary of the disputed points.

**Tiered review.** The desk applies a tier:

- **Standard.** Counterparty accepts the corporation's paper with only cosmetic edits, or the redline hits only playbook-acceptable positions on playbook clauses. Deal-desk analyst can approve without counsel review; contract can go to signature.
- **Non-standard.** Redline crosses one or more playbook-acceptable boundaries but does not cross a walk-away. Deal-desk analyst routes to in-house counsel for review, applying playbook trade-offs pre-approved. Counsel confirms, negotiates specific points, and returns to sales.
- **Bespoke.** Redline crosses one or more walk-away positions, or the counterparty is proposing terms the playbook does not address (novel data-residency, novel AI-usage terms, uncapped liability, government-contracting flowdowns). Deal-desk analyst routes to in-house counsel; counsel decides whether to escalate to outside counsel or to executive (CFO, CEO) for commercial approval on the deviation.

The tier determines both who touches the deal and the turnaround target. A standard deal at Series C should close same-day; a bespoke deal at any stage may take 2 to 4 weeks and requires executive sponsorship.

## Escalation-to-outside-counsel decision framework

Not every non-standard deal warrants outside-counsel engagement. Outside counsel is expensive and slow compared to in-house counsel with the playbook. The decision framework should be published so that in-house counsel and deal-desk can apply it consistently.

Common escalation triggers:

- **Deal size above a threshold.** Typical thresholds: $250k ARR at Series A, $500k at Series B, $1M or more at Series C. The threshold captures deals where the tail-risk exposure is meaningful and where the counterparty is likely represented by sophisticated outside counsel on their side.
- **Unfamiliar regulated industry.** First deal in healthcare (HIPAA business-associate agreement flowdowns), financial services (GLBA, NYDFS Part 500, FFIEC guidance), education (FERPA), or a new jurisdiction. Outside counsel with the sector specialty should touch the first deal in each sector; subsequent deals in that sector should be handleable by in-house counsel using the sector-specific supplement to the playbook.
- **Government contracting.** Federal, state, or local government deals bring flowdown clauses (FAR / DFARS for federal, state-specific for state), Buy American Act, security requirements (CMMC, FedRAMP), and audit rights that the standard-commercial playbook does not cover. Always outside counsel for the first several government deals.
- **Aggressive IP terms.** Any customer claim to ownership of the Service, IP indemnification obligations without the modify / replace / refund escape, or joint-development structures where IP allocation matters.
- **Large uncapped liability.** Any request for uncapped liability beyond the corporation's standard carve-outs (gross negligence, wilful misconduct, fraud) — especially uncapped IP indemnification, uncapped data-breach indemnification, or uncapped consequential damages.
- **Non-standard indemnification.** Indemnification for third-party service providers, indemnification for customer's regulatory compliance, indemnification for customer's own employees' actions.
- **Custom data-residency.** Requirements to keep Customer Data within a specific geography, in a customer-controlled key-management environment, or in a sovereign-cloud region. These often require infrastructure changes and separate contractual commitments — engineering, legal, and procurement all need to weigh in.
- **Novel AI terms.** Counterparty demands about training data, model output ownership, hallucination liability, human-review commitments, or usage of counterparty data for model training. See [chapter 06](./06-ai-and-model-contracts-inbound-and-outbound.md).

The framework should be a one-page document with a decision tree, published in the same location as the playbook.

## Redline discipline

The mechanics of how redlines are exchanged materially affect cycle time and outcome quality.

- **Track-changes with named authors.** All edits made in Word with track changes on, with the reviewer's name attached. Anonymous edits (accepted-and-reintroduced changes without attribution) are unacceptable — they hide the origin of a proposed change and make it impossible to reconstruct the negotiation history.
- **Comment-driven rationale.** Every substantive edit gets a comment explaining the reason ("moving cap from 12 months to 24 months per procurement policy XYZ" or "removing this clause — see our fallback matrix on MFN"). Bare redlines with no rationale invite escalation and slow the cycle.
- **Three-round expectation.** The negotiation should conclude within three redline rounds — the counterparty's initial markup, the corporation's response, the counterparty's reply, and either close or handoff to a phone call. Redlines that stretch beyond three rounds are a signal that the parties are talking past each other in writing and need to synchronise verbally.
- **When to stop redlining and pick up the phone.** Two or three round trips into a redline exchange, if the parties are still on the same three or four clauses, the marginal value of another round of written edits is low. A 30-minute call between the corporation's counsel and the counterparty's counsel resolves more than a week of email in most cases. Sales operations should facilitate this call, not sit through it.
- **The "we'll agree to your language but for these two changes" close.** A powerful negotiation move: the corporation accepts the counterparty's proposed language wholesale except for a small number (two or three) of specific, named changes. This closes the negotiation by making the counterparty commit to accepting or rejecting a short list rather than continuing to iterate on the full clause. Use once, near the end of the negotiation.

## Metrics that matter

Legal ops is a measurable function. Publish these metrics quarterly to the executive team and to sales leadership:

- **Contract cycle time.** Median and 90th-percentile days from initial redline receipt to signature. Trend line quarter-over-quarter is the primary indicator of process health.
- **Redline count per deal.** Number of round trips before signature, segmented by deal size and by tier. A rising redline count is a signal that the playbook is out of sync with the market and needs revision.
- **Fallback-position hit rate.** Percentage of deals that closed on the ideal, acceptable, or walk-away position for each playbook-covered clause. When the corporation is consistently forced past acceptable on a specific clause, the acceptable position is likely too aggressive for current market practice.
- **Escalation rate.** Percentage of deals that were routed as non-standard or bespoke rather than standard. A rising escalation rate is a signal that the standard playbook needs to be broadened, or that a new counterparty segment (industry, geography, deal size) is being under-served.
- **Post-signature obligations met.** Percentage of signed deals where post-signature commitments (SOC 2 delivery, insurance certificate delivery, DPA schedule updates, security-questionnaire refresh, MFN pricing lookback) are met on time. Requires the CLM ([chapter 07](./07-clm-stack-signature-storage-obligation-tracking.md)) to track obligations; failure to meet post-signature obligations is a breach and can expose the corporation to termination-for-cause.
- **Cost per deal.** Total legal-ops-and-outside-counsel cost divided by number of deals closed, segmented by deal size and tier. Trend line indicates whether the function is scaling with ARR growth.

## Playbook maintenance

The playbook is a living document. Formalise the revision cadence.

- **Quarterly review** with sales leadership and outside counsel. Walk the metrics dashboard, identify the clauses where the corporation is consistently forced past acceptable, and decide whether the playbook position should change. Common outcomes: promoting a walk-away to acceptable when market practice has shifted, tightening an acceptable position when the corporation's leverage has improved (post-fundraise, post-market-leader status), adding a new clause when a novel term has become common in redlines (AI-related terms are the current example).
- **Trigger-based updates** when specific events occur: a change in the corporation's insurance program (updates the LoL cap and indemnification carve-out ceilings), a new regulatory obligation (a new state privacy law affects the DPA position — see [mod-110](../mod-110-privacy-data-governance-and-sector-compliance/)), a strategic pivot (new customer segment, new product line), or a significant loss (a deal walked away over a specific clause).
- **"Win/loss data says X clause is now acceptable"** mechanic. The playbook should reference sales win/loss data. If the corporation is losing 15% of enterprise deals on the MFN clause and the deals lost are worth more than the aggregate pricing risk from accepting a narrowly-scoped MFN, the acceptable position on MFN should move. This decision is made jointly by sales, finance, and legal, not by legal alone.
- **Change log.** Every revision is logged with the date, the person who approved it, the rationale, and a link to the underlying deal or market signal that drove the change. When a redline dispute two years later turns on why a clause was written a certain way, the change log is the record.

## Concrete example (i): fallback matrix for limitation of liability, mid-market SaaS deal

Illustrative fallback matrix for a mid-market SaaS deal in the $100k–$500k ARR range, non-regulated industry.

| Sub-clause | Ideal | Acceptable | Walk-away |
|---|---|---|---|
| Consequential damages waiver | Mutual full waiver of indirect, consequential, incidental, special, punitive, and lost-profits damages | Mutual waiver with narrow carve-out for lost profits arising from breach of confidentiality by either party | Removal of mutual waiver, or one-sided waiver in counterparty's favour |
| Direct-damages cap | 12 months of fees paid by customer in the 12 months preceding the claim | 24 months of fees; separately-negotiated fee-based cap for month-to-month customers | Uncapped direct liability; cap set as a fixed dollar amount unrelated to fees |
| Enhanced-remedy: breach of confidentiality | 2x fees paid in the prior 12 months | 3x fees | Uncapped |
| Enhanced-remedy: IP indemnification | 2x fees paid in the prior 12 months, subject to the modify / replace / refund escape | 3x fees, escape preserved | Uncapped, or escape removed |
| Enhanced-remedy: data breach / DPA breach | 2x fees paid in the prior 12 months | 3x fees | Uncapped, or an amount exceeding the Cyber tower limit |
| Enhanced-remedy: gross negligence, wilful misconduct, fraud | Uncapped | Uncapped | N/A — always uncapped |

Reasoning: The direct-damages cap is set at fees to align with the corporation's revenue exposure on the deal. The 2x super-cap on the enumerated carve-outs is calibrated to the corporation's Cyber and Tech E&O tower ([mod-105](../mod-105-workplace-safety-and-insurance-program/)); a 3x super-cap is generally within tower limits at this deal size. Uncapped-for-gross-negligence-etc. is the industry standard and non-negotiable in both directions. If the counterparty demands uncapped liability for data breach, the deal moves to bespoke and requires CFO approval based on a written risk assessment.

## Concrete example (ii): fallback matrix for DPA breach-notification window

Illustrative fallback matrix for the data-breach notification obligation in the DPA, non-regulated industry, customer processing personal data of EU / UK residents (GDPR applies).

| Sub-clause | Ideal | Acceptable | Walk-away |
|---|---|---|---|
| Trigger event | "Confirmed Security Incident affecting Customer Data" following provider's investigation | "Confirmed Security Incident" or "reasonable belief that a Security Incident has occurred" following provider's initial triage | "Any suspected incident, anomaly, or security alert" (triggers notification on every SOC alert, unworkable) |
| Notification window | Without undue delay and in any event within 72 hours of provider's confirmed determination | 48 hours; 24 hours acceptable if trigger is "confirmed" (not "suspected") | Less than 24 hours from initial detection; measured in hours from a SOC alert; no confirmation window before the clock starts |
| Content of notification | Nature of the incident, categories of data affected (to the extent known), likely consequences, measures taken or proposed, and provider's contact person | Same as ideal, plus a commitment to update customer with additional detail as investigation progresses | Requirement to disclose provider's other customers' data or provider's internal security configurations |
| Delivery method | Email to the customer's designated security contact, with contemporaneous notice through the provider's status page | Email plus telephone follow-up to designated contact | Requirement to notify customer's entire organisation, or requirement to notify third parties (regulators, individuals) on customer's behalf without customer instruction |
| Override for law-enforcement instruction | Provider may delay notification if instructed by law enforcement or a regulator; customer notified as soon as legally permissible | Same as ideal | Notification obligation that overrides law-enforcement instruction |
| Cooperation | Provider will reasonably cooperate with customer's incident-response investigation and any regulatory-notification obligations customer owes to individuals or regulators | Same as ideal, plus commitment to make forensics reports available under NDA on request | Requirement to indemnify customer for its regulatory notification costs regardless of fault |

Reasoning: The 72-hour window aligns with GDPR Article 33 (controller's notification obligation) and is the industry ceiling. Customers routinely ask for 24 or 48 hours; the acceptable position preserves the "confirmed determination" trigger, which is the operationally meaningful defence against being forced to notify on every SOC alert. The walk-away positions are the ones that would put the corporation in the position of promising the impossible or of taking on the customer's own regulatory-compliance obligations without contractual scaffolding.

## Summary

- The contract playbook is a per-clause table of ideal, acceptable, and walk-away positions, together with pre-approved trade-offs and negotiation moves, that turns contract negotiation from a bespoke exercise into a repeatable operational process.
- Coverage focuses on the two dozen clauses that actually draw redlines: limitation of liability, indemnification, IP ownership, warranty, termination for convenience, SLA credits and enhanced remedy, MFN, audit rights, renewal, assignment, governing law, confidentiality term, data-breach notification, publicity, and insurance.
- Internal-legal-turn SLA scales with stage: 3 to 7 business days at pre-seed / seed with a part-time outside counsel; 3 to 5 business days at Series A with a first in-house counsel; 24 to 48 hours at Series B with a legal-ops team; same-day for standard bundles at Series C+.
- The deal-desk model tiers each deal as standard, non-standard, or bespoke and routes accordingly; standard deals close without counsel review, bespoke deals engage outside counsel and executive approval.
- The escalation-to-outside-counsel framework triggers on deal size, unfamiliar regulated industry, government contracting, aggressive IP terms, large uncapped liability, non-standard indemnification, custom data residency, or novel AI terms.
- Redline discipline — track changes with named authors, comment-driven rationale, three-round expectation, phone calls when redlines stall, and the "we'll agree to your language but for these two changes" close — keeps cycle time low and outcome quality high.
- Metrics — cycle time, redline count per deal, fallback-position hit rate, escalation rate, post-signature obligations met, cost per deal — measure the legal-ops function and drive quarterly playbook revision.
- The playbook is a living document, revised quarterly with sales and outside counsel and updated whenever the corporation's insurance program, regulatory environment, market position, or product line changes.
- Chapter 01 owns the document architecture; this chapter owns the negotiation-and-triage discipline that makes those documents scale.
