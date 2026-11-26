---
id: m-cardano-rule-changes
type: measurement
title: "Ten DReps hold half of the voting power that sets Cardano's rules"
description: "Ten DReps hold half of the voting power that sets Cardano's rules."
status: developing
visibility: public
network: net-cardano
dimension: dim-rule-changes
value: 10
unit: DReps
threshold: "half of DRep voting power; a hard fork needs 60% of DRep stake, 51% of pool stake and the Constitutional Committee"
as_of: 2026-11-18
verified: main
decided_on_ledger: true
tags: [rule-changes, cardano]
links:
  - rel: derived-from
    to: src-koios
  - rel: derived-from
    to: src-cip-1694
created: 2026-11-19
updated: 2026-11-20
---

At epoch 668, 847 delegated representatives held voting power. The largest 10 held 50.3% of it, the largest 15
held 60%, and the largest 27 held 75%.

No single body can change the rules. A hard fork needs 60% of DRep stake, 51% of stake pool stake and the
Constitutional Committee (seven members, two thirds of them). So the true smallest group is larger than ten; the
figure given is the most concentrated of the three bodies.

Counted on registered DReps with voting power. It is not adjusted for inactive DReps or for the 131 million ADA
delegated to "always no confidence". The 10.46 billion ADA delegated to "always abstain" is outside the count.

The concentration is visible because the votes are recorded.
