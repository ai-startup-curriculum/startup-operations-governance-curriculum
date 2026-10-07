# 1. Job architecture and the leveling framework

> Without a ratified job architecture the corporation does not have a compensation system — it has a backlog of Slack-negotiated exceptions that happen to add up to a payroll file.

## Motivation

Every other artifact this module produces — the cash-and-equity bands in [chapter 02](./02-cash-and-equity-bands-per-level-per-geography.md), the benchmarking source selection in [chapter 03](./03-benchmarking-data-sources-by-stage.md), the annual comp cycle in [chapter 04](./04-annual-comp-cycle.md), the pay-transparency postings required under state statutes and the EU Pay Transparency Directive (Directive (EU) 2023/970) in [chapter 05](./05-pay-transparency-compliance.md) — assumes that a specific hire fits a specific *level* in a specific *function track*. Without that, every downstream artifact is a one-off negotiation and the comp system is a backlog of exceptions.

The symptom pattern is specific and recurring. Titles proliferate without a shared meaning ("Senior Engineer II," "Lead Engineer," "Staff Engineer, L5," "Principal Engineer, Platform"), and no one in the room can say which of those is senior to which. Bands are negotiated in Slack between the hiring manager and the founder-CEO on offer day, forty minutes before the offer letter goes out. Managers who cannot get the cash-comp adjustment their star IC asked for promote them instead, so promotion is used as a comp-adjustment instrument rather than a scope-change signal. Engineering and Product disagree at the first joint planning meeting about whether an "E5" and a "P5" are peers. The CA / CO / WA / NYC / IL / WA state-mandated external pay-range posting the recruiting coordinator published last week turns out to be inconsistent with the comp statement the new hire actually received, triggering a reconciliation incident that the Head of People and GC have to work through together (see [mod-103 chapter 03](../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md)).

Then Series-B people diligence lands and the lead's diligence counsel asks for the leveling framework, the band-to-level map, and the calibration-council minutes for the last four cycles. A corporation that cannot produce those three documents in the first diligence response spends the next two weeks producing them under time pressure, with the deal clock running.

This chapter builds the job architecture and the leveling framework from the ground up: why it exists, which function tracks it covers, how the IC and manager ladders run in parallel, what distinguishes one level from the next, who owns the calibration ritual, and what drift modes the calibration ritual exists to prevent. The chapter speaks to the Head of People, the Head of Total Rewards (if that role has been added), the founder-CEO who still ratifies exec levels, and the function leaders (CTO, CPO, CRO, CFO, GC, CDO) whose tracks are being codified.

The chapter does not build the engineering-ladder competencies themselves to full depth — that is `cto-curriculum`'s territory. It does not build GTM-plan comp architecture — that is `startup-product-gtm-curriculum`'s territory and this module's [chapter 07](./07-sales-comp-plan-design.md). It does not stand up the promotion machinery or the performance-review feed that assigns people to levels — that is [mod-107](../mod-107-performance-promotion-and-offboarding/)'s territory. What this chapter owns is the *shape* of the architecture that all those other systems slot into.

## Why a job architecture exists

Five distinct problems collapse into a single ratified artifact when the corporation stands up a job architecture.

### Inconsistent titles across functions and hires

The first symptom is title proliferation. Two engineers hired two months apart carry titles — "Senior Software Engineer" vs. "Lead Software Engineer" — that neither the hiring manager nor the hires can defensibly say are at the same level or at different levels. A year later the manager promotes one and not the other, and the second one escalates. Without a ratified title-to-level map, every title conversation is a founder-adjudicated edge case.

### Slack-negotiated bands on offer day

The second symptom is comp decisions made in Slack. The hiring manager asks the founder-CEO at 4:40pm on a Friday whether they can "stretch" the offer by $15k because the candidate has a competing offer; the founder-CEO says yes; the offer goes out; six weeks later the new hire's base lands above a tenured peer's and the manager has a comp-equity problem the Head of People has to solve retroactively. A ratified band at each level is the discipline that makes the "stretch" conversation structured: inside the band, no approval; above the band, documented exception with named approver.

### Promotion inflation as a workaround for flat comp

The third symptom is promotion-as-comp-adjustment. A manager cannot adjust the IC's base inside the current band — the IC is already at the band ceiling, or the function's merit budget is spent — but can "promote" the IC to the next level, where the band is wider, and recover the comp adjustment that way. Over several cycles the IC population quietly shifts right on the leveling distribution with no corresponding shift in scope or impact, and the corporation ends up with a staff-heavy, mid-level-light engineering organisation that cannot explain itself at Series-B diligence. Chapter 08 — [comp-architecture failure modes](./08-comp-architecture-failure-modes.md) — covers promotion inflation and the related level-compression failure mode in depth.

