# Exercise 04 — Foreign-qualification trigger analysis across states

> Estimated time: **~2 hours** · Related chapter: [04 — Foreign qualification across states](../04-foreign-qualification-across-states.md)

## Problem statement

You are the corporate secretary of a Delaware C-Corporation that has grown quickly to a remote-first workforce spread across the United States. The board has asked you: **"Where do we need to be foreign-qualified today, and what is the penalty exposure if we skip any of them?"**

Your job is to produce a state-by-state analysis, a qualification-priority ranking, and a cost model.

## Fact pattern

Delaware C-Corporation, formed 18 months ago. Headquartered in San Francisco, California. Current footprint:

| State | Nature of presence                                                            |
| ----- | ----------------------------------------------------------------------------- |
| CA    | HQ, 12 employees, office lease.                                               |
| NY    | 3 remote employees (Brooklyn, Manhattan, Buffalo). No office.                 |
| TX    | 2 remote employees (Austin, Houston). No office.                              |
| WA    | 4 remote employees (Seattle). No office.                                      |
| MA    | 1 remote employee (Cambridge). No office.                                     |
| CO    | 1 remote employee (Denver). No office.                                        |
| IL    | 1 remote employee (Chicago). No office.                                       |
| FL    | 1 remote employee (Miami). No office. Additionally: a small in-state customer conference the company has attended for the last three years, staffed by two salespeople for four days each visit. |
| NV    | No employees. Corporate finance workshop held once in Las Vegas last year. Board dinner. |
| NJ    | No employees. One paying customer with an ongoing SaaS subscription paid to the corporation's out-of-state bank account. |

The corporation is currently qualified to do business only in Delaware (its state of incorporation). It has never registered as a foreign corporation anywhere else.

## Requirements

Produce the following.

### Part A — State-by-state qualification analysis

For each of the ten jurisdictions above, produce a row in a matrix with:

1. **Qualification required?** — Yes / No / Grey.
2. **Trigger** — the specific fact or facts that support your conclusion (e.g., "12 in-state employees plus office lease" or "no continuous presence, single trade-show attendance likely under safe-harbour").
3. **Statutory citation** — the state's foreign-qualification statute and any safe-harbour list (e.g., Cal. Corp. Code § 191(c); N.Y. B.C.L. § 1301; the state-specific equivalent). Cite the specific subsection where possible.
4. **Penalty exposure if not qualified** — cite the state's penalty statute (e.g., Cal. Corp. Code § 2203; N.Y. B.C.L. § 1312; equivalents). Quantify where possible.
5. **Estimated first-year cost of qualifying** — filing fees, first-year franchise / entity tax, registered-agent fee, and any state-specific requirement (e.g., New York's post-formation publication requirement).

### Part B — Qualification-priority ranking

Rank the "Yes" states in the order the corporation should qualify. Consider (a) size of penalty exposure, (b) likelihood a lawsuit or contract enforcement would land in that state, (c) diligence sensitivity (a Series-A candidate that is unqualified in its HQ state is a bigger red flag than an unqualified single-remote-employee state), and (d) speed / cost of qualification.

### Part C — Grey-area recommendation

For each "Grey" jurisdiction, write a one-paragraph recommendation: qualify anyway (belt-and-suspenders), monitor and re-evaluate at a specific trigger, or take the "safe-harbour" position and document the analysis. Name the trigger for re-evaluation.

### Part D — Cost model

A single spreadsheet or table summarising:

- **First-year cost of full qualification** across every "Yes" state — filing fees + first-year franchise / entity tax + first-year registered-agent fees + any state-specific one-time costs. Provide a total.
- **Annual recurring cost** — ongoing franchise / entity taxes + annual-report fees + registered-agent renewals.
- **Cost of consolidating registered-agent representation** with one commercial provider (CSC, CT, Cogency, InCorp) vs. state-by-state agents.

### Part E — Compliance calendar addendum

For every state you recommend qualifying in, extend the corporation's existing compliance calendar with:

- The state's annual-report / statement-of-information cadence.
- The state's franchise-tax or entity-tax cadence.
- Registered-agent renewal.
- Any state-specific first-year filings (e.g., California SI-550 within 90 days of qualification).

## Starter guidance

- The single most useful primary source per state is the Secretary of State's business-services website (search: `[state] Secretary of State foreign corporation qualification`) plus the state's business-corporation code. Cite the actual statute; do not rely on secondary sources for penalty amounts without confirming against the state code.
- The safe-harbour lists in each state's foreign-qualification statute are your friend. Read Cal. Corp. Code § 191(c) and its equivalent in each state before flagging borderline items as "qualification required."
- Employees generally mean qualification. Payroll registration in the state's employment-tax system typically requires the entity to exist as a legally-qualified entity in the state; a PEO / HRIS integration will typically block payroll for an unregistered state.
- New York has an unusual **publication requirement** for newly-qualified foreign corporations (six weeks in two newspapers in the county of the designated in-state office). Include the cost in your model. <!-- needs-research: verify the current publication requirement under N.Y. B.C.L. § 1304 and typical NYC-county publication costs; the requirement has been historically significant. -->
- California imposes an $800 minimum franchise tax per year for corporations, payable to the Franchise Tax Board (Form 100). Include it in the first-year cost.
- Use `<!-- needs-research: ... -->` for any per-state fee you cannot confirm from a primary source before publication.

## Deliverables

- `qualification-analysis.md` — the state-by-state matrix (Parts A + C).
- `qualification-priority.md` — the priority ranking with reasoning (Part B).
- `qualification-cost-model.md` (or `.xlsx`, `.csv`) — the cost model (Part D).
- `compliance-calendar-addendum.md` — the calendar extension (Part E).

## Acceptance criteria

The analysis is acceptable if:

1. Every state has a defensible Yes / No / Grey answer with statutory citation.
2. Every penalty exposure cites the state's actual penalty statute.
3. The priority ranking has explicit reasoning, not just "big states first."
4. The cost model is a real number the CFO can approve against, not a placeholder.
5. Grey-area analyses name a specific trigger for re-evaluation.
6. Compliance-calendar entries have owners, cadence, and reminder-lead-time.
