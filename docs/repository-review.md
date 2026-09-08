# Repository and pattern review

What was looked at before building this list, and what was taken from it. No editorial
content, description, category wording, or dataset was copied from any of these sources.

## Reviewed

| Source | What it is | What it was useful for |
|---|---|---|
| [sindresorhus/awesome](https://github.com/sindresorhus/awesome) — `awesome.md` | The Awesome list quality requirements | Entry format, table-of-contents expectation, licensing guidance, badge rules |
| [GitHub Docs — community profiles](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/about-community-profiles-for-public-repositories) | Platform documentation | The community health file set GitHub actually checks for |
| [GitHub Docs — syntax for issue forms](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms) | Platform documentation | Required keys and element types for `.github/ISSUE_TEMPLATE/*.yml` |
| Established curated lists in this subject area | Community lists with substantial history | Structural patterns that hold up at scale, and the failure modes that do not |

One decision is specific to this repository and worth recording.

AI-content detectors are the product this audience is sold hardest, and they are absent.
That costs the repository the single most searched query a teacher brings to a list like this.

It was still the right call. A detector's output is an accusation, its error rate is not
published in a form anyone can check, and the person who pays for a false positive is a student
with no way to audit it. Recommending one would contradict the rule the rest of the list is
built on. The exclusion is argued in the README rather than left as a gap, so a teacher who
came looking finds a position instead of an oversight.

## What was adopted

**One entry format, without exception.** Every entry takes the same shape:

```text
- **[Name](https://example.com/)** — What it does, in one sentence. `Freemium` `Web`
```

Deviation is what makes a list unscannable and unparseable, and it costs more than it appears
to.

**A contents block that maps one-to-one onto the headings.** Every `##` section appears in
it, every anchor resolves, and the block fits on one screen.

**Per-entry metadata from a closed vocabulary.** Pricing and platform labels mean the same
thing here as in every other TiorAI repository, so they can be relied on rather than read.

**An explicit review date.** Most lists in this space carry no freshness signal at all, so a
reader cannot distinguish a list reviewed last week from one abandoned two years ago.

**A written selection policy.** What qualifies, what does not, how entries are ordered, and a
plain statement that there is no paid placement, sponsorship, or affiliate link.

## What was deliberately not adopted

**Size as a selling point.** Several lists in this space advertise their entry count. A list
nobody can finish reading has not curated anything, and the counts are usually inflated by
dead links nobody has checked.

**Year-branded naming.** `awesome-<topic>-2026` reads as current for a few months and as
abandoned forever afterwards.

**The Awesome badge.** It signifies acceptance into the official Awesome index. This
repository has not been submitted, so displaying it would be a false claim.

**Deep hierarchy.** No `###` subcategories inside the list body. That is the point at which
these lists stop being navigable.

**Emoji as meaning.** Decorative only at best, and inaccessible at worst.