### Cross-function miscalibration

The fourth symptom is cross-function drift. Engineering has an E5 band. Product has a P5 band. The two bands were authored at different times by different leaders against different benchmark cuts. A year later the Engineering E5 cash band is materially above the Product P5 cash band, or vice versa, and the first joint planning meeting between an E5 and a P5 surfaces the gap. The architecture is the forcing function that keeps the "equivalent level across functions" claim meaningful.

### Pay-transparency and diligence reconciliation

The fifth symptom is the external audience. Pay-transparency statutes (CO Equal Pay for Equal Work Act, CA SB 1162, NYC Local Law 32, NY State S9427A, WA Equal Pay and Opportunities Act, IL HB 3129, and the growing adopting-state list — defer the current state-by-state matrix to [mod-103 chapter 07](../mod-103-employment-law-and-contract-design/07-state-law-variance-across-california-new-york-illinois-washington-colorado.md) and this module's [chapter 05](./05-pay-transparency-compliance.md)) require that external job postings carry a pay range. The EU Pay Transparency Directive (Directive (EU) 2023/970, transposition deadline 2026-06-07) requires a documented, objective, gender-neutral set of criteria used to evaluate and compare roles across the corporation's EU workforce. Both regimes require, in effect, that the corporation have a ratified job architecture before any offer letter leaves the building. Series-B+ people diligence asks for the same artifact under a different name.

## Function tracks the architecture covers

A mature architecture carries parallel tracks for every function the corporation actually employs people in. The default track list for a Series-B US tech corporation:

- **Engineering** — the richest ladder, usually the first one authored. Nuances defer to `cto-curriculum`.
- **Product** — product management, product operations.
- **Design** — product designers, researchers, content designers, design-ops.
- **Data / ML** — data engineers, data scientists, ML engineers, ML research, applied science. Depending on scale, Data / ML may be its own track or sit inside Engineering.
- **Sales (GTM)** — AE ladder (SMB AE / Mid-Market AE / Enterprise AE / Strategic AE), SDR / BDR ladder, SE ladder, Sales Management ladder.
- **Marketing** — product marketing, content, growth, demand generation, brand, communications.
- **Customer Success** — CSMs, Technical Account Managers, Support Engineers, Solutions Architects (depending on how the corporation splits post-sales).
- **Operations / BizOps** — business operations, strategy, chief-of-staff-adjacent roles.
- **Finance** — accounting, FP&A, treasury, controller stack. The Finance-leveling nuances the CFO owns defer to `startup-finance-fundraising-curriculum` mod-111.
- **People** — recruiting, HRBP, L&D, Total Rewards, People Operations.
- **Legal** — commercial counsel, employment counsel, privacy / regulatory, paralegal.

Two decisions get made every time a new function stands up.

### Decision 1 — does it get its own track, or does it sit inside a parent track?

A new "AI Research" team of three can be a sub-track of Engineering (shared E-ladder, shared band) or its own track (research-scientist ladder with distinct competencies and a distinct band authored against a different market cut — foundation-model research is a materially different market from product engineering). The decision depends on how the corporation hires and promotes the function. If AI-research hires come from a market where competency expectations and benchmark data differ meaningfully from the Engineering baseline, the function needs its own track. If not, it sits inside Engineering with a role-family tag.

### Decision 2 — who ratifies the new track?

A new track changes the shape of the architecture. The leveling-council (see below) ratifies the standup; the Head of People or Head of Total Rewards owns the drafting; the function leader supplies the competency inputs. Without the ratification step, new tracks drift into existence through recruiter-written job descriptions and nobody can later say when the track started or who approved it.

## IC and manager parallel ladders

A single-ladder architecture — one path from new-grad to C-suite that runs through people management — forces every would-be senior IC to become a manager to progress in comp or title. That is a known organisational failure mode: the corporation loses senior ICs who do not want to manage, promotes ICs into management who are not suited to it, and ends up with a management layer that is thicker and less skilled than its IC bench.

The dual-ladder convention solves this by running two ladders at the same height.

### The dual-ladder convention

The IC ladder runs the full height of the architecture. A Staff / Principal / Distinguished IC is a peer of a Director / VP in cash, equity, and (in some conventions) title weight. The IC's scope is deep technical / design / research leadership of a system, product area, or technical direction; the manager's scope is people and organisational leadership. Both ladders exist. Neither is subordinate to the other.

### The "manager tax" vs. "manager premium" debate

Two conventions exist for how to band managers relative to equivalent-level ICs:

- **Manager premium.** A first-line manager (M1) sits slightly above the equivalent IC level (E4 → E5 range) in cash and equity, on the rationale that the manager's role carries additional scope and the market pays for people leadership. This is the more common convention at later stage and in larger organisations.
- **Manager tax (or manager parity).** A first-line manager sits at or slightly below the equivalent IC level in cash and equity, on the rationale that the IC path is higher-variance (deep expertise, named-expert market) and the manager path is lower-variance (replaceable people leadership). This is the less common convention and is usually a deliberate statement about what the corporation values.

The debate is less important than the discipline. The corporation picks a convention and sticks with it. Mid-cycle convention changes are visible to the whole org inside two weeks (see [chapter 04](./04-annual-comp-cycle.md)).

### The compression trap

The commonest dual-ladder failure mode is **IC-ladder compression**: the manager ladder runs up through VP and SVP, but the IC ladder stops two levels short — the top IC is a "Staff" or "Senior Staff," with no Principal or Distinguished tier. The effect is that any IC who wants to progress past Staff must either leave or move to the manager track. The IC-ladder "ceiling" becomes a retention trap for the corporation's most technically senior ICs. The fix is to extend the IC ladder to the full height of the manager ladder — a Principal IC as a Director peer, a Distinguished IC as a VP peer, a Fellow as an SVP or C-suite peer. Chapter 08 covers level-compression failure modes in depth.

## Level definitions

A level is a *competency band*, not a title. A level definition should let a calibration committee, given a candidate's work history and current scope, place the candidate inside one level and defensibly exclude the levels above and below. Four dimensions do most of the distinguishing work.

- **Scope** — the size of the thing the person operates on. From task (a well-defined piece of work with clear acceptance criteria) → feature (an end-to-end user-facing capability) → system (a non-trivial technical system with ongoing lifecycle) → product area (a coherent slice of product with multiple systems) → function or org (a cross-team or cross-function remit).
- **Complexity** — the ambiguity in the problem space. From "known pattern, known solution" → "known pattern, new problem" → "ambiguous problem requiring design judgment" → "problem definition itself is contested and requires framing" → "problem does not exist yet; the person is defining the frontier."
- **Autonomy** — the person's reliance on supervision. From supervised (needs direction on what to do and how to do it) → self-directed (needs direction on what, figures out how) → sets direction (identifies what should be worked on and gets others aligned) → sets strategy (identifies what the function or org should be working on multi-year).
- **Impact** — the radius of the person's effect. From self (own output) → team (team's output) → function (function's trajectory) → company (company's trajectory) → industry (industry-visible impact).

