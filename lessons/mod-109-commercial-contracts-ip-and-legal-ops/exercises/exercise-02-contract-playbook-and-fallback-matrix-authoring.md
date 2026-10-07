# Exercise 02 — Contract playbook and fallback-position matrix authoring

> Estimated time: **~8 hours** · Related chapter: [02 — The contract playbook and fallback-position matrix](../02-contract-playbook-and-fallback-position-matrix.md)

## Problem statement

Lumenark Systems is a Series-B B2B SaaS corporation selling an observability-and-incident-response product into mid-market and enterprise engineering orgs. The corporation closed its $48M Series B seven months ago, is 130 employees, Delaware C-corp, and runs 60-80 commercial closes per quarter — approximately 15 enterprise deals (ACV >= $100k), the balance mid-market new-logo and self-serve-expansion. The customer-contract suite from [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md) (MSA, SLA, DPA, security exhibit, AUP) is already published as the corporation's paper; the problem is operational, not architectural. Lumenark's general counsel sits as a single headcount with support from an outside firm on retainer; the deal-desk function sits inside revenue operations and currently escalates roughly 45% of counterparty redlines back to counsel because there is no written fallback matrix to clear the markup against. The internal legal-turn is averaging 7 business days per redline round and the CRO has told the executive team that compressing standard-tier turnaround to 48 hours is a Q-ahead board commitment.

Three deals currently sit mid-redline as the test cases this playbook has to clear on first pass. **Deal (i):** a $380k enterprise deal with a US-headquartered logistics corporation where the counterparty has struck the mutual consequential-damages waiver and inserted a demand for uncapped liability on IP infringement; counterparty counsel is from a top-tier litigation firm and the redline arrived with no supporting rationale. **Deal (ii):** a $90k mid-market deal with a venture-backed fintech where the counterparty has inserted both a feature MFN ("any feature offered to any customer must be offered here") and a 30-day termination for convenience, each with no commercial concession offered in exchange. **Deal (iii):** a $220k enterprise deal where the counterparty is a regulated financial-services firm demanding on-site audit rights twice per calendar year with 48 hours' notice, scoped to any system processing their data. The general counsel has eight weeks to walk into a joint sales-and-legal operating review with (a) the clause-indexed fallback matrix, (b) the deal-desk routing rules that tier each inbound deal, (c) a published legal-turn SLA calibrated to deal tier and stage, (d) the escalation-to-outside-counsel trigger list, (e) worked recommendations on all three in-flight deals, and (f) the governance pattern that keeps the playbook from going stale. Author the full package.

## Requirements

### Part A — Clause-indexed fallback-position matrix

Author the matrix in the chapter 02 **ideal / acceptable / walk-away / trade-offs / rationale** structure. Draft operative row text for each clause below; do not summarise. Each row names the ideal (what Lumenark opens with — its published paper), the acceptable (what the deal desk may close on without counsel escalation), the walk-away (the point at which the deal is routed to counsel or declined), the pre-approved trade-offs (what Lumenark will give up on this clause in exchange for holding on a named sibling clause), and the rationale a deal-desk analyst or counsel will cite when applying the position.

