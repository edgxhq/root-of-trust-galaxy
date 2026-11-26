---
id: oracle-price-feeds
type: concept
title: "Prices brought in by an oracle network"
description: "Prices from outside the ledger, delivered by an oracle network. The ledger records faithfully what it was told."
status: seed
visibility: public
verified: secondary
level: bridged
tags: []
links:
  - rel: instance-of
    to: level-bridged
  - rel: derived-from
    to: src-cardano-org-2026-05-20-integrations
created: 2026-11-20
updated: 2026-11-20
---

A program on a ledger cannot see the price of anything outside it. An oracle network brings the price in. A
status report of 20 May 2026 lists "Pyth Network pricing oracles" among the integrations live on Cardano.

By the distance test this is the same position as a bridge. If the oracle's operators failed or colluded, the
ledger would record the wrong price just as faithfully as the right one, and could guarantee nothing about it.
That is not a criticism of any oracle. It says where the trust sits.