### Worked level rubric — engineering IC ladder (E1 → E7)

The rubric below is illustrative; the full depth of engineering competencies — code quality, system design, operational maturity, cross-team influence, technical judgment — is the subject of `cto-curriculum`. The step-change-per-level view this chapter cares about:

- **E1 — New-grad / Associate Engineer.** Scope: well-defined task. Complexity: known pattern, known solution. Autonomy: supervised; needs direction on what to do and often on how. Impact: self. Ramp-oriented level; most ICs leave the level within 12–24 months.
- **E2 — Software Engineer.** Scope: multiple tasks, small features. Complexity: known pattern applied to new problems inside the team's domain. Autonomy: self-directed on tasks; supervised on features. Impact: self and immediate team.
- **E3 — Software Engineer II / Mid.** Scope: features end-to-end. Complexity: ambiguous problems inside the team's domain requiring design judgment. Autonomy: self-directed on features; identifies and raises risks. Impact: team.
- **E4 — Senior Engineer.** Scope: systems; owns a non-trivial technical system across its lifecycle. Complexity: ambiguous problems requiring design and operational judgment; brings best practice from outside the team. Autonomy: sets direction for own work and influences team direction. Impact: team and adjacent teams.
- **E5 — Staff Engineer.** Scope: product area or multiple systems; technical leader for a cross-system concern (reliability, platform, data). Complexity: contested problem definitions; frames problems for the team and the function. Autonomy: sets technical direction for a product area. Impact: function.
- **E6 — Senior Staff / Principal Engineer.** Scope: multiple product areas or a function-level technical concern. Complexity: multi-year technical bets; identifies problems the function should be solving. Autonomy: sets technical direction for the function or across functions. Impact: company. Peer tier to a Director of Engineering in cash and equity.
- **E7 — Distinguished Engineer / Fellow.** Scope: company-level technical direction or an industry-visible technical remit. Complexity: shapes the frontier the company operates on; the problems are the ones the industry has not solved. Autonomy: sets multi-year technical strategy. Impact: company and industry. Peer tier to a VP or SVP of Engineering in cash and equity. The level exists even if currently unfilled — leaving it unauthored invites the compression trap above.

