---
id: m-bitcoin-scaling
type: measurement
title: "Bitcoin keeps its root small on purpose and carries more in channels beside it"
description: "The size of a block is fixed by the consensus rules. Payments beyond that are made in channels and settled on the ledger."
status: developing
visibility: public
network: net-bitcoin
dimension: dim-scaling
summary: "Small on purpose; channels beside it"
facets:
  in_root: "Kept small on purpose. The size of a block is fixed by the consensus rules."
  beside: "Lightning: payments through a network of channels, each opened and closed on Bitcoin."
  building: "Not written up here."
unit: "a description"
threshold: "the design as its own documents describe it"
as_of: 2026-11-20
verified: main
tags: [scaling, bitcoin]
links:
  - rel: derived-from
    to: src-bip-0141
  - rel: derived-from
    to: src-lightning-bolts
created: 2026-11-20
updated: 2026-11-20
---

In the root: "The new rule is block weight ≤ 4,000,000." The limit is part of the consensus rules, and keeping
it there is a choice: a small block is one that many people can check.

Beside the root: "Lightning is a protocol for making fast payments with Bitcoin using a network of channels."

What is being built to carry more has not been written up here.
