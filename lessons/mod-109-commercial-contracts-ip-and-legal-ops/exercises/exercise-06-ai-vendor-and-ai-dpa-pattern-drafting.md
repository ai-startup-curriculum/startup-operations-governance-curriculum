# Exercise 06 — AI vendor and AI-DPA pattern drafting

> Estimated time: **~10 hours** · Related chapter: [06 — AI vendor contracts and the AI-DPA pattern](../06-ai-vendor-contracts-and-ai-dpa-pattern.md)

## Problem statement

Resolvra Inc. is a Series-B Delaware C-corp selling an AI-assisted customer-support product into enterprise. The product performs automated response drafting, inbound-ticket summarisation, and routing-recommendation against the customer's support corpus and live ticket stream. Resolvra is 95 FTE, closed a $38M Series B four months ago led by a growth-stage firm, and ships through a direct-sales GTM into mid-market and enterprise accounts. The product uses two foundation-model providers behind the scenes: one for completion-style summarisation and response drafting, one for embedding and retrieval against the customer's historical ticket corpus. Both are consumed through API; neither is self-hosted; neither is fine-tuned.

Resolvra is in-flight on its first Fortune-100 opportunity — a US-headquartered financial-services firm with roughly 240,000 end-users under one of its retail-banking lines — on a $650k ACV deal. The customer's privacy office has routed a 23-page AI-transparency addendum into the deal and the deal cannot close without a redline back. The addendum demands six operative commitments: (i) explicit disclosure of every foundation model that touches customer data, with model-provenance and training-data-source assertions; (ii) a binding commitment that customer inputs will not be used to train the model provider's foundation models; (iii) a human-in-the-loop guarantee for any downstream decision affecting the customer's end-users (including routing decisions that collide with the customer's regulated-communications obligations); (iv) IP indemnification for third-party claims arising from AI-generated output; (v) a model-change-notification obligation (30-day customer notice window; customer veto right for changes the customer deems breaking); (vi) a right to require EU-only processing and EU-only data residency for a defined subset of records (specifically, records tagged as relating to EU data subjects under the customer's own GDPR data-classification taxonomy).

Resolvra's current upstream contracts are not aligned to those commitments. The paid-tier commercial agreement with the completion provider (call it Provider A) includes a signed addendum opting out of training-on-inputs; it also carries a 30-day sub-processor-change notice right that the provider reserves for its own cloud-infrastructure sub-processors — meaning Provider A has 30 days' notice coming *in* on hyperscaler changes, which pins Resolvra's maximum outbound notice window. The standard-tier commercial agreement with the embedding provider (Provider B) was signed two years ago, has never been refreshed, and the general counsel (external, three months in-seat) has not re-read it since joining; the current terms are unknown. Neither provider has delivered Annex XII GPAI documentation to Resolvra; neither has been formally confirmed on model-provenance; neither has been confirmed on EU-region-endpoint availability.

The general counsel has roughly five weeks to walk into the Fortune-100 customer's privacy-office review with a redlined addendum back, and roughly nine weeks to close the deal. The forcing function on the upstream contracts is immediate: the outbound commitments cannot be made honestly without closing the upstream gaps first. The general counsel owns the end-to-end two-sided paper stack; the head of product owns the model-provenance disclosure form; the head of engineering owns the sub-processor-list sync; the CFO owns the AI-indemnification cap sizing against the current insurance tower.

Author the full package.

## Requirements

### Part A — Two-role gap audit

Author the audit document the general counsel will circulate to the exec team before the upstream re-paper and the outbound redline. Present as a table that:

1. **Maps each of the six downstream customer demands** (disclosure, training-opt-out, human-in-the-loop, IP indemnity, model-change-notice, EU-residency) to the specific upstream vendor-contract term in Provider A's and Provider B's current paper that would need to support it.
2. **Identifies the gap** for each row — where the current paper is silent, where it is thin, where it is contradictory, where the general counsel has not yet re-read the Provider B agreement and so cannot answer. "Unknown — Provider B agreement under re-review" is a legitimate gap entry; invented terms are not.
3. **Names the specific clauses to re-paper upstream** before the Fortune-100 deal signs — the clause label (input-data confidentiality, training-on-inputs prohibition, model-provenance disclosure, sub-processor list and change-notification, EU AI Act GPAI addendum, data-residency, breach-notification, IP-indemnity) and the operative change the general counsel will seek.
4. **Flags the Provider A 30-day sub-processor notice ceiling** against the customer's 30-day outbound ask — the inbound-outbound alignment chapter 06 names as the structural minimum.
5. **Carries a disposition column** per row: close before signature, document as balance-sheet exposure, escalate to CEO, defer.

### Part B — Inbound AI-DPA / vendor-contract redline

Author the operative clause text — not a summary — Resolvra will send to each of Provider A and Provider B as the re-paper redline. Clauses to draft:

1. **Input-data confidentiality.** The clause limiting the provider's use of Resolvra's inputs (prompts, retrieval-context documents, embeddings, tool-call arguments) to the stated inference-processing purpose and prohibiting secondary use for analytics, competitive-product evaluation, or model improvement.
2. **Output-IP ownership.** The clause granting Resolvra ownership of outputs to the extent the provider has rights to convey, including the non-uniqueness caveat chapter 06 names and an acknowledgement of the US Copyright Office position on AI-generated-output copyrightability.
3. **Training-on-inputs prohibition.** The clause prohibiting use of Resolvra's inputs or derived outputs to train, fine-tune, evaluate, or improve the provider's foundation models or any content-safety or classifier model; address the abuse-detection retention caveat chapter 06 names.
4. **Model-provenance disclosure.** The clause requiring the provider to identify the model family and version serving Resolvra's traffic, commit to a deprecation-notice window, and prohibit silent-version substitution.
5. **Sub-processor list and change-notification.** The clause requiring the provider to publish and maintain its sub-processor list and to give Resolvra notice sufficient to support Resolvra's 30-day outbound notice to its own customers. Explicitly address the Provider A 30-day infrastructure sub-processor notice right and whether it is acceptable or must be renegotiated.
6. **EU AI Act GPAI addendum.** The clause requiring the provider to deliver Annex XII downstream-provider documentation under Article 53(1)(b), the Article 53(1)(c) copyright-compliance policy, and the Article 51 systemic-risk classification with Article 55 compliance evidence where applicable. Defer the EU AI Act regulatory depth — prohibited practices, high-risk-system conformity assessment, the AI Office enforcement mechanic — to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/).
7. **Data-residency.** The clause committing the provider to EU-only processing for the subset of Resolvra traffic the customer tags as EU-resident, and the notice mechanic if the provider proposes to change the region.
8. **Breach-notification.** The clause committing the provider to breach notification on a timeline (24–48 hours from provider's discovery) that supports Resolvra's 72-hour customer-facing commitment per [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md).

Author each clause in the operative form Resolvra will send; do not fabricate the provider's current language. Where the clause is contingent on verifying the current enterprise-term posture of a named provider, flag `<!-- needs-research: ... -->` rather than inventing a quote.

### Part C — Outbound AI-transparency addendum to the Fortune-100 customer

Author the operative clause text — not a summary — Resolvra will send back as the redline to the customer's 23-page addendum. The clauses must align 1:1 with the six demands and must not promise anything the inbound stack from Part A/B cannot deliver. Draft:

1. **Foundation-model disclosure.** The AI-in-the-loop clause disclosing which foundation-model providers serve which product features, which model family and version-tier is deployed, and the training-data-source assertion Resolvra can honestly carry (bounded by what Provider A and Provider B have confirmed).
2. **Training-opt-out pass-through.** The clause committing Resolvra to no-training-on-customer-inputs and passing through the upstream providers' no-training commitments; name the specific scope and the opt-in exception for customer-specific fine-tunes.
3. **Human-in-the-loop guarantee.** The clause committing Resolvra to no automated adverse decision on the customer's end-users without meaningful human review, bounded by the operating reality of a routing-and-summarisation product; address the "meaningful" word chapter 06 flags.
4. **IP-indemnification.** The clause offering IP indemnity for third-party claims arising from AI-generated output; the operative text here is drafted in Part D and cross-referenced from this clause.
5. **Model-change-notification.** The clause committing Resolvra to 30 days' advance notice before material model-provenance changes, and the operative treatment of the customer's veto right — including the customer-termination-of-affected-feature carve-out chapter 06 names in place of a right to force a model-provider switch.
6. **EU-residency.** The clause committing Resolvra to EU-only processing for the subset of records the customer tags as EU-resident, with the inbound regional-endpoint availability as the enabling condition.

Also list the clauses Resolvra will flag as **mutual-amendment-only** — the subset where the customer cannot unilaterally update the terms (e.g., training-opt-out, IP-indemnity cap) and where any change requires both signatures. Reference the handbook-vs-contract reservation-of-rights discipline from [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md).

### Part D — AI-indemnification clause

Author the operative text of the AI-IP-indemnification clause in the outbound addendum. Design:

1. **Cap structure.** The practical cap sized against Resolvra's current cyber-liability and IP-liability insurance tower and the two upstream providers' indemnity caps. Reference [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/) for the insurance-tower sizing; do not invent the dollar figure for Resolvra's tower or the upstream caps — flag with `<!-- needs-research: ... -->` and note what the CFO must confirm before the clause is sent. Pin the structure (super-cap vs. aligned-to-general-liability-cap vs. uncapped) and name the defensible position.
2. **Carve-outs.** The exclusions mirroring the upstream carve-outs plus the customer-side carve-outs: (i) customer prompt-injection or jailbreak attempts, (ii) customer modification of outputs without the Resolvra human-in-the-loop step, (iii) use outside the licensed-purpose statement, (iv) failure to follow Resolvra's published usage guidance (reference the AUP under [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md)), (v) customer's own inputs infringing third-party IP. Author each carve-out in operative form.
3. **Remedy mechanic.** The procure-licence / modify / refund sequence Resolvra will offer, aligned to the base IP-indemnity architecture in [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md).
4. **Sub-indemnification pass-through posture from upstream.** The clause acknowledging that Provider A's and Provider B's indemnity programmes run to Resolvra, not to the customer; the customer's claim is against Resolvra; Resolvra's recovery is a separate action. Document the delta between the inbound coverage and the outbound exposure as the balance-sheet item the CFO carries. Reference the [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/) risk-register entry.

### Part E — Hallucination-and-output-accuracy posture

Author the hallucination-and-accuracy memo the general counsel will circulate to the sales organisation and the CS organisation, and the corresponding clause text in the outbound addendum. Cover:

1. **Warranty posture.** The chapter 06 practitioner default — no warranty of accuracy, no warranty of hallucination-rate cap, no warranty of correctness, no warranty of bias-freedom — in conspicuous UCC § 2-316-compliant form. Author the operative disclaimer text.
2. **AUP implication.** The customer-side acceptable-use obligations that interact with the hallucination posture — customer agrees to review AI-generated routing and response drafts before external communication to the customer's own end-users. Defer the AUP document itself to [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md) and reference the operative obligation that the AUP will carry.
3. **Disclosure-and-human-in-the-loop operating pattern.** The product-side pattern that the AI output is labelled as AI-generated inside the customer's agent-facing UI, that no AI output is auto-sent to the customer's end-user without the customer's own agent confirming, and that Resolvra does not operate a "no-touch" send mode. Name the operating pattern in a form the product team can implement against.
4. **Customer-side-obligation flow-down.** The clause committing the customer to the review-before-use posture in regulated-decision contexts, with the carve-out that the obligation is the customer's and failure to carry it collapses Resolvra's indemnity under Part D (cross-reference Part D's carve-out iv).

### Part F — Sub-processor-and-model-provenance disclosure architecture

Author the sub-processor and model-provenance disclosure architecture the engineering, product, and legal functions will operate against. Cover:

1. **Public sub-processor list.** The customer-facing sub-processor list that identifies Provider A and Provider B by name, their primary cloud sub-processors as sub-sub-processors (bounded by what each provider has disclosed), the processing purpose, the data categories, and the processing region. Author the list in the form it will be published.
2. **Model-provenance disclosure form.** The disclosure artefact Resolvra will publish and attach to the outbound addendum — model family, provider, version pinning posture (family and version-tier, not point-release), training-cut-off disclosure where the provider makes it available, GPAI-systemic-risk flag per Article 51. Flag `<!-- needs-research: ... -->` on any provider-specific disclosure Resolvra has not yet confirmed in writing.
3. **Model-change-notification mechanic.** The 30-day notice window, the customer-veto posture (feature-termination right in place of model-provider-switch demand), the termination-of-affected-feature right, and the material-change definition that triggers the clock.
4. **Engineering process to keep the public list in sync with production.** The named operating cadence — the engineering review that confirms the production model-provenance matches the published disclosure, the sub-processor-list review in the quarterly consistency-check chapter 06 names, the trigger that forces an interim update. Defer the CLM-side sub-processor-list mechanic — the versioning, the automated change-notification distribution, the acknowledgement-tracking — to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md).

## Starter guidance

- Chapter 06 is the primary reference. The two-role framing (buy-side AI-DPA and sell-side AI-transparency addendum) maps directly to Parts B and C; the gap audit in Part A is the operational discipline chapter 06 names as the quarterly consistency check applied once, under deal pressure, before signature.
- The Fortune-100 deal's 23-page addendum is the forcing function on the whole package. Ducking any of the six demands — "we will consider this" or "subject to further review" — is a fail. Resolvra either covers the demand, redlines back with a bounded commitment it can keep, or documents the gap as a balance-sheet item the CFO carries.
- The Provider B contract that the general counsel has not re-read is the forcing function on Part A. The gap row for Provider B is "unknown pending re-review"; the Part B redline for Provider B is written against the reasonable baseline a Series-B legal function would open with; the operative draft is contingent on the re-read. Do not fabricate Provider B's current terms.
- No invented real model-provider contract clauses. Do not fabricate "Anthropic's exact training-opt-out language" or "OpenAI's exact DPA Article 5"; the student negotiates the clauses in Part B as Resolvra's opening redline. Flag with `<!-- needs-research: ... -->` any point that requires verifying the current enterprise-term posture of a named provider.
- No invented real company names anywhere; "Resolvra Inc." is the fictional corporation and the two providers are left as Provider A and Provider B. The customer is "the Fortune-100 financial-services firm" with no invented name.
- Current EU AI Act phasing — prohibited-practices from Feb 2025, GPAI-model provisions from Aug 2025, high-risk-system provisions from Aug 2026 — gets `<!-- needs-research: ... -->` because the phasing is still subject to AI Office implementing acts and delegated acts. Flag every reference to specific effective dates.
- Specific indemnity-cap figures from the upstream providers get `<!-- needs-research: ... -->`. Chapter 06 names caps as varying widely across providers and tiers; the general counsel confirms against the current published enterprise agreement rather than quoting from memory.
- The internal AI acceptable-use policy interaction and the AI-literacy training discipline (Article 4 EU AI Act obligation on AI literacy for staff operating AI systems) live in [mod-108](../../mod-108-culture-employee-experience-and-dei/). Reference the Tier-C ban on consumer AI tools for business data; do not re-author the internal AUP.
- The SecReview / VendorReview depth, the risk-register entry for the inbound-outbound indemnity delta, and the cyber-liability tower sizing live in [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/). Reference the deferrals; do not author the mechanics.
- Nothing in this exercise is a legal determination that overrides counsel. The general counsel is the owner of the signed paper; the student authors the operative drafts and the redlines that counsel will finalise.

## Deliverables

- `two-role-gap-audit.md` — Part A.
- `inbound-ai-dpa-redlines.md` — Part B.
- `outbound-ai-transparency-addendum.md` — Part C.
- `ai-indemnification-clause.md` — Part D.
- `hallucination-posture-memo.md` — Part E.
- `sub-processor-and-provenance-architecture.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. Part A's gap-audit table maps each of the six downstream customer demands to the specific upstream vendor-contract term that must deliver it, names the gap honestly (including "unknown pending Provider B re-review" where applicable), lists the specific clauses to re-paper, flags the Provider A 30-day sub-processor-notice ceiling against the customer's 30-day outbound ask, and carries a per-row disposition.
2. Part B's inbound redline authors operative clause text (not a summary) for each of input-data confidentiality, output-IP ownership (with the non-uniqueness and Copyright-Office caveats chapter 06 names), training-on-inputs prohibition, model-provenance disclosure, sub-processor list and change-notification, EU AI Act GPAI addendum (deferring regulatory depth to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/)), data-residency, and breach-notification.
3. Part C's outbound addendum authors operative clause text (not a summary) for each of the six customer demands, aligns 1:1 so no outbound promise is uncovered upstream per the Part A audit, and names the specific clauses Resolvra will flag as mutual-amendment-only.
4. Part D's AI-indemnification clause specifies the cap structure (sized against the insurance tower in [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/) and the upstream caps, with `<!-- needs-research: ... -->` on dollar figures), the carve-outs (customer prompt-injection, customer modification without human-in-the-loop, use outside licensed purpose, failure to follow published usage guidance, customer-input IP violation), the remedy mechanic (procure-licence / modify / refund) referencing [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md), and the sub-indemnification pass-through posture documenting the inbound-outbound delta as a balance-sheet item.
5. Part E's hallucination posture authors the UCC § 2-316-compliant disclaimer text in conspicuous form, references the AUP interaction in [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md), names the disclosure-and-human-in-the-loop operating pattern in product-implementable form, and authors the customer-side review-before-use flow-down clause with the Part D carve-out cross-reference.
6. Part F publishes the sub-processor list naming Provider A and Provider B with primary cloud sub-sub-processors (bounded by what each provider has disclosed), the model-provenance disclosure form, the model-change-notification mechanic (30-day notice, customer-veto treated as feature-termination right rather than model-switch demand), and the engineering sync process, deferring the CLM-side mechanic to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md).
7. No real model-provider contract clauses are invented; Part B is Resolvra's opening redline and the current enterprise-term posture of each named provider is flagged with `<!-- needs-research: ... -->` where it bears on the draft.
8. No real company names are invented; the Fortune-100 customer and the two providers are referenced by role only.
9. `<!-- needs-research: ... -->` is propagated on current EU AI Act phasing, current enterprise-terms posture of named model providers, specific indemnity-cap figures from upstream providers, Resolvra's current cyber-liability / IP-liability tower limits, and any provider-specific regional-endpoint or hyperscaler-dependency claim the student cannot verify from a current source.
10. Deferrals to sibling modules and chapters are named explicitly: [mod-108](../../mod-108-culture-employee-experience-and-dei/) for the internal AI acceptable-use policy and the Article 4 AI-literacy training discipline; [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/) for EU AI Act regulatory depth, GDPR joint-controller analysis, and sector-specific privacy rules; [mod-112](../../mod-112-enterprise-risk-insurance-and-compliance/) for the risk-register entry, SecReview depth, and insurance-tower sizing; [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md) for the base IP-indemnity architecture and the AUP; [chapter 07](../07-clm-stack-and-legal-ops-graduation.md) for the CLM-side sub-processor-list mechanic.
11. The two-sided consistency discipline chapter 06 names (every outbound commitment supported by an inbound commitment, or documented as balance-sheet exposure with insurance sizing) is applied visibly across Parts A, C, D, and F — a reader can trace each outbound promise back to its upstream support row in the Part A audit.
12. Nothing is left as `[TBD]` or `[FILL IN]`; every unknown is either a `<!-- needs-research: ... -->` flag with a named verification step, a deferral to a named sibling module, or an explicit "pending Provider B re-read" entry in the Part A audit.
