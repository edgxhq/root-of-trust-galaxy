---
id: m-cardano-node-software-builders
type: measurement
title: "Five organisations are paid by recorded vote to build or maintain Cardano's node software"
description: "Treasury withdrawals voted on the ledger in 2025 and 2026 pay for the main node, its smart-contract engine, and two independent node implementations."
status: developing
visibility: public
network: net-cardano
dimension: dim-merge-rights
scored: false
value: 5
unit: "organisations paid by recorded vote to build or maintain the node's software"
threshold: "treasury withdrawals ratified and enacted on the ledger, 2025 and 2026"
as_of: 2026-11-20
verified: main
tags: [merge-rights, node-software, cardano]
links:
  - rel: derived-from
    to: src-koios-governance-actions
  - rel: derived-from
    to: src-amaru-releases
  - rel: related
    to: m-cardano-node-software-planned
    note: "two of them are building separate implementations"
created: 2026-11-20
updated: 2026-11-20
---

Read from Cardano's ledger. Treasury withdrawals ratified by recorded vote and enacted in 2025 and 2026 pay
for:

- the main node's core development and maintenance: Input Output, and Ensurable Systems with it;
- Plutus, the engine that runs smart contracts: Input Output and VacuumLabs;
- Amaru, a separate node in Rust, in 2025 and again in 2026: the Amaru project, which PRAGMA publishes;
- Dingo, a separate node in Go: Blink Labs.

That is five organisations, and two of the teams are building nodes that would make the software link less of
a single point of failure. Each payment passed a vote that anyone can read on the ledger.

This is context, not a count of who could take a link: it is not part of the score. It sits beside who can
merge the code ([[m-cardano-merge-rights]]) because it says who pays the people who do.
