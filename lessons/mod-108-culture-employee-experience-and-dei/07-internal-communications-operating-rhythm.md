# 7. The internal-communications operating rhythm

> Internal comms is a calendared instrument, not a vibe. A defensible rhythm sets the cadence of all-hands, CEO letters, AMAs, and skip-levels; classifies every announcement by decision-status and channel; codifies which categories of information are held confidential before broadcast; and choreographs the crisis lane so the corporation is not composing its response for the first time when the incident is live.

## Motivation

The most common internal-comms failure is not a single bad email; it is the *absence of a rhythm* that the workforce can rely on. Employees adjust to whatever cadence the corporation actually operates against, and they infer meaning from every deviation. When the CEO cancels the third all-hands in a row, the org concludes there is bad news being withheld. When the monthly written update lands five weeks after the last one, the org concludes the CEO has stopped writing them. The signal is the cadence, not any particular message.

Four failure modes to build against.

- **The disappearing all-hands.** The corporation runs a weekly all-hands, misses one for a legitimate reason (an offsite, a board week), misses the next one because "we didn't have anything to share," and the cadence quietly drifts to fortnightly and then monthly. Attendance craters because the meeting has stopped being predictable. When the corporation eventually needs the all-hands to communicate something important, the muscle has atrophied and the moment lands badly.
- **The Slack-leak that gets ahead of the announcement.** An executive change is under discussion in a private channel of three people. One of the three tells their peer. Within 48 hours a screenshot is circulating in a general channel. The formal announcement, when it finally lands, is now defensive rather than authoritative — and the workforce has learned that important news is discovered on Slack rather than heard from leadership. The corporation has ceded the announcement to rumour.
- **The unanswerable AMA question.** The CEO opens the floor at the all-hands. A senior IC asks a pointed question about a rumoured layoff. The CEO stumbles, gives a non-answer, and the recording circulates. What was intended as a signal of transparency becomes a signal that transparency has limits the CEO cannot honestly acknowledge. The AMA format made the failure worse than a written response would have.
- **The tone-deaf crisis update.** Production is down for six hours. The engineering team is heads-down on the fix. Nobody communicates to the rest of the company for four of those six hours. Sales is on live customer calls with no talking points. Support is fielding tickets with no ETA. The corporation absorbs a preventable second-order damage cost — internal panic and external inconsistency — because there was no pre-agreed playbook for who owns internal updates during an incident.

The purpose of this chapter is to teach you to author an internal-comms operating rhythm that is predictable enough to be trusted, disciplined enough to survive an incident, and honest enough that the workforce reads the cadence and infers "we are being told the things that can be told." That means seven separate decisions, each with a defensible pattern, wired to the sibling operating cadences without being merged into them.

## The seven operating decisions

1. **All-hands cadence and pattern.** How often, agenda, who owns, length, recording and async cascade, attendance norms.
2. **Executive-communication cadence.** CEO weekly update, monthly CEO letter, quarterly business review, skip-level office hours, leadership-team retro.
3. **CEO Q&A / AMA pattern.** Anonymous submission, live-vs-written mechanic, CEO prep, hostile-question handling.
4. **Announcement taxonomy.** Informational / decision-required / feedback-invited classes, channel norms, response expectations.
5. **Confidential-communications operating norm.** Board decisions, executive changes, layoffs, MNPI handling.
6. **Cross-time-zone / remote-inclusive communications norm.** Recorded all-hands, written follow-up, rotating times, async decisions.
7. **Crisis-comms playbook.** Outage, security incident, PR incident, layoff, executive departure — who owns messaging and at what cadence.

Skip any one and the failure modes above are the predictable output.

## Decision 1 — All-hands cadence and pattern

Cadence should track stage and headcount, not founder preference.

