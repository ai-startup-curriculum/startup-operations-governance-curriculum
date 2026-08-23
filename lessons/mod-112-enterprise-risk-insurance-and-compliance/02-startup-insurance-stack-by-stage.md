# 2. The startup insurance stack, by stage

> The insurance stack is a stage-triggered assembly, not a one-time purchase. Each line addresses a specific risk that becomes real at a specific point — first hire, first paying customer, first outside director, first international engineer.

## Motivation

An early-stage company that thinks about insurance only at renewal time is buying two of the wrong things and missing three of the right ones. Insurance is one of the most efficient risk-transfer tools available to a startup — but only when the stack is assembled in the right order, at the right stage, with the right broker, and with the discipline that the answers on the application are **warranties** the company can defend under audit.

This chapter is the stack-assembly map. It covers what to buy, when to buy it, why, and where the D&O and workers-comp deep-dives live. It does **not** cover the enterprise-risk-management operating framework above it (see [chapter 01](./01-enterprise-risk-management-operating-framework.md)) or the cyber-insurance operational layer beneath it (see [chapter 03](./03-cyber-insurance-and-incident-response-coordination.md)).

## First principles

Two working conventions before naming the lines.

**Occurrence vs. claims-made triggers.** An **occurrence-triggered** policy covers events that happen during the policy period, whenever the claim is later made. A **claims-made** policy covers claims first made against the insured during the policy period (subject to a retroactive date). General Liability is typically occurrence; Tech E&O, Cyber, EPLI, D&O, and Fiduciary are claims-made. The practical consequence: **claims-made policies must be continuously renewed or a tail (Extended Reporting Period) purchased at termination**, or historical exposure becomes uninsured.

**Application answers are warranties.** Every material representation on an insurance application — MFA deployed on all administrative access, wage-and-hour compliance, no known incidents, revenue-recognition method, EDR on all endpoints — is a warranty the insurer will read at claims time. Misrepresentation, even innocent, can void coverage. The signatory (typically the CEO, CFO, or Head of Ops) must be able to defend every answer against operating reality.

## Stage-by-stage assembly

The stages below track a venture-backed C-corp. Adjust for hardware-heavy or lab-heavy startups, which reach some lines earlier.

### Idea → pre-seed

**General Liability (GL) — occurrence.** Third-party bodily-injury and property-damage coverage. Trigger: your first office (even a WeWork seat), your first in-person event, your first vendor requiring a Certificate of Insurance. Often bundled with commercial-property coverage (laptops, office contents) as a **Business Owner's Policy (BOP)**. Cost is modest and the coverage is the baseline every landlord, event venue, and enterprise customer will ask for.

**Workers' Compensation.** The moment the first W-2 employee starts, workers-comp is a **statutory requirement** in every state that has a comp system (all except Texas as a subscribing default — see [chapter 07](./07-workers-comp-multi-state-posture.md)). Set up before the start date, not after.

Everything else is optional at this stage. Founders can defer D&O, EPLI, and Tech E&O until real customers, real employees, or a real outside board seat make them necessary.

### Seed

**Technology Errors & Omissions (Tech E&O) + Cyber — claims-made.** Trigger: first paying customer. Tech E&O covers the company's professional-services and technology-products liability — claims that the product failed, was defective, missed a spec, or caused a customer economic loss. In modern markets, Tech E&O is nearly always bundled with **Cyber** — the two triggers frequently overlap and separate policies create coverage-allocation fights. Detailed cyber-coverage design and the incident-response coordination layer live in [chapter 03](./03-cyber-insurance-and-incident-response-coordination.md).

**Employment Practices Liability Insurance (EPLI) — claims-made.** Trigger: any headcount growth above the founder team; a common formal trigger is the first ten employees. Covers wrongful-termination, harassment, discrimination, retaliation, and related employment claims. **Wage-and-hour** claims are the largest EPLI exposure by settlement dollar and are typically **excluded** or heavily sub-limited (a common sub-limit sits at $100k–$250k defence-only). Read the wage-and-hour endorsement carefully; California employers in particular should insist on the highest wage-and-hour sub-limit the broker can source.

