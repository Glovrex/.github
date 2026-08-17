<div align="center">

<img src="https://raw.githubusercontent.com/TraceFold/tracefold/main/assets/brand/hero-glovrex.png" alt="Glovrex" width="820">

<br>

**[Tracefold](https://github.com/TraceFold/tracefold)** &nbsp;·&nbsp;
[Field notes](https://glovrex.com) &nbsp;·&nbsp;
[What we refuse to claim](#what-we-do-not-claim) &nbsp;·&nbsp;
[The audit](#how-the-work-is-checked) &nbsp;·&nbsp;
[Contact](#contact)

</div>

---

> Software that changes something should be able to say what it changed, put it back, and
> hand you proof — without asking you to take its word for any of the three.

Most systems record what happened after the fact. A log is a claim by the thing being
audited, and a claim by the audited party is the one kind of evidence an auditor cannot
use. We work one step earlier: hold the inverse **before** the change lands, and make the
result checkable by someone who trusts nobody involved.

## What is here

**[Tracefold](https://github.com/TraceFold/tracefold)** — the substrate. A change is held
with a checked inverse before it is applied, and every verdict becomes a receipt a third
party can verify offline, with no network and no trust in whoever issued it. Rust, single
binary, Apache-2.0.

## What we do not claim

Three things, said here so nobody has to discover them later.

**Not every change is reversible.** Where an inverse cannot be constructed, that is an
input to the decision, not a footnote. The system refuses rather than pretends.

**A policy is not an intent.** The tool checks that a change satisfies the rule it was
given. Whether that rule was the right one to write is a question no verifier can answer,
and we do not market as though it could.

**This is not finished.** It is under adversarial audit right now, and the results of that
audit are published whether they flatter us or not — which brings us to the next section.

## How the work is checked

Someone is paid attention to break it, in rounds. Each round reports the high-severity
holes it found; each repair is re-attacked in the round after. What that has produced:

| round | 8 | 9 | 10 | 11 | 12 | 13 |
|:--|--:|--:|--:|--:|--:|--:|
| **holes found** | 4 | 4 | 1 | 2 | 2 | 3 |

It goes up as well as down. A number that only ever improves is a number nobody is really
testing, so the rounds where it climbed are on the table with the rest.

## How we work

Every claim carries its own denominator. A result says what it measured, under what
conditions, how many times, and what it did not look at. Where something is unproven it is
labelled unproven and stays that way until it is not. The limits ship beside the features,
and they ship first.

## Contact

mahirhir@glovrex.com &nbsp;·&nbsp; [glovrex.com](https://glovrex.com)
