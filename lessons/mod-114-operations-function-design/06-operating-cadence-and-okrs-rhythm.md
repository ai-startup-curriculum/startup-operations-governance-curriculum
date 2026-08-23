# 6. Operating cadence and the OKRs rhythm

> A well-run scale-up runs on a metronome: a weekly ops review, a monthly business review, a quarterly OKRs cycle, an annual plan and offsite. Get the metronome right and the company self-organises around it; get it wrong and every function invents its own tempo and none of them agree.

## Motivation

Ask a struggling scale-up "how do you run the business?" and you often get one of two answers. Either "we have a lot of meetings" (and no rhythm — a dense calendar of overlapping check-ins where nothing gets decided), or "we hold a quarterly all-hands and mostly wing it in between" (and no discipline — a big theatrical event with no operating loop).

The alternative — a **layered operating cadence** — is not novel. Andy Grove's *High Output Management* codified the weekly one-on-one and the operations review at Intel in the 1980s. Andrew Grove's OKRs practice, transmitted to John Doerr and then to Google, Intuit, and thousands of scale-ups, structured the quarterly goal-setting layer. Christina Wodtke's *Radical Focus* and *The Team That Managed Itself* rebuilt the practical mechanics for a modern software company. Verne Harnish's *Scaling Up* and the Rockefeller Habits framework sit alongside as an alternative execution rhythm popular with founder-led private companies. The through-line across all of them is the same: **weekly for tactics, monthly for operating results, quarterly for goals, annually for plan and strategy.**

This chapter authors that rhythm — what happens at each layer, who owns it, what the artifacts are, and how it interlocks with the CFO's monthly-close cycle. It defers the OKRs canon depth to [chapter 07](./07-scaling-up-greiner-adizes-org-evolution.md) (which houses the broader organisational-evolution canon in which OKRs sits) and the executive-team operating rhythm to [chapter 09](./09-executive-team-operating-rhythm.md) (which authors the E-team meeting choreography specifically).

## The four-layer cadence

### Layer 1 — Weekly ops review

The **weekly ops review** is the tactical operating meeting. It happens at the executive-team level (weekly E-team meeting — see [chapter 09](./09-executive-team-operating-rhythm.md)) and cascades down through every layer of the org (weekly leadership meetings inside each function). The COO / CoS chairs the E-team weekly; each functional VP chairs the weekly inside their function.

**Purpose.** Review KPIs and operating metrics at the current-week level; surface open decisions; unblock cross-functional issues; assign follow-through owners.

**Standing agenda (90-minute default):**
- **KPIs / operating metrics — 20 minutes.** Traffic-light review of the metrics dashboard. Green: on plan; no discussion. Yellow: slipping; owner explains; team decides whether to intervene. Red: breach; owner explains; team decides remediation.
- **Open decisions — 20 minutes.** A short list of decisions the team needs to make this week. Each decision has a designated owner and a recommendation; the meeting either endorses, modifies, or defers with a clear next step.
- **Cross-functional blockers — 20 minutes.** Issues that touch multiple functions and need the room to unblock. The COO / CoS mediates.
- **Topic-of-the-week (rotating, 20 minutes).** A deep-dive rotated across functions — one week a hiring update from People, another a pipeline update from CRO, another a systems-migration update from Ops. Not a decision meeting; an information-sharing meeting.
- **Follow-through review — 10 minutes.** Last week's action items reviewed for closure. Anything outstanding gets re-owned or escalated.

**Artifacts.**
- **Dashboard** — the executive-team KPI dashboard, refreshed weekly, single canonical source (BI tool or spreadsheet — the source is less important than the fact of one canonical source).
- **Action-item log** — every action item, with owner, due date, status. Reviewed at the top of the next week.
- **Decision log** — every decision, with rationale, owners, and re-look date if applicable. Fed into the corporate record for the material ones.

**Sizing.** 60 minutes at Series A / early Series B (small executive team, less cross-functional load); 90 minutes at Series B / C (denser executive team, more cross-functional coordination); rarely more than 120 minutes — beyond that, the meeting becomes an update session rather than a working session.

