---
id: m-bitcoin-block-production
type: measurement
title: "Three mining pools make more than half of Bitcoin's blocks"
description: "Three mining pools make more than half of Bitcoin's blocks."
status: developing
visibility: public
network: net-bitcoin
dimension: dim-block-production
value: 3
unit: "mining pools"
threshold: "more than half of blocks"
as_of: 2026-11-19
verified: main
tags: [block-production, bitcoin]
links:
  - rel: derived-from
    to: src-mempool-space
  - rel: derived-from
    to: src-edi
created: 2026-11-19
updated: 2026-11-19
---

Over the year to 19 November 2026, Foundry USA made 27.9% of blocks, AntPool 18.3% and F2Pool 13.1%: 59.3%
together. Over the last month the same three made 62.7%. The Edinburgh index gave the same count of three on 3 May
2026.

A pool coordinates many miners, and miners can move to another pool, so this is concentration of who assembles
blocks, not of who owns the machines.