### Parallel ladders at a glance

- **Product (P1–P5+).** Scope progresses from feature → product area → multi-product → function → company product strategy. Complexity progresses from execution of a defined roadmap → shaping the roadmap → shaping the strategy. Autonomy and impact follow the engineering parallel.
- **Design (D1–D5+).** Scope progresses from component / screen → flow → product area → cross-product system (design-system, research function) → company design direction.
- **Data / ML (DS1–DS5+ / MLE1–MLE5+).** Scope progresses from analysis task → model → pipeline → platform → function-level data direction. The applied-research vs. production-ML split is sometimes two sub-tracks.
- **GTM / Sales.** The convention is role-named rather than number-named: AE → Senior AE → Enterprise AE → Strategic AE, with a parallel SDR / BDR → Senior SDR → SDR Manager ladder, a parallel SE ladder, and a parallel Sales Management ladder (Sales Manager → Director → VP → CRO). Scope progresses from quota segment size and deal complexity rather than from scope / complexity in the engineering sense.
- **Finance.** Analyst → Senior Analyst → Manager → Senior Manager → Director → VP → CFO, with sub-tracks for Accounting, FP&A, and Treasury. The CFO-owned leveling nuances defer to `startup-finance-fundraising-curriculum` mod-111.
- **People.** Coordinator → Specialist → Manager → Director → VP → CPO, with sub-tracks for Recruiting, HRBP, Total Rewards, and L&D.
- **Legal.** Paralegal → Counsel → Senior Counsel → Managing Counsel → Deputy GC → GC. The GC level is a founder-and-board-ratified exec hire and should not be arbitrarily assigned an "E-equivalent" by analogy — see the drift mode below.

## Leveling calibration norms

The architecture is only as good as the ritual that keeps it from drifting. Five norms do most of the work.

### Calibration-committee cadence

A calibration committee meets inside the annual comp cycle (see [chapter 04](./04-annual-comp-cycle.md)) and at any mid-cycle event where a promotion or an above-band exception is proposed. The committee reviews every proposed level assignment, promotion, and above-band exception against the ratified level definitions, with the hiring manager or promoting manager present to defend the proposal. The decision rights sit with the committee, not with the manager; the manager recommends. The actual promotion-decision machinery and the performance-review feed that supplies evidence to the committee are owned by [mod-107](../mod-107-performance-promotion-and-offboarding/).

### Calibration-against-hire-letter audit

Once per cycle, the committee samples a non-trivial fraction of the last cycle's offer letters and asks: did the level assigned on the letter match the level the hire has been performing at twelve months in? Systematic over-levelling at hire — the "we had to level them up to close the offer" pattern — is the leading indicator of band drift and the most reliable early signal of promotion inflation. The audit output is reported to the comp committee as a Stage-4 artifact in the annual cycle.

### Cross-function leveling council

Before any new function stands up its own ladder, a cross-function leveling council (chaired by the leveling librarian, with representation from every existing track) reviews the proposed ladder and ratifies the equivalence claim ("D5 is a peer of E5 is a peer of P5"). The council also reviews proposed changes to any existing ladder before ratification. Without a cross-function body, each function drifts on its own clock.

### Leveling librarian ownership

A single named owner — typically the Head of People at Series-A, the Head of Total Rewards at Series-B+ once that role has been added — owns the master level-definition document, the title-to-level map, and the calibration-committee minutes. The librarian is the arbiter of "is this the current version of the level rubric" and the publisher of the version-controlled definition.

### Annual revision cadence

Level definitions are revised once per year, synchronised with the annual comp cycle. Mid-cycle revisions are reserved for new-function standups and documented material errors; everything else waits. The revision is ratified by the comp committee alongside the band refresh.

## Drift modes the calibration norms exist to prevent

The following three drift modes are what the ritual above is designed to catch. [Chapter 08](./08-comp-architecture-failure-modes.md) covers the full failure-mode library and the fixes; this chapter names the three most directly connected to leveling.

### Function-by-function inflation

