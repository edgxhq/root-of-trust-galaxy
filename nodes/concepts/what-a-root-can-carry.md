---
id: what-a-root-can-carry
type: concept
title: "What can be built on a root"
description: "How safe a root is and how much it can do are different questions. This is the second one."
status: developing
visibility: public
tags: [method, capability]
links:
  - rel: related
    to: method-shortest-stave
    note: "the first question: how safe"
  - rel: related
    to: distance-from-the-root
    note: "what a root cannot do is built at a distance"
created: 2026-11-19
updated: 2026-11-20
---

The shortest-stave test asks how safe a root is. It says nothing about how much the root can do. A ledger can
be very hard to capture and still offer one service.

Three things are recorded for each root: whether it can run programs, whether it can carry assets other than
its own coin, and how it is built to carry more. The first two decide which type of root it is: see
[[class-general]], [[class-built-in]] and [[class-money]].

Two cautions. This is not a ranking of worth: a narrow root can be the right design, and more features mean
more that can fail. And it does not feed the score: a root's safety is still its shortest stave.

Capability and distance are linked. What a root cannot do itself gets built somewhere else, and whatever is
built somewhere else is reached through a bridge or another ledger, at a distance from the root. See
[[distance-from-the-root]].
