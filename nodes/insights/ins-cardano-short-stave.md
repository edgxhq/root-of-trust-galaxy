---
id: ins-cardano-short-stave
type: insight
title: "Cardano's shortest stave is the diversity of its node software, and only operators can raise it"
description: "One implementation makes the blocks. Others are nearly ready, and they count only when stake pools run them."
status: developing
visibility: public
verified: agent
confidence: high
tags: [cardano, node-software, stake-pools]
links:
  - rel: supports
    to: m-cardano-node-software
  - rel: derived-from
    to: v-cardano-partition-2025
  - rel: related
    to: v-ethereum-client-bug-2025
    note: "what a second client is worth"
created: 2026-11-19
updated: 2026-11-24
---

By the shortest-stave test Cardano's score today is 1. One node implementation still makes nearly all of its
mainnet blocks ([[m-cardano-node-software]]).

The cost of that was shown on 21 November 2025, when a malformed transaction exploited a bug and split the
chain. Funds were safe and the network converged again within 14.5 hours, after operators upgraded.

Raising the stave is under way. By 22 November 2026, five implementations had made blocks on mainnet, four of
them for the first time that month. Their share is still small.

This is the one stave that cannot be raised by developers or by a vote. A second implementation counts when
stake pool operators choose to run it.
