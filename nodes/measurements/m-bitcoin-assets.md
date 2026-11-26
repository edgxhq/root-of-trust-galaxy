---
id: m-bitcoin-assets
type: measurement
title: "Tokens on Bitcoin are a convention read by outside software"
description: "Bitcoin tracks one asset. Tokens are written into transactions and interpreted by separate software."
status: developing
visibility: public
network: net-bitcoin
dimension: dim-assets
value: 1
unit: "step on a three-step scale"
threshold: "what the ledger itself enforces"
as_of: 2026-11-19
verified: main
tags: [assets, bitcoin]
links:
  - rel: derived-from
    to: src-ordinals-docs
created: 2026-11-19
updated: 2026-11-19
---

Bitcoin's ledger tracks one asset. Tokens exist on it by convention. The Runes documentation says "Rune
protocol messages, called runestones, are stored in Bitcoin transaction outputs", and the same handbook says
ordinal theory "can be used without any changes to the Bitcoin network".

So the node records the data, and separate indexing software reads it and works out who owns what. The root
guarantees that the data was recorded and in what order. It does not check the token's rules.
