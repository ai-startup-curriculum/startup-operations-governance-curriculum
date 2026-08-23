# 5. NDAs and MNDAs

> The PIIA covers the corporation's people. The NDA covers everyone else who sees confidential information — customers, vendors, candidates, recruits, investors. Get the direction (mutual vs. one-way) and the exceptions right, and disputes stay small.

## Motivation

The PIIA ([chapter 04](./04-employee-piia.md)) governs the corporation's relationship with its own people. The NDA and MNDA (mutual NDA) govern every *other* confidential-information exchange the corporation has — with prospects and customers during sales conversations, with vendors during evaluations, with candidates during interviews that go into product-and-strategy detail, with recruits before an offer is signed, with investors before a term sheet, with acquisition targets and acquirers during exploratory conversations, with commercial partners during integration scoping.

An NDA is a low-drama document that trades a small amount of drafting discipline up front for a large amount of clarity when a dispute arises. It is often the first substantive contract two counterparties sign; the tone of the NDA negotiation tends to set the tone of the commercial negotiation that follows.

This chapter is short by design. The NDA is not conceptually complex. The failure modes are (i) using the wrong direction (one-way when it should be mutual, or vice versa), (ii) omitting the standard exceptions, (iii) drafting a broken injunctive-relief or attorneys'-fees clause, (iv) using an off-the-internet template that has never been reviewed, or (v) not signing one at all when the corporation clearly should have.

## One-way NDA vs. mutual NDA (MNDA): who is disclosing to whom

The direction of the NDA determines who bears the confidentiality obligation:

- **One-way NDA (unilateral NDA).** One party (the Discloser) is disclosing Confidential Information to the other party (the Recipient); the Recipient owes the confidentiality obligation; the Discloser does not. Use when the information flow is genuinely one-directional.
- **Mutual NDA (MNDA).** Both parties may exchange Confidential Information; both owe the confidentiality obligation, each with respect to the other's information. Use when the information flow is (or may become) two-directional.

The choice is not political — it reflects the actual expected information flow. The failure mode is defaulting to the wrong direction because of laziness or template mismatch.

**When one-way is right.**

- Candidate NDA at the interview stage before an offer is signed. The corporation shares its confidential product-and-strategy details; the candidate shares their résumé and general professional background (typically not "confidential information" in the trade-secret sense). One-way from the corporation to the candidate.
- Customer / prospect NDA during a sales conversation about a novel product feature. The corporation shares roadmap and technical detail; the customer shares little of confidential value beyond what is publicly known about their business. One-way from the corporation to the customer, in principle — but see below on why this often becomes mutual.
- Vendor NDA when the corporation is evaluating a vendor's proprietary product. The vendor shares product details; the corporation shares nothing beyond a general description of its use case. One-way from the vendor to the corporation.

**When mutual is right.**

- Customer / prospect conversations that touch the customer's confidential business data (their revenue, their internal metrics, their customer list, their compliance posture, their competitive position). Both sides share confidential information; the NDA should be mutual.
- Partnership / integration / co-marketing evaluations. Both sides share business plans and technical detail. Mutual.
- Acquisition or investment conversations. Both sides share sensitive information. Mutual.
- Recruit conversations with senior executives who share information about their current or former employer's strategy in the course of the interview. Mutual.
- Enterprise-vendor evaluations where the corporation is sharing usage details, integration data, and internal processes. Mutual.

**Why one-way often becomes mutual anyway.** In many practical situations that look one-way, the receiving side will insist on mutuality because (i) they cannot cleanly compartmentalise conversations that touch their own confidential business, (ii) their legal team's default template is mutual, or (iii) they want protection against inadvertent disclosure of their own information during the conversation. Enterprise customers will almost always insist on mutual NDAs for sales conversations of any depth. The corporation should be willing to sign a mutual NDA in most sales and partner contexts; the practical downside of mutuality (the corporation now owes confidentiality on the counterparty's information) is small, because a well-drafted MNDA has the same exceptions on both sides.

The negotiation cost of arguing for one-way when mutual is what the counterparty expects is usually higher than the incremental risk of signing mutual.

## The standard exceptions: already-known, publicly-available, independently-developed, compelled disclosure

Every NDA (one-way or mutual) has a standard exception clause that carves out information that would otherwise fall inside the "Confidential Information" definition but that should not be treated as confidential because the receiving party's obligation would be unfair or impractical.

The four canonical exceptions:

