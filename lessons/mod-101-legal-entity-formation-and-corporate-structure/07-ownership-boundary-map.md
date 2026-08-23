# 7. Ownership boundary map

> What this module owns, and where each adjacent question is handed off.

## Motivation

Curriculum modules routinely collide at their edges. A founder's restricted stock is both an *entity* question (was it issued under a valid stock plan by a duly-authorised board?) and a *founder-team* question (what is the vesting schedule and the co-founder equity split rationale?). A priced-round preferred financing is both an *entity* question (does the charter authorise the new series?) and a *fundraising* question (how does dilution work, what is a 1x non-participating preference?). This chapter draws the line. It is short because clarity is the goal.

## What this module owns

**mod-101 owns the entity layer.** Concretely:

- **Entity choice** — Delaware C-Corp vs. LLC vs. S-Corp vs. PBC vs. non-Delaware corp, with the decision framework and the exception cases (see [chapter 01](./01-choose-the-us-legal-entity.md)).
- **Formation package** — Certificate of Incorporation, Bylaws, Initial Board Consent, adoption of the equity incentive plan (as an act of the corporation), Founders' Stock Purchase Agreements *from the corporation's perspective* (that they were validly authorised and issued), Initial Stockholder Consent (see [chapter 02](./02-stand-up-the-entity.md)).
- **Corporate record** — minute book structure, share ledger discipline, board and stockholder consents, indemnification agreements, D&O policy scope, registered agent, EIN, state tax registrations (see [chapter 03](./03-corporate-record-and-compliance-calendar.md)).
- **Foreign qualification** — when required, where, how, and the penalty exposure for skipping (see [chapter 04](./04-foreign-qualification-across-states.md)).
- **Compliance calendar** — Delaware franchise tax, Delaware annual report, foreign-state annual reports, federal Form 3921 / 3922, and the discipline of maintaining the calendar (see [chapters 03](./03-corporate-record-and-compliance-calendar.md) and [06](./06-series-a-corporate-record-cleanup.md)).
- **Subsidiary structure decisions** — when to add a Delaware subsidiary and why; when *not* to (see [chapter 05](./05-subsidiary-structure-design.md)).
- **Series-A "corporate-record-in-shambles" diagnostic and cleanup** — the diagnostic pattern and the retroactive-cleanup playbook (see [chapter 06](./06-series-a-corporate-record-cleanup.md)).

## What this module hands off

### To [mod-102 — Founding-Team Legal Architecture](../mod-102-founding-team-legal-architecture/)

- **The founder-side substance of stock issuance** — the co-founder equity-split conversation, the vesting-and-cliff design choice, the "dead-equity" problem, the double-trigger acceleration debate, the departed-founder repurchase mechanics.
- **The IP-assignment substance** — the Proprietary Information and Inventions Assignment (PIIA), the pre-employment invention carveouts (Cal. Lab. Code § 2870 and equivalents), the DTSA whistleblower-immunity notice (18 U.S.C. § 1833(b)(3)), the copyright work-for-hire language.
- **Founder-side conflict-of-interest analysis** — DGCL § 144 interested-director transactions from the founder's seat, the *Caremark* oversight duty on a founder-director, the anti-founder-loyalty-conflict baseline.
- **The founder-employment relationship** — employee vs. contractor for founders, the defer-salary-for-equity trade, founder severance / departure playbook.
- **The founder-diligence failure teardown** — un-signed founder IP assignments, un-filed 83(b)s on the founder side, un-mutual equity splits.

mod-101 confirms that the *entity* validly authorised the founder issuances. mod-102 owns everything about the *founders themselves* — how they contracted with the corporation and each other.

### To `startup-finance-fundraising-curriculum`

