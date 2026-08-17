# Glovrex

A lab working on one question: when software changes something, can the change be undone,
and can a stranger check that it was?

## What is here

**[Tracefold](https://github.com/TraceFold/tracefold)** — the substrate. A change is held
with a checked inverse before it lands, and every verdict becomes a receipt a third party
can verify offline, with no network and no trust in whoever issued it.

## What we do not claim

- Not that every change is reversible. Where an inverse cannot be built, that fact is an
  input to the decision, and it is written down rather than smoothed over.
- Not that a policy expresses anyone's intent. The tool checks that a change satisfies the
  rule, not that the rule was the right one to write.
- Not that this is finished. It is under adversarial audit, and the results of that audit
  are published whether they are good or not.

## How the work is checked

Someone is paid attention to break it, in rounds. Each round reports the high-severity
holes it found; each repair is re-attacked in the next round. The count so far, by round:

| round | 8 | 9 | 10 | 11 | 12 | 13 |
|---|--:|--:|--:|--:|--:|--:|
| high-severity holes found | 4 | 4 | 1 | 2 | 2 | 3 |

It goes up as well as down. That is the point of publishing it — a number that only ever
improves is a number nobody is really testing.

## Contact

mahirhir@glovrex.com · [glovrex.com](https://glovrex.com)