1. **Limitation of liability.** The direct-damages cap (months-of-fees basis), the mutual consequential / indirect / incidental / punitive / lost-profits waiver, and the super-cap structure for the enumerated enhanced-remedy carve-outs. Separately treat the always-uncapped carve-outs (gross negligence, wilful misconduct, fraud).
2. **Indemnification.** IP indemnification (scope of covered claims, the modify / replace / refund escape, the combination-claim and open-source carve-outs), customer-content indemnification (reciprocal, AUP-breach-triggered), and the procedure-and-control block (notice, sole-vs-joint control of defence, settlement-consent discipline).
3. **IP ownership.** Service and provider-developed IP, Customer Data (ownership and the Lumenark-side processing licence), and feedback / aggregated / de-identified usage data (perpetual-licence posture, re-identification prohibition, model-training interaction — defer the AI-specific overlay to [chapter 06](../06-ai-vendor-contracts-and-ai-dpa-pattern.md)).
4. **Warranty.** Functionality warranty (conformance to documentation), performance warranty (workmanlike-manner-and-industry-standards), the explicit disclaimer of implied warranties, the cure-and-sole-remedy mechanic.
5. **Termination for convenience.** Provider-side TfC (treat as "not permitted" at the ideal), customer-side TfC (notice window and the pro-rata-refund posture), and the carve-out mechanic for enterprise procurement policies that require TfC.
6. **SLA credits and enhanced remedy.** The tiered-credit structure, the "sole and exclusive remedy" discipline, and the chapter-01-aligned termination-for-cause right on sustained SLA miss. Cross-reference the SLA architecture in [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md).
7. **MFN.** The baseline "no MFN" ideal, the narrow pricing-MFN acceptable (same SKU, same tier, same contract length, same ARR band, scoped to net-new signatures in the measurement window, counterparty-expense audit), and the walk-aways (feature MFN, terms MFN, undefined-scope pricing MFN).
8. **Audit rights.** SOC 2 Type II in lieu of on-site as the ideal; the regulated-vertical acceptable (once-per-year, 30 days' notice, counterparty expense, business hours, NDA, scoped to systems processing the counterparty's data); the walk-aways (on-demand audit, audit of source code or other-customer data, audit by a competitor).
9. **Renewal and auto-renewal.** The auto-renew-with-notice ideal, the notice-window acceptable range, the uplift-cap acceptable range, the affirmative-renewal carve-out for enterprise procurement, and the walk-away floor on notice duration.
10. **Assignment and change-of-control.** The affiliate-and-successor carve-out posture, the "consent not unreasonably withheld" acceptable, and the competitor carve-out walk-away.
11. **Insurance minimums.** CGL, Professional Liability / Tech E&O, Cyber, Workers' Comp, Employer's Liability, Umbrella — the ideal coverage ladder, the enterprise-vertical acceptable ladder, and the walk-aways (additional-insured on E&O / Cyber, uninsurable waivers of subrogation). Pin the ladder to the insurance-tower reality described in [mod-112](../../mod-112-insurance-and-risk-financing/); do not propose caps or additional-insured positions that exceed the tower's actual ceiling. Flag any specific insurance-tower-ceiling figures not in the chapter with `<!-- needs-research: ... -->`.

For every row, name at least one **pre-approved trade-off** (e.g., "if counterparty demands 24-months-fees cap on LoL direct, Lumenark may hold the ideal on indemnification super-cap at 2x fees") and one **rationale sentence** a deal-desk analyst can read back verbatim to sales or counterparty counsel.

### Part B — Deal-desk routing rules

Author the written routing rules the deal-desk analyst will apply against each inbound redline. Cover:

1. **Deal-tier definitions.** Specific threshold-based definitions for **self-serve** (no human negotiation permitted — clickwrap only, cite the AUP), **mid-market** (named ACV range), **enterprise** (named ACV threshold), and **strategic** (named ACV threshold plus the qualitative overlay — regulated vertical, named-account target, cross-sell to a Lumenark investor's portfolio, board-level introduction). Name the thresholds for Lumenark specifically.
2. **Clear-alone authority.** The clause-level and tier-level thresholds that let a deal-desk analyst approve a redline on their own — a redline that hits only Part A acceptable positions, a counterparty markup that accepts Lumenark's paper with cosmetic edits, an order-form-only change that does not touch the MSA.
3. **Route-to-counsel threshold.** The specific triggers that route the deal to the Lumenark general counsel: any redline that crosses an acceptable boundary, any new clause the matrix does not cover, any counterparty counsel from a named top-tier litigation firm, any regulated-vertical first-deal (feed Part D).
4. **Route-to-executive-sponsor threshold.** The specific triggers that route the deal to the CRO (commercial sign-off) or the CEO/CFO (deviation sign-off): any walk-away position the deal team wants to accept anyway, any uncapped-liability concession, any TfC-without-matching-cancellation-fee concession, any strategic-account exception.
5. **Routing-decision timestamp.** The CLM-side evidence the analyst drops into the deal record on every routing decision — the clause(s) that triggered the routing, the matrix row(s) consulted, the decision outcome, the timestamp. Defer the CLM mechanics to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md); the chapter-02-owned mechanic is the decision discipline.

### Part C — Internal legal-turn SLA

Author the published commitment to sales. Cover:

1. **Named hours per tier.** The SLA target in business hours (not business days — the 48-hour target is the forcing function) for each of **standard** (clean deal-desk clearance), **non-standard** (counsel review within the matrix), and **bespoke** (counsel plus executive-sponsor or outside-counsel loop). Separately name the SLA for the first-round turnaround vs. subsequent redline rounds.
2. **Clock definitions.** When the clock starts (complete submission, counterparty's redline attached, deal-tier assigned) and when it pauses (counterparty's turn, incomplete submission, holiday-period adjustment). Lumenark operates US-east and US-west; address the time-zone discipline.
3. **At-risk escalation path.** The named operating step when the SLA is at risk — who the deal-desk analyst escalates to, who sales learns from, the written-notice-to-counterparty discipline when the delay is Lumenark-side. Do not duck the "SLA miss" case; chapter 02 is explicit that missed SLA counts against the legal-ops metric.
4. **Measurement cadence.** The metric Lumenark will publish quarterly against the SLA target (median turnaround, 90th-percentile turnaround, miss rate by tier), and the review surface — the joint sales-and-legal operating review where the number is read. Reference the chapter 02 metrics-that-matter list.

### Part D — Escalation-to-outside-counsel trigger list

Author the one-page trigger document the general counsel will publish alongside the playbook. The list is the chapter-02 escalation-to-outside-counsel framework translated into Lumenark-specific triggers. Cover at minimum:

1. **Deal-size trigger.** The named ACV threshold above which outside counsel is automatically looped (Lumenark is Series B — chapter 02 names $500k as a typical Series-B threshold; adopt or depart explicitly).
2. **Clause-level triggers.** Named clause-level escapes that force outside-counsel review regardless of deal size: uncapped liability on Lumenark's ordinary performance, loss of control of defence on an indemnified claim, TfC without a matching cancellation fee, novel data-residency requirement, custom encryption or key-management obligation, aggressive IP-ownership demand (counterparty claim to Service IP, provider-improvements IP, or feedback-licence loss).
3. **Counterparty-signal triggers.** Counterparty counsel from a named top-tier litigation firm, counterparty's past-litigation history flagged in diligence, counterparty-is-a-regulator (government-contracting flowdown).
4. **Vertical-first-deal triggers.** First deal in healthcare (HIPAA business-associate flowdowns), financial services (GLBA, NYDFS Part 500, FFIEC guidance), education (FERPA), federal / state / local government (FAR / DFARS, state-specific flowdowns, CMMC / FedRAMP). Deal (iii) sits in this category — call it out.
5. **Novel-AI-term trigger.** Any counterparty demand about training-data use, output ownership, hallucination liability, human-review commitments, or counterparty-data use for model training. Defer the substantive AI-contract architecture to [chapter 06](../06-ai-vendor-contracts-and-ai-dpa-pattern.md).
6. **Cost-and-cadence discipline.** The outside-counsel-rate budget pattern the general counsel will track — a soft budget per tier, the trigger that escalates spend to CFO review. Flag any specific outside-counsel hourly-rate ranges with `<!-- needs-research: ... -->`; do not invent benchmarks.

### Part E — Three worked redline scenarios

For each of the three in-flight deals from the problem statement, walk the deal through the Part A / B / C / D framework and produce a specific accept / counter / walk recommendation. Each worked scenario must include:

