---
id: m-cardano-block-production
type: measurement
title: "Between 14 and 56 operators hold half of Cardano's block production"
description: "Between 14 and 56 operators hold half of Cardano's block production."
status: developing
visibility: public
network: net-cardano
dimension: dim-block-production
value: 14
value_hi: 56
unit: "operator groups"
threshold: "more than half of stake (Koios labels) or of blocks (Edinburgh index)"
as_of: 2026-11-19
verified: main
tags: [block-production, cardano]
links:
  - rel: derived-from
    to: src-koios
  - rel: derived-from
    to: src-edi
created: 2026-11-19
updated: 2026-11-19
---

Grouping pools by the operator labels Koios keeps, 14 groups held more than half of active stake on 19 November
2026 (6 held a third, 38 held two thirds). The largest were Coinbase 12.1%, Figment 5.7%, Chuck Bux 5.4% and
AdaLite 4.8%.

The Edinburgh Decentralisation Index, grouping by its own method, counted 56 entities for more than half of block
production on 2 July 2026, out of 804 seen.

The two figures differ because of how pools are grouped, not because of the date. Both are kept: the lower one
is the more cautious.
