---
id: m-solana-block-production
type: measurement
title: "Between 30 and 39 operators hold more than half of Solana's stake"
description: "Grouped by who runs them, as far as the network's own records show, 30 operators hold more than half of Solana's stake. Counted one validator at a time, 39 do."
status: developing
visibility: public
network: net-solana
dimension: dim-block-production
value: 30
value_hi: 39
unit: "operator groups"
threshold: "more than half of active stake"
as_of: 2026-11-21
verified: main
tags: [block-production, solana]
links:
  - rel: derived-from
    to: src-solana-rpc
  - rel: derived-from
    to: src-validators-solutions
created: 2026-11-19
updated: 2026-11-21
---

Read from the network's own records on 21 November 2026: 685 validators with stake. One validator at a time, the
largest 39 hold more than half of active stake.

This link counts validators under one operator once, where that can be known, as it counts Cardano's stake pools.
Grouped that way, 30 operators hold more than half (14 hold a third, 59 hold two thirds). Validators are joined
when they publish the same name, website or Keybase name; when they share a withdraw authority, the key that
controls a validator's earnings; or when one holder owns at least 90% of the stake on each. The validator named
Bybit Staking shares its withdraw authority with the one named P2P.org, so P2P.org's validators and Bybit's count
once. Seven holders each own nearly all the stake on two large validators that publish no name, and each pair
counts once.

The true number may be lower. 33 of the largest 60 validators publish no name, and 28 of those keep all their
rewards (100% commission), so their stake is placed there by arrangement, not drawn by what they pay. This research
could not tie them to one another beyond the pairs above.

A separate tracker counted 17 validators for a third on 18 November; this read gives 18.

## History

- 19 November 2026: 39, counted one validator at a time (659 validators).