| Stage | Cadence | Length | Recording | Rationale |
|---|---|---|---|---|
| Pre-seed / seed (<25) | Weekly, informal | 30 min | Optional | Everyone is in one room (physical or virtual); the all-hands is the operating meeting |
| Series-A (25–75) | Weekly | 30–45 min | Required | Cadence matters more than production value; keep the muscle |
| Series-B (75–250) | Bi-weekly | 45–60 min | Required, with written summary | Weekly is now too frequent to sustain quality content; bi-weekly forces preparation |
| Growth (250–1,000) | Monthly, with mid-month written update | 60–75 min | Required, with structured async cascade | Company is too large for genuine dialogue at the meeting; the written channel does more of the work |
| Late / pre-IPO (1,000+) | Monthly, plus function-level all-hands on off-weeks | 60 min | Required, with translated versions where warranted | Corporate all-hands loses signal; function-level cascade carries the operating detail |

The default is that the CEO owns the all-hands agenda and runs it personally. Delegating the agenda to the chief of staff or head of people is fine; delegating the presence of the CEO is not. The all-hands is one of the two forums (the other is the CEO letter) where the workforce takes a direct read on the CEO's engagement with the company.

**Agenda template.** A defensible all-hands is not a stack of exec-team updates. It is a shaped forty-five minutes.

- **Opening (5 min).** CEO frames the meeting: what we are here to discuss, what is new since last time, one specific call-out that references the values ([chapter 01](./01-values-behaviours-and-anti-values.md)).
- **Business update (10 min).** Metrics that matter this cycle, delivered against the plan the workforce has already seen. Do not surprise the workforce with a metric they have never been told about.
- **Function or theme deep-dive (15 min).** One function or one cross-cutting theme goes deep. Rotate across cycles so every function surfaces two or three times a year.
- **People moments (5 min).** New joiners, promotions, values-recognition call-outs, meaningful anniversaries. This is where culture is reinforced.
- **CEO Q&A / AMA (10 min).** See Decision 3 below. Non-negotiable — the all-hands does not close without live questions.

**Attendance-and-participation norms.** Attendance is expected of all employees; recordings and written summaries are for time-zone-excluded staff and legitimate conflicts, not for opt-out convenience. Cameras-on norms belong to the meeting culture in [chapter 05](./05-remote-hybrid-and-rto-policy.md); do not re-litigate them here. Question participation should be actively invited from the least-senior person in the room first, echoing the "say the uncomfortable thing" value pattern.

**Recording and async cascade.** Record every all-hands; publish the recording within 24 hours; publish a written summary (2–3 paragraphs plus the metrics and any decisions communicated) within 48 hours. Time-zone-excluded staff should be able to catch up in fifteen minutes of reading rather than an hour of video. The tool stack that carries this cascade is [chapter 05](./05-remote-hybrid-and-rto-policy.md).

## Decision 2 — Executive-communication cadence

The all-hands is the flagship. The rest of the executive-comms surface is a portfolio of narrower instruments, each with its own cadence and owner.

| Instrument | Cadence | Length / format | Owner | Purpose |
|---|---|---|---|---|
| CEO weekly update | Weekly | 200–400 word Slack / email post | CEO | Sustained signal; low-ceremony pulse between all-hands |
| Monthly written CEO letter | Monthly | 800–1,500 word long-form email or memo | CEO | Considered narrative on strategy, priorities, wins, losses |
| Quarterly business review (internal) | Quarterly | 60–90 min meeting + written pack | CEO + exec team | Metrics against plan; strategic re-baseline; what changed and why |
| Skip-level office hours | Monthly per exec | 30-min slots, 4–6 employees per session | Each exec independently | Direct read on the org two levels down; unmediated signal |
| Leadership-team retro | Monthly | 60–90 min, closed room | Exec team + facilitator | Team-effectiveness reflection; how the exec team is operating |

**CEO weekly update.** A short, cheap-to-produce artefact that lands in a predictable channel on a predictable day (Friday afternoon is the mainstream default). Two or three bullets on the week: one on business, one on people, one on customer. When the CEO has nothing new to say, the update still ships — "quiet week, deep focus on the pricing rebuild" is a valid update. Silence is not.