1. **Tier determination.** The Part B tier the deal lands in and the named-threshold reason.
2. **Clause-by-clause disposition.** For each counterparty markup, the matrix row that governs it (Part A), the position (ideal / acceptable / walk-away) the markup lands against, and the accept / counter / walk recommendation.
3. **Exact counter-language.** When the recommendation is counter, the specific clause text Lumenark will send back — pulled from the acceptable position in Part A. Author the operative clause, not a summary.
4. **Rationale citation.** The specific sentence the deal-desk analyst or counsel will cite to the counterparty in the comment attached to the counter (chapter 02's comment-driven-rationale discipline).
5. **Escalation decision.** Whether the deal routes to counsel (Part B threshold), to executive sponsor (Part B threshold), or to outside counsel (Part D trigger) — with the named trigger that forced the routing.

Specifically address:
- **Deal (i)** — the $380k enterprise deal with the struck consequential-damages waiver and the uncapped-IP-infringement liability demand. At least one Part D trigger fires here; name it.
- **Deal (ii)** — the $90k mid-market deal with feature MFN and 30-day TfC. The feature MFN is a Part A walk-away; the TfC is at the Part A acceptable edge. Treat both.
- **Deal (iii)** — the $220k enterprise deal with twice-yearly on-site audit on 48 hours' notice from a regulated financial-services counterparty. Part A audit-rights row governs; Part D vertical-first-deal trigger likely fires. State the counsel-sign-off step.

### Part F — Playbook governance

Author the governance document the general counsel will publish alongside the playbook. Cover:

1. **Review cadence.** The quarterly joint-review-with-sales-leadership rhythm from chapter 02 — participants (general counsel, head of deal desk, CRO, outside-counsel partner), agenda spine (metrics read, acceptable-position pressure-test, matrix revisions), named meeting cadence.
2. **Revision triggers.** The event-driven revisions that force an out-of-cycle update: new product line, new regulated vertical, new jurisdiction, new insurance tower ([mod-112](../../mod-112-insurance-and-risk-financing/) linkage — a change to the Cyber or Tech E&O tower moves the LoL cap and super-cap ceilings), new case law or statutory change, a lost deal over a specific clause, a counterparty-side pattern-of-markup across multiple deals that signals market shift.
3. **Approval authority.** The named sign-off chain for a matrix revision: who proposes (deal-desk analyst, counsel, sales), who approves at each tier (general counsel for acceptable-position shifts, CRO and CFO for walk-away-becomes-acceptable shifts, CEO for strategic-posture shifts), who logs the change.
4. **Versioning convention.** The CLM-stored version-of-record pattern — semantic version numbering, dated change log, link to the deal or market signal that drove the change. Defer the CLM mechanics to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md); the chapter-02-owned mechanic is the version-of-record discipline.
5. **Training programme.** The onboarding and refresher training the deal desk, sales, and counsel receive on the playbook — new-hire ramp (named weeks), quarterly refresher after the review cycle, named-counterparty-pattern deep-dives when a new vertical opens. Cross-reference [chapter 03](../03-vendor-contract-suite-and-onboarding-workflow.md) where the mirrored vendor-side playbook training is covered.
6. **Change-log retention.** The retention posture — the change log is the record counsel reaches for when a dispute two years later turns on why a clause was written a specific way. Name the retention period and the surface where the log lives.

## Starter guidance

- Chapter 02 is the primary reference and provides illustrative tables for most Part A rows. Lift the row structure; do not lift the numeric defaults without pressure-testing them against Lumenark's actual deal mix and insurance tower.
- The ACV distribution in the problem statement is the forcing function on Part B tier definitions. 15 enterprise deals (ACV >= $100k) per quarter and the balance mid-market and self-serve-expansion is the shape the thresholds must fit. Do not duck the self-serve tier — chapter 02 is explicit that self-serve closes should be clickwrap-only.
- The 48-hour standard-tier target in Part C is the executive commitment, not a stretch goal. Build the SLA back from that commitment and name the headcount and tooling assumptions it rests on.
- Do not invent real counterparty counsel names, real top-tier-litigation-firm rate ranges, or real benchmark statistics for outside-counsel hourly rates, MFN-breach damages, or SLA-miss termination patterns. Any such figure gets `<!-- needs-research: ... -->` and a note on the refresh step.
- Defer the AI-specific clause architecture (training-data use, output ownership, hallucination liability) to [chapter 06](../06-ai-vendor-contracts-and-ai-dpa-pattern.md); the chapter 02 playbook names the escalation trigger, not the substantive answer.
- Defer the CLM mechanics (obligation tracking, signature workflow, version-of-record storage) to [chapter 07](../07-clm-stack-and-legal-ops-graduation.md); the chapter 02 playbook consumes the CLM, it does not design it.
- Defer the vendor-side mirror of the playbook — Lumenark on the counterparty side of a procurement contract — to [chapter 03](../03-vendor-contract-suite-and-onboarding-workflow.md). The customer-side playbook and the vendor-side playbook have different ideal rows; do not conflate them.
- Pin the Part A insurance ladder and the LoL / indemnification super-cap ceilings to the [mod-112](../../mod-112-insurance-and-risk-financing/) tower structure. Chapter 02 is explicit that a cap exceeding the tower by an order of magnitude is a walk-away; do not propose one without flagging the insurance interaction.
- Defer the DPA-side data-breach-notification and processor-flowdown mechanics to [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/); the chapter 02 playbook names the notification-window position, not the state-and-sector overlay.
- Nothing in this exercise is a legal determination. The clause-text drafts in Part E are operational drafts the general counsel signs off; counsel sign-off is a named step in the worked scenarios, not a hand-wave.

