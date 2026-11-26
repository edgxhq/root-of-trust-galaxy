---
id: ins-midnight-pools-projection
type: insight
title: "If Cardano's pools held all of Midnight's seats, about twelve operators would make most of its blocks"
description: "A projection, not a measurement: Midnight's 130 seats filled from Cardano's live stake by the Partner Chains Toolkit's own rule. No network of Midnight's runs this today."
status: developing
visibility: public
verified: main
confidence: medium
tags: [midnight, block-production]
links:
  - rel: related
    to: m-midnight-block-production
    note: "today's count, beside which this projection sits"
  - rel: related
    to: m-cardano-block-production
    note: "the stake it is drawn from"
  - rel: derived-from
    to: src-koios
  - rel: derived-from
    to: src-midnight-rpc
  - rel: derived-from
    to: src-partner-chains-ariadne-v2
created: 2026-11-24
updated: 2026-11-24
---

**A projection, not a measurement.** Midnight's published plan is for Cardano's stake pools to make its blocks, in a
share that is a setting. On 24 November 2026 no network of Midnight's did: read from its own endpoint, its committee
had 130 seats, all permissioned, and no pool was registered, on mainnet or on its Preview test network.

This asks what its block-production link would count if every seat went to Cardano's pools. It takes every
registered Cardano pool with stake as Koios listed them on 24 November 2026 (2,660 pools in 1,954 operator groups) as
candidates, and fills Midnight's 130 seats by the Partner Chains Toolkit's own rule: each pool gets the whole number
of seats its stake is due, and the rest are drawn by weight. Over 2,000 draws, the smallest group of operators holding
more than half of the seats was 12 at the median (9 to 16 in nine draws out of ten), or 49 pools (43 to 55). On the
same data, Cardano's own stake gives 14 groups.

It assumes every pool registers, the most favourable case; fewer would leave it more concentrated. Today's count is 7
of 13 permissioned candidates ([[m-midnight-block-production]]). The two are counted in different units, candidates
today and operator groups in the projection, so the comparison is rough.
