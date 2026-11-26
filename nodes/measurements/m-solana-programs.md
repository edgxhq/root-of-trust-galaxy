---
id: m-solana-programs
type: measurement
title: "Solana runs general programs"
description: "Programs deployed by anyone are run by every validator."
status: developing
visibility: public
network: net-solana
dimension: dim-programs
value: 2
unit: "step on a three-step scale"
threshold: "what the ledger itself can run"
as_of: 2026-11-19
verified: main
tags: [programs, solana]
links:
  - rel: derived-from
    to: src-solana-docs
  - rel: derived-from
    to: src-solana-rpc
created: 2026-11-19
updated: 2026-11-19
---

Solana's documentation: "In the Solana ecosystem, 'smart contracts' are called programs." Read from the
network's RPC on 19 November 2026, the accounts that hold its two token programs are marked executable and are
owned by the program loader, which is what a deployed program looks like on the chain.
