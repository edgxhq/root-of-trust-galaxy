---
id: claim-pools-tie-is-a-setting
type: claim
title: "The share of Midnight's blocks made by Cardano's stake pools is a setting, not a rule"
description: "The whitepaper plans pool-made blocks, but the share is a parameter and a proposal would make it configurable."
status: developing
visibility: public
verified: main
confidence: high
tags: [midnight]
links:
  - rel: derived-from
    to: src-midnight-node-config
  - rel: derived-from
    to: src-mps-0034
  - rel: derived-from
    to: src-partner-chains-readme
  - rel: derived-from
    to: src-hoskinson-2023-08-30
  - rel: contradicts
    to: src-midnight-whitepaper
    note: "the plan of record is pools only"
  - rel: related
    to: rule-or-setting
    note: "the distinction it applies"
created: 2026-11-19
updated: 2026-11-19
---

**For.** The repository's mainnet configuration sets 10 permissioned seats and 0 pool seats, as a parameter.
A proposal in Midnight's process calls native NIGHT staking "the first piece of network sovereignty" and says
the pools' share "needs to be configurable". The framework's README says "Version 1 is exclusive to Cardano."
Charles Hoskinson said in 2023 that the balance "is completely up to the person who's launching the partner
chain".

**Against.** The whitepaper says "the role of producing blocks will require that prospective Midnight block
producers be Cardano SPOs". Nothing found says Midnight will take validators from another chain; the second
resource proposed is NIGHT itself. The proposal is open for comment, not adopted.

Both are true: the plan of record is pools, and nothing fixes it.