**Monthly CEO letter.** Long-form, considered, published in a durable place (an internal blog, a Notion space, or a mailing archive). This is the artefact new joiners will read to understand what the CEO has been thinking about over the past year. It is worth the CEO's time to draft personally, with a chief-of-staff edit pass. Ghostwriting the CEO letter is a category error — the workforce can tell within two paragraphs.

**Quarterly business review (internal QBR).** Distinct from the operations-function QBR that lives in [mod-114](../mod-114-operations-function-design/) and from the board pack that lives in [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/). The internal QBR is the all-employee version — plan-versus-actual, key strategic bets, what the executive team learned this quarter, what the next quarter's priorities are. It is a longer, deeper cousin of the all-hands, held once a quarter and often paired with the quarter-boundary all-hands.

**Skip-level office hours.** Every exec holds monthly office-hour slots open to employees two levels below them. The point is unmediated signal — an exec who only hears from their direct reports has a filtered picture. Slots should be bookable by any employee, not gated by the direct-report chain. Notes are not published (the office hour is a listening forum, not a broadcast one), but recurring themes surface at the leadership-team retro.

**Leadership-team retro.** A closed monthly session where the executive team discusses how *the executive team* is operating — what decisions were made well, which were made badly, what the team dynamic is producing. Facilitator (often the chief of staff or an outside coach) is recommended. This is not published anywhere; the output is the team-effectiveness improvement, not an artefact.

**Why the portfolio has to be a portfolio.** Founders frequently ask whether one strong instrument can substitute for the others — a great monthly letter in place of a weekly update, a great all-hands in place of skip-levels, a great QBR in place of the leadership retro. The answer is no, and the reason is that each instrument reaches a different audience through a different mechanism. The weekly update sustains presence between all-hands; the monthly letter carries considered narrative that no live meeting can match; the skip-level is unmediated signal from the org that no filtered channel produces; the leadership retro protects the exec team from becoming the source of its own dysfunction. Substituting one for another loses a distinct signal that the others do not replace.

<!-- needs-research: prevailing benchmarks on CEO-weekly-update adoption vs monthly-letter adoption in the Series-B to growth range; anecdote is heavy, data is thin -->

## Decision 3 — The CEO Q&A / AMA pattern

The AMA is the highest-leverage and highest-risk five minutes of the all-hands. Design it deliberately.

**Anonymous submission channel.** Questions are collected in advance through an anonymous submission tool (Slido, Pigeonhole, or a dedicated Slack workflow). Anonymity is preserved through the tool — the CEO and the moderator see the question text, not the submitter. Submissions open 48 hours before the all-hands and close two hours before, so that the CEO has time to prepare answers.

**Live vs written mechanic.** Two viable patterns:

- **Live-answer-with-upvoting.** Questions are visible to the workforce in advance and upvoted. The CEO answers the top 3–5 upvoted questions live in the all-hands. Any question not answered live gets a written response within one week. This pattern makes it obvious what the workforce actually wants to hear about.
- **Written-response-with-live-follow-up.** The CEO publishes written answers to all submitted questions in the day before the all-hands; live time is used for follow-up discussion on the most consequential answers. This pattern is better for a larger workforce and for questions that need a considered rather than reflexive answer.

Pick one and stick to it. Switching between patterns confuses the workforce and reads as evasion.

**CEO prep discipline.** The CEO does not walk into the AMA cold. The chief of staff prepares a briefing 24 hours before the all-hands: the submitted questions grouped by theme, the recommended framing for each, the specific facts the CEO needs to have at fingertips. For any question that touches confidential terrain (board decisions, executive changes, MNPI — see Decision 5), the briefing pre-drafts the "here is what I can and cannot say" response. The CEO should never be improvising on those topics.

**Handling the hostile question.** The hostile question is the one that lands with an implicit accusation — "why did the exec team decide X when everyone knows Y" — and demands the CEO defend a position under time pressure in front of the workforce. Three tactics:

