---
id: m-cardano-programs
type: measurement
title: "Cardano runs general programs"
description: "Plutus scripts are run by the ledger itself, within limits set by protocol parameters."
status: developing
visibility: public
network: net-cardano
dimension: dim-programs
value: 2
unit: "step on a three-step scale"
threshold: "what the ledger itself can run"
as_of: 2026-11-19
verified: main
tags: [programs, cardano]
links:
  - rel: derived-from
    to: src-cardano-docs-plutus
  - rel: derived-from
    to: src-koios
created: 2026-11-19
updated: 2026-11-19
---

Cardano's documentation: "Plutus is the native smart contract language for Cardano. It is a Turing-complete
language". Scripts are run by every node as part of checking a transaction, within limits set by protocol
parameters. Read from the chain on 19 November 2026, a block may use up to 72,000,000 units of memory and
20,000,000,000 steps.
