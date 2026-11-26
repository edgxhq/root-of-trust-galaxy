---
id: m-ethereum-assets
type: measurement
title: "On Ethereum other assets are programs the ledger runs"
description: "A token is a program that keeps its own balances, run by every node."
status: developing
visibility: public
network: net-ethereum
dimension: dim-assets
value: 2
unit: "step on a three-step scale"
threshold: "what the ledger itself enforces"
as_of: 2026-11-19
verified: main
tags: [assets, ethereum]
links:
  - rel: derived-from
    to: src-ethereum-org-erc20
created: 2026-11-19
updated: 2026-11-19
---

Ethereum's documentation: "If a Smart Contract implements the following methods and events it can be called an
ERC-20 Token Contract and, once deployed, it will be responsible to keep track of the created tokens on
Ethereum." The token's rules are whatever its program says, and every node runs that program, so the ledger
enforces them.
