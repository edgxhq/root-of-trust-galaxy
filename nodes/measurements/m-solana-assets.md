---
id: m-solana-assets
type: measurement
title: "On Solana other assets are handled by programs on the ledger"
description: "Tokens are kept by a shared token program that every validator runs."
status: developing
visibility: public
network: net-solana
dimension: dim-assets
value: 2
unit: "step on a three-step scale"
threshold: "what the ledger itself enforces"
as_of: 2026-11-19
verified: main
tags: [assets, solana]
links:
  - rel: derived-from
    to: src-solana-docs
  - rel: derived-from
    to: src-solana-rpc
created: 2026-11-19
updated: 2026-11-19
---

Solana's documentation: "The Token Program contains all the instruction logic for interacting with tokens on
the network (both fungible and non-fungible)." Read from the network's RPC on 19 November 2026, both token
programs are deployed, executable accounts.