## Deliverables

- `fallback-matrix.md` — Part A.
- `deal-desk-routing.md` — Part B.
- `legal-turn-sla.md` — Part C.
- `escalation-triggers.md` — Part D.
- `redline-worked-scenarios.md` — Part E.
- `playbook-governance.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. Part A's fallback matrix covers each of the eleven clause families named in the requirements (LoL, indemnification, IP ownership, warranty, TfC, SLA credits, MFN, audit, renewal, assignment, insurance), in the chapter 02 ideal / acceptable / walk-away / trade-offs / rationale structure, with operative row text rather than summaries.
2. Each Part A row carries at least one pre-approved trade-off (hold-X-in-exchange-for-giving-Y) and one rationale sentence a deal-desk analyst can read verbatim to counterparty counsel.
3. Part A's insurance row and the LoL / indemnification super-cap rows pin to the [mod-112](../../mod-112-insurance-and-risk-financing/) tower reality — any cap, super-cap, or additional-insured position beyond the tower is explicitly flagged as a walk-away or carries a `<!-- needs-research: ... -->` marker on the specific tower-ceiling figure.
4. Part B names the four deal tiers (self-serve, mid-market, enterprise, strategic) with Lumenark-specific thresholds, the clear-alone authority, the route-to-counsel threshold, the route-to-executive-sponsor threshold, and the CLM evidence discipline.
5. Part C's SLA names hours (not days) per tier, the clock-start and clock-pause definitions, the at-risk escalation path, and the quarterly measurement cadence tied to the chapter 02 metrics-that-matter list. The 48-hour standard-tier target is honoured, not quietly relaxed.
6. Part D's trigger list covers deal-size, clause-level, counterparty-signal, vertical-first-deal, and novel-AI-term triggers, plus the outside-counsel budget-and-escalation pattern; any outside-counsel-rate figure not in the chapter carries a `<!-- needs-research: ... -->` marker.
7. **Part E's three worked scenarios each include the tier determination, the clause-by-clause disposition, the exact counter-language pulled from the Part A acceptable position, the rationale citation, and the escalation decision tied to a named Part B or Part D trigger.** A worked scenario that recommends "accept" or "walk" without the matrix-row citation is unacceptable.
8. Part E deal (i) names at least one Part D escalation trigger (uncapped IP indemnification, counterparty counsel from a top-tier litigation firm, or struck mutual consequential-damages waiver); deal (ii) treats both the feature MFN (Part A walk-away) and the TfC separately; deal (iii) names the regulated-financial-services vertical-first-deal trigger and the counsel-sign-off step.
9. Part F covers the quarterly review cadence, the revision triggers (including the [mod-112](../../mod-112-insurance-and-risk-financing/) insurance-tower interaction), the approval-authority chain, the versioning convention, the training programme, and the change-log retention posture.
10. Deferrals to sibling modules and sibling chapters are named explicitly where the chapter 02 ownership boundary assigns the mechanic elsewhere — [chapter 01](../01-customer-contract-suite-msa-sla-dpa-security-aup.md) for the underlying clause text and SLA architecture, [chapter 03](../03-vendor-contract-suite-and-onboarding-workflow.md) for the vendor-side mirror, [chapter 06](../06-ai-vendor-contracts-and-ai-dpa-pattern.md) for AI-specific clauses, [chapter 07](../07-clm-stack-and-legal-ops-graduation.md) for the CLM mechanics, [mod-110](../../mod-110-privacy-data-governance-and-sector-compliance/) for the DPA state-and-sector overlay, and [mod-112](../../mod-112-insurance-and-risk-financing/) for the insurance-tower ceilings.
11. Any benchmark, hourly-rate, or market figure not in chapter 02 or resources.md is flagged with `<!-- needs-research: ... -->` — specific outside-counsel hourly-rate ranges, specific insurance-tower ceiling figures, specific MFN-breach damages patterns, specific SLA-miss termination data. No real counterparty names, no real law-firm names, and nothing left as `[TBD]` or `[FILL IN]`.
12. The Lumenark Systems fictional-company frame is maintained throughout; no real-company names are invented, and the three in-flight deals from the problem statement are the test cases Part E walks end-to-end.
