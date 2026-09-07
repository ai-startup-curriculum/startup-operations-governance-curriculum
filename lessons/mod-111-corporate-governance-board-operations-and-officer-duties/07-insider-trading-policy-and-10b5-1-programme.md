# 7. Insider trading policy and the 10b5-1 programme

> An insider-trading policy is the corporation's first-line control against a strict-liability federal-securities regime — and after the December 2022 SEC amendments, the 10b5-1 programme is a disclosed, auditable governance system, not a private arrangement between an insider and a broker.

## Motivation

Insider-trading enforcement is asymmetric. A single trade by a director in the days before an earnings surprise can produce an SEC investigation, a shareholder derivative demand, a Section 16(b) disgorgement suit, a press cycle, and — under the misappropriation theory — personal criminal exposure. None of those outcomes requires the corporation itself to have done anything wrong; the corporation nonetheless bears the reputational cost and the D&O tower absorbs the defense (see [chapter 06](./06-directors-and-officers-insurance.md)).

The controls a private company builds now — a written insider-trading policy, a blackout calendar, a pre-clearance workflow, a 10b5-1 template, and Section 16 filing infrastructure — become mandatory disclosures under Item 408 of Reg S-K the moment the corporation goes public. Adopting them pre-IPO (see [chapter 09](./09-ipo-readiness-and-transition-to-public-governance.md)) both reduces enforcement risk and prevents the awkward "we do not currently have such a policy" disclosure in the first 10-K.

This chapter walks the statutory baseline, the corporate policy, the blackout and pre-clearance workflow, the redesigned 10b5-1 rule, and the Section 16 and Section 13 filing regimes that surround it.

## Statutory baseline

### Rule 10b-5 and the three theories

Section 10(b) of the Securities Exchange Act of 1934 (15 U.S.C. § 78j(b)) makes it unlawful to use "any manipulative or deceptive device or contrivance" in connection with the purchase or sale of any security. Rule 10b-5 (17 C.F.R. § 240.10b-5), promulgated by the SEC in 1942, is the operative anti-fraud rule. Insider trading is a judicial gloss on Rule 10b-5 — Congress has never enacted a stand-alone insider-trading statute — and the law rests on three theories:

