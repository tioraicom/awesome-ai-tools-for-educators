# Candidate pool

What was considered for this list, what was verified, and what was left out.

Two things are deliberately absent, and neither is an oversight:

- **Internal scores and per-product rejection notes.** Editorial scoring stays out of a
  public repository. Exclusions below are given as neutral categories, not as judgements
  about named companies.
- **A per-candidate TiorAI URL map.** Capturing a TiorAI link for every candidate would
  produce exactly the backlink list this portfolio's own rules prohibit.

## Sources of candidates

| Source | Role |
|---|---|
| TiorAI's published AI tools catalogue | Read-only, used to shortlist candidates and to confirm product identity. No description or stored URL was carried through |
| Direct knowledge of the category | Used to fill gaps the catalogue does not cover well and to remove products that have since shut down or been absorbed |
| The vendor's own site | The authority for every fact that ships: current name, canonical URL, pricing tier, platform support |

Category assignment, pricing, and platform labels from the catalogue were treated as
*signals*, never as published values. The catalogue's own taxonomy is far too large and too
redundant to publish, so this repository defines its own.

## Pool

| Stage | Count |
|---|---:|
| Candidates considered | 0 |
| Shortlisted after scope filtering | 0 |
| **Published** | **74** |

## Why candidates were dropped

- **It grades without showing its evidence.** The largest exclusion in the marking
  category, and the reason several well-funded products are absent.
- **It is an AI-content detector.** Excluded on accuracy grounds, and because the
  cost of a false positive falls on a student rather than on the buyer.
- **It is an institutional system.** Attendance, timetabling, and student records are
  bought by a school, not chosen by a teacher.
- **It is general productivity software.** A teacher's calendar is everybody's
  calendar; that list already exists.
- **It belongs to the student list.** Study tools were left in
  `awesome-ai-tools-for-students` rather than duplicated here.

## Verification

Every published entry had its official URL resolved over HTTP before release, following
redirects to the canonical destination. 74 distinct external URLs were checked:
61 answered normally, 13 returned a bot-protection or rate-limit
response, and 0 were broken.

A `401`, `403`, `405`, `429`, or `999` was never treated as evidence that a site is dead. Each
was re-probed by a second route and reasoned about rather than acted on automatically. No
entry was removed on the basis of a single failed request.

Time-sensitive facts — pricing tier, whether a free plan still exists, product availability,
renames, acquisitions, shutdowns, platform support — were re-checked against the vendor at
build time regardless of what the catalogue record said.
