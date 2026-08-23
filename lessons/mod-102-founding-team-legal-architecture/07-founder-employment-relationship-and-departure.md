# 7. The founder-employment relationship and the departure playbook

> Founders are employees. Compensating them, offboarding them, and — sometimes — replacing them is a governance problem, not an HR footnote.

## Motivation

The founder's relationship with the corporation is layered: they are a stockholder (via the SPA and 83(b) — chapters 02 and 03), they are typically a director (chapter 06), and they render services to the corporation. The services-side of that relationship — how the founder is engaged, how they are compensated, what happens when a founder leaves — is the subject of this chapter. It is easy to get wrong for two reasons: the founder often designs their own compensation (a § 144 issue — chapter 06), and the assumption of forever-together makes departure planning feel unnecessary until a departure happens.

The prescription: treat the founder-employment relationship as an employment relationship with an employer (the corporation) that has real obligations to the founder-employee, and design the departure playbook before it is needed.

## Employee vs. independent contractor: the answer is almost always employee

At formation, some founders try to be "independent contractors" to the corporation. The intuition is: reduce payroll-tax friction, avoid W-2 wage-and-hour rules, sidestep unemployment-insurance registration. The reality is that a full-time founder who serves as an officer, sits on the board, has decision authority over the corporation's operations, and is present at the corporation's principal place of business essentially every workday almost never satisfies any of the applicable "independent contractor" tests.

The tests worth knowing:

- **IRS common-law test** (from Rev. Rul. 87-41 and the current Publication 15-A) — behavioural control (does the corporation control what work is done and how?), financial control (does the worker have unreimbursed business expenses; can they realise profit or loss?), and the nature of the relationship (is there a written contract; are there employee benefits; is the relationship expected to continue indefinitely?). A full-time founder-CEO fails behavioural and relationship prongs decisively.
- **Federal Fair Labor Standards Act (FLSA) "economic realities" test** — variously formulated. The 2024 US Department of Labor rule (29 C.F.R. Part 795) restored a six-factor totality-of-circumstances test. <!-- needs-research: verify the current status of the 2024 DOL final rule on independent contractor classification (29 C.F.R. Part 795) after any 2025–2026 rulemaking or litigation. --> A founder-CEO fails as a matter of law.
- **State-law ABC tests** — California (Labor Code § 2775, codifying *Dynamex Operations West, Inc. v. Superior Court*, 4 Cal. 5th 903 (2018) and AB 5), Massachusetts (M.G.L. c. 149 § 148B), and several other states apply a strict three-part ABC test: (A) free from control, (B) work outside the usual course of the hiring entity's business, and (C) customarily engaged in an independently-established trade of the same nature. Prong (B) alone disqualifies a founder-CEO — the CEO's work is the exact usual course of the corporation's business.
- **State corporate-law implications.** Officers under DGCL § 142 are presumed to be employees; the DGCL says nothing that would support treating an officer as a contractor for corporate-law purposes.

