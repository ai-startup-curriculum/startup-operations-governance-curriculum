# Exercise 05 — Founder conflict-of-interest teardown

> Estimated time: **~3 hours** · Related chapter: [06 — Founder conflict-of-interest baseline](../06-founder-conflict-of-interest.md)

## Problem statement

The three-founder corporation is now 18 months into its life. The board has three seats: Alex (CEO / founder-director), Priya (CTO / founder-director), and one outside director recruited at the seed round. A number of transactions and situations have accumulated that touch DGCL § 144, the *Caremark* oversight duty, the corporate-opportunity doctrine, and the anti-loyalty-conflict baseline. Your job is to (a) diagnose each item, (b) draft the § 144 cleansing consent (or the retroactive ratification), and (c) produce a *Caremark* oversight upgrade the board can adopt at its next meeting.

Every fact pattern below has a diagnostic pathway in chapter 06. Do not invent facts beyond what is given. Where a `<!-- needs-research -->` marker in chapter 06 flags the 2024 DGCL § 144 amendments (SB 313 / SB 21), treat the safe-harbor architecture in the chapter as the operating spine and note that the specific statutory text should be re-verified against current DGCL before any real-world drafting.

## Facts

### Item 1 — The training-dataset license

Priya (CTO) owns 100% of an LLC that owns a specialised training dataset the corporation needs. The proposed license is $50k / year for 3 years plus a $200k up-front fee. Priya obtained three comparable-dataset quotes from independent vendors: $65k, $80k, and $55k / year, each with higher up-front fees than $200k. Priya wants to sign the license this quarter.

### Item 2 — The spouse-hire

Alex's spouse was hired 14 months ago as a "senior product manager" at $180k / year. There is no board consent authorising the hire, the salary, or any of the terms. The spouse's compensation was set by Alex unilaterally. The spouse's title, responsibilities, and market-comparability are all reasonable; the process is not.

### Item 3 — The founder-equity refresh

Marcus (VP GTM) is being considered for a founder-equity refresh of 500,000 additional shares of common stock at $0.75 per share (the current 409A valuation). The proposal is being circulated by Alex; Marcus is a founder and an officer but not a director. The corporation does not yet have a compensation committee.

### Item 4 — The ignored *Caremark* red flag

Two months ago, the corporation's Head of Security escalated a series of privileged-access-key rotations that had not occurred in over 12 months. The escalation reached Alex and Priya via email. Alex acknowledged the email; the item was not added to a board agenda. Last week the corporation was notified of a suspected unauthorised access to a customer-data snapshot. The board has not formally discussed either the pre-incident escalation or the current incident.

### Item 5 — The corporate opportunity

Priya was approached at a conference by a former colleague seeking a technical co-founder for a new startup building distributed inference tooling — squarely in the corporation's business. Priya has not disclosed the approach to the board. The approach is 6 weeks old.

### Item 6 — The moonlighting

Marcus disclosed on formation day that he holds an outside advisory position with a portfolio company of his prior employer's VC arm (annual $10k stock compensation). The corporation's board consent at formation day acknowledged the arrangement. This month, the portfolio company changed its go-to-market focus and now overlaps with the corporation's target market.

### Item 7 — The prior-employer overhang

An old email surfaced in a broader legal-hold review indicating that Alex's prior-employer PIIA has an assignment clause slightly broader than Alex represented on formation day. The prior employer has not asserted any claim. There is no active dispute.

## Requirements

### Part A — Item-by-item diagnostic

For each of the seven items, produce a diagnostic entry (≤ half a page each) covering:

1. **What kind of conflict / duty issue.** DGCL § 144 interested-director or interested-officer transaction? *Caremark* oversight duty? Corporate opportunity? Moonlighting / competitive activity? Prior-employer overhang?
2. **Who is interested / has the duty issue.**
3. **Cleansing pathway.** DGCL § 144(a)(1) disinterested-director approval, § 144(a)(2) disinterested-stockholder approval, § 144(a)(3) substantive fairness, DGCL § 122(17) corporate-opportunity waiver, or *Caremark* board oversight upgrade.
4. **Retroactive vs. prospective.** Which items require ratification of past conduct vs. clean-authorisation of a forthcoming action?
5. **Documentation the record needs.** Board consent recital elements, market-comparability memo, disclosure attestations, resignations, etc.

### Part B — Draft the § 144 board consents

Draft the specific board-consent language that cleanses each of the § 144 items (Items 1, 2, 3, and 6). Each consent must include, per chapter 06's "Documentation the § 144 process needs" section:

- Identity of the interested director / officer.
- Nature of the relationship or interest.
- Material terms of the transaction.
- Market-comparability or fairness rationale (for Item 1, use the three quotes explicitly; for Item 2, describe the market-comparability analysis to be performed).
- Recusal of the interested director.
- Affirmative vote of the disinterested director(s).
- Where applicable (Item 3, if you determine the disinterested-director approval is insufficient given no comp committee exists), the disinterested-stockholder approval route.

For Item 2 (spouse hire), draft the retroactive ratifying consent, not a fresh authorising consent. Chapter 06's "seed-Series-A pattern" section is the reference. Include the market-comparability finding and the ratification of historical payments.

For Item 6 (moonlighting), draft either a revised board consent updating the formation-day authorisation or a determination that the arrangement now requires termination or a new corporate-opportunity waiver under DGCL § 122(17).

### Part C — Corporate-opportunity waiver (Item 5)

For Item 5, produce (a) the § 122(17) analysis of whether the opportunity presented to Priya was a corporate opportunity, (b) a board consent either accepting the opportunity for the corporation, waiving it, or ratifying Priya's non-participation (if she declined the approach), and (c) a note on whether the formation-day founder agreement or charter includes any pre-existing DGCL § 122(17) renunciation that would have preempted the analysis, plus a recommendation on whether to add one going forward.

