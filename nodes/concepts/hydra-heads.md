---
id: hydra-heads
type: concept
title: "Hydra heads"
description: "A group of parties transact among themselves off the main ledger and settle on it. Any one of them can close and take out what is theirs."
status: developing
visibility: public
verified: main
level: rooted
tags: []
links:
  - rel: instance-of
    to: level-rooted
  - rel: derived-from
    to: src-hydra-docs
  - rel: related
    to: cardano-scaling-design
    note: "work done beside the ledger"
created: 2026-11-19
updated: 2026-11-20
---

A Hydra head is opened by locking funds on Cardano, run among its participants, and closed by a transaction on
Cardano. Its documentation: "Many transactions and arrangements can occur within a single Hydra head, with
deposits, decommits, and final settlement recorded on the main chain."

If the participants fall out, the ledger settles it: "An honest party can use signed snapshots to contest an
outdated close, provided it monitors Cardano within the contestation period." The root can enforce the
outcome, which is what "rooted" means. The condition matters: a party has to be watching during that period.

Read in the documentation for version 2.4.2 on 20 November 2026.