**Conclusion:** every full-time founder-officer is a W-2 employee. Attempting to structure them as a 1099 contractor creates worker-misclassification exposure (back-payroll-taxes plus penalties on the corporation side; loss of the founder's participation in W-2-specific benefits and protections; potential officer-personal-liability under state wage-and-hour statutes for the misclassifying officer). The narrow exceptions — a technical co-founder who is genuinely rendering discrete services on a project-by-project basis, is genuinely retained by other clients, and has no officer role — are so rare in a venture-track startup that they should not be assumed.

## The founder offer letter and employment agreement

Every founder gets a written offer letter or employment agreement at formation, alongside the SPA and PIIA. The document memorialises:

- **Position and duties.** Title (CEO, CTO, President, etc.) and a functional-area description. Titles are legible to investors and the outside world; the functional-area description prevents later "that's not my job" disputes.
- **Start date.** For vesting-start-date purposes and for tax purposes.
- **Compensation.** Base salary (see next section); bonus structure if any; benefits eligibility; equity (cross-references the SPA rather than re-describing it).
- **At-will employment.** Almost universal in the US (Montana is the notable exception). At-will means either party can terminate the relationship at any time, for any reason (or no reason) that is not otherwise unlawful. At-will status typically coexists with severance and acceleration provisions that give the founder economic protection on involuntary termination.
- **Reference to the PIIA and the SPA.** The offer letter is not a substitute for the PIIA or the SPA; it should cross-reference both.
- **Confidentiality reminders and DTSA notice** — often echoed in the offer letter, in addition to the PIIA (chapter 05).
- **Severance triggers and treatment.** What the founder gets on termination without cause, resignation for good reason, death, or disability (see the departure playbook below).
- **Restrictive covenants** — non-solicitation of employees and customers post-termination, subject to state-law enforceability limits ([mod-103](../mod-103-employment-law-and-contract-design/) has depth). Non-competes are rare and increasingly limited.
- **Choice of law and dispute resolution.** Typically Delaware or the corporation's principal-place-of-business state. Some agreements include mandatory arbitration; that is a policy choice with tradeoffs beyond this chapter's scope.

The offer letter should be signed by the corporation (by the board's designated signer or an authorised officer, per DGCL § 142) and by the founder. The corporate record archives it alongside the SPA and PIIA.

## The founder-comp tradeoff: defer for equity, or take a market salary

Founder compensation at seed / early-Series-A has two poles:

- **Defer salary for equity.** The founder takes no salary (or a nominal salary — sometimes $1 / year or $12k / year — enough to satisfy any wage-and-hour minimum and to establish the employment relationship). The founder's economic return is the equity, potentially amplified by a lower runway burn that lets the corporation raise less capital and preserve more of the founder's ownership through the round.
- **Take a market-clearing salary.** The founder takes a salary calibrated to their pre-startup market rate, or to a moderated version of it. Common seed / Series-A founder salaries are in the $100k–$200k range, sometimes higher for founders with families or geographic cost-of-living constraints. Market data sources (Kruze Consulting's annual startup founder-compensation surveys, Pave startup comp benchmarks, Carta compensation reports) publish per-stage medians. <!-- needs-research: cite current-year founder-compensation medians from at least two sources (Kruze, Pave, Carta) before drafting a specific range in a memo. -->

The tradeoff is not a moral one; it is a corporate-finance and personal-finance question:

- **Defer-for-equity** preserves runway but pushes personal-finance risk onto the founder. It is workable if the founder has personal savings, no dependents, or a supportive family financial situation. It becomes untenable when the founder cannot pay the mortgage.
- **Market-salary** de-risks the founder personally and reduces the "founder-burnout-from-personal-finance" failure mode. It costs the corporation cash that has to come from either extra dilution at the seed / Series-A or from post-financing operating cash. Given how much investor conversations focus on founder resilience through a multi-year plan, taking a moderate market salary is often the better answer.
- **Middle-path formations.** Reduced salary during the first 6–12 months while the corporation validates the market, then a scheduled bump on hitting a milestone (Series-A close, revenue target). Documented in the offer letter or in a subsequent compensation-committee (or § 144-cleansed board) approval.

**Do not:**

- **Do not pay the founder in equity as compensation without a board consent authorising the grant, cleansing the § 144 conflict, and running a § 409A valuation to establish fair market value.** Founder shares are the *original-issuance* founder restricted stock (chapter 02). Follow-on grants to a founder-officer are ordinary equity comp, priced against a 409A valuation, granted under the plan, and cleansed under § 144.
- **Do not "accrue" unpaid salary as a contingent liability to the founder.** Deferred / accrued salary that has no board approval and no market rationale creates a contingent claim on the corporation that is legible as an insider debt in diligence. If salary is deferred, either genuinely defer to nothing (no future claim) or authorise the deferral via board consent with defined repayment terms.
- **Do not treat the founder as exempt from wage-and-hour rules if they are on a non-trivial salary.** State-law exempt-status tests apply. Federal FLSA exempt-executive rules generally cover a full-time CEO, but the underlying analysis needs to be run. <!-- needs-research: verify current FLSA exempt-executive salary threshold ($43,888 / year effective July 1, 2024; scheduled increase to $58,656 January 1, 2025; status subject to 2024–2025 litigation) before writing a specific number. -->

## The founder-severance and founder-departure playbook

A co-founder departure at Series-A is not a rare event. Public data suggests it happens frequently — the framing that a co-founder change or departure is a real base-rate event at Series-A is worth designing for on formation day. <!-- needs-research: verify the "Carta ~30% co-founder-departure-by-Series-A" statistic before citing a specific number; sources for founder-departure rates through funding rounds include Carta insights reports, Startup Genome, and CB Insights, but the exact figures vary by cohort and methodology. --> The specific number matters less than the plan.

The playbook has three parts: (i) the ex-ante design (what the SPA and offer letter say happens on each separation trigger), (ii) the departure conversation (how the corporation, the board, and the departing founder handle the event), and (iii) the paperwork and cap-table treatment.

### Ex-ante design

Restate the separation matrix that the SPA (chapter 02) and offer letter document:

- **Voluntary resignation.** Vested equity stays; unvested subject to repurchase at cost; no severance; no acceleration.
- **Termination for cause.** Vested equity stays (unless a specific clawback clause applies for cause-based misconduct); unvested subject to repurchase at cost; no severance; no acceleration; departing founder subject to continuing PIIA / DTSA / trade-secret obligations.
- **Termination without cause.** Vested equity stays; unvested subject to repurchase at cost; typically 3–12 months of accelerated vesting; severance (typically 3–12 months of salary and continuation of benefits under COBRA at corporation expense for the severance period); COBRA subsidy; potentially a lump-sum bonus.
- **Resignation for good reason.** Treated as termination without cause. "Good reason" is defined narrowly — usually a material reduction in duties, title, or compensation, or a required relocation beyond a defined distance, subject to a cure period after written notice from the founder.
- **Death or disability.** Vested equity stays; unvested typically subject to a defined acceleration (often 12 months, sometimes 100%); severance treatment defined by policy; family retains vested shares subject to standard transfer restrictions.
- **Change-of-control acceleration.** As described in chapter 02, market-standard double-trigger (change-of-control + involuntary termination within a defined window) applies at some fraction (often 100% for founders). Single-trigger is uncommon and typically resisted by investors; the transaction-mechanics view lives in `startup-exit-curriculum`.

The founder agreement (chapter 01) reflects these terms in narrative form; the SPA and offer letter make them binding.

### The departure conversation

When a departure is contemplated — either because a founder wants to leave, because the board wants a founder to leave, or because the board wants to change a founder's role in a way the founder finds unacceptable — the corporation runs a structured playbook:

1. **Convene the board.** The board discusses the situation with the CEO (or, if the departing founder is the CEO, with the lead director or the independent directors) present, without the departing founder if that founder is a director and the conflict is direct.
2. **Engage counsel.** Outside counsel — the corporation's regular counsel, not the founder's personal counsel — is engaged to advise on the corporation's obligations, the § 144 cleansing of any founder-side terms, and the drafting of the separation agreement.
3. **Cleanse the § 144 conflict.** Any material change to the departing founder's compensation, severance, or equity treatment is an interested-director / interested-officer transaction. Disinterested-director approval and, where warranted, disinterested-stockholder approval are required (chapter 06).
4. **Draft the separation agreement.** The document memorialises the departure date, the severance treatment, the vesting treatment (including any accelerated vesting), the continued PIIA / DTSA obligations, cooperation with pending matters, non-disparagement (mutual is standard), a release of claims (from the founder to the corporation; and, if the corporation is offering material consideration, sometimes from the corporation to the founder), and the treatment of any outstanding advances or expense reimbursements.
5. **Consider the ADEA / OWBPA-compliant release period.** For founders age 40 or older, a release of federal age-discrimination claims requires the Older Workers Benefit Protection Act (OWBPA) formalities: 21 days to consider (or 45 for a group release), 7 days to revoke after signing, written disclosure of the eligibility factors. <!-- needs-research: confirm current OWBPA requirements are unchanged; the 21/45/7 formalities have been stable but should be re-verified against 29 C.F.R. Part 1625 before drafting a specific release. --> An untimely or non-OWBPA-compliant release does not bar age-discrimination claims.
6. **Coordinate with cap-table and share-ledger updates.** The repurchase of unvested shares (chapter 02) is documented in a board consent, executed on the share ledger, and reflected on the cap-table platform (Carta / Pulley). Vested shares stay with the departing founder and continue to be subject to standard transfer restrictions.
7. **Board and stockholder resignations.** If the departing founder is a director, they resign the board seat (in writing). If they are an officer, they resign each officer position. If they are a stockholder with voting rights on outstanding matters, the corporation confirms whether the resignation triggers any procedural obligations.
8. **Communication plan.** Internal message to the team, external message to customers / partners / press if warranted. The communication should be truthful, respectful, and tightly scoped; over-elaboration creates future defamation exposure.
9. **Return of property and off-boarding hygiene.** Return of laptops, badges, credentials; revocation of system access; termination of email forwarding; retention of the corporation's confidential information subject to continuing PIIA obligations.

### The paperwork trail Series-A will read

A departed founder's file, viewed at Series-A diligence, should contain:

- The original SPA and 83(b) receipt.
- The original PIIA (with DTSA notice).
- The original offer letter.
- The separation agreement (with signatures and OWBPA compliance where applicable).
- The board consent approving the separation terms, cleansed under § 144.
- The board consent approving the repurchase of unvested shares (if repurchase was exercised).
- The share-ledger entries reflecting the repurchase and the departure-date vested count.
- The updated cap-table snapshot.
- The letter of resignation from the board seat and any officer positions.
- Any subsequent side letters or amendments.

Missing any of these creates a diligence exception. The lead investor's counsel will not object to a clean departure documented against the playbook; they *will* object to a departure that looks improvised.

## Departed-founder equity treatment: what happens on the cap table

A common failure pattern: a departed founder's residual position on the cap table becomes the subject of a Series-A renegotiation because the corporation did not exercise the repurchase right cleanly, or because the vested-shares count was miscalculated at the departure date, or because the departed founder's continuing rights (right of first refusal on transfers, notice rights) were not memorialised.

The clean-departure state:

- **Vested shares** — the departed founder holds them as a passive common-stockholder, subject to the transfer restrictions in their original SPA (ROFR, transfer restrictions). No voting rights beyond the ordinary common-stock voting rights. No board rights. No employment rights. No further ongoing obligations beyond the surviving PIIA / DTSA / trade-secret obligations.
- **Unvested shares** — repurchased at cost by the corporation via a board consent, cancelled from the share ledger, and returned to the authorised-but-unissued pool. Repurchase price paid to the departed founder via check or wire, with confirmation in the corporate record.
- **Dilution treatment** — the departed founder's vested shares are diluted pro-rata with all other common stock in subsequent financings; there is nothing special that protects the departed founder against dilution beyond their vested-share count times their pro-rata dilution.
- **Communication with the departed founder** — the corporation confirms in writing (via the separation agreement or a follow-up notice) the final vested count, the repurchase, and any surviving obligations. This is protective for both sides.

At Series-A, the departed founder appears on the cap table as a common-stockholder with a defined share count, no board rights, and no employment relationship. The lead investor's diligence question ("who is X and why do they still hold Y shares?") is answered with a one-paragraph reference to the departed-founder file. Clean.

The messy state: the departed founder holds their full pre-departure position because the repurchase was never exercised; they retained a "consulting" role that was never terminated; the separation agreement was verbal; there is a pending unresolved severance-payment dispute. The Series-A lead insists on cleaning it up before closing. This is expensive and, worst case, requires cash payments to the departed founder to buy their consent to a clean-up.

## Concrete example: the CTO-departure playbook in action

A four-person founding team at month 22, four months before an anticipated Series-A. The CTO wants to leave to found a different company. The remaining founders are supportive.

Playbook execution:

1. The board convenes without the CTO (who is a director). The CEO and outside director agree on a separation plan.
2. Outside counsel engaged to draft the separation agreement.
3. The board approves, via written consent with the CTO recusing:
   - CTO departure date (30 days out to allow for transition).
   - Severance: 3 months' base salary, continued benefits under COBRA at corporation expense for 3 months.
   - Acceleration: 3 months of additional vesting on the departure date (standard for termination without cause per the SPA; extended here to 3 months regardless of characterisation as termination-vs-resignation because the situation is amicable).
   - Repurchase of remaining unvested shares (post-acceleration) at par per the SPA.
   - Continued PIIA and DTSA obligations, plus a limited non-solicit of the corporation's employees for 12 months.
   - Full mutual release of claims, with OWBPA-compliant formalities (CTO is 42, over 40 threshold).
   - Non-disparagement (mutual).
   - Board resignation and CTO / officer position resignations effective on the departure date.
4. The board consent cleanses the § 144 conflict: the CTO recuses; the remaining two disinterested directors approve.
5. The separation agreement is signed. The CTO takes 21 days to consider (per OWBPA), signs on day 15, retains the 7-day revocation right, does not revoke.
6. Repurchase of unvested shares is executed via a second board consent authorising the repurchase, delivery of the repurchase price ($625.50 for 6,255,000 unvested shares at $0.0001 par), and cancellation on the ledger.
7. Cap-table platform (Carta) updated. Vested count = 2,745,000 shares of common stock, held by CTO as a passive common-stockholder.
8. Internal announcement to the team; short external note to the corporation's customers and partners; no press release.
9. CTO returns laptop, revokes credentials, signs a certification confirming return of confidential information.
10. Series-A diligence four months later: the CTO's file is complete; the lead investor's counsel notes the clean departure and moves on.

Total elapsed time: ~5 weeks. Total counsel cost: modest. Total cap-table clarity: high.

## Summary

- Founders are W-2 employees of the corporation. Attempting to classify them as independent contractors creates worker-misclassification exposure and does not survive federal or state tests.
- Every founder gets a signed offer letter or employment agreement at formation, cross-referencing the SPA and PIIA and documenting position, compensation, at-will status, severance, and confidentiality obligations.
- Founder compensation is a defer-for-equity vs. market-clearing-salary tradeoff. Follow-on equity grants to founders are cleansed § 144 transactions, granted under the plan at 409A-supported strike prices.
- Design the founder-departure playbook on formation day. Series-A is not the time to invent the separation matrix.
- The separation playbook: convene the board; engage counsel; cleanse the § 144 conflict; draft the separation agreement with OWBPA-compliant releases where applicable; execute the repurchase of unvested shares; update the ledger and cap-table; coordinate resignations and communication.
- Departed founders leave with vested shares (subject to transfer restrictions), the unvested shares repurchased at cost, and defined surviving obligations. The clean-departure file is what the Series-A investor reads and accepts.
