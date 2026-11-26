---
id: dim-programs
type: dimension
title: "Can it run programs"
description: "Whether the root itself can run application logic, and how general that logic can be."
status: developing
visibility: public
group: capability
scale: steps
steps: ["Transfers only", "Limited scripts or built-in functions", "General programs"]
steps_short: ["transfers only", "limited", "general"]
question: "Can it run programs?"
short: PROGRAMS
order: 1
tags: [method, capability]
links:
  - rel: part-of
    to: what-a-root-can-carry
created: 2026-11-19
updated: 2026-11-19
---

Whether the root itself can run application logic. Three steps: transfers only; limited scripts or a fixed set
of built-in functions; general programs that anyone can deploy.

This is not a measure of safety. A root that runs fewer kinds of program has less that can go wrong. It is a
measure of how much can be built on the root itself. What cannot be built there has to be built somewhere
else, and reaching it means a bridge or another ledger: see [[distance-from-the-root]].
