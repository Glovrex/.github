<div align="center">

<img src="https://github.com/TraceFold/tracefold/releases/download/brand-assets/banner.png" alt="" width="900">

# glovrex

*provenance before the fact*

**Undo is a feature. Reversibility is a property.**

<p>
<a href="https://github.com/TraceFold/tracefold"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/tracefold-ece7da?style=for-the-badge&labelColor=ece7da&logo=github&logoColor=0b0a09"><img alt="tracefold" src="https://img.shields.io/badge/tracefold-0b0a09?style=for-the-badge&labelColor=0b0a09&logo=github&logoColor=ece7da"></picture></a>
<a href="https://glovrex.com"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/field%20notes-ece7da?style=for-the-badge&labelColor=ece7da"><img alt="field notes" src="https://img.shields.io/badge/field%20notes-0b0a09?style=for-the-badge&labelColor=0b0a09"></picture></a>
<a href="#what-we-do-not-claim"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/what%20we%20refuse%20to%20claim-ece7da?style=for-the-badge&labelColor=ece7da"><img alt="what we refuse to claim" src="https://img.shields.io/badge/what%20we%20refuse%20to%20claim-0b0a09?style=for-the-badge&labelColor=0b0a09"></picture></a>
</p>

</div>

---

> Software that changes something should be able to say what it changed, put it back, and
> hand you proof — without asking you to take its word for any of the three.

Most systems record what happened after the fact. A log is a claim by the thing being
audited, and a claim by the audited party is the one kind of evidence an auditor cannot
use. We work one step earlier: hold the inverse **before** the change lands, and make the
result checkable by someone who trusts nobody involved.

## What is here

**[tracefold](https://github.com/TraceFold/tracefold)** — the substrate. A change is held
with a checked inverse before it is applied, and every verdict becomes a receipt a third
party can verify offline, with no network and no trust in whoever issued it. Rust, single
binary, Apache-2.0.

## What we do not claim

| | |
|:--|:--|
| **Not every change is reversible** | Where an inverse cannot be constructed, that is an input to the decision, not a footnote. The system refuses rather than pretends |
| **A policy is not an intent** | The tool checks that a change satisfies the rule it was given. Whether that rule was the right one to write is a question no verifier can answer |
| **This is not finished** | It is under adversarial audit now, and the results are published whether they flatter us or not — see below |

## How the work is checked

Someone is paid attention to break it, in rounds. Each round reports the high-severity
holes it found; each repair is re-attacked in the round after.

| round | 8 | 9 | 10 | 11 | 12 | 13 |
|:--|--:|--:|--:|--:|--:|--:|
| **holes found** | 4 | 4 | 1 | 2 | 2 | 3 |

It goes up as well as down. A number that only ever improves is a number nobody is really
testing, so the rounds where it climbed sit on the table with the rest.


## Contact

[glovrex.com](https://glovrex.com)
