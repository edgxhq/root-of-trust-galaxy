---
id: m-ethereum-programs
type: measurement
title: "Ethereum runs general programs"
description: "Programs deployed by anyone are run by every node."
status: developing
visibility: public
network: net-ethereum
dimension: dim-programs
value: 2
unit: "step on a three-step scale"
threshold: "what the ledger itself can run"
as_of: 2026-11-19
verified: main
tags: [programs, ethereum]
links:
  - rel: derived-from
    to: src-ethereum-org-smart-contracts
  - rel: derived-from
    to: src-ethereum-rpc
created: 2026-11-19
updated: 2026-11-19
---

Ethereum's documentation: "A 'smart contract' is simply a program that runs on the Ethereum blockchain."
Programs are run by every node, within a limit on the work one block may hold. Read from a public node on 19
November 2026, that limit was 60,000,000 units of gas.