Engineering keeps shipping Staff titles for retention; Product does not; the two ladders drift. After two cycles the Engineering E5 band is populated by ICs doing E4 work and the Product P5 band is still populated by ICs doing P5 work. Cross-function joint work surfaces the gap. The cross-function leveling council and the calibration-against-hire-letter audit are the two norms that catch this.

### Scope creep inside a level

An E5 who has been at level for four years has absorbed additional scope informally — mentoring, cross-team pulls, incident command — without a corresponding promotion. On paper the IC is doing E6 work. Over time the band stops meaning "scope and complexity of this kind"; it means "tenure past some threshold." The calibration-against-hire-letter audit catches the inverse (over-levelling at hire); the annual cycle's calibration committee catches this (under-levelling against actual scope).

### New-function ladder-standup drift

The corporation hires a GC and the hiring team arbitrarily calls the role "E7-equivalent" because that is the band that produced a defensible cash number. There is no legal-track ladder; the equivalence is invented in the offer-letter approval conversation. Six months later the first Senior Counsel hire sits inside a function whose ladder has no definition, and the GC-to-Senior-Counsel comp relationship is a one-off. The cross-function leveling council is the norm that catches this: no new function stands up a ladder (or borrows an equivalence) without council ratification.

## Adjacent-module handoffs

The architecture connects to several adjacent systems. The handoff rules are:

- **Engineering-track leveling nuances** (what distinguishes an E4 from an E5 at the competency level — code review quality, incident command, system design judgment) defer to `cto-curriculum`. This module owns the *shape* of the ladder; the competency depth is engineering-leadership territory.
- **GTM-track leveling nuances** (what distinguishes an Enterprise AE from a Strategic AE — deal complexity, named-account mechanics, pod structure) defer to `startup-product-gtm-curriculum`.
- **Finance-track leveling nuances** (what distinguishes a Senior FP&A Manager from a Director of FP&A — scope of the planning cycle, board-materials ownership, treasury remit) defer to `startup-finance-fundraising-curriculum` mod-111.
- **Promotion decisions and the performance-review feed** that assigns people to levels defer to [mod-107](../mod-107-performance-promotion-and-offboarding/). This module ratifies the levels; mod-107 operates the promotion machinery against them.
- **Offer-letter pay-transparency reconciliation** — the moment at which an external posting's pay range must be consistent with the internal band for the level — defers to [mod-103 chapter 03](../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md).
- **Cash-and-equity bands sit on top of levels** — see [chapter 02](./02-cash-and-equity-bands-per-level-per-geography.md). A level without a ratified band is not operable.

## A worked example — Vireo Labs, Series-B

Vireo Labs is a fictional Series-B developer-tools corporation, roughly 140 employees, headquartered in San Francisco with a remote-first US workforce and a nascent London office. Vireo raised its Series-B eighteen months ago; a compensation committee is in place and has ratified the equity-grant guidelines (see [mod-105 chapter 01](../mod-105-equity-compensation-policy-and-comp-committee/01-grant-guidelines-by-level-and-function.md)). The Head of People was hired at Series-A and has been operating a Head-of-Total-Rewards-adjacent remit; the role is being formally split in the current fiscal year.

### First-pass track list

Vireo's architecture covers eight tracks at Series-B:

- **Engineering** (E1–E7). The richest ladder, drafted jointly with the CTO against the `cto-curriculum` reference material.
- **Product** (P2–P6). No P1 — Vireo does not hire new-grad PMs at this stage.
- **Design** (D2–D5). The current senior-most designer is at D4; D5 exists but is unfilled.
- **Data / ML** (DS2–DS6 for data science, MLE2–MLE6 for ML engineering). Sits as its own track rather than inside Engineering because the hiring market and competency expectations differ meaningfully.
- **GTM** — AE / Senior AE / Enterprise AE / Strategic AE ladder; SDR / Senior SDR / SDR Manager ladder; SE ladder; Sales Management ladder (Sales Manager / Director / VP / CRO).
- **Marketing** (MK2–MK5) and **Customer Success** (CS2–CS5) run as separate tracks under the CRO.
- **Finance** (F2–F6), **People** (HR2–HR5), **Legal** (L2–L5 with a GC exec slot above). Finance competency depth defers to `startup-finance-fundraising-curriculum` mod-111; People and Legal competencies are drafted by Vireo's Head of People and GC respectively.
- **Operations / BizOps** (BO3–BO5). Three ICs plus a chief-of-staff role that is explicitly off-ladder and sits in the exec org under the CEO.

### Parallel ladders