1. **Restate charitably.** "The question underneath that, as I hear it, is [X]. Let me answer X." This buys thinking time and reframes the hostility without dismissing the substance.
2. **Acknowledge what is true.** Never argue with the factual premise of a hostile question you cannot cleanly refute. "You are right that we made that decision and it has not worked out the way we hoped" is an answer that costs nothing and buys enormous credibility.
3. **Defer with a specific commitment when the honest answer is "I don't know yet."** "I don't have a good answer today. I will publish a written response by Friday." Then publish it. The workforce forgives an "I don't know"; they do not forgive a bluff that gets caught.

**Cadence.** AMA runs at every all-hands. Do not skip it "because we're short on time" — skipping the AMA is the loudest possible signal that the executive team is uncomfortable with questions.

**The written-follow-up discipline.** Every question submitted through the anonymous channel that is *not* answered live at the all-hands gets a written response within one week, published in the same channel where the questions were collected. The written-follow-up backlog is a leading indicator of AMA health — a backlog that consistently runs three or four weeks late signals that the CEO is treating the AMA as ceremonial. The chief of staff owns the tracker and is empowered to escalate an ageing question directly to the CEO.

**When the honest answer is "not yet."** Some questions cannot be answered because the decision has not been made, the diligence is not complete, or the answer touches confidential terrain (Decision 5). The disciplined response is to say so specifically — "we are considering this, we expect to have a position by [date]" — and then to come back on that date with either the answer or an updated timeline. What breaks trust is not "not yet"; it is "not yet" repeated indefinitely with no reference to the previous "not yet."

## Decision 4 — Announcement taxonomy

Every announcement falls into one of three classes. The classification determines the channel and the response expectations.

| Class | Definition | Default channel | Response expectation |
|---|---|---|---|
| Informational | Sharing news, no action required from the recipient | Broadcast Slack channel (`#announcements`) + email digest for high-signal items | Read acknowledgement not required; questions in-thread welcome |
| Decision-required | A decision has been made; recipients must act (adopt a new tool, follow a new policy, etc.) | Named Slack channel + email + confirmation mechanism (form, emoji-ack) | Explicit acknowledgement required by a stated deadline |
| Feedback-invited | Input is being sought before a decision is finalised | Dedicated Slack channel with structured prompt, or Notion / Coda doc with comment access | Contributions welcome within a stated window; the window closes and the decision is made |

**Channel discipline.** `#announcements` is broadcast-only, moderated, low-volume. Discussion happens in threads or in topic channels, not in the announcement channel. This keeps the signal-to-noise ratio of `#announcements` high enough that the workforce actually reads it.

**Response-expectation discipline.** The three classes carry different expectations, and the announcer must say which. An informational note that reads as decision-required produces false urgency; a decision-required note that reads as informational produces missed adoption. Draft with the class in the subject line: `[Info]`, `[Decision]`, `[Feedback]` tags are ugly but load-bearing.

**Volume discipline.** A workforce that receives seven `[Decision]` notices in a week is a workforce that has stopped reading them. The head of people or chief of staff should hold a soft budget on announcement volume — no more than one or two decision-required announcements per week absent an unusual cycle. Everything else is either informational (goes into the digest) or is not important enough to broadcast.

**Authorship discipline.** Every announcement carries a named author and a named owner for follow-up questions. "From the executive team" is a red flag — it means no individual is on the hook for defending the content. The author should be the exec who owns the decision, not the chief of staff who drafted the words. This has a second-order benefit: the workforce learns which exec owns which surface area from the by-line pattern, which shortens the path for future questions.

## Decision 5 — The confidential-communications operating norm

Some categories of information are, by design, held confidential before broadcast. The norm is not "everything is transparent" — the norm is "everything that can be shared is shared on a predictable cadence; some things cannot be shared before a specific event, and the workforce understands why."

Codify the following categories explicitly in the handbook ([chapter 02](./02-employee-handbook-nlrb-compliant-post-stericycle.md)).

