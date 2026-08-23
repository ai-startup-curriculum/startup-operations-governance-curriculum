# 6. Founder conflict-of-interest baseline

> A founder who wears both a director hat and a personal-interest hat is one bad transaction away from a stockholder lawsuit. DGCL § 144 and *Caremark* are the guardrails.

## Motivation

A founder in a Delaware C-corp is usually three things simultaneously: a *stockholder* (they own founder common stock), an *officer* (CEO, CTO, President), and a *director* (they sit on the initial board). Each hat carries its own duties, and the duties collide whenever the founder's *personal* interest — a related-party transaction, a business opportunity, a moonlighting commitment, a prior IP claim — touches the corporation's business. This chapter walks the four founder-conflict exposures that show up most often at seed and Series-A: DGCL § 144 interested-director transactions, the *Caremark* oversight duty, corporate-opportunity doctrine, and the anti-loyalty-conflict baseline (moonlighting, competitive activity, pre-existing IP disputes).

Board-operations depth — the full fiduciary-duty framework, duty of care vs. duty of loyalty, the demand-futility doctrine, the D&O program design — belongs to [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/). This chapter's ownership is: the founder-specific conflicts a founding team needs to see on formation day and manage across the first several years.

## DGCL § 144: interested-director transactions

**DGCL § 144(a)** provides that no contract or transaction between the corporation and one or more of its directors or officers, or between the corporation and any other entity in which one or more of its directors or officers are directors or officers, or have a financial interest, shall be void or voidable solely because the director or officer is present at or participates in the meeting of the board or committee which authorises the contract or transaction, or solely because the director's or officer's votes are counted for the purpose, if — one of three cleansing conditions is met:

1. **Disclosure and disinterested-director approval** — the material facts as to the director's relationship or interest and the contract or transaction are disclosed or known to the board or committee, and the board or committee in good faith authorises the transaction by the affirmative votes of a majority of the disinterested directors, even though the disinterested directors constitute less than a quorum; or
2. **Disclosure and disinterested-stockholder approval** — the material facts are disclosed or known to the stockholders entitled to vote thereon, and the transaction is specifically approved in good faith by the vote of the stockholders; or
3. **Substantive fairness** — the contract or transaction is fair as to the corporation at the time it is authorised, approved, or ratified.

The Delaware Bar substantially amended § 144 in 2024 (SB 313). <!-- needs-research: verify the exact scope and effective-date treatment of the 2024 DGCL § 144 amendments (SB 313 / SB 21 depending on session naming) — the amendments expanded and clarified the safe-harbor structure and codified certain aspects of the controlling-stockholder-transaction framework previously developed in Delaware case law (MFW, KKR/Cornerstone). --> The safe-harbor architecture above is the operating spine; the amendments should be reviewed against current statute text before drafting a specific interested-director consent.

### What counts as an "interested" director transaction for a founder-director

- The corporation licenses IP *from* the founder (rather than the founder assigning it under the PIIA).
- The corporation buys equipment, services, or facilities *from* a company the founder owns.
- The corporation hires the founder's spouse, sibling, or close family member.
- The corporation invests in — or receives investment from — an entity in which the founder holds a material stake.
- The corporation extends a loan, advance, or expense reimbursement to the founder outside of ordinary-course compensation.
- The corporation grants the founder equity (a follow-on grant, an option refresh, a repricing) — this is compensation and is analytically an interested-director transaction unless authorised by an independent compensation committee.
- The corporation acquires or sub-licenses a technology or product line from an entity the founder controls.
- A change to the founder's own compensation, severance, indemnification, or grant terms.

Any of these should be flagged, disclosed on the record, and cleansed through the § 144 process. The mechanic — even at a founder-heavy board with two founder-directors and no independents — is:

1. The interested founder-director recuses from the deliberation and the vote.
2. The other director(s) receive full disclosure of the material facts.
3. The disinterested director(s) authorise the transaction by affirmative vote, in good faith.
4. The consent minutes reflect the disclosure, the recusal, and the vote.

For a two-founder board where both founders are interested (e.g., an equity refresh to both), the disinterested-stockholder approval route (§ 144(a)(2)) may be needed, or the transaction is approved by an independent director appointed for the purpose, or the corporation demonstrates substantive fairness (§ 144(a)(3)).

