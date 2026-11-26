---
id: dim-scaling
type: dimension
title: "How it is built to carry more"
description: "Where a root's design puts extra work: inside the root, beside it and settled on it, or in something still being built. Described, not scored."
status: developing
visibility: public
group: capability
scale: words
facets:
  - key: in_root
    label: "In the root itself"
  - key: beside
    label: "Beside the root, settled on it"
  - key: building
    label: "Being built"
question: "How is it built to carry more?"
short: SCALING
order: 3
tags: [method, capability]
links:
  - rel: part-of
    to: what-a-root-can-carry
  - rel: related
    to: distance-from-the-root
    note: "work done beside a root sits at a distance from it"
created: 2026-11-20
updated: 2026-11-20
---

How a root is designed to carry more than it does today. This is described in words, in three places, and it
is not scored.

- *In the root itself.* What the ledger does to carry more on its own: checking transactions side by side,
  larger blocks, a limit that can be raised.
- *Beside the root, settled on it.* Work done off the ledger by a group or a second network that settles on
  the root. By the distance test this work is "rooted" at best: see [[distance-from-the-root]].
- *Being built.* Work that is public and under way, with how far it has got.

**Why there is no figure for transactions a second.** A transaction on one ledger is not the same amount of
work as a transaction on another. One may be a single payment. Another may pay hundreds of people, move
several assets and run a program. Cardano's own proposal for more capacity says: "TPS is not an appropriate
metric", because it "does not account for transaction size or computational complexity, making systems with
smaller transactions appear 'faster' while providing less utility". So no such figure is given here for any
network.

**Why there is no ranking either.** The choices trade against safety. A root that carries more itself asks
more of the machines that run it, which shows up in who can host it. A root that stays small pushes work
outward, to a distance. Which is right depends on what the root is for.

Where an entry says "not written up here", that is this research's gap and an open contribution.
