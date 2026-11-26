---
id: m-midnight-rule-changes
type: measurement
title: "Ten governance keys, in two bodies, could change Midnight's rules"
description: "A change needs two thirds of a six-member Council and two thirds of a nine-member Technical Committee. Whose keys they are is not published."
status: developing
visibility: public
network: net-midnight
dimension: dim-rule-changes
value: 10
unit: "governance keys: 4 of 6 on the Council and 6 of 9 on the Technical Committee (whose they are is not published)"
threshold: "two thirds of each of two bodies, both required"
as_of: 2026-11-18
verified: main
tags: [rule-changes, midnight]
links:
  - rel: derived-from
    to: src-midnight-node-governance
  - rel: derived-from
    to: src-midnight-docs-nodes
  - rel: derived-from
    to: src-midnight-whitepaper
created: 2026-11-24
updated: 2026-11-24
---

Midnight's runtime (its node repository on 18 November 2026) sets two governance bodies, a Council and a Technical
Committee. A motion needs at least two thirds of each, and both must approve; it then runs with the runtime's highest
privilege, which applies upgrades to the rules, sets the network's parameters, and can pause the chain or put it into
safe mode. Motions are recorded on Midnight's ledger.

Membership of both bodies is held on Cardano and followed by every node. The mainnet configuration in the repository
lists six Council members and nine on the Technical Committee, so ten keys acting together could change the rules.
Whose keys they are is not published, so keys are counted here, not parties; if one organisation holds several, the
number of parties is lower. The live membership on Cardano was not read.

The tokenomics whitepaper describes this as a beginning: "a phased approach is expected to be implemented to
progressively decentralize the Midnight governance framework".