- **`mod-104` (or its numbered equivalent)** owns the **priced-round preferred-stock and cap-table mechanics** — the Series Seed / Series A / Series B document set (Certificate of Designations, Investors' Rights Agreement, Voting Agreement, Right of First Refusal & Co-Sale, Stock Purchase Agreement), the option-pool math and its shuffle, 1x non-participating preference and its variants, liquidation-waterfall analysis, anti-dilution mechanics, protective provisions.
- **`mod-108` (or its numbered equivalent)** owns the **cap-table modelling** — dilution modelling, 409A valuation methodology, Rule 701 aggregate-value caps, tax-preference mechanics, downround waterfall analysis.

mod-101 owns *whether the charter authorises the corporation to issue preferred stock and whether the board and stockholder consents authorising a series are validly executed*. The **economics** of the preferred (how much money for what fraction, at what preference stack) belong to the finance-and-fundraising curriculum.

### To [mod-113 — International Expansion & Global Workforce](../mod-113-international-expansion-and-global-workforce/)

- **International subsidiary formation depth** — per-country statutory-form choice, local director / statutory-agent requirements, local tax and social-insurance registrations, transfer-pricing documentation, permanent-establishment analysis, VAT / GST registrations, parent's disclosure and withholding obligations.
- **International workforce mechanics** — Employer of Record vs. direct hire, work-authorisation and immigration, cross-border payroll, benefits harmonisation.

mod-101 owns the *decision* to add an international subsidiary and the general consequence stack. mod-113 owns the country-specific execution.

### Other adjacent handoffs

- **[mod-103 — Employment Law, Worker Classification & Contract Design](../mod-103-employment-law-and-contract-design/)** owns the employee-facing legal architecture — W-2 vs. 1099 classification, FLSA exempt / non-exempt, offer letters, employee PIIAs, NDAs, non-compete landscape, EEOC framework.
- **[mod-105 — Equity-Compensation Policy & the Compensation Committee](../mod-105-equity-compensation-policy-and-comp-committee/)** owns equity-comp *policy* on top of the plan mod-101 stands up — grant guidelines, refresh cadence, exec-comp packages, comp-committee charter and independence progression.
- **[mod-109 — Commercial Contracts & IP & Legal Ops](../mod-109-commercial-contracts-ip-and-legal-ops/)** owns commercial-contract architecture — MSAs, SOWs, customer contracts, vendor contracts, and IP-licensing outside of the JV / holdco / opco context covered here.
- **[mod-111 — Corporate Governance, Board Operations & Officer Duties](../mod-111-corporate-governance-board-operations-and-officer-duties/)** owns board-operations depth — quarterly board packs, board committees, board evaluations, officer fiduciary-duty depth, *Caremark* oversight, D&O program architecture beyond the formation-day baseline.
- **[mod-112 — Enterprise Risk, Insurance & Compliance](../mod-112-enterprise-risk-insurance-and-compliance/)** owns the enterprise-risk and insurance program in depth (D&O tower structure, EPLI, Cyber, E&O), on top of the formation-day D&O placement covered here.

## The rule the module enforces

A question in the diligence room typically belongs to exactly one module. When a diligence request lands, ask:

- Is it about the *entity* — its choice, its formation documents, its corporate record, its qualification footprint, its compliance calendar? → **mod-101.**
- Is it about the *founders' contracts with the corporation and with each other* — their SPAs, their IP assignments, their departure mechanics? → **mod-102.**
- Is it about the *economics of a priced round or a cap-table model*? → **startup-finance-fundraising-curriculum.**
- Is it about *another country*? → **mod-113.**
- Is it about *employees other than founders*? → **mod-103 / mod-104 / mod-105 / mod-106 / mod-107 / mod-108** depending on the specific question.
- Is it about *board operating machinery or director fiduciary duty depth*? → **mod-111.**

## Summary

- This module owns the *entity* layer. Its handoffs are precise: founder-substance to mod-102, priced-round economics to the finance-and-fundraising track, international execution to mod-113.
- Boundaries in a curriculum are a service to the learner and to the operating COO / GC. When a question shows up, the boundary map tells you where the answer lives.
- The rest of the Startup Operations & Governance track builds on top of a validly-formed, properly-maintained entity. Get this module right, and every downstream module has firmer ground to stand on.
