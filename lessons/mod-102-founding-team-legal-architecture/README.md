# mod-102 — Founding-Team Legal Architecture

> Founder agreements, restricted stock + 83(b), mutual IP assignment (PIIA), DTSA-compliant whistleblower notice, anti-conflict baseline.

**Track:** Startup Operations & Governance (level 50) · **Stage:** PRE-SEED / SEED · **Pillar:** legal · **Hours:** 24

## Why this module exists

[mod-101](../mod-101-legal-entity-formation-and-corporate-structure/) stood up the entity — the Delaware C-corporation with its filed charter, adopted bylaws, appointed board, and formation-day board consent that authorised the founders' issuances. This module authors everything on the *founder* side of that same formation event: the founder agreement (equity split with rationale, roles, decision authority, dispute resolution, walk-away and re-vesting), the Stock Purchase Agreement (vesting, cliff, repurchase-at-cost), the § 83(b) election that starts the capital-gains clock, the mutual IP assignment (PIIA) with the DTSA whistleblower-immunity notice and state-law invention-assignment carveouts, the founder-side conflict-of-interest architecture (DGCL § 144, *Caremark*, corporate opportunity, anti-loyalty-conflict baseline), and the founder-employment relationship with its severance and departure playbook.

Each of these documents is easy to get wrong. Missing 83(b)s, un-signed PIIAs, missing SPAs, undocumented equity splits, un-cleansed § 144 transactions, dead-equity departed founders — every incoming COO or GC inherits some subset of these defects at Series-A, and the retroactive-cleanup work is far more expensive than the formation-day discipline that would have prevented them. This module is the discipline.

## Chapters