### The seed-Series-A pattern

A recurring pattern at seed / Series-A: the corporation has been paying the founder's spouse as a "contractor" or as a full-time employee for the past 14 months; there is no board consent authorising the arrangement; the spouse's compensation was set by the founder unilaterally. On diligence, this is an interested-officer transaction that was never cleansed. The fix — retroactive board ratification with (i) disclosure to the disinterested director(s), (ii) a documented finding of substantive fairness (market-comparable compensation), and (iii) a resolution ratifying the historical payments — is straightforward but must be done deliberately.

The cleaner path: run every related-party transaction through the § 144 mechanic at the time it happens. Board consents for related-party transactions are cheap. Retroactive ratifications are more expensive and legible as a diligence exception.

### Documentation the § 144 process needs

A defensible § 144 board consent for a related-party transaction includes:

- The identity of the interested director / officer.
- The nature of the relationship or interest (family relationship; equity stake; direct financial interest).
- The material terms of the transaction (price, scope, term).
- The market-comparability analysis or fairness rationale.
- The recusal of the interested director.
- The affirmative vote of the disinterested director(s).
- Where applicable, disclosure to and approval by the disinterested stockholders (with the notice, information statement, and vote tally attached).

Standard-form templates for interested-director / interested-officer transaction consents are available from every startup-focused firm's document library (see mod-101's [resources.md](../mod-101-legal-entity-formation-and-corporate-structure/resources.md) for pointers).

## The *Caremark* oversight duty and the founder-director

**In re Caremark International Inc. Derivative Litigation**, 698 A.2d 959 (Del. Ch. 1996), established that directors have an affirmative duty to make a good-faith effort to implement and monitor a corporate information and reporting system to identify law-compliance risks. A director who consciously fails to implement any reporting system, or consciously ignores red flags from an existing system, can face personal liability for the resulting corporate harm.

