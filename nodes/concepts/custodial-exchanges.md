---
id: custodial-exchanges
type: concept
title: "Coins held for you by an exchange"
description: "A balance on an exchange is the exchange's record, not the ledger's."
status: seed
visibility: public
verified: secondary
level: unrooted
tags: []
links:
  - rel: instance-of
    to: level-unrooted
  - rel: derived-from
    to: src-defillama-cardano
created: 2026-11-20
updated: 2026-11-20
---

DefiLlama counts centralised exchanges among the largest holders of value on Cardano. Many people first hold
ADA this way.

A balance on an exchange is the exchange's own record, not the ledger's. If the exchange failed, the root
would guarantee nothing about it, however the coins are held behind the scenes. That is "unrooted" in this
research's terms. Moving the coins to a wallet of one's own puts them back on the root.