**Directors & Officers (D&O) — claims-made.** Trigger: first outside board seat (typically the seed lead's board observer or director). D&O covers directors and officers for wrongful acts in that capacity — mismanagement claims, breach-of-fiduciary-duty claims, disclosure claims. Three coverage "sides":

- **Side A** — direct payment to individual directors and officers when the company **cannot** indemnify them (insolvency, statutory prohibition, derivative suit where indemnification is barred). Non-negotiable at the seed / Series-A moment; a good outside director will not take the seat without confirmation of Side A coverage.
- **Side B** — reimburses the company for indemnification payments to directors and officers.
- **Side C** — entity coverage for the company itself in securities claims. Standard at private-company D&O, becomes central at IPO and public-company D&O.

The full **D&O design detail** — Broad-Form vs. traditional forms, retention structure, priority-of-payments language, Side A DIC (difference-in-conditions) layers, the interplay with the DGCL § 145 indemnification agreement, and the audit-committee reporting on D&O — lives in [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/). This chapter records only that D&O enters the stack at seed / Series-A and belongs on the audit-committee agenda.

### Series A

Firm up everything from seed. In addition:

**Umbrella (Excess Liability).** Trigger: contractually-required limits exceed primary policy limits. Umbrella / excess policies sit on top of GL, Employer's Liability (Part B of workers-comp), Auto (where applicable), and sometimes D&O and E&O — raising available limits without buying larger primary policies. A typical structure at Series A layers a $5M umbrella above GL and Auto; larger customers may require $10M or more.

**Commercial Auto (if applicable).** Trigger: company-owned vehicles or a regular pattern of employee driving on company business. Where employees use personal vehicles for company business ("hired and non-owned"), a **Hired & Non-Owned Auto** endorsement on GL or a stand-alone policy fills the gap — many small-employer auto claims fall into this seam.

### Series B

**Fiduciary Liability — claims-made.** Trigger: sponsoring an ERISA-covered plan (typically the 401(k)). ERISA imposes personal fiduciary liability on plan fiduciaries — the officers who make plan decisions — for breach of prudence, loyalty, or diversification duties. Fiduciary Liability is the specific insurance for those claims; it is **not** covered by D&O (D&O policies exclude ERISA claims by design). The benefits and 401(k) substance is owned in [mod-106](../mod-106-compensation-architecture-and-total-rewards/); this line belongs on the mod-112 stack.

**Crime / Fidelity (Commercial Crime).** Trigger: employees have access to funds, negotiable instruments, or wire-transfer authority — effectively, any company with a finance function. Covers employee dishonesty (theft by insiders), funds-transfer fraud (a wire sent under fraudulent instructions), and computer fraud. **Social-engineering / impersonation fraud** — the classic "CEO email tells the controller to wire $200k to a new vendor" pattern — sits in a well-known gap between Crime and Cyber policies. Read the social-engineering endorsement carefully; ensure it is affirmative coverage, not a sub-limit hidden in either policy.

**Employed Lawyers.** Trigger: an in-house legal team exists. Covers claims against employed attorneys for acts in their in-house capacity. Small line; matters primarily to the general counsel and their team.

### Pre-IPO

**D&O — IPO-track uplift.** Trigger: S-1 preparation. The D&O programme is materially restructured for IPO — larger Side C limits, Side A DIC layers, book-of-limits stacked with multiple insurers, and a public-company-form Broad-Form policy. Handled in [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).

**Representations & Warranties (R&W).** Trigger: negotiating an M&A transaction (as seller or buyer). Buy-side R&W policies allow the buyer to transfer seller-representation liability from an indemnity escrow to an insurer — reducing seller escrow / holdback amounts and giving the buyer a solvent counterparty for post-closing breach claims. Underwriting requires a diligence-copy review, a signed no-claims declaration, and a specific retention structure. <!-- needs-research: cite the current R&W market benchmark retention (historically 0.75%–1% of enterprise value) and typical premium rate on limit (historically ~2.5%–3.5%) once verified against current broker benchmarks. -->

**Key-Person Life.** Trigger: a lender or a strategic investor demands it as a condition of financing, or the board judges that the death or disability of a specific individual would materially impair the enterprise value. Rare in venture practice — a strong case is a solo founder with an exceptional funding structure, a scientist whose IP contribution is central and inseparable, or a debt covenant that requires it.

## The broker relationship

Insurance is placed through a broker — not directly with the carrier for most lines. A **startup-focused broker** understands the stage-by-stage assembly above, has depth on Tech E&O + Cyber + D&O forms, and has claims-advocacy staff who represent your interests when a claim goes into dispute.

Names commonly cited in the venture ecosystem:

- **Embroker** — https://www.embroker.com/
- **Vouch** — https://www.vouch.us/
- **Newfront** — https://www.newfront.com/
- **Woodruff Sawyer** — https://woodruffsawyer.com/
- **Marsh** — https://www.marsh.com/
- **Aon** — https://www.aon.com/

(Listing is descriptive, not an endorsement.) At seed and Series A, a full-service digital-first broker (Embroker / Vouch / Newfront) is usually sufficient. By Series B or when the D&O programme becomes complex, larger brokers (Woodruff Sawyer, Marsh, Aon) bring depth on public-company forms, R&W, and specialty markets.

A **good broker** delivers placement, benchmarking against similar-stage peers, application discipline, claims advocacy, mid-term policy amendments as headcount and geography change, and a proactive renewal timeline. A **bad broker** delivers a spreadsheet of quotes and no advice. Interview at least two brokers for any placement over $50k in annual premium.

The **ownership boundary**: the broker is the intermediary; the company (specifically the **head of Ops or GC + CFO combination**) owns the risk-transfer strategy. Never delegate the read of the policy to the broker alone. Policies are contracts, and the party reading them for the company's benefit is the company.

## Application discipline

Insurance applications are underwriting instruments. The answers are treated as **material representations** — reliance on which the carrier issued the policy. Misrepresentation, even innocent, can void coverage; deliberate misrepresentation can constitute fraud.

The checklist for a serviceable application-review workflow:

- **A single owner** for each application — typically the Head of Ops, GC, or CFO — who assembles inputs from each attesting function (CISO for cyber controls, VP People for wage-and-hour and headcount, CFO for revenue and financials, GC for prior claims and litigation).
- **Source the answers from operating reality.** Do not answer "MFA on all administrative access" if MFA is bypassed on the break-glass account — either fix the bypass first or answer accurately with the exception noted.
- **The signatory reads the application before signing.** The CEO or CFO who signs is attesting personally to the accuracy of every answer. Read the questions and answers, not just the signature page.
- **Retain the application and every supporting attachment** in the corporate insurance record for the full statute-of-limitations period on any coverage question. If a claim arises three years later and the carrier alleges misrepresentation, the record is the defence.

Application questions have hardened materially since 2020 on cyber (see [chapter 03](./03-cyber-insurance-and-incident-response-coordination.md)) and since 2023 on AI (some carriers now require attestations about model-governance and AI-safety programmes). Assume the questions will get harder each renewal.

## Renewal cadence — the 90-day-out checklist

Renewals for D&O, Cyber, and EPLI in a hard market cannot be handled in the last two weeks before expiration. The disciplined pattern:

- **T-120 days.** Broker kick-off. Review current programme, discuss appetite for restructuring, agree markets to approach.
- **T-90 days.** Application drafts circulated to internal signatories. Loss-run pulled from carriers. Financials assembled.
- **T-60 days.** Applications submitted. Broker markets. Underwriter Q&A rounds begin.
- **T-45 days.** First indications from markets. Discuss whether to accept, negotiate, or approach additional markets.
- **T-30 days.** Terms finalised. Binding order to broker.
- **T-15 days.** Policy documents received. **Read them.** Compare against binding order for material differences. Address any deviations before bind.
- **T-0.** Renewal effective.

Cyber and D&O in a hard market should start earlier — 150 days is not too aggressive if the last renewal was painful.

## Stage-by-stage summary table

| Stage | GL / BOP | Workers-Comp | Tech E&O + Cyber | EPLI | D&O | Umbrella | Fiduciary | Crime | R&W |
|---|---|---|---|---|---|---|---|---|---|
| Pre-seed | ✔ | on first hire | — | — | — | — | — | — | — |
| Seed | ✔ | ✔ | ✔ | ✔ (first ~10 FTE) | ✔ (first outside board seat) | — | — | — | — |
| Series A | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | — | — | — |
| Series B | ✔ | ✔ | ✔ | ✔ | ✔ (uplift) | ✔ | ✔ (on 401(k)) | ✔ | — |
| Pre-IPO | ✔ | ✔ | ✔ (uplift) | ✔ (uplift) | ✔ (IPO restructure) | ✔ (uplift) | ✔ | ✔ | ✔ (if M&A track) |

Premium and limit magnitudes are deliberately absent from this table — those depend on revenue, headcount, geography, industry, loss history, and current market conditions, and inventing numbers would mislead. Benchmarks come from the broker at each renewal.

## Ownership boundary

- **The insurance stack strategy and the broker relationship**: this chapter.
- **The cyber-insurance operational layer and incident-response carrier coordination**: [chapter 03](./03-cyber-insurance-and-incident-response-coordination.md).
- **Workers-comp state-by-state posture and classification codes**: [chapter 07](./07-workers-comp-multi-state-posture.md).
- **D&O coverage design in detail, including Sides A/B/C, DGCL § 145 indemnification agreement interplay, and audit-committee reporting**: [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).
- **Fiduciary Liability benefits interaction (401(k), medical, disability plan design)**: [mod-106](../mod-106-compensation-architecture-and-total-rewards/).
- **International-employer liability, foreign-employer's-liability endorsements, and global insurance programme structure**: [mod-113](../mod-113-international-expansion-and-global-workforce/).

## Summary

- **The insurance stack is stage-triggered.** GL and workers-comp from day one; Tech E&O + Cyber, EPLI, and D&O at seed / Series A; Fiduciary, Crime, and Umbrella at Series B; R&W and D&O uplift at pre-IPO.
- **Occurrence vs. claims-made trigger matters at termination.** Claims-made lines require a tail (Extended Reporting Period) or continuous renewal, or historical exposure goes uninsured.
- **Application answers are warranties.** Assemble applications from operating reality, review with the attesting function, and let the signatory read before signing. Retain the file.
- **Choose a startup-focused broker deliberately** and treat them as intermediary, not owner of the risk-transfer strategy.
- **The 90-day-out renewal cadence** is the difference between a placed renewal and a scramble; hard-market Cyber and D&O want 120+.
- **D&O detail lives in [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/)**; **workers-comp posture lives in [chapter 07](./07-workers-comp-multi-state-posture.md)**; **cyber-insurance operational coordination lives in [chapter 03](./03-cyber-insurance-and-incident-response-coordination.md)**. This chapter is the stack-assembly map that sits between them.
