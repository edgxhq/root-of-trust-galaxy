---
id: m-cardano-target-pools
type: measurement
title: "Cardano's protocol aims for 500 pools of equal size"
description: "Cardano's protocol aims for 500 pools of equal size."
status: developing
visibility: public
network: net-cardano
dimension: dim-block-production
value: 500
unit: "pools (the protocol's target, k)"
threshold: "protocol parameter at epoch 668"
scored: false
as_of: 2026-11-19
verified: main
tags: [block-production, cardano]
links:
  - rel: derived-from
    to: src-koios
created: 2026-11-19
updated: 2026-11-19
---

The parameter k is 500. A pool's rewards stop growing at about 78 million ADA, and all 21.5 billion ADA of active
stake would fit in about 276 pools of that size. No governance action has proposed changing k. Context, not part
of the score.