The Delaware Supreme Court reinvigorated Caremark in **Marchand v. Barnhill**, 212 A.3d 805 (Del. 2019) (Blue Bell Creameries listeria outbreak — board had no committee, no monitoring system, no reporting mechanism for food-safety issues), and subsequent decisions (In re Clovis Oncology, In re Boeing, Firemen's Retirement System v. Sorenson, and others) have raised the practical stakes for boards in "mission-critical" risk areas.

For a founder-director at a seed / Series-A company, the *Caremark* baseline is not "have a committee for every risk area." It is:

- **The board actually meets and documents its meetings.** Board consents for material actions; regular board meetings at a defined cadence; minutes recording the substance of what was discussed (mod-111 depth).
- **The board attends to the corporation's known material risks.** For a fintech, financial-controls and BSA/AML monitoring. For a health-tech, HIPAA and clinical-safety. For an AI-infrastructure company, security incidents, model-safety incidents, data-privacy incidents, and open-source-license compliance. The board's regular agenda should include a compliance report from management on the identified material risks.
- **Red flags trigger response, not silence.** If a founder-director learns of a material compliance issue (a data-privacy breach, an SEC subpoena, an employee complaint of harassment, an OSHA notice), that founder-director's duty is to raise the issue at the board, drive an investigation, and drive a response. Silence — or worse, active concealment — is where personal Caremark liability attaches.
- **A reporting channel exists for employees to raise concerns.** The whistleblower policy (chapter 05 mentions the DTSA-side echo) is a Caremark-supportive discipline.

The founder-director who "does not want to be a director" and disengages from governance is not opting out of Caremark liability — they are creating it. Serving as a director carries an active oversight duty.

### The "mission-critical risk" carve-out

*Marchand* and its progeny distinguish "mission-critical" risks (food safety at a food company, drug safety at a pharma company, aircraft safety at an aerospace company) from ordinary business risks. Mission-critical risks require a specifically-designed board-level monitoring system. For an AI-infrastructure startup, the mission-critical risks arguably include:

- **Model safety and misuse** — depending on the product (frontier-model risks, biosecurity risks, misuse channels).
- **Data-privacy and security** — customer data protection is often a mission-critical trust issue.
- **Open-source license compliance** — if the product depends materially on open-source components with copyleft or attribution obligations.
- **Export control** — if the product is subject to EAR/ITAR (dual-use technology, encryption, defense-adjacent applications).

The board does not need a committee for each of these at formation. It does need a specific plan to receive information on each — a regular compliance report, a defined escalation channel, a documented risk register. Building this into the founder-director's operating cadence early is much cheaper than retrofitting it in response to an incident.

## Corporate-opportunity doctrine

Delaware fiduciary law imposes a "corporate opportunity" duty on directors and officers: an opportunity that comes to the individual in their fiduciary capacity, that is in the corporation's line of business or of practical advantage to it, and that the corporation is financially able to undertake, must be presented to the corporation before the individual can pursue it personally. If the individual takes the opportunity without disclosure and disinterested-board waiver, the corporation can sue to impose a constructive trust on the resulting benefit.

**DGCL § 122(17)**, added in 2000, permits a corporation to renounce, in its charter or by board resolution, any interest or expectancy in specified corporate opportunities. This is the mechanic that lets a founder who sits on multiple boards, or who has an outside consulting practice, or who is a limited partner in a venture fund, structure their outside activities without automatic corporate-opportunity liability.

For a founder-director at a new corporation, the correct discipline is:

- The **charter or founder agreement** identifies categories of activity the corporation is renouncing an interest in (e.g., outside board seats disclosed at formation; passive investment activity below a defined threshold).
- **New opportunities that arise during service** and that fall inside the corporation's business must be disclosed to the board and either accepted or waived.
- **The founder's outside activities are documented on formation day** so that later "was that a corporate opportunity?" disputes have a baseline.

This dovetails with the anti-conflict clauses in the founder agreement ([chapter 01](./01-co-founder-equity-split-and-founder-agreement.md)) and the moonlighting section of the PIIA ([chapter 04](./04-piia-mutual-ip-assignment.md)).

## The anti-founder-loyalty-conflict baseline

Beyond the DGCL § 144 and Caremark analyses, three founder-specific loyalty-conflict patterns show up so often that they warrant their own attention.

### Moonlighting

A founder who continues to work part-time for a former employer, who consults for other startups, or who runs a paid side-project during their service to the corporation creates three risks:

- **IP contamination.** Work done for a third party while the founder is subject to the corporation's PIIA may create ownership disputes over what work belongs to whom.
- **Time-and-attention breach.** The founder-employment relationship (chapter 07) typically requires the founder to devote their full time and attention to the corporation. Undisclosed moonlighting breaches that covenant.
- **Corporate opportunity.** Work for a third party that is in the corporation's line of business is a corporate opportunity the founder is arguably taking for themselves.

The correct baseline: no moonlighting except for pre-disclosed, board-consented arrangements captured on formation day and reviewed on any material change.

### Competitive activity

A founder starting or investing in a competitor is a per se loyalty breach. The clean baseline: no ownership of or work for a competitor during service, and — for a defined post-departure window — no work for a direct competitor (subject to state-law limits on non-competes; California is the strictest limit, but even in California a genuine trade-secret misappropriation claim can reach analogous conduct).

The founder agreement (chapter 01) and the PIIA (chapter 04) codify this at the contract level. The DGCL fiduciary duties (duty of loyalty) codify it at the equity level.

### Pre-existing IP disputes and the "unresolved former employer" problem

A founder who leaves a previous employer to found a new company sometimes carries an unresolved IP-ownership or non-compete claim from the previous employer. The consequences at formation are severe:

- The previous employer may assert an ownership claim over the founder's contributed pre-formation IP. If the claim has any traction, the corporation's ownership of that IP is contested.
- A pending or threatened non-compete claim by the previous employer can result in injunctive relief that pauses or limits the founder's work at the new corporation.
- Series-A diligence will ask directly about prior-employer obligations, and the answers become representations in the Series-A Stock Purchase Agreement.

The correct baseline:

- **Formation-day disclosure.** Every founder discloses, on formation day, any prior-employer agreements, restrictive covenants, or pending disputes. The disclosure is captured in the PIIA's Prior Inventions schedule (for IP claims) and in the founder agreement / employment agreement representations (for restrictive covenants).
- **Formation-day cleanup.** If a prior-employer obligation is genuinely contested, resolve it before or shortly after formation — either through a release from the prior employer, a legal opinion supporting the founder's position, or an explicit disclosed risk in the corporate record.
- **Do not paper over.** A prior-employer risk that is not disclosed at formation becomes a much worse problem at Series-A when investor counsel finds it.

## Interaction with D&O insurance and indemnification

The formation-day corporate record (see [mod-101 chapter 03](../mod-101-legal-entity-formation-and-corporate-structure/03-corporate-record-and-compliance-calendar.md)) includes:

- The DGCL § 102(b)(7) director exculpation clause in the charter.
- The DGCL § 145 indemnification enabling clause in the charter and mandatory indemnification in the bylaws.
- A stand-alone Indemnification Agreement between the corporation and each director / officer.
- A D&O insurance policy at appropriate limits.

These are the founder-director's protection against personal liability for good-faith performance of the fiduciary duties. Neither exculpation nor indemnification covers *loyalty* breaches — a founder-director who takes a corporate opportunity, who profits from an interested-director transaction that was not cleansed, or who acts in bad faith is *not* protected. Exculpation, indemnification, and D&O cover *care* mistakes (including many Caremark claims, subject to policy exclusions), not loyalty violations.

The founder-director should understand this asymmetry before signing the indemnification agreement: the corporation's protective architecture supports good-faith mistakes; it does not protect self-dealing.

## Concrete example: the § 144 process in action

The corporation needs to license a specialised training dataset from a limited-liability company that Founder A owns 100% of (and controls). The proposed license is $50k / year for 3 years, plus a $200k up-front fee, with terms otherwise industry-standard.

The § 144 workflow:

1. Founder A discloses to the board: her ownership of the LLC, the specific relationship, the material commercial terms of the proposed license, and the market-comparability analysis (three quotes from comparable-quality datasets from independent vendors: $65k, $80k, $55k, plus higher up-front fees).
2. The board consent recites the disclosure and Founder A's recusal.
3. The two remaining directors (Founder B and an outside director appointed on formation day) review the terms, discuss the comparable-quotes analysis, and vote to approve the license by affirmative vote.
4. The consent notes the § 144(a)(1) safe-harbor approval, attaches the market-comparability memo, and is signed by all three directors (Founder A signs to acknowledge her recusal; only the disinterested directors' votes count for approval).
5. Founder A signs the license agreement on behalf of her LLC; another authorised officer signs on behalf of the corporation.
6. The corporate secretary files the consent, the license, and the supporting memo in the minute book.

The transaction is now cleansed. Even if a future stockholder plaintiff challenges the transaction, the disinterested-director approval under § 144(a)(1) shifts the burden and, combined with the fairness support, produces a defensible position.

Compare the counterfactual: Founder A signs the license on both sides without a board consent, without disclosure, and at the market-cheap end of the range. Three years later, a Series-A investor asks about the license, discovers Founder A owns the counterparty, and — depending on facts — either asks for a ratifying consent (with the founder's continuing recusal), a renegotiation of the terms, or a full unwinding of the license. All of this is more expensive and legibly worse than the ten minutes of § 144 process at the time.

## Summary

- A founder wears three hats — stockholder, officer, director — and the duties collide at every self-interested transaction. The Delaware default is DGCL § 144: disclose, recuse, cleanse.
- Interested-director transactions include related-party purchases, family hires, corporation loans to founders, follow-on equity grants without an independent comp committee, and any transaction between the corporation and a founder-controlled entity. Cleanse through disinterested-director approval, disinterested-stockholder approval, or documented substantive fairness.
- The *Caremark* oversight duty requires directors to implement and monitor a compliance-reporting system; ignoring red flags creates personal liability. For a founder-director at a seed / Series-A company, this means real board meetings, documented minutes, agendas covering identified risks, and a reporting channel for employees.
- Corporate-opportunity doctrine binds founder-officers and founder-directors; DGCL § 122(17) allows the corporation to renounce specified categories of opportunity, which is how outside board seats and passive investments get authorised at formation.
- The anti-loyalty-conflict baseline covers moonlighting (no undisclosed outside work), competitive activity (no work for or ownership of competitors), and pre-existing IP disputes (disclose and clean up at formation, not at Series-A).
- Director exculpation, indemnification, and D&O cover *care* mistakes. They do not cover *loyalty* breaches. Founders should understand the asymmetry before relying on the protective architecture.