1. **Already known.** Information that the receiving party already possessed, free of any obligation of confidentiality, before receiving it from the disclosing party.
2. **Publicly available.** Information that is or becomes generally known to the public through no fault of the receiving party.
3. **Independently developed.** Information that the receiving party independently develops without use of or reference to the disclosing party's Confidential Information.
4. **Received from a third party.** Information that the receiving party rightfully receives from a third party who is not itself under an obligation of confidentiality to the disclosing party.

A fifth exception, distinct from the "carve-outs" above because it is *not* about categories of information but about *permitted disclosures*, is:

5. **Compelled disclosure.** Disclosure required by court order, subpoena, or legal or regulatory process — with a requirement (where legally permissible) that the receiving party give the disclosing party prompt written notice so the disclosing party can seek a protective order.

And, as with the PIIA, the DTSA whistleblower-immunity carveout under 18 U.S.C. § 1833(b) should be added or acknowledged so that the receiving party's ability to report suspected illegal conduct to a government agency is not impaired.

Omitting any of the four category exceptions creates an unenforceable or unfair obligation and invites the receiving party to push back or refuse to sign. Include all four in every NDA.

## Definition of "Confidential Information"

The definition should be:

- **Broad enough** to cover the categories of information the parties actually exchange — technical, business, financial, personnel, product, roadmap, customer / supplier, strategy — plus a catch-all for information a reasonable person would understand to be confidential.
- **Narrow enough** to not swallow the obvious (e.g., a general description of the disclosing party's business, publicly-available information about the disclosing party's products).
- **Optionally, requires a marking** — "written information marked as confidential" or "orally disclosed information identified as confidential at disclosure and confirmed in writing within thirty days." The marking requirement is common in vendor / enterprise NDAs and adds a mild operational discipline. Startup-to-customer NDAs often omit the marking requirement because it slows down real conversations.

**Term of the confidentiality obligation.** Common structures:

- **Fixed period.** 2, 3, or 5 years from the effective date. Standard for commercial-conversation NDAs.
- **Indefinite for trade secrets, fixed for other confidential information.** More protective of the disclosing party. Common in NDAs with high-technical-value information.
- **Term tied to the underlying relationship.** "For the term of the parties' engagement plus X years." Common in NDAs that attach to an underlying agreement.

Enterprise counterparties often push for shorter terms. The negotiation typically settles at 3–5 years for general confidential information.

## Purpose and permitted use

An NDA should specify the **purpose** for which the receiving party may use the Confidential Information — evaluating a potential business relationship, evaluating a specific transaction, performing services under an underlying agreement, evaluating employment. Use for any purpose beyond the specified purpose is a breach.

A well-drafted purpose clause is narrow enough to be meaningful (not "any legitimate business purpose") but broad enough to allow the actual conversation the parties want to have.

## Ownership: information stays with the discloser

Standard clause: nothing in the NDA transfers ownership of, license to, or other right in the Confidential Information from the disclosing party to the receiving party. The receiving party has permission to *use* the information for the specified purpose; the receiving party does not *own* it. On termination or on request, the receiving party returns or destroys the Confidential Information (with a carve-out for backups made in the ordinary course of IT operations and for retention required by law, subject to continuing confidentiality on retained copies).

## Dispute-resolution clauses

The four practical clauses that matter when a dispute arises:

- **Governing law.** Which state's law governs interpretation. Common choices: the corporation's home state (Delaware or California for many startups), the counterparty's home state, or a neutral state. Delaware is a common compromise for commercial contracts because Delaware's courts are experienced in commercial disputes. California is common when a California-based corporation contracts with California-based counterparties.
- **Venue and jurisdiction.** Which court has jurisdiction to hear disputes. Common choices: the state or federal courts of the corporation's home state, with an exclusive-forum-selection clause. Or arbitration under AAA or JAMS rules ([chapter 09](./09-arbitration-and-class-action-waivers.md) treats arbitration separately for employment; commercial NDA arbitration is a different animal governed by the Federal Arbitration Act as commercial contracts).
- **Injunctive relief and specific performance.** A statement that money damages are inadequate for breach of confidentiality and that the disclosing party is entitled to seek injunctive relief in addition to any other remedies at law or in equity, without the need to post a bond. This clause matters because a trade-secret disclosure that has occurred cannot be undone with damages; the disclosing party needs an injunction to stop further disclosure. Courts generally recognise this, but the express clause removes any argument.
- **Attorneys' fees.** A prevailing-party or one-way (in favour of the disclosing party) attorneys'-fees provision. This shifts the economics of enforcement and is often included in favour of both parties in a mutual NDA (the prevailing party recovers fees) or in favour of the disclosing party in a one-way NDA. California has restrictions on one-way attorneys'-fees provisions (Cal. Civ. Code § 1717 converts a one-way provision to a mutual one in contract-based fee awards); the practical effect in California is a mutual prevailing-party clause.