**Board decisions before all-hands.** Decisions taken at a board meeting are frequently discussed in the executive team in the days that follow but are not communicated to the workforce until the executive team has agreed on framing. The window from board decision to workforce communication should be days, not weeks — a longer window invites leak and speculation. The specific board-side dynamics of what may and may not be disclosed are owned by [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).

**Executive changes before all-hands.** An executive departure or a new executive hire is choreographed. The pattern: (1) the departing or arriving executive's direct reports are told first, in person; (2) the affected function is told next, within the same day; (3) the broader company is told at the next all-hands or, if the news cannot wait, via a same-day written announcement from the CEO. Rumour beating the announcement is a choreography failure — see [mod-107 chapter 07](../mod-107-performance-promotion-and-offboarding/07-executive-team-offboarding.md) for the full executive-offboarding playbook.

**Layoff announcement choreography.** A reduction in force is the highest-stakes internal communication the corporation ever runs, and it is almost always the moment when trust is either preserved or destroyed. The choreography — who is told first, in what order, by whom, with what written materials, and how the surviving workforce is addressed — is owned by [mod-107 chapter 06](../mod-107-performance-promotion-and-offboarding/06-rif-and-layoff-playbook-under-warn.md). The internal-comms norm to embed in this chapter is that no layoff announcement lands via Slack broadcast; the affected employees hear from a human first, and the surviving workforce hears at a named forum with the CEO present.

**Material non-public information handling.** For near-public (late-stage) and public corporations, some categories of information are legally sensitive: pending M&A, undisclosed financial results, material contract wins or losses. Reg FD (17 CFR §§ 243.100–243.103) constrains how a public issuer may selectively disclose material information. Internally, the practical rule is that MNPI is discussed on a strict need-to-know basis, is not shared in broadcast channels, and is subject to a trading blackout for anyone who receives it. The deep treatment of officer duties, Reg FD compliance, and insider-trading policy lives in [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/); the internal-comms norm here is simply that MNPI does not go into `#announcements`.

**The "why we cannot say more" norm.** The most under-used sentence in confidential comms is "there is a category of thing we do not discuss publicly until [event], and I cannot say more today." Teaching the workforce that this sentence exists — and that it is used honestly, not as a shield — is more valuable than any particular disclosure. When the workforce knows the rule, silence on a specific topic is read as "the rule applies here" rather than as "they are hiding something." This norm is authored explicitly in the handbook and referenced by name in AMA prep whenever a submitted question touches confidential terrain.

## Decision 6 — Cross-time-zone / remote-inclusive communications norm

A workforce spread across three or more time zones cannot rely on a synchronous all-hands to reach everyone. Design the comms rhythm to be legible asynchronously.

**Recorded all-hands with structured async cascade.** Every all-hands is recorded, published within 24 hours, and paired with a written summary within 48 hours. The written summary carries the metrics, the decisions, and links to any resources referenced — it is designed so that an employee who could not attend can catch up in fifteen minutes of reading.

**Rotating meeting times.** If the all-hands runs at 10:00 US-Pacific weekly, the European team joins at 18:00 and the APAC team is asleep. Rotate the live time across cycles — some at US-morning, some at US-evening / EU-morning, some at APAC-friendly — so no single geography carries the recording burden every week.

**Async decision-making default.** The default for a decision that does not require live discussion is a written proposal with a comment window (typically 3–5 business days). This is the mechanism by which decisions get made across time zones without forcing a synchronous meeting at an unfriendly hour. The proposal template names: the decision to be made, the options considered, the recommended option, the decision-owner, the comment window, and the date the decision will be finalised.

**Naming the excluded geography honestly.** No rotation is perfectly fair; one geography always draws the short straw on any given cycle. The healthy pattern is to name it out loud — "this week's all-hands is at a bad hour for APAC; we will run the next one at a friendlier time and APAC's questions will get first slot in the AMA" — rather than pretend the schedule is symmetrical. Acknowledgement costs nothing and it is the difference between a workforce that feels included and a workforce that feels tolerated.