The IC ladder runs the full height — a Distinguished Engineer (E7) sits as a VP-of-Engineering peer in cash and equity, and a Principal (E6) sits as a Director-of-Engineering peer. The manager ladder (M4 first-line / M5 senior manager / D1–D2 director / VP / SVP) carries a manager-premium convention: a first-line engineering manager (M4) is banded between E4 and E5, with the midpoint closer to E5. The convention is documented in the leveling librarian's master document and reviewed annually.

### Leveling librarian and calibration cadence

The Head of Total Rewards (post-split) is the leveling librarian. The calibration committee is three members: Head of People, Head of Total Rewards, and a rotating function leader for each session. The committee meets monthly during the annual comp-cycle window (see [chapter 04](./04-annual-comp-cycle.md)) and quarterly at other times. The cross-function leveling council (one representative per track plus the librarian) meets twice per year to ratify changes to the architecture.

The calibration-against-hire-letter audit is a standing Stage-4 agenda item at the comp committee's annual-cycle meeting. The audit samples the previous cycle's offer letters at a documented sampling rate and reports the fraction of hires whose actual twelve-month scope matches the level assigned on the offer letter. <!-- needs-research: a defensible sampling rate for a Series-B population of ~140 and the audit-finding thresholds that should trigger a band or definition revision. -->

### Pending open items

- **Data / ML sub-track split.** The current Data / ML track has drifted toward production ML engineering; the applied-research hiring Vireo is doing for a new foundation-model team may require a sub-track with distinct competencies. The leveling council has it on the agenda for the next session.
- **GC-and-legal-track equivalence.** The GC was hired six months ago and the equivalence claim ("GC is a VP peer in cash and equity") was ratified by the comp committee at the time but has not been formally reconciled with the newly authored Legal track. The leveling librarian owns the reconciliation.
- **London-office level mapping.** Vireo's first UK hire is pending. The level definitions are intended to be geography-neutral; the bands that sit on top are not (see [chapter 02](./02-cash-and-equity-bands-per-level-per-geography.md)). The UK posting will need to satisfy UK pay-transparency expectations and, by 2026-06-07, the EU Pay Transparency Directive for any EU hires — the architecture's role is to supply the "objective, gender-neutral criteria used to evaluate and compare roles" the directive requires.

## Summary

- The job architecture is the artifact every other compensation decision assumes. Without it, titles proliferate, bands get Slack-negotiated on offer day, promotions get used as comp adjustments, cross-function peers drift, and Series-B people diligence surfaces reconciliation gaps the corporation cannot close under time pressure.
- The architecture covers parallel function tracks (Engineering, Product, Design, Data / ML, GTM, Marketing, CS, Ops, Finance, People, Legal) with two standing decisions each time a new function stands up: own-track vs. parent-track, and who ratifies.
- Dual IC and manager ladders run at the same height. The IC ladder must run the full height of the manager ladder (Principal as Director peer, Distinguished as VP peer, Fellow as SVP peer) or the corporation falls into the compression trap and loses senior ICs. The corporation picks a manager-premium or manager-parity convention and sticks with it.
- Levels are competency bands distinguished by scope, complexity, autonomy, and impact. The engineering IC rubric (E1 new-grad through E7 Fellow) is a worked example; Product, Design, Data / ML, GTM, Finance, People, and Legal have parallel ladders. Deep engineering-ladder competencies defer to `cto-curriculum`; GTM-ladder nuances defer to `startup-product-gtm-curriculum`; finance-ladder nuances defer to `startup-finance-fundraising-curriculum` mod-111.
- Calibration norms — a committee cadence inside the annual cycle, a calibration-against-hire-letter audit, a cross-function leveling council, a named leveling librarian, and an annual revision cadence — are what keep the architecture from drifting across functions and across time.
- The three drift modes the norms exist to catch are function-by-function inflation, scope creep inside a level, and new-function ladder-standup drift. [Chapter 08](./08-comp-architecture-failure-modes.md) covers the full failure-mode library and fixes.
- The architecture hands off to [chapter 02](./02-cash-and-equity-bands-per-level-per-geography.md) (bands sit on top of levels), [chapter 04](./04-annual-comp-cycle.md) (the cycle is where calibration happens), [mod-107](../mod-107-performance-promotion-and-offboarding/) (promotion and performance-review machinery), and [mod-103 chapter 03](../mod-103-employment-law-and-contract-design/03-offer-letter-architecture-and-pay-transparency.md) (offer-letter pay-transparency reconciliation).
