# Exercise 02 — Certificate of Incorporation & bylaws authoring drill

> Estimated time: **~3 hours** · Related chapter: [02 — Stand up the entity](../02-stand-up-the-entity.md)

## Problem statement

You have decided (from exercise 01) that a Delaware C-Corporation is the right entity for the founding team. It is formation day. Produce the filing-ready **Certificate of Incorporation** and adoption-ready **Bylaws** for the corporation, defensible against a Series-A counsel readback.

You will not merely fill blanks in a template — you will make specific, documented choices for each material decision the two documents embody.

## Requirements

### Part A — Certificate of Incorporation

Produce a Delaware Certificate of Incorporation (COI) suitable for filing with the Delaware Secretary of State. The COI must include, at minimum:

1. **Corporate name** — including a valid Delaware corporate indicator. Confirm the name choice against the Delaware Division of Corporations name search (document that you did so).
2. **Registered office and registered agent** — a Delaware street address and a named registered agent. Choose from a commercial provider (CSC, CT, Cogency, InCorp) and record the reasoning for the choice.
3. **Purpose clause** — the standard general-purpose clause under DGCL § 102(a)(3).
4. **Authorized shares** — total number of shares of common stock and (if applicable) preferred stock the corporation is authorized to issue. Document:
   - The specific number of common shares authorized and why (e.g., accommodating founder issuances, initial option pool, and headroom for a seed round).
   - The specific par value chosen (typically $0.00001 to $0.0001) and its franchise-tax implication under the Assumed Par Value Capital Method.
   - Whether preferred stock is authorized on formation day, and whether it is authorized as "blank-check preferred" under DGCL § 151 with board discretion to designate series.
5. **Director exculpation** — a clause under DGCL § 102(b)(7) limiting director personal liability, with the statutory carve-outs.
6. **Officer exculpation** — if included, a clause under the 2022 DGCL amendment to § 102(b)(7) limiting officer personal liability (narrower scope than director exculpation).
7. **Indemnification enabling clause** — referencing DGCL § 145 and confirming indemnification of directors and officers to the fullest extent permitted by law.
8. **Forum-selection clause** — Delaware Court of Chancery as exclusive forum for internal corporate-affairs disputes, plus a federal-forum clause for Securities Act claims (see *Salzberg v. Sciabacucchi*, 227 A.3d 102 (Del. 2020)).
9. **Incorporator block** — name, address, and signature line for the incorporator.

### Part B — Bylaws

Produce the initial Bylaws for the corporation. The bylaws must address, at minimum:

1. **Offices** — principal executive office and Delaware registered office.
2. **Stockholder meetings** — annual meeting cadence (satisfying DGCL § 211(b)), special-meeting mechanics, notice periods, quorum (typically a majority of outstanding voting shares), voting by proxy.
3. **Stockholder action by written consent** — whether permitted under DGCL § 228, and by what vote threshold.
4. **Board of directors** — number (fixed or a range), how vacancies are filled (DGCL § 223), removal, resignation, and compensation.
5. **Board meetings** — regular and special meetings, notice, telephonic-meeting permission, quorum, and unanimous written consent under DGCL § 141(f).
6. **Committees** — the board's power to create committees (audit, compensation, nominating and governance), and the scope of authority that may be delegated.
7. **Officers** — required and permitted officer positions, appointment by the board, term, and duties (referencing DGCL § 142).
8. **Indemnification** — mandatory indemnification of directors and officers under DGCL § 145 to the fullest extent permitted by law, plus advancement of expenses under an undertaking.
9. **Stock certificates / uncertificated shares** — permit uncertificated shares under DGCL § 158.
10. **Amendment** — bylaw amendment procedure (board and/or stockholder).
11. **Fiscal year** — designated fiscal year.

## Starter guidance

- Do not copy a random template off the internet without reading it. Cooley, Wilson Sonsini, Orrick, Gunderson Dettmer, Fenwick, and Latham & Watkins each publish standard startup formation packages that are widely used; if you use one, cite it and note any choice you made that deviates from the template default.
- For **authorized shares**, run the Delaware franchise-tax math both ways (Authorized Shares Method and Assumed Par Value Capital Method) for a hypothetical formation-day gross-asset value (e.g., $0). Attach the calculation. See the Delaware Division of Corporations franchise-tax calculator: https://corp.delaware.gov/paytaxes/.
- For **director count**, favour a specific reasoning for the range. A single-founder-director on formation day is common; a two-co-founder board is also common; a five-seat board with three vacant is unusual at formation and creates governance questions.
- For **forum selection**, if you choose to include the federal-forum clause for Securities Act claims, cite the Delaware Supreme Court's holding in *Salzberg v. Sciabacucchi*.
- The COI is filed with the Delaware Secretary of State; the bylaws are adopted internally. Confirm which document a specific provision belongs in — some (e.g., indemnification) can appear in both.

## Deliverables

- `certificate-of-incorporation.md` (or `.docx`, `.pdf`) — filing-ready COI.
- `bylaws.md` (or `.docx`, `.pdf`) — adoption-ready bylaws.
- `formation-choices-memo.md` — a 1–2 page memo documenting the material choices in each document, with the reasoning and any statute or precedent cited.
- `authorized-shares-tax-math.md` — the franchise-tax math for your chosen authorized-share count and par value, both methods.

## Acceptance criteria

The package is acceptable if:

1. Every material COI and bylaws choice is *documented* — a reader can reconstruct the reasoning without asking questions.
2. The authorized-share count and par value are defensible under both franchise-tax methods, with the math attached.
3. The COI and bylaws are internally consistent (e.g., the bylaws' authorized-officers list does not exceed roles the COI or DGCL permits; the bylaws' quorum rules do not contradict the COI).
4. Statute citations (DGCL sections) are correct.
5. Nothing is left as `[FILL IN]` or `[TBD]` — every field is populated or explicitly flagged as "N/A on formation day, to be added at [event]" with the event named.
