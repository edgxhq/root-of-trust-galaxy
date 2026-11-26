---
id: dim-node-software
type: dimension
title: "Whose software they run"
description: "The independent implementations of the node that are actually producing blocks."
status: developing
visibility: public
kind: accident
question: "Whose software they run?"
short: SOFTWARE
order: 2
tags: [method, node-software]
links:
  - rel: part-of
    to: method-shortest-stave
created: 2026-11-19
updated: 2026-11-26
---

The independent implementations of the node that are actually producing blocks, counted the way every other link
is: the smallest number that together carry more than half of block production. An implementation that exists
but makes no blocks does not count yet. A fork of the main implementation shares most of its bugs, so lineages
are counted, not names.

A second implementation raises the count only when it carries enough stake or hash power that no single one has
a majority. Until then a bug in the main one still reaches most of the network.

This link is different in kind from most of the others. A count of 1 here does not mean one party is in charge:
an implementation is written and reviewed by many people, and who can change it is a separate link ([[dim-merge-rights]]).
It means one fault could reach most of the network at once. That has happened, on Cardano among others, and the usual result
is a stall or a split that is repaired, not a theft. So it is counted, and it is labelled as a risk "by accident",
apart from the links a small group could take "by agreement". See [[method-shortest-stave]].