**The clauses to avoid overreaching on.** A "liquidated damages" clause specifying a fixed dollar amount for breach is fragile — courts often treat liquidated-damages clauses as unenforceable penalties if the fixed amount is not a reasonable estimate of actual damages. A clause purporting to waive the receiving party's constitutional right to a jury trial or to file a whistleblower complaint is unenforceable in many jurisdictions and creates enforceability risk for the rest of the agreement. A clause purporting to bind the receiving party's affiliates or successors without their signed acknowledgement is fragile.

## Ancillary standard clauses

The other clauses that appear in a well-formed NDA:

- **No obligation to enter a further transaction.** Neither party is obligated by the NDA to enter any business relationship or transaction; the NDA solely governs confidentiality.
- **No warranty on the Confidential Information.** The disclosing party makes no representation or warranty about the accuracy or completeness of the Confidential Information.
- **Independent contractors / no partnership.** The NDA does not create a partnership, joint venture, agency, or employment relationship between the parties.
- **Notices.** Where notices are sent (physical or electronic address for each party).
- **Assignment.** The NDA is not assignable by either party without the other's consent, except (typically) to an affiliate or successor by merger.
- **Amendment and waiver.** Any amendment must be in writing signed by both parties; no waiver unless written.
- **Severability.** If any provision is unenforceable, the remainder of the NDA continues.
- **Counterparts.** May be executed in counterparts and by electronic signature.
- **Effective date and signatures.** Effective date; corporation's signature block (by an authorised officer per DGCL § 142); counterparty signature block.

## When the NDA is (and isn't) really necessary

The NDA is not automatically the right first step. Categories:

- **Genuinely confidential exchanges.** Sales conversations that get into unreleased product detail, integration scoping that touches architecture, acquisition or investment discussions, senior-executive recruit conversations. NDA is warranted; execute one before the substantive conversation.
- **Publicly-discussable material.** Pitch conversations with investors at the very early stage; general product demos; press or analyst briefings; general recruiting conversations. NDA is often *not* warranted; asking an investor or a journalist to sign an NDA is often received as unprofessional and can chill the conversation. The corporation is generally better off keeping the demo or the pitch to publicly-discussable material and reserving the NDA for the next-stage conversation.
- **Investor conversations.** Traditional VC investors have a strongly-held norm of *not signing NDAs at first pitch* because they see many similar businesses and cannot practically track NDA obligations across every meeting. Asking a top-tier VC to sign an NDA at first pitch is often a signal that the founder does not understand how investor conversations work. Once the conversation moves to substantive diligence (post-term-sheet or in the run-up to a term sheet), an NDA is standard and expected.
- **Recruit conversations at the top of the funnel.** No NDA. The corporation should describe the role, the team, the product, and the general business publicly. Save the NDA for the offer stage.
- **Recruit conversations at the offer stage.** NDA is warranted, one-way or mutual depending on how deeply the recruit is being brought into strategy and product detail. This is the "candidate NDA" referenced above.

Signing NDAs indiscriminately creates a portfolio of confidentiality obligations the corporation has to manage. Signing NDAs never is imprudent for genuinely confidential exchanges. The judgment is contextual.

## Common failure modes

- **Using the wrong direction.** Signing a one-way NDA (corporation as Recipient) when the corporation is actually the primary Discloser, or vice versa, imposes obligations that don't match the information flow and can be an enforcement obstacle.
- **Omitting the standard exceptions.** A counterparty that reads the draft will insist. Include them proactively.
- **Overbroad "Confidential Information" definition.** A definition that includes "any information provided by the disclosing party" without exception language is unenforceable in many jurisdictions.
- **Indefinite duration for non-trade-secret information.** Fragile. Prefer a defined period for non-trade-secret Confidential Information with indefinite treatment for trade secrets, or a defined period across the board.
- **Missing injunctive-relief clause.** The disclosing party may still be able to seek an injunction, but the express clause removes the ambiguity.
- **Missing DTSA whistleblower carveout.** For NDAs that reach individuals (candidates, contractors), include the 18 U.S.C. § 1833(b) notice — same reasoning as the PIIA.
- **NDA that swallows the underlying deal.** When the parties sign a subsequent master services agreement or business contract that includes its own confidentiality provisions, the two documents' provisions can conflict. The subsequent agreement should either supersede the NDA on that subject or explicitly incorporate it.
- **Signature by an unauthorised individual.** The NDA is only binding on parties whose authorised signer executes it. A random employee signing an NDA on behalf of the corporation without actual or apparent authority may not bind the corporation, and vice versa.
- **Not executing at all.** The corporation has a substantive conversation with a customer or vendor about confidential information without first getting an NDA signed. If a dispute later arises, the corporation is arguing common-law trade-secret protection without a contractual overlay — a materially weaker position.

