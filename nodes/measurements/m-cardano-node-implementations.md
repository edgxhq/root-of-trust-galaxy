---
id: m-cardano-node-implementations
type: measurement
title: "Five node implementations have made blocks on Cardano's mainnet"
description: "By Intersect's count on 22 November 2026, five node implementations have produced blocks on Cardano's mainnet. One of them still makes nearly all the blocks, so the count for the link stays at 1."
status: developing
visibility: public
network: net-cardano
dimension: dim-node-software
scored: false
value: 5
unit: "node implementations that have made blocks on mainnet"
threshold: "at least one block on mainnet"
summary: "5 have made blocks on mainnet"
as_of: 2026-11-22
verified: main
tags: [node-software, cardano]
links:
  - rel: derived-from
    to: src-intersect-weekly-update-138
  - rel: related
    to: m-cardano-node-software
    note: "the count for the link: how many implementations would have to share a fault to reach more than half of block production"
  - rel: related
    to: m-cardano-node-software-planned
    note: "two of the five, Amaru and Dingo, count as work that is close"
created: 2026-11-25
updated: 2026-11-25
---

Context for the node-software link, not part of the score. Intersect's weekly update of 22 November 2026, read
on 24 November, says: "Five node implementations have now produced blocks on mainnet: cardano-node, Amaru, Dingo,
cardano-bean and TSUNAGI."

This says how many implementations exist and have made a block. It does not say how block production is shared
between them. The link asks how many implementations would have to share a fault to reach more than half of block
production. That is still 1, because cardano-node makes nearly all of the blocks. Two of the others, Amaru and
Dingo, pass the test for work that is close, and would lift the count to 2 as they make more of the blocks.