1. [Co-founder equity split and the founder agreement](./01-co-founder-equity-split-and-founder-agreement.md) — the equity-split conversation, the seven variables to price on the record, roles and decision authority, dispute resolution, walk-away and re-vesting mechanics, the dead-equity trap.
2. [Founders' restricted stock, vesting, and the repurchase right](./02-founders-restricted-stock-and-repurchase.md) — the Stock Purchase Agreement end-to-end; restricted stock vs. options; the 4/1 vesting default; the repurchase right at cost as the mechanic that makes vesting real; double-trigger CoC acceleration; transfer restrictions.
3. [The 83(b) election and the founder tax clock](./03-83b-election-and-founder-tax-clock.md) — § 83(a) vs. § 83(b); the absolute 30-day deadline; how to file; the failure modes and the narrow retroactive-cleanup options; § 1202 QSBS interaction.
4. [The mutual IP assignment (PIIA)](./04-piia-mutual-ip-assignment.md) — present-assignment language (*Stanford v. Roche*); work-made-for-hire + assignment backstop; the Prior Inventions schedule; Cal. Lab. Code § 2870 and multi-state carveouts; confidentiality and disclosure obligations; who signs and when.
5. [The DTSA whistleblower-immunity notice and the trade-secret baseline](./05-dtsa-whistleblower-and-trade-secret-baseline.md) — 18 U.S.C. § 1833(b)(3) mechanics; the enhanced-remedy stack that the notice preserves; the "reasonable measures" program that keeps trade-secret protection viable; retroactive cleanup.
6. [Founder conflict-of-interest baseline](./06-founder-conflict-of-interest.md) — DGCL § 144 interested-director transactions; the *Caremark* oversight duty and its "mission-critical risk" carve-out; corporate-opportunity doctrine and DGCL § 122(17); the anti-loyalty-conflict baseline (moonlighting, competitive activity, pre-existing IP disputes).
7. [The founder-employment relationship and the departure playbook](./07-founder-employment-relationship-and-departure.md) — W-2 employee (not contractor); founder offer letter and employment agreement; defer-salary-for-equity vs. market-clearing salary; the separation matrix; the departure playbook including OWBPA-compliant releases; departed-founder equity treatment on the cap table.
8. [Founder-diligence failure teardown and retroactive cleanup](./08-founder-diligence-failure-teardown.md) — the four recurring defects (un-signed PIIAs, un-filed 83(b)s, missing SPAs, un-mutual equity treatment) diagnosed and cured; the retroactive-cleanup playbook.
9. [Ownership boundary map](./09-ownership-boundary-map.md) — what this module owns vs. what it hands off to mod-101, mod-103, mod-105, mod-111, `startup-finance-fundraising-curriculum`, and `startup-exit-curriculum`.

## Exercises

- [exercise-01 — Co-founder equity-split conversation drill](./exercises/exercise-01-co-founder-equity-split-conversation-drill.md)
- [exercise-02 — Founders' restricted stock and 83(b) authoring](./exercises/exercise-02-founders-restricted-stock-and-83b-authoring.md)
- [exercise-03 — PIIA and invention-carveout drafting](./exercises/exercise-03-piia-and-invention-carveout-drafting.md)
- [exercise-04 — DTSA whistleblower notice and trade-secret baseline](./exercises/exercise-04-dtsa-whistleblower-notice-and-trade-secret-baseline.md)
- [exercise-05 — Founder conflict-of-interest teardown](./exercises/exercise-05-founder-conflict-of-interest-teardown.md)
- [exercise-06 — Co-founder departure and repurchase playbook](./exercises/exercise-06-co-founder-departure-and-repurchase-playbook.md)
- [exercise-07 — Founder-diligence failure teardown and retroactive cleanup](./exercises/exercise-07-founder-diligence-failure-teardown-and-retroactive-cleanup.md)

## Resources

- [resources.md](./resources.md) — primary statutes, IRS publications, DOL / EEOC references, DGCL sections, and standard-form pointers cited across the chapters.

## Ownership boundary (quick reference)

This module owns the **founder legal architecture.** It hands off:

- **Entity-side machinery** (charter, bylaws, board consents as corporation-side acts, corporate record, franchise tax) → [mod-101 — Legal Entity Formation & Corporate Structure](../mod-101-legal-entity-formation-and-corporate-structure/).
- **Employee-side legal architecture** (non-founder offer letters, W-2 vs. 1099 for the broader workforce, FLSA, restrictive-covenant depth, EEOC) → [mod-103 — Employment Law, Worker Classification & Contract Design](../mod-103-employment-law-and-contract-design/).
- **Equity-comp policy for the broader team** (grant guidelines, refresh cadence, comp committee) → [mod-105 — Equity-Compensation Policy & the Compensation Committee](../mod-105-equity-compensation-policy-and-comp-committee/).
- **Priced-round preferred-stock and cap-table mechanics** → `startup-finance-fundraising-curriculum`.
- **Change-of-control transaction mechanics** (including single-trigger acceleration analysis and CoC-accel implementation) → `startup-exit-curriculum`.
- **Board-operations depth and officer-duty depth beyond the founder slice** → [mod-111 — Corporate Governance, Board Operations & Officer Duties](../mod-111-corporate-governance-board-operations-and-officer-duties/).

See [chapter 09](./09-ownership-boundary-map.md) for the full boundary map.

## Prerequisites

- [mod-101 — Legal Entity Formation & Corporate Structure](../mod-101-legal-entity-formation-and-corporate-structure/). The founder-side documents here reference the corporation-side documents authored there.
- `startup-foundations` — startup-as-a-system, the founder's operating loop.
- Comfort reading statutes and standard-form legal documents (Cooley, Wilson Sonsini, Orrick, Gunderson, Fenwick, Latham public model forms; NVCA priced-round set; see [resources.md](./resources.md)).

## What "done" looks like

By the end of this module you can, for a hypothetical founding team, produce and defend:

1. A founder agreement — equity split with rationale, roles and decision authority, dispute resolution, walk-away and re-vesting mechanics — signed by every founder.
2. A signed founder Stock Purchase Agreement for each founder, with vesting, repurchase right at cost, and market-standard double-trigger acceleration.
3. A timely-filed § 83(b) election for each founder with a certified-mail receipt in the corporate record.
4. A signed founder PIIA for each founder, with present-assignment language, work-for-hire + assignment backstop, complete Prior Inventions schedule, applicable state-law invention-assignment carveouts, and the DTSA whistleblower-immunity notice.
5. A founder-employment agreement or offer letter for each founder, cross-referencing the SPA and PIIA, with the compensation, at-will status, severance triggers and treatment, and continuing obligations documented.
6. A § 144 cleansing checklist for the corporation's related-party transactions, and a plan for the board's *Caremark* oversight discipline.
7. A written founder-departure playbook — the separation matrix, the counsel-engagement checklist, the § 144 cleansing steps, the OWBPA-compliant release, the cap-table update, the communication plan.
8. A Series-A-grade "Founder Documentation State" diagnostic memo for an existing messy founder file, with a retroactive-cleanup plan.