### Layer 2 — Monthly business review (MBR)

The **monthly business review** is the operating meeting at monthly cadence. It happens after the month-end close (the CFO's monthly close cycle produces the closed-books financials, typically by the 5th–10th business day of the following month — see the finance-fundraising curriculum). <!-- needs-research: confirm the specific chapter path in startup-finance-fundraising-curriculum mod-111 for the monthly close cycle chapter that this cadence coordinates with. -->

**Purpose.** Review the closed-book monthly financials; review the KPI results against the monthly plan; review risks and open strategic topics; take cross-function-alignment decisions that need a monthly cadence rather than weekly.

**Standing agenda (2.5-hour default):**
- **Financials — 30 minutes.** CFO walks the closed-book financials: revenue by segment, gross margin, operating expense by department, cash and runway, key balance-sheet items. Variance to plan and to prior month; commentary on drivers.
- **KPI review — 30 minutes.** Deeper KPI review than weekly — trailing 3–6 months of trend, cohort analysis for retention / expansion / churn metrics, funnel-conversion detail. BizOps prepares.
- **Departmental reviews — 45 minutes (in rotation).** Each department (rotating) presents a deeper review — GTM one month, Product one month, Engineering one month, People one month. Not every department every month; a rotation over the quarter covers each.
- **Strategic topic — 30 minutes.** One strategic topic per MBR — pricing, hiring plan, competitive positioning, customer segmentation. The CoS coordinates the topic selection against the CEO's strategic priorities.
- **Risks / open decisions — 15 minutes.** Elevated risks and cross-function decisions that need the room.

**Attendance.** Executive team plus the leaders of the departmental reviews on the agenda for that month. Sometimes the board's independent director (if any) attends as an observer; sometimes not.

**Artifacts.**
- **MBR pack** — a 20–40 slide document produced by BizOps, distributed 24 hours in advance as a pre-read.
- **MBR minutes** — the CoS / BizOps captures decisions and action items, distributes within 48 hours.
- **Follow-through** — MBR action items feed into the weekly ops review's follow-through review.

**Timing.** Held in the second or third week of the month, after the CFO's close but before the last week (which is often consumed with month-end / quarter-end preparations for the current month). The exact date is set for the year and diarised.

### Layer 3 — Quarterly OKRs cycle

The **quarterly OKRs cycle** is the goal-setting and goal-review layer. It runs on a 90-day beat, with four operating anchors:

- **Q(n) setting.** In the last two weeks of Q(n−1), the E-team drafts and finalises the Q(n) company-level OKRs. Each function drafts and finalises the Q(n) function-level OKRs that cascade or connect. The COO / CoS runs the process; the CEO owns the company-level OKRs.
- **Mid-quarter check-in.** ~Week 6 of the quarter. A full-day working session (or a half-day, depending on size) where each function reports progress against Q(n) OKRs, calls the risk on any at-risk OKRs, and either commits to a corrective plan or explicitly downgrades expectations.
- **Retrospective.** ~Week 12 of the quarter (in parallel with Q(n) setting). Each OKR is scored (typically 0.0–1.0 or Red/Yellow/Green). The retrospective focuses on the *why* of any misses — was the goal wrong, the execution wrong, or the environment wrong? — not on blame.
- **Recalibration.** Between retrospective and setting for Q(n+1), the E-team discusses whether the company-level OKRs need directional change based on the retrospective. Occasionally the annual plan gets re-anchored here.

**OKRs canonical structure.**

Every OKR has:
- **One Objective** — a qualitative aspiration for the quarter, stated in language the team finds motivating.
- **3–5 Key Results** — quantitative, measurable, time-bound outcomes that constitute achievement of the Objective. Written such that "if all key results hit, the objective is achieved" is true.

Every function typically owns **3–5 Objectives per quarter**. Any more and the function is thin across too many priorities; any fewer and the OKRs aren't structuring the work. The whole-company OKRs are typically **3–5** total across the executive team.

**OKRs vs. KPIs.** KPIs are the *operating metrics* the business runs on (revenue, gross margin, ARR, CAC, LTV, retention, employee count). OKRs are the *goals* for the quarter, often *changes* to KPIs or *initiatives* that support them. A common failure mode is treating KPIs as OKRs (setting the OKR to "hit $10M revenue" when revenue is a KPI that's already being tracked continuously) — the OKR should articulate what needs to *change* to get there.

**Grading and stretch.** The Google / OKRs canon (per Doerr's *Measure What Matters* and the earlier Grove/Intel practice) treats **0.7 as a good score** — OKRs are set as stretch goals, and consistently scoring 1.0 means they weren't stretch. This is culturally hard for teams accustomed to "meeting the goal = success." Ceremonies at grading time — explicit acknowledgement that 0.7 is the target, not a failure — build the culture.

**Cascade vs. connect.** The classic cascade model (company OKRs → function OKRs → team OKRs → individual OKRs) works at some scales and breaks at others. Christina Wodtke's *Radical Focus* argues for a **connected** model — each level's OKRs are its own, and the connection to the level above is explicit but not mechanical. In practice, most scale-ups run a hybrid: cascade at the function level (company → function is tight); connect at the team / individual level (team OKRs support function OKRs but are authored by the team).

<!-- needs-research: verify the Wodtke framing of "connected" vs. "cascaded" OKRs from *Radical Focus* and *The Team That Managed Itself*, and the Doerr framing of the 0.7 grading convention from *Measure What Matters*. -->

### Layer 4 — Annual planning and annual offsite

The **annual planning cycle** is the strategic layer. It runs on an annual beat, anchored 6–8 weeks in advance of the fiscal-year start.

**Timing.** For a calendar-year fiscal year, annual planning runs roughly November–December for the following year; for a fiscal year that starts in April (common for some UK / Japan / India-domiciled operations), 6–8 weeks earlier.

**Standard flow.**

1. **CEO strategy pre-read (Week −8 to −6).** The CEO drafts a 5–10 page strategy memo — where the company is going in the next 12 months, what's changing from the prior year, the key bets, the key risks. Distributed to the E-team.
2. **Executive-team offsite (Week −6 to −4).** Multi-day (typically 2–3 days) off-site with the E-team. Day 1: reset on strategy against the CEO memo. Day 2: draft the annual plan — top-of-house OKRs, financial plan, hiring plan, key initiatives. Day 3: cross-function alignment on how the plan translates to each function's own operating plan.
3. **Financial plan authoring (Week −4 to −2).** CFO and BizOps translate the strategic direction into a bottom-up financial plan — revenue by segment, headcount by function, opex by department, capex, cash and runway. The plan lands as the operating budget for the year.
4. **Functional operating plans (Week −4 to −1).** Each function authors its own 12-month operating plan — hiring plan, roadmap, quarterly OKRs skeleton. The COO / CoS reviews for cross-function coherence.
5. **Board approval (Week −2 to 0).** The board approves the annual operating plan and budget at the last board meeting of the prior year, per the delegation-of-authority policy. See [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).
6. **All-hands rollout (Week 0 to +2).** The CEO presents the annual plan to the company at an all-hands. Function leads present their functional plans and Q1 OKRs at team-level all-hands within the first 2–3 weeks.

**Artifacts.**
- **Strategy memo** (CEO-authored) — the strategic pre-read.
- **Annual plan** (COO / CoS-authored) — the operating plan document that translates strategy into execution.
- **Financial plan** (CFO-authored) — the budget, headcount plan, cash-runway model.
- **Functional plans** (function leads) — each function's own plan.
- **All-hands deck** — the company-facing translation.

**The annual offsite.** The E-team offsite is often more than a planning exercise; it is a team-formation and executive-culture event. Location varies (some CEOs favour in-office simplicity; some favour a physical remove). Facilitation by an outside coach (particularly a Lencioni-trained team coach — see [chapter 09](./09-executive-team-operating-rhythm.md)) is common at growth stage.

## The four-layer interlock

The four layers are not independent — they interlock. A well-run cadence has explicit **hand-offs** between the layers.

- **Weekly → Monthly.** Weekly KPI slippage becomes a monthly-review agenda item if the slippage persists. The MBR is not surprised by anything the weekly ops review already knows.
- **Monthly → Quarterly.** Persistent MBR themes — "we've missed the retention target three months running" — become quarterly OKRs or drive OKRs recalibration.
- **Quarterly → Annual.** Quarterly OKRs retrospectives inform the annual plan. Persistent quarterly slippage on a bet is a signal the annual plan needs adjustment.
- **Annual → Quarterly.** The annual plan sets the direction the Q1 OKRs execute against. Q1 setting is not a blank sheet; it's the first 90 days of the annual plan.

The interlock is what makes the rhythm coherent. Without it, each layer runs disconnectedly — the annual plan announced in January is never revisited; the quarterly OKRs are set independent of the annual plan; the monthly review discusses financials while the OKRs go unmentioned. A well-run cadence keeps all four in conversation.

## Interaction with the CFO's monthly close cycle

The MBR (Layer 2) is downstream of the CFO's month-end close. The close cycle produces:

- **Closed-book financial statements** (P&L, balance sheet, cash flow) for the month.
- **Variance analysis** against budget and against the prior period.
- **Commentary** on drivers of variance.

The MBR uses these as its financial input. The COO / CoS coordinates the MBR date to fall **after** the close is complete but **before** the CFO's board-pack preparation for any board meeting in that month (so the MBR discussion informs the board pack, not the other way around).

**Typical calendar for a monthly-close company:**
- **Business day 1** — close begins.
- **Business day 5–8** — close complete; management financials available.
- **Business day 10–12** — MBR held.
- **Business day 15–20** — board pack prepared (if a board meeting that month).
- **Business day 20–25** — board meeting.

For companies with weekly or bi-weekly close (rare at scale-up stage, more common at very finance-mature growth-stage companies), the interaction compresses. For companies with a slower close (common at early stage where the accounting function is small), the MBR may run against management financials that aren't fully closed — with the CFO's caveats on the number.

<!-- needs-research: confirm the specific chapter path in the startup-finance-fundraising-curriculum for the monthly close cycle chapter and any specific cadence references. -->

## The board-preparation interaction

The CoS partners with the CFO on **board-preparation** (see [mod-111 chapter 02](../mod-111-corporate-governance-board-operations-and-officer-duties/02-board-cadence-and-materials.md)). The operating cadence feeds the board pack:

- The **MBR pack** is the raw material for the board financial section.
- The **quarterly OKRs retrospective** is the raw material for the board's "operating results" section.
- The **annual plan** is the raw material for the annual budget / plan approval at the board.
- The **decisions and consents** taken through the operating cadence that require board notification or approval feed into the board's consent-agenda or resolutions.

The CoS's product is not the board pack itself (the CFO's product per the mod-111 boundary) — it is the *cadence discipline* that produces the raw material the board pack draws from.

## Concrete example — Series-B SaaS operating cadence

**Company:** Series-B B2B SaaS, 130 employees, calendar-year fiscal, monthly close by business day 7.

**Weekly cadence.**
- **Monday 9:00–10:30.** E-team weekly ops review. COO chairs. Dashboard, decisions, blockers, rotating topic, follow-through.
- **Monday 11:00–12:00.** Function-lead weekly meetings (each VP with their team). Function-level dashboard, decisions, blockers.
- **Wednesday 15:00–16:00.** Cross-function BizOps meeting — Strategic Finance, Analytics, PMO alignment on the KPI dashboard and the current-quarter OKRs.

**Monthly cadence.**
- **Business day 5.** CFO close complete; MBR pack authoring begins.
- **Business day 10.** MBR pack distributed as pre-read.
- **Business day 11 (2nd Thursday).** MBR — 2.5 hours. E-team plus the departmental review presenters for that month.
- **Business day 13.** MBR minutes and action items distributed.

**Quarterly cadence.**
- **Week 12 of Q(n).** Q(n) retrospective — half-day E-team session, function-level self-scores collected in advance.
- **Weeks 12–13 of Q(n) / Week 1 of Q(n+1).** Q(n+1) OKRs setting — E-team drafts company-level; each function drafts function-level in parallel.
- **Week 1 of Q(n+1).** All-hands rollout of the new quarterly OKRs.
- **Week 6 of Q(n+1).** Mid-quarter check-in — half-day.

**Annual cadence.**
- **Late October.** CEO strategy memo distributed.
- **First week of November.** E-team offsite — 3 days off-site.
- **November–early December.** Financial plan authored by CFO / BizOps; functional plans by each VP.
- **Mid-December.** Board meeting — annual operating plan and budget approved.
- **Early January.** All-hands rollout.

**Coordination points.**
- **Weekly-to-monthly.** The Monday ops review surfaces KPI-slippage themes that become MBR agenda items.
- **Monthly-to-quarterly.** MBR-recurring themes go into the quarterly retrospective input.
- **Quarterly-to-annual.** Quarterly retrospectives inform the annual-plan pre-read.
- **Board-pack alignment.** MBR pack feeds the board pack; the CoS distributes to the corporate secretary function per [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).

## Common failure modes

- **No canonical dashboard.** Every meeting has its own numbers; the numbers disagree; time is spent reconciling instead of deciding. Fix: BizOps owns the canonical dashboard; every meeting uses it or explicitly extends from it.
- **MBR before close is complete.** The MBR runs against management-estimate financials; the closed numbers land later and disagree; the MBR discussion was against a wrong picture. Fix: gate the MBR on close completion, even if that means moving the meeting date.
- **OKRs set without engagement.** OKRs cascaded top-down without function-level engagement; the functions treat them as an imposed exercise; grading is either theatre or absent. Fix: OKRs setting is a two-way exchange — company draft → function response → alignment discussion → publish.
- **OKRs never graded.** OKRs published at the start of the quarter, never mentioned in-quarter, never scored at the end. Fix: mid-quarter check-in and end-of-quarter retrospective are non-negotiable calendar items.
- **KPIs treated as OKRs.** The company sets the revenue KPI as an OKR every quarter; the OKRs mechanic never structures the *change* the team is committing to. Fix: OKRs are about the *deltas*, not the steady-state metrics.
- **Annual plan announced and forgotten.** The plan is authored in December, presented in January, and never revisited. Fix: the plan is the input to the four quarterly OKRs cycles; quarterly retrospectives explicitly reference plan progress.
- **Rhythm imposed from the top, not adopted.** The CEO or COO announces the rhythm; the executive team does not commit; meetings run late, get skipped, or degrade. Fix: the rhythm is adopted with executive-team commitment; the CoS enforces the discipline; the CEO models it.

## Summary

- Four operating layers — **weekly ops review, monthly business review, quarterly OKRs cycle, annual planning + offsite** — form the metronome of a well-run scale-up.
- **Weekly** (60–90 min): KPIs, decisions, blockers, rotating topic, follow-through. E-team level; cascaded to each function.
- **Monthly** (2.5 hrs): financials from the closed books, KPI deep-dive, rotating departmental review, strategic topic, risks and decisions. Gated on the CFO's monthly close.
- **Quarterly**: OKRs setting → mid-quarter check-in → retrospective → recalibration. Grounded in the Grove / Doerr / Wodtke canon; typically 3–5 OKRs per level; 0.7 as a stretch-goal target.
- **Annual**: CEO strategy memo → E-team offsite (2–3 days) → financial plan → functional plans → board approval → all-hands rollout. 6–8 weeks in advance of fiscal-year start.
- The **interlock** between layers is what makes the rhythm coherent — weekly feeds monthly feeds quarterly feeds annual, and back.
- The **MBR interacts with the CFO's monthly close cycle** (see the finance-fundraising curriculum) — the MBR runs after close completion and before board-pack preparation, so its output informs the board.
- The **CoS partners with the CFO on board preparation** ([mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/)) — the operating cadence produces the raw material for the board pack.
- [Chapter 07](./07-scaling-up-greiner-adizes-org-evolution.md) situates this rhythm inside the broader org-evolution canon (Scaling Up, Rockefeller Habits, Greiner, Adizes); [chapter 09](./09-executive-team-operating-rhythm.md) authors the executive-team-specific rhythm in depth.