**Cross-time-zone meeting norms.** For meetings that must be synchronous, publish agenda 24 hours in advance, share slides and any pre-read at the same time, and record with intent to publish. The full tool stack — the video platform, the transcription layer, the async-notes discipline — is [chapter 05](./05-remote-hybrid-and-rto-policy.md).

## Decision 7 — The crisis-comms playbook

A crisis is not the moment to be composing your response for the first time. Pre-draft the playbook for the five most common crisis categories.

The categories differ in owner, cadence, and legal-review gate, but they share a common structure: a named internal-comms lead, a first-update deadline measured in minutes or hours, a defined update cadence during the incident, and an after-action review to feed the playbook forward.

| Crisis category | Who owns internal messaging | First update deadline | Update cadence during incident | Cross-reference |
|---|---|---|---|---|
| Production outage / service incident | Incident commander (on-call) → internal-comms lead within 30 min | 30 min from declaration | Every 30–60 min in a named channel until resolved | [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) for incident-response mechanics |
| Security incident / breach | CISO + general counsel jointly; CEO informed immediately | Within 2 hours (delay only for legal review) | Daily written update until contained; heavy legal gate on content | [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/) for the security-incident-response side |
| PR incident (external story, viral complaint) | Head of comms / CEO + general counsel | Same day | Daily until narrative stabilises | External comms out of scope; internal norm only |
| Layoff | CEO + head of people; no delegation | Choreographed to the hour (see mod-107 ch. 06) | Written CEO follow-up within 24 hours; all-hands within 48 hours | [mod-107 chapter 06](../mod-107-performance-promotion-and-offboarding/06-rif-and-layoff-playbook-under-warn.md) |
| Executive departure | CEO personally | Same day if not pre-choreographed | All-hands within 48 hours; written follow-up | [mod-107 chapter 07](../mod-107-performance-promotion-and-offboarding/07-executive-team-offboarding.md) |

**General principles across categories.**

- **Name the owner before the crisis.** The internal-comms lead for each crisis category is a named role, not "whoever is around." Publish the on-call rota for internal comms alongside the engineering on-call rota.
- **Communicate before you have answers.** "We are investigating; we will update in 30 minutes" is a valid first update. Silence in the first hour of a visible incident is the worst possible signal.
- **Separate what is known from what is being investigated.** Every update explicitly labels each fact as `[confirmed]`, `[investigating]`, or `[unknown]`. This is what protects the corporation from a follow-up update contradicting the previous one.
- **Coordinate with external comms without merging channels.** What the corporation says publicly and what it says internally have to be consistent, but the internal version is usually more candid on cause and next steps. The internal-comms lead and the external-comms lead work from the same fact set; the external cadence is out of scope here.
- **After-action review.** Every crisis triggers an after-action review within two weeks, with the outcome documented and shared. This is how the playbook improves cycle over cycle; the incident-management mechanics live in [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/).
- **Dedicated channel per incident.** Spin up a named `#incident-<slug>` channel at the moment the incident is declared. All updates go there in cadence; discussion happens in threads; the operational war-room happens in a separate closed channel. This keeps the workforce-facing feed clean and preserves an auditable timeline for the after-action review.
- **The CEO shows up.** For any crisis category above, the CEO appears in the internal-comms lane personally at least once during the incident — even if the operational owner is elsewhere on the exec team. CEO absence during a visible incident is read as absence full stop, and it is corrosive to trust in a way that is expensive to repair afterwards.

## Concrete example: a Series-B, 200-person B2B SaaS company across three time zones

A hypothetical B2B SaaS company, Series-B, 200 employees. Headquarters in San Francisco (US-Pacific); engineering hub in London (UK); customer-success team distributed across APAC (Sydney and Singapore). Five-person exec team, twenty-eight managers. CEO founder-in-seat. Chief of staff owns comms rhythm operationally; head of people owns the confidential-comms handbook.

**Cadence surface.**

