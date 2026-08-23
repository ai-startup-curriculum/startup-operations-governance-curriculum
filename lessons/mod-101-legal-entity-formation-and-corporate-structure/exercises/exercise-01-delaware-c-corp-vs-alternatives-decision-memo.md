# Exercise 01 — Delaware C-Corp vs. alternatives decision memo

> Estimated time: **~2 hours** · Related chapter: [01 — Choose the US legal entity](../01-choose-the-us-legal-entity.md)

## Problem statement

You are the incoming COO / GC of an early-stage startup. The three co-founders are one week away from forming an entity. They have asked you a single question: **"Delaware C-Corp, or something else?"** — and they want a signed decision memo before they file anything.

Your job is to produce that memo — for one of the fact patterns below — with a defensible recommendation, the alternatives considered, and the reasoning that would survive a Series-A counsel readback two years from now.

## Fact patterns (pick one)

**Fact pattern A — Standard venture-track SaaS**
- Three technical co-founders. All US persons.
- Product: developer-tooling SaaS for AI infrastructure teams.
- Plan: raise a seed round in ~9 months, Series A in ~24 months.
- HQ: San Francisco, initially remote across CA / WA / NY.
- IP: founders have written pre-formation prototype code; ownership sits with the founders individually today.

**Fact pattern B — Mission-locked climate startup**
- Two co-founders — one climate scientist, one product operator. Both US persons.
- Product: hardware-plus-software system for industrial carbon capture.
- Plan: raise a seed round from climate-focused funds in ~12 months, likely dilutive government grant funding in parallel, Series A in ~30 months.
- Mission commitment: founders want it *legally* binding that the board must weigh climate impact against stockholder value.
- HQ: Boston; a first hire expected in Texas.

**Fact pattern C — Solo-founder bootstrapped consultancy pivoting to product**
- One founder, US person, currently running a self-employed AI consulting practice.
- Wants to keep the consultancy revenue flowing while building a product that may or may not warrant raising outside capital in ~18–24 months.
- Founder wants to pay self-employment tax efficiently in the meantime and use business losses against consulting income.
- HQ: home office in Austin; no employees.

## Requirements

Produce a **2–4 page decision memo** structured as follows.

1. **Recommendation** — one sentence: which entity (jurisdiction and form), full stop.
2. **The four questions** — walk explicitly through the decision framework from [chapter 01](../01-choose-the-us-legal-entity.md):
   - Will this company raise institutional venture capital within 24 months?
   - Does the founder team need pass-through tax treatment right now?
   - Is mission-lock a material commitment the founders want legally binding on the board?
   - Does an S-corp election optimise tax without foreclosing option value?
3. **Alternatives considered** — for each of the three alternatives you did not choose (of DE C-Corp, DE LLC, S-Corp, DE PBC, non-DE Corp), explain why it was rejected in one paragraph each. "Rejected because" should reference substance (VC ineligibility, tax friction, mission-lock, cost of later conversion), not sentiment.
4. **Consequences the founders should understand about the recommended entity** — at minimum: entity-level tax vs. pass-through; QSBS eligibility; expected annual compliance cost (Delaware franchise tax, registered agent, home-state filings); what will need to change if the plan changes.
5. **Cost of getting this wrong** — a specific paragraph on what a later conversion / reincorporation / re-election would cost in time, dollars, and re-execution of equity documents.
6. **Sign-off block** — space for each founder to sign confirming they have read and understood the memo. This memo is the artifact that goes into the corporate record before formation day.

## Starter guidance

- Anchor the recommendation to the *plan* the founders describe, not to a generic "startups usually pick X." If the plan says institutional capital in 24 months, the entity choice is basically decided; the memo is showing your work.
- For fact pattern B, actually read DGCL §§ 362–368 (Delaware Public Benefit Corporation subchapter) before writing. A PBC is a legally distinct commitment; if you recommend it, the memo needs to say what "specific public benefit" you would identify in the charter and how the directors' balancing duty operates.
- For fact pattern C, seriously evaluate the LLC and the S-corp. The venture-track answer is not always right; document why you land where you land.
- Do not invent case studies or "70% of venture-backed startups do X" figures. The memo cites statutes and IRS provisions where it cites anything.
- Where you would need a specific numeric input (franchise-tax estimate for a chosen authorized-share count, expected 409A valuation, expected fund LP mix) that you cannot know, flag the assumption explicitly.

## Acceptance criteria

The memo is acceptable if a Series-A counsel reading it two years later would:

1. Be able to reconstruct the entity-choice reasoning without asking for context.
2. See explicit engagement with each of the four framework questions.
3. See each rejected alternative treated seriously — not dismissed in a sentence.
4. Find the recommendation defensible on the record even if the plan changed after formation (e.g., "the founders' plan at the time was X; the entity choice was correct for that plan; the current situation is Y, and here is the conversion path").
5. Find no invented facts or unattributed claims.

## Deliverable

- `entity-choice-memo.md` (or `.pdf`) — the memo itself, signed by all founders.
- One paragraph of self-critique at the bottom: what part of the recommendation are you least confident about, and what would change your mind?