## The template library

An operating corporation should maintain a small NDA template library:

- **Standard MNDA (mutual NDA)** — the default for most commercial conversations.
- **Standard one-way NDA (corporation as discloser)** — for candidate conversations, some vendor evaluations.
- **Standard one-way NDA (corporation as recipient)** — for vendor evaluations where the vendor is genuinely the primary discloser.
- **Enterprise-friendly MNDA variant** — with the specific clauses enterprise customers commonly insist on (mutual, prevailing-party fees, defined-term, Delaware or NY governing law, injunctive relief, dispute-resolution ladder). The corporation can offer this on first ask to reduce negotiation friction.

Each template should be reviewed by outside counsel on adoption and reviewed on a defined cadence (annually or when the corporation enters a new state / country / market segment).

## Concrete example: an MNDA for a customer sales conversation

Acme Robotics (Delaware C-Corp, San Francisco) enters a sales conversation with Global Widgets Corp. (New York corporation, headquartered in NYC) about a potential enterprise deployment of Acme's product. Both sides expect to exchange confidential information — Acme will discuss unreleased features and roadmap; Global Widgets will discuss its manufacturing processes, throughput data, and internal metrics.

An MNDA is executed before the substantive technical conversation. Key terms:

- **Parties.** Acme Robotics, Inc. and Global Widgets Corp.
- **Purpose.** Evaluating a potential business relationship for the deployment of Acme's software in Global Widgets' manufacturing environment.
- **Confidential Information.** Broad definition covering technical, business, financial, product, roadmap, personnel, customer / supplier, and strategy information disclosed by either party; catch-all for information a reasonable person would understand to be confidential; marking requirement omitted (real-time sales conversation).
- **Standard exceptions.** Already-known, publicly-available, independently-developed, rightfully-received-from-third-party.
- **Compelled disclosure.** Notice-and-opportunity-to-seek-protective-order.
- **DTSA whistleblower carveout.** Included.
- **Term.** 3 years from the effective date; indefinite for trade secrets.
- **Purpose limitation.** Use only for the specified purpose; no other use.
- **No ownership transfer.** Recipient gets a permission to use, not ownership.
- **Return / destruction on request.** With IT-backup carveout and continuing confidentiality on retained copies.
- **Governing law.** Delaware.
- **Venue.** State or federal courts in Delaware; mutual consent to jurisdiction.
- **Injunctive relief.** Available; no bond required.
- **Attorneys' fees.** Mutual prevailing-party.
- **No obligation for further transaction.** Standard.
- **No warranty on the information.** Standard.
- **Independent contractors.** Standard.
- **Signatures.** Acme's VP of Sales (authorised per delegation policy from the CEO); Global Widgets' authorised signatory.

The MNDA is short — 3 to 4 pages of substance. It is signed before the sales team's technical demo call. If the sales conversation progresses to a term sheet or contract, the subsequent MSA will typically include its own confidentiality provisions that either supersede or reference the MNDA.

## Summary

- The NDA / MNDA covers everyone the corporation exchanges confidential information with outside its own workforce — customers, vendors, candidates, recruits, investors, partners.
- Choose the direction (one-way vs. mutual) to match the actual information flow. Enterprise counterparties usually insist on mutual; the corporation should be willing to sign mutual in most commercial conversations.
- Include the four standard exceptions (already known, publicly available, independently developed, received from a third party), the compelled-disclosure clause, and — for NDAs reaching individuals — the DTSA whistleblower-immunity carveout.
- The dispute-resolution clauses that matter: governing law, venue and jurisdiction, injunctive relief (with no bond), and prevailing-party attorneys' fees.
- Common failure modes: wrong direction, omitted exceptions, overbroad definition, indefinite duration for non-trade-secret information, missing injunctive-relief language, unauthorised signature, or no NDA when one was needed.
- Maintain a small template library (standard MNDA, one-way variants, enterprise-friendly MNDA) and offer the enterprise-friendly variant on first ask to reduce negotiation friction.
- Do not sign NDAs indiscriminately (top-of-funnel investor pitches and general recruiting conversations typically do not need them) and do not skip NDAs where they belong (any substantive exchange of confidential information — sales, integration, partnership, recruit-at-offer, acquisition, investment).