- **Classical theory.** A corporate insider (director, officer, employee) who trades in the corporation's securities on the basis of material non-public information ("MNPI") breaches a fiduciary duty owed to the corporation's stockholders. This is the *Chiarella v. United States*, 445 U.S. 222 (1980), and *Dirks v. SEC*, 463 U.S. 646 (1983), line.
- **Misappropriation theory.** A person who owes a duty of trust or confidence to the *source* of MNPI (not to the issuer's stockholders) and trades on that information breaches a duty to the source. *United States v. O'Hagan*, 521 U.S. 642 (1997), upheld this theory and extended Rule 10b-5 to outsiders (an M&A lawyer trading on a client's takeover bid, a spouse trading on pillow-talk information, a printer trading on a proxy statement in production).
- **Tipper-tippee liability.** A tipper who discloses MNPI in breach of a duty is liable if the disclosure produces a "personal benefit" to the tipper (*Dirks*), which can be pecuniary, reputational, or the gift of a trading opportunity to a trading relative or friend. A tippee is liable if the tippee knew or had reason to know of the tipper's breach.

Rule 10b5-2 (17 C.F.R. § 240.10b5-2) identifies specific relationships that create a "duty of trust or confidence" for misappropriation purposes: an express agreement of confidentiality; a history, pattern, or practice of sharing confidences such that the recipient knew or should have known the source expected confidentiality; and receipt from a spouse, parent, child, or sibling (subject to a rebuttal for arm's-length family relationships).

### Rule 10b5-1(b) — "on the basis of"

Rule 10b5-1(b) defines when a trade is made "on the basis of" MNPI: the trader was aware of the MNPI at the time of the trade. "Aware" is broader than "used" and closes the "I had the information in my head but did not think about it when I traded" defense. The affirmative defenses in Rule 10b5-1(c) — including the 10b5-1 plan defense discussed below — exist precisely because the "aware" standard is otherwise unforgiving.

## The corporate insider-trading policy

### Coverage

A well-drafted policy covers:

- All directors, officers, employees, and contractors of the corporation and its subsidiaries.
- Family members sharing a household with a covered person, and any other family member whose transactions are directed by or subject to the influence of a covered person.
- Entities (trusts, family LLCs, foundations) controlled by a covered person or in which a covered person has a pecuniary interest.
- Former employees and directors for a defined tail period (commonly through the end of the first open window after departure, or until any MNPI known at departure becomes public).

Coverage attaches on hire and is reinforced by an initial attestation. Re-attestation runs annually with the code-of-ethics attestation (see [chapter 05](./05-fiduciary-duties-and-the-business-judgment-rule.md) on the compliance-oversight component of the duty of loyalty).

### MNPI definition and examples

Information is **material** if a reasonable investor would consider it important in deciding whether to buy, hold, or sell the security, or if it would significantly alter the total mix of information available. It is **non-public** until it has been broadly disseminated (typically by press release, Form 8-K, or a Reg FD-compliant call) and the market has had time to absorb it (customarily one full trading day after dissemination, though the policy should specify).

Illustrative categories of information that are presumptively material:

| Category | Examples |
| --- | --- |
| Financial results | Unannounced quarterly / annual earnings, revenue misses or beats, guidance changes, restatements |
| Corporate transactions | M&A negotiations, joint ventures, spin-offs, divestitures, significant asset sales |
| Capital markets | Debt or equity financings, share repurchase programs, dividend changes, credit-rating actions |
| Customers and pipeline | Major customer wins or losses, large-contract awards or terminations, significant supplier disruptions |
| People | CEO / CFO transitions, board departures, senior-executive misconduct investigations |
| Legal / regulatory | Government investigations, material litigation developments, regulatory approvals or denials |
| Cyber and operations | Material cybersecurity incidents (also Item 1.05 Form 8-K), major operational outages, data breaches |
| Products | Product launches, regulatory clearances (FDA approvals, export licenses), safety recalls |

The policy should say plainly that the list is illustrative and that any doubt resolves in favor of not trading and consulting the general counsel.

### Prohibited transactions

Even outside blackout windows and even without MNPI, the policy should prohibit:

- **Short sales.** Section 16(c) of the Exchange Act already prohibits Section 16 insiders from short-selling the issuer's equity securities; the policy extends this to all covered persons.
- **Hedging.** Collars, prepaid variable forwards, equity swaps, zero-cost collars, and any derivative that offsets a decrease in the value of the issuer's securities. Item 407(i) of Reg S-K requires public companies to disclose in the proxy whether they permit hedging by directors, officers, and employees; the market-standard answer is "no."
- **Pledging.** Pledging company shares as collateral for a loan or holding company shares in a margin account, both because forced sales can occur during blackouts and because significant pledges attract negative proxy-advisor scrutiny (ISS, Glass Lewis).
- **Standing and limit orders.** Standing and stop-loss orders that can execute at any time inside a blackout. The exception is orders placed inside a validly adopted 10b5-1 plan.
- **Derivatives.** Trading in puts, calls, or other derivative securities on the corporation's stock outside of employer-granted equity awards.
- **Front-running family and friends.** Directing or tipping trades by family, friends, or professional associates in advance of the covered person's own trades.

### Attestation cadence

At hire (as part of onboarding paperwork), annually (bundled with the code-of-ethics and conflicts-of-interest attestation coordinated by the corporate secretary — see [chapter 03](./03-corporate-secretary-function.md)), and on promotion into a role that triggers pre-clearance or Section 16 status.

## Blackout / open-window calendar

### Regular quarterly blackout

The regular blackout closes the trading window from a defined number of days before the end of each fiscal quarter through the second full trading day after the earnings release. A 2-week (14-calendar-day) pre-quarter-end close is common; some companies use a 3-week or month-end close, and Q4 is often longer because of the audit cycle. The open window between blackouts is typically 3-6 weeks per quarter.

### Special (event-driven) blackouts

The general counsel imposes a special blackout when a discrete pool of covered persons is likely to be aware of MNPI: an active M&A negotiation, a restatement investigation, a material litigation development, a major financing, or a materiality determination on a cybersecurity incident. Special blackouts are typically not announced with their subject-matter reason — the notice itself would leak the MNPI — but instead sent to the affected group with instruction not to trade until further notice.

### Illustrative annual calendar

For a calendar-fiscal-year company that releases earnings mid-way through the second month after quarter-end:

| Quarter | Blackout opens | Earnings release (illustrative) | Window opens | Window closes (next blackout) |
| --- | --- | --- | --- | --- |
| Q1 | March 17 | May 8 | May 11 (2nd trading day after release) | June 16 |
| Q2 | June 17 | August 6 | August 10 | September 16 |
| Q3 | September 17 | November 5 | November 9 | December 17 |
| Q4 | December 18 | February 12 (following year) | February 16 | March 16 |

Actual dates are set each year by the general counsel and communicated by a window-opening email and a window-closing email to all covered persons.

## Pre-clearance workflow

### Scope

Pre-clearance is mandatory for:

- All Section 16 insiders (directors and Section 16 officers designated by the board — typically the CEO, CFO, principal accounting officer, general counsel, and any other officers performing a policy-making function).
- Beneficial owners of more than 10% of any class of registered equity.
- Any covered person in a functional group with routine MNPI access — finance and accounting, legal, investor relations, corporate development, executive administrative staff, and often VP-level and above across all functions.

### Process

A written pre-clearance request (form or ticketing-system entry) submitted to the general counsel or a designated compliance officer, at least 24-48 hours before the intended trade. The reviewer confirms:

1. The window is open and no special blackout applies to the requester.
2. The requester represents no awareness of MNPI.
3. For Section 16 insiders, Rule 144 volume and manner-of-sale limits are not exceeded (relevant for affiliates selling restricted or control securities), and the trade will not create a Section 16(b) short-swing exposure.
4. Any 10b5-1 plan in effect covers or does not conflict with the trade.
5. Sarbanes-Oxley § 306(a) pension-blackout rules do not apply (rare, but relevant during 401(k) plan blackouts).

Written approval is issued and is typically valid for a short window (3-5 business days). If the trade is not executed within the approval window, a fresh pre-clearance is required. Approvals do not immunize the trade — the insider remains responsible for confirming they lack MNPI at the moment of trading.

### Tracking

Log the request, approval or denial, and executed trade in a tracker. Options range from a spreadsheet maintained by the paralegal to a Notion / SharePoint workflow to purpose-built modules inside Diligent Boards, Workiva, or the executive-brokerage pre-clearance system (Shareworks / Morgan Stanley at Work, Fidelity Stock Plan Services, E*TRADE Corporate Services). Integration with the brokerage prevents an approved trade from being executed after MNPI arrives, and prevents a non-approved trade from being executed at all.

## Rule 10b5-1 trading plans

### The affirmative defense

Rule 10b5-1(c)(1) provides an affirmative defense to Rule 10b-5 liability where the person can demonstrate that, before becoming aware of MNPI, they had:

1. Entered into a binding contract to purchase or sell the security, instructed another person to purchase or sell the security for the instructing person's account, or adopted a written plan for trading securities; **and**
2. The contract, instruction, or plan either (i) specified the amount, price, and date of the transactions, (ii) included a written formula or algorithm for determining amount, price, and date, or (iii) did not permit the person to exercise any subsequent influence over how, when, or whether to effect purchases or sales (and any person exercising such influence was not aware of MNPI); **and**
3. The transaction was pursuant to the contract, instruction, or plan.

Additionally, the plan must be entered into in good faith and not as part of a plan or scheme to evade Rule 10b-5.

### December 2022 amendments

The SEC adopted substantial amendments to Rule 10b5-1 in Release Nos. 33-11138 and 34-96492 (December 14, 2022) <!-- needs-research: verify exact release numbers and adopting-release citation format -->. Substantive rule amendments were effective February 27, 2023; the corresponding disclosure amendments applied to filings that cover the first full fiscal period beginning on or after April 1, 2023 (with a limited deferral for smaller reporting companies) <!-- needs-research: verify exact effective / compliance dates for disclosure amendments and any smaller-reporting-company deferrals -->.

Substantive changes:

- **Cooling-off period.** For directors and Section 16 officers, the later of (i) 90 days after adoption or modification and (ii) two business days after the disclosure in the Form 10-Q or 10-K covering the fiscal quarter of adoption, capped at 120 days. For non-issuer persons other than directors and officers, 30 days. Issuer repurchase plans under 10b5-1 do not have a cooling-off period under the final rule <!-- needs-research: verify final rule position on issuer-plan cooling-off — the proposal included a 30-day period but the adopting release position should be confirmed -->.
- **Good-faith certification.** Directors and Section 16 officers must include a written representation in the plan certifying that at the time of adoption they are not aware of MNPI about the issuer or its securities and are adopting the plan in good faith and not as part of a plan or scheme to evade Rule 10b-5.
- **Ongoing good-faith requirement.** The insider must have acted in good faith with respect to the plan — post-adoption acts, including cancellations, modifications, or attempts to influence execution, may cause loss of the affirmative defense.
- **Single-plan limitation.** No more than one 10b5-1 plan may be in effect at any one time, subject to narrow exceptions: (i) sell-to-cover plans that authorize only sales necessary to satisfy tax-withholding obligations on the vesting of equity awards (other than options), where the insider has no control over the timing of the sales; and (ii) later-adopted plans whose trades cannot begin before all trades under the earlier plan are completed or the earlier plan is terminated (though the cooling-off period is measured from the later plan's own adoption date if the earlier plan is terminated early).
- **Single-trade-plan limitation.** No more than one plan designed to effect a single transaction (a "single-trade plan") in any 12-month period, subject to the same sell-to-cover exception.

### Disclosure — Reg S-K Item 408

- **Item 408(a).** Quarterly disclosure in Form 10-Q and Form 10-K of any adoption, modification, or termination during the quarter of a "Rule 10b5-1 trading arrangement" or "non-Rule 10b5-1 trading arrangement" by a director or Section 16 officer, including the material terms (name and title of the person, date of adoption / modification / termination, duration, aggregate number of securities). The plan's pricing terms need not be disclosed.
- **Item 408(b).** Annual 10-K disclosure of whether the issuer has adopted insider-trading policies and procedures reasonably designed to promote compliance, and if not, why not. The policy itself must be filed as Exhibit 19 to the Form 10-K under Item 601(b)(19) of Reg S-K.
- **Form 4 checkbox.** Form 4 was amended to include a checkbox indicating whether the reported transaction was made pursuant to a plan intended to satisfy the affirmative-defense conditions of Rule 10b5-1(c).

### Worked adoption timeline

Assume a Section 16 officer adopts a 10b5-1 plan on August 12 — the first day of the open window following Q2 earnings released on August 6. The corporation's Q3 Form 10-Q will disclose the adoption and is expected to be filed on November 5.

| Event | Date |
| --- | --- |
| Plan adoption (good-faith certification signed) | August 12 |
| Q2 window closes | September 16 (blackout for Q3 begins) |
| 90 days after adoption | November 10 |
| Q3 Form 10-Q disclosing adoption | November 5 |
| Two business days after Q3 10-Q disclosure | November 7 |
| **First permitted trade date** (later of the two, capped at 120 days) | **November 10** |
| Cap (120 days after adoption) | December 10 |

If the Q3 10-Q were delayed to December 5, the two-business-day disclosure gate (December 9) would still fall inside the 120-day cap (December 10), and trading could begin December 9. If the 10-Q were delayed past December 10, the 120-day cap would govern and trading could begin December 10 regardless.

## Section 16 filings

### Filing matrix

Section 16(a) of the Exchange Act requires every director, every officer designated as a Section 16 officer, and every beneficial owner of more than 10% of a registered class of equity to file:

| Form | Trigger | Deadline | Purpose |
| --- | --- | --- | --- |
| Form 3 | Becoming a director, Section 16 officer, or 10% owner | Within 10 days of the triggering event (or, for IPO, on the effective date of the Section 12 registration) | Initial statement of beneficial ownership |
| Form 4 | Any change in beneficial ownership (open-market trade, grant, option exercise, gift, most RSU vestings) | Within 2 business days of the transaction (limited exceptions for certain deferred-reporting transactions) | Transaction report |
| Form 5 | Fiscal year-end, if any transactions were exempt from Form 4 reporting or a Form 4 was missed | Within 45 days of fiscal year-end | Annual catch-up |

All forms are filed on EDGAR by the corporation's filing agent (typically the transfer agent, or a specialist such as DFIN, Workiva, or Business Wire). The insider must have EDGAR filing codes (CIK, CCC, filer ID). Powers of attorney executed at onboarding authorize the corporate secretary and named counsel to sign filings on the insider's behalf.

### Worked example — Form 4

A director sells 5,000 shares in the open market on Tuesday, September 15, through the corporation's designated broker after receiving pre-clearance the prior Friday.

- The broker confirms execution to the corporate secretary Tuesday afternoon.
- The corporate secretary or filing agent drafts Form 4 Wednesday.
- The director's power of attorney authorizes signature.
- The Form 4 is filed on EDGAR **by 10:00 p.m. Eastern on Thursday, September 17** (the second business day after the transaction).
- If the trade was executed under a 10b5-1 plan, the plan checkbox on Form 4 is selected and the plan's adoption date is disclosed in the footnote.

Late Form 4 filings are disclosed in the following year's proxy statement under Item 405 of Reg S-K, and repeated lateness attracts proxy-advisor scrutiny and negative ISS "say-on-pay" recommendations.

### Section 16(b) short-swing profit disgorgement

Section 16(b) requires any Section 16 insider to disgorge to the corporation any profit realized from a matched purchase-and-sale (or sale-and-purchase) of the issuer's equity securities within any 6-month period. The rule is:

- **Strict liability.** No intent, no use of MNPI, and no fiduciary breach is required.
- **Recovery.** The corporation may sue; if it does not, any stockholder may bring a derivative action, with the plaintiff's counsel typically fee-shifted from the recovery.
- **Matching.** Courts apply a "lowest-in / highest-out" matching that maximizes disgorgement, not FIFO.

This is why pre-clearance systematically checks for six-month lookback conflicts. It is also why the December 2022 rule amendments' single-plan limitation matters operationally: a Section 16 insider who runs simultaneous plans risks matching a plan-driven sale against a plan-driven purchase within six months.

### Section 16(c) — short-sale prohibition

Section 16(c) prohibits Section 16 insiders from selling short or selling equity securities they do not own (sale against the box). The corporate policy extends this prohibition to all covered persons.

## Section 13 beneficial-ownership filings

### Schedule 13D and 13G

Any person who directly or indirectly acquires beneficial ownership of more than 5% of a registered class of voting equity securities is required to file:

- **Schedule 13D.** The default "active investor" disclosure. Original filing deadline was 10 calendar days after crossing 5%; the SEC's October 10, 2023 amendments accelerated this to 5 business days <!-- needs-research: verify current 13D initial filing deadline and effective date post-2023 amendments -->. Amendments under Rule 13d-2(a) are required promptly upon a material change (typically construed as within 2 business days).
- **Schedule 13G.** The short-form disclosure available to (i) qualified institutional investors (Rule 13d-1(b)), (ii) passive investors holding less than 20% (Rule 13d-1(c)), and (iii) exempt investors (Rule 13d-1(d)). Deadlines and amendment triggers are shorter under the 2023 amendments than under prior practice.

### Practical relevance to the corporation

The corporation tracks 13D and 13G filings against its stock ledger for cap-table completeness (see [mod-101](../mod-101-entity-formation-and-corporate-governance-foundations/)), for engagement outreach by investor relations, and to identify potential activist accumulations. Filings by directors and officers who cross the 10% threshold overlap with Section 16 filings; filings by external investors are separate.

## Practical operating model

- **Policy adoption pre-IPO.** The insider-trading policy is adopted by board resolution during IPO readiness (see [chapter 09](./09-ipo-readiness-and-transition-to-public-governance.md)) so that Item 408(b) disclosure in the first 10-K attaches to a real policy. Many companies adopt the policy substantially earlier — as a matter of hygiene, as a condition of a large secondary or tender, or because a major investor requires it in a subscription agreement.
- **Annual attestation.** Bundled with the code-of-ethics and conflicts-of-interest attestation coordinated by the corporate secretary.
- **Blackout communications.** Quarterly window-opening and window-closing emails to all covered persons from the general counsel. Special-blackout emails to a smaller list, drafted to avoid signaling the underlying MNPI.
- **10b5-1 template.** Maintained by outside securities counsel with the general counsel; refreshed after every material SEC rule change. Insiders adopt on the broker's plan document but subject to a corporate approval process that (i) confirms the window is open, (ii) collects the good-faith certification, and (iii) queues the plan for Item 408 disclosure.
- **Quarterly disclosure loop.** Legal and investor relations jointly prepare Item 408 disclosure inputs for each 10-Q and 10-K, tied into the disclosure-controls process (see [chapter 04](./04-standing-committees-audit-compensation-nominating.md) on audit committee oversight of disclosure controls).
- **Section 16 filing infrastructure.** Owned by the corporate secretary with a designated filing agent (transfer agent or specialist such as DFIN, Workiva, or NetRoadshow). Powers of attorney and EDGAR filing codes for every Section 16 insider are collected at onboarding.
- **Broker integration.** Section 16 insiders concentrate brokerage at a single broker (E*TRADE Corporate Services, Fidelity SPS, Shareworks / Morgan Stanley at Work) with the pre-clearance and 10b5-1 workflow integrated end-to-end. Concentration is a compliance requirement, not a preference — it enforces the pre-clearance gate and ensures the corporate secretary receives execution confirmations in time for Form 4 filing.

## Coordination boundary

- This chapter owns the insider-trading policy and the 10b5-1 programme end-to-end: policy drafting, blackout calendar, pre-clearance workflow, plan template, Section 16 filings, Section 13 tracking, and Item 408 disclosure.
- Equity-compensation grant mechanics — RSU vesting schedules, ISO / NSO exercise mechanics, sell-to-cover elections, employer-share-withholding elections, and the equity-award ledger that feeds Section 16 transaction reporting — live in [mod-105](../mod-105-equity-compensation-policy-and-comp-committee/). This chapter consumes the ledger and reports the transactions; mod-105 owns the underlying awards.
- IPO adoption sequencing of the policy, including the drafting of the first-year blackout calendar and the S-1 disclosure of governance policies, lives in [chapter 09](./09-ipo-readiness-and-transition-to-public-governance.md).
- CFO-side earnings-release scripts, Reg FD safe-harbor procedures for guidance disclosures, and IR outreach protocols during blackouts sit in the [startup-finance-fundraising curriculum](../../../startup-finance-fundraising-curriculum/), which owns the disclosure-side counterpart to the trading-side policy owned here.
- Enterprise risk mapping — including reputation risk from insider-trading enforcement and coordination with the D&O tower — sits in [mod-112](../mod-112-enterprise-risk-and-insurance-programme/).

## Summary

- Rule 10b-5 covers three theories of insider-trading liability: classical, misappropriation, and tipper-tippee. "Aware" (not "used") is the standard under Rule 10b5-1(b), which is why affirmative defenses matter.
- The corporate insider-trading policy defines coverage (employees, contractors, family, controlled entities), MNPI, prohibited transactions (short sales, hedging, pledging, standing orders), and attestation cadence.
- Regular quarterly blackouts and event-driven special blackouts operate through a window-opening / window-closing communications rhythm run by the general counsel.
- Pre-clearance is mandatory for Section 16 insiders and 10% owners, extended in practice to all functional groups with routine MNPI access, and integrated with the executive brokerage.
- Rule 10b5-1 provides an affirmative defense if the plan is adopted in good faith without MNPI and specifies the trades or delegates to a broker without MNPI. The December 2022 amendments imposed cooling-off periods, good-faith certifications, a single-plan limitation, a single-trade-plan annual limit, Form 4 checkbox reporting, and Item 408 quarterly disclosure.
- Section 16 filings — Form 3 (initial), Form 4 (2 business days), Form 5 (annual catch-up) — are strict-deadline obligations owned by the corporate secretary through a filing agent. Section 16(b) short-swing profits are strict-liability disgorgeable. Section 16(c) prohibits short sales.
- Section 13D / 13G beneficial-ownership filings sit adjacent — the corporation tracks them for cap-table and IR purposes.
- The programme is adopted pre-IPO, disclosed under Item 408 once public, and coordinates with equity comp (mod-105), IPO readiness (chapter 09), CFO-side disclosure (startup-finance-fundraising curriculum), and enterprise risk (mod-112).
