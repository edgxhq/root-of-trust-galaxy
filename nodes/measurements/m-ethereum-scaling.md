---
id: m-ethereum-scaling
type: measurement
title: "Ethereum raises its root a little at a time and carries more on networks beside it"
description: "The limit on a block can be moved by the makers of blocks. Most growth is meant to happen on layer-two networks that post their data to Ethereum."
status: developing
visibility: public
network: net-ethereum
dimension: dim-scaling
summary: "A limit that can be raised; rollups beside it"
facets:
  in_root: "A limit on the work in each block, which the makers of blocks can move a little with each block."
  beside: "Layer-two networks: rollups run transactions outside Ethereum and post the data to it."
  building: "Not written up here."
unit: "a description"
threshold: "the design as its own documents describe it"
as_of: 2026-11-20
verified: main
tags: [scaling, ethereum]
links:
  - rel: derived-from
    to: src-eip-1559
  - rel: derived-from
    to: src-ethereum-rpc
  - rel: derived-from
    to: src-ethereum-org-scaling
created: 2026-11-20
updated: 2026-11-20
---

In the root: the limit on work in a block was 60,000,000 units of gas when read on 19 November 2026, and the
rules let each block move it by less than a 1,024th.

Beside the root, in its documentation's words: "Layer 2 is a collective term for solutions designed to help
scale your application by handling transactions off the Ethereum Mainnet (layer 1) while taking advantage of
the robust decentralized security model of Mainnet." "Rollups perform transaction execution outside layer 1
and then the data is posted to layer 1 where consensus is reached." How much of the root's guarantee reaches a
given rollup varies, and is a question of distance.

What is being built to carry more has not been written up here.