| Instrument | Cadence | Duration | Owner | Channel |
|---|---|---|---|---|
| All-hands | Bi-weekly, alternating Thursday US-morning / Thursday US-evening | 60 min | CEO (agenda: chief of staff) | Zoom, recorded; summary in Notion |
| CEO weekly update | Every Friday | 300 words | CEO | `#ceo-updates` Slack channel |
| Monthly CEO letter | First Monday of the month | 1,000–1,500 words | CEO | Notion long-form; email to all-staff |
| Internal QBR | Once per quarter, week 11 | 90 min | CEO + exec | Zoom + written pack in Notion |
| Skip-level office hours | Monthly per exec | 30-min slots | Each exec | Calendly bookable by any employee |
| Leadership-team retro | Monthly, first Thursday | 90 min | Facilitator (chief of staff) | Closed session |
| AMA | Every all-hands | 10 min live + written follow-up within 1 week | CEO | Slido for submissions; live in all-hands |

**All-hands agenda template.** Opening (5 min); business update against the quarterly plan (10 min); function or theme deep-dive on rotation (15 min); people moments (5 min); CEO AMA on the top-upvoted Slido questions (10 min); wrap and preview of the next all-hands (5 min).

**Announcement taxonomy in use.**

| Announcement type | Channel | Response expectation | Volume budget |
|---|---|---|---|
| `[Info]` — new hires, product launches, customer wins | `#announcements` + weekly digest | Read welcome, no action | Unlimited into digest; 2–3/week into `#announcements` |
| `[Decision]` — new policy, new tool adoption, deadline changes | `#announcements` + email + emoji-ack in-thread | Explicit ack required by stated deadline | 1–2/week soft cap |
| `[Feedback]` — draft proposal open for input | Dedicated Slack channel or Notion doc with comment access | Comment during window (3–5 business days typical) | As needed |

**Cross-time-zone treatment.** All-hands recorded and published within 12 hours; written 3-paragraph summary within 24 hours; rotating meeting time so London joins live for six of twelve annual all-hands and APAC joins live for four. Async decision-making default for anything that does not require live discussion; standard comment window is 4 business days for a company-wide decision, 2 business days for a function-level one.

**Confidential-comms norms encoded in the handbook.** Board decisions are shared with the workforce at the next all-hands (or within 5 business days by written CEO note if the next all-hands is more than a week away). Executive changes follow the mod-107 ch. 07 choreography — direct reports first (in person), affected function same day, workforce at the next all-hands. Layoffs follow the mod-107 ch. 06 playbook — no Slack-broadcast announcement, human conversation first, surviving-workforce all-hands within 24 hours of the last individual conversation. Company is not yet subject to Reg FD (still private), but the handbook flags that MNPI handling will tighten materially at the point of a public offering, referencing [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/).

**Crisis-comms roster.** On-call rota for internal-comms lead published in Slack alongside the engineering on-call rota. For production outages: incident commander notifies internal-comms lead within 30 min; internal-comms lead posts every 30 min in `#incident-live` until resolution. For a security incident: CISO and general counsel co-own; CEO in the loop immediately; workforce update within 2 hours (subject to legal review). For a PR incident: head of marketing and general counsel draft; CEO signs off before internal publication. Layoff and executive-departure playbooks reference mod-107 chapters 06 and 07 directly rather than duplicating the mechanics.

The rhythm above consumes roughly one FTE-day per week of chief-of-staff time on comms production and coordination, three to four hours per month of CEO writing time on the monthly letter, and roughly one hour per exec per month on skip-level office hours. It is boring and predictable, which is again the point — the workforce knows what to expect and knows what a deviation from the rhythm means.

## Ownership boundary

This chapter owns the internal-comms operating rhythm, taxonomy, and crisis playbook as a **culture-and-comms** instrument. It defers to sibling modules on a set of adjacent questions.

