---
id: ins-shortest-stave
type: insight
title: "A network holds trust only up to its shortest stave"
description: "Counting block producers and stopping is the trap. Every link has to be counted, and the lowest count is the score."
status: developing
visibility: public
verified: agent
confidence: high
tags: [method]
links:
  - rel: derived-from
    to: method-shortest-stave
  - rel: supports
    to: m-bitcoin-block-production
  - rel: supports
    to: m-xrp-ledger-standing-keys
  - rel: supports
    to: m-cardano-node-software
  - rel: supports
    to: m-ethereum-node-software
  - rel: supports
    to: m-bitcoin-node-software
  - rel: supports
    to: m-solana-node-software
  - rel: supports
    to: m-xrp-ledger-node-software
  - rel: related
    to: ins-cardano-short-stave
    note: "what one network is doing about its short stave"
created: 2026-11-19
updated: 2026-11-23
---

A barrel holds water only up to its shortest stave. A thousand block producers do not help if one party can
rewrite the rules, or one bug can reach every node.

Counted this way, every network here has a short stave. Bitcoin's block assembly sits with three pools. The
XRP Ledger's default validators come from two published lists. Cardano's blocks are made by one node
implementation. Ethereum has the most implementations, and by some trackers one of them sits near half.

Which stave is short differs. So does whether anything is being done about it, and whether it can be seen at
all.

On the figures counted from February to November 2026, every network here scores 1, and for each the stave at 1 is
the diversity of its node software: one implementation makes most or all of its blocks. The score does not tell them apart. What does
is the rest: how far the other staves stand above it, and whether the short one is being raised. On Cardano, recorded
votes are paying for two more implementations ([[ins-cardano-short-stave]]).
