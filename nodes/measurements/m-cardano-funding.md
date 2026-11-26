---
id: m-cardano-funding
type: measurement
title: "Twenty DReps hold the share needed to approve spending from Cardano's treasury"
description: "Twenty DReps hold the share needed to approve spending from Cardano's treasury."
status: developing
visibility: public
network: net-cardano
dimension: dim-funding
value: 20
unit: DReps
threshold: "67% of DRep voting power, plus the Constitutional Committee"
as_of: 2026-11-18
verified: main
decided_on_ledger: true
tags: [funding, cardano]
links:
  - rel: derived-from
    to: src-koios
  - rel: derived-from
    to: src-cip-1694
created: 2026-11-19
updated: 2026-11-20
---

Core development is paid from a common treasury. A withdrawal needs 67% of DRep stake and the Constitutional
Committee; stake pools do not vote on it. At epoch 668 the largest 20 DReps held that share.

Same caveats as for rule changes: counted on registered DReps with voting power, and the committee's agreement is
needed as well.