Include an updated version of the anti-conflict clause in the founder agreement (exercise 01) or PIIA (exercise 03) that requires ex ante disclosure of external opportunities in this space.

### Part D — *Caremark* oversight upgrade (Item 4)

Item 4 is the *Caremark* red-flag failure. Chapter 06 identifies four elements of the founder-director's *Caremark* baseline. Produce:

1. **Root-cause analysis.** Was this a duty-to-implement failure (no reporting system) or a duty-to-respond failure (system existed, red flag was ignored)? Distinguish per *Marchand v. Barnhill*, 212 A.3d 805 (Del. 2019).
2. **Board-consent record.** A retroactive board consent memorialising the corporation's response to the current incident — engagement of forensic counsel, customer notification obligations under state breach-notice statutes (do not invent the state statutes — flag them as a `needs-research` item if the customer footprint is not given).
3. **Ongoing oversight program.** A written program for board-level oversight of the corporation's "mission-critical" risks. Chapter 06 identifies model safety and misuse, data-privacy and security, open-source-license compliance, and export control as likely candidates for an AI-infrastructure company. Pick the three most relevant to this corporation and describe how the board will receive regular reporting on each.
4. **Whistleblower / reporting channel.** Confirm the corporation has one (from exercise 04's trade-secret baseline) or produce it now. Chapter 06 notes that the channel is *Caremark*-supportive.

### Part E — Prior-employer overhang cleanup (Item 7)

Produce a short (1-page) plan addressing Item 7:

- Confirm the extent of the prior representation Alex made on formation day.
- Assess whether the newly-surfaced language actually materially expands the prior employer's claim.
- Recommend disclosure treatment: (i) internal-only recognition (do nothing), (ii) approach the prior employer for a release, (iii) obtain a legal opinion supporting Alex's position, or (iv) disclose on the Series-A schedule of exceptions.
- Note the *Caremark* implication of *not* disclosing the item to the full board.

### Part F — Design memo

A 1–2 page memo tying the pieces together:

- Which items are curable vs. disclosable.
- Which items require action by a specific date (Item 4's data-breach response has notification obligations that may be time-boxed).
- The relationship between the DGCL § 144 process and the indemnification / D&O program (chapter 06 notes that exculpation and indemnification protect *care* mistakes, not *loyalty* breaches).

## Starter guidance

- Chapter 06 is the primary reference. Do not go past what it authorises without a note.
- For § 144(a)(1) approval, the interested-director recusal is essential — chapter 06 walks the mechanic step-by-step in the "concrete example." Model your consent after that structure.
- The 2024 DGCL amendments (SB 313 / SB 21) expanded the safe-harbor structure and codified aspects of the controlling-stockholder-transaction framework; chapter 06 flags this as a `<!-- needs-research -->` item. Note the current statutory text in your design memo but do not invent specific amendment language.
- Do not treat "the spouse's salary is market-comparable" as sufficient cleansing on its own — the § 144 process requires the *procedural* elements (disclosure, recusal, disinterested vote) *and* either substantive fairness or disinterested approval.
- For the corporate-opportunity item, DGCL § 122(17) is the mechanic that allows a corporation to renounce pre-defined categories in the charter or by board resolution. Chapter 06 covers this.
- Do not attempt to draft a *Caremark*-compliant risk-committee charter — mod-111 owns the depth. Draft the founder-scale oversight cadence.
- The reporting channel for whistleblowers should be genuinely usable (a real email address, a defined process) — a "policy paragraph without infrastructure" is a Caremark-adjacent defect.
- Reference the `<!-- needs-research -->` markers in chapters 05 and 06 for evolving statutory / rule status; do not fabricate current-state conclusions.

## Deliverables

- `conflict-diagnostic-memo.md` — Part A. Seven diagnostic entries.
- `section-144-board-consents.md` — Part B. Four (or more) board-consent drafts.
- `corporate-opportunity-waiver.md` — Part C.
- `caremark-oversight-program.md` — Part D. Including the retroactive incident-response consent, the ongoing oversight program, and the whistleblower channel confirmation.
- `prior-employer-overhang-plan.md` — Part E.
- `conflict-teardown-design-memo.md` — Part F.

## Acceptance criteria

The package is acceptable if:

1. Every item is correctly classified (§ 144 interested-director / interested-officer, *Caremark*, corporate opportunity, moonlighting, prior-employer overhang).
2. Every § 144 board consent includes the seven documentation elements from chapter 06.
3. The spouse-hire ratification (Item 2) is drafted as *retroactive* and includes both the market-comparability finding and the ratification of historical payments.
4. The Marcus refresh (Item 3) either (a) is approved by disinterested-director consent with clear disclosure and 409A support, or (b) is deferred pending independent-director / comp-committee formation with a written rationale.
5. The corporate-opportunity item (Item 5) references DGCL § 122(17) and produces a defensible board record.
6. The *Caremark* upgrade (Item 4) distinguishes duty-to-implement vs. duty-to-respond and produces a written oversight program with named risks and a reporting cadence.
7. The whistleblower / reporting channel exists in writing and names the receiving mailbox / process.
8. The prior-employer overhang plan (Item 7) makes a specific recommendation and identifies the *Caremark* implication of concealment.
9. Statutory citations (DGCL § 144, § 122(17), § 145, § 102(b)(7)) and case citations (*In re Caremark International Inc. Derivative Litigation*, 698 A.2d 959 (Del. Ch. 1996); *Marchand v. Barnhill*, 212 A.3d 805 (Del. 2019)) are correct.
10. The design memo acknowledges that exculpation, indemnification, and D&O protect *care* mistakes but not *loyalty* breaches.
