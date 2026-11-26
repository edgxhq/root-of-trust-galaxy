---
id: m-cardano-pools-producing
type: measurement
title: "939 stake pools made blocks in one epoch, down from 1,134 in July 2022"
description: "939 stake pools made at least one block in epoch 667, in November 2026, down from 1,134 in epoch 350, in July 2022. Both are counted the same way from on-chain block records."
status: developing
visibility: public
network: net-cardano
dimension: dim-block-production
value: 939
unit: "pools that made a block in the epoch"
threshold: "epoch 667"
scored: false
as_of: 2026-11-18
verified: main
tags: [block-production, cardano]
links:
  - rel: derived-from
    to: src-koios
created: 2026-11-19
updated: 2026-11-26
---

In epoch 667, from 10 to 15 November 2026, 939 pools made at least one block, out of 2,883 registered. This is a
count of producers, not of how few could control production, so it is context and not part of the score.

How it is counted: every block of the epoch in Koios's block records, grouped by the pool that made it. Counted again
that way on 26 November 2026: 21,517 blocks, from 939 pools.

## History

- Epoch 350, from 9 to 14 July 2022: 1,134 pools made at least one block, from 20,958 blocks. Counted the same way on
  26 November 2026.