- **Operations-function cadence (WBR, QBR, board pack, planning cycle)** is owned by [mod-114](../mod-114-operations-function-design/). The internal-QBR communicated to employees in this chapter and the operating-QBR that drives the business belong to different rhythms — choreographed (same underlying quarter, same underlying metrics) but not merged. Do not conflate them.
- **Board-facing communications and executive-session dynamics** are owned by [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/). This chapter covers what the workforce hears; that module covers what the board hears and what may not be said outside the executive session.
- **Officer-fiduciary-duty constraints on CEO speech** during a live deal, an investigation, or a securities-sensitive window are owned by [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/). This chapter's crisis and confidential-comms guidance assumes a general counsel is in the loop on any communication that touches those constraints.
- **External / press / investor communications** are out of scope for this chapter. Internal-comms and external-comms must be consistent, but the external mechanics — press releases, investor updates, analyst briefings — belong elsewhere.
- **Engineering-org rituals** (sprint reviews, on-call retros, tech-strategy syncs) live in `cto-curriculum`. Do not fold them into the company-wide comms rhythm.
- **GTM-org rituals** (pipeline review, deal review, forecast cadence) live in `startup-product-gtm-curriculum`. Same non-fold rule.

The rule of thumb: if the question is "what does the workforce hear, in what forum, on what cadence," this chapter owns it; if the question is "what does the executive team decide about the business, and in what forum," a sibling module owns it.

## Summary

- Internal comms is a calendared instrument; the workforce reads the cadence, not any single message, and infers whether the corporation is trustworthy on communication.
- Seven decisions to make deliberately: all-hands cadence, executive-comms portfolio, AMA pattern, announcement taxonomy, confidential-comms norm, cross-time-zone norm, crisis playbook.
- All-hands cadence tracks stage: weekly at seed / Series-A, bi-weekly at Series-B, monthly at growth stage. Record every one; publish a written summary within 48 hours; do not skip.
- Executive-comms portfolio: CEO weekly update, monthly written CEO letter, internal QBR, monthly skip-level office hours per exec, monthly leadership-team retro. Each has a defensible cadence; ghostwriting the CEO letter is a category error.
- AMA runs at every all-hands with anonymous submission; the CEO prepares from a chief-of-staff brief; hostile questions are handled by restating charitably, acknowledging what is true, or committing to a written follow-up.
- Announcement taxonomy: `[Info]` / `[Decision]` / `[Feedback]`. Match channel and response expectation to the class; hold a volume budget on decision-required broadcasts.
- Confidential-comms norm encodes: board decisions before all-hands, executive changes before all-hands (see [mod-107 chapter 07](../mod-107-performance-promotion-and-offboarding/07-executive-team-offboarding.md)), layoff choreography (see [mod-107 chapter 06](../mod-107-performance-promotion-and-offboarding/06-rif-and-layoff-playbook-under-warn.md)), MNPI handling for near-public / public corporations (see [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/) and Reg FD, 17 CFR §§ 243.100–243.103).
- Cross-time-zone default: recorded all-hands with written summary, rotating live times, async decision-making with a stated comment window.
- Crisis playbook covers outage, security incident, PR incident, layoff, executive departure — each with a named internal-comms owner and a first-update deadline. Pre-draft; do not compose during the crisis. Incident-response mechanics cross-reference [mod-112](../mod-112-enterprise-risk-insurance-and-compliance/).
- Effectiveness of the comms rhythm is measured through the engagement programme in [chapter 04](./04-engagement-measurement-and-action-planning.md); the tool stack that carries the rhythm is [chapter 05](./05-remote-hybrid-and-rto-policy.md); the values that shape tone (transparency, direct communication) come from [chapter 01](./01-values-behaviours-and-anti-values.md); the confidential-comms norms are documented in the handbook per [chapter 02](./02-employee-handbook-nlrb-compliant-post-stericycle.md).
- Operations-function cadence (WBR, QBR, board pack, planning) belongs to [mod-114](../mod-114-operations-function-design/); board-facing comms and officer-duty constraints belong to [mod-111](../mod-111-corporate-governance-board-operations-and-officer-duties/); external / press / investor comms are out of scope. Choreographed with those rhythms, not merged.
- See [exercise-07](./exercises/exercise-07-internal-communications-operating-rhythm-authoring.md) for the drill.
