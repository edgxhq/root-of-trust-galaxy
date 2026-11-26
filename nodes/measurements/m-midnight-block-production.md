---
id: m-midnight-block-production
type: measurement
title: "Seven of thirteen permissioned candidates make more than half of Midnight's blocks"
description: "Midnight's blocks come in turn from 130 seats held by thirteen permissioned candidates, ten each. Seven make more than half; which operator holds which is not published, and no seat is held by a Cardano pool."
status: developing
visibility: public
network: net-midnight
dimension: dim-block-production
value: 7
unit: "permissioned candidates, each with an equal share of the seats (who holds each is not published)"
threshold: "more than half of blocks; finality needs two thirds of the seats"
as_of: 2026-11-24
verified: main
tags: [block-production, midnight]
links:
  - rel: derived-from
    to: src-midnight-rpc
  - rel: derived-from
    to: src-midnight-node-config
  - rel: derived-from
    to: src-midnight-docs-nodes
  - rel: derived-from
    to: src-midnight-docs-consensus
  - rel: derived-from
    to: src-midnight-blog-2026-02-17
  - rel: derived-from
    to: src-midnight-blog-2026-02-24
  - rel: derived-from
    to: src-mps-0030
created: 2026-11-24
updated: 2026-11-24
---

Read live from Midnight's own public endpoint on 24 November 2026: its committee has 130 seats, all for permissioned
candidates and none for stake pools registered on Cardano, and thirteen candidates hold ten seats each. Its
documentation describes the validators as "Permissioned nodes operated by Federated Node Operators (FNOs). Stake Pool
Operators (SPOs) supported at a later date", and a problem statement in its own process says "Today Midnight is
operated by a small, federated committee."

Blocks are made in turn: under AURA, in Midnight's documentation, "Validators take turns in a round-robin fashion". So
each candidate makes an equal share, and seven make more than half. Finality (GRANDPA) needs two thirds.

Seven organisations were named in February 2026 as federated node operators: Google Cloud, Blockdaemon, AlphaTON,
Shielded Technologies, Pairpoint by Vodafone, eToro and MoneyGram. Which of them holds which candidate is not
published. Candidates are counted here, not operators; if one operator holds more than one, the number of independent
parties is lower.

No network of Midnight's makes blocks with Cardano's pools today: on its Preview test network, read the same day, the
seats were six, all permissioned, and no pool was registered. The published plan is to hand block production to
Cardano's stake pools, and their share is a setting (see Midnight's ties).

## History

- 18 November 2026: counted from the node repository's mainnet setting, 10 seats for permissioned candidates and none
  for pools, as 6 of 10 seats. The live setting, read on 24 November, replaced it.
