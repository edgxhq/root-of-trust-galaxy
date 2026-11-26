---
id: public-root-of-trust
type: concept
title: "Public root of trust"
description: "A root of trust that nobody owns: anyone can check it, no one can quietly change it, and it maintains itself."
status: developing
visibility: public
tags: [lineage]
links:
  - rel: refines
    to: root-of-trust
  - rel: related
    to: method-shortest-stave
    note: "how hard it is to capture"
  - rel: related
    to: distance-from-the-root
    note: "how everything else relates to it"
created: 2026-11-19
updated: 2026-11-19
---

A public root of trust is a ledger that can serve as a root without belonging to anyone. Three properties
set it apart from the older kinds.

- **Anyone can check it.** The record and the rules are open.
- **No small group can change it.** Every link that could be captured is spread across many independent
parties. See [[method-shortest-stave]].
- **It maintains itself.** Changes to its rules and payment for its upkeep are decided by its own recorded
process, not by a company or a foundation standing outside it.

"Self-contained, self-evolving and as decentralised as possible" is the short form. The last property is
what lets a root survive a threat nobody planned for.

The claim that follows is modest: there should be one such root for a given set of facts, and everything
connected to it should say how far from it it stands. See [[distance-from-the-root]]. It is not a claim
that other ledgers have no value or that bridges should go.
