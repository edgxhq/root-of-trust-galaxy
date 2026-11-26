---
id: m-midnight-standing-keys
type: measurement
title: "Midnight's validator list and its emergency switches sit with its two governance bodies"
description: "Which validators count is a list of permissioned seats, and the chain can be paused or put into safe mode. Both sit with the same ten governance keys."
status: developing
visibility: public
network: net-midnight
dimension: dim-standing-keys
value: 10
unit: "governance keys: the same two bodies as for rule changes"
threshold: "two thirds of each of two bodies, both required"
as_of: 2026-11-18
verified: main
tags: [standing-keys, midnight]
links:
  - rel: derived-from
    to: src-midnight-node-governance
  - rel: derived-from
    to: src-midnight-node-config
  - rel: derived-from
    to: src-midnight-docs-nodes
created: 2026-11-24
updated: 2026-11-24
---

Standing powers, as this research counts them, include a list that decides which validators count and switches that
can stop a chain. Midnight has both today. Its blocks come only from permissioned seats
([[m-midnight-block-production]]), whose list is held on Cardano under a script whose rules were not read here. Its
runtime lets its highest privilege pause transactions, force safe mode for up to seven days, change system parameters
(the share of seats among them) and apply runtime upgrades. That privilege is reached only through the two governance
bodies, so the smallest group holding these powers is the same ten keys as for rule changes
([[m-midnight-rule-changes]]). It is not "none", the strongest answer, which has to be shown.
