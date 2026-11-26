---
id: ins-recorded-rules-can-be-counted
type: insight
title: "Only a recorded decision can be counted"
description: "Where rule changes are on-chain votes, the smallest deciding group can be measured. Where they are made off-chain, there is nothing to measure."
status: developing
visibility: public
verified: agent
confidence: medium
tags: [rule-changes]
links:
  - rel: supports
    to: m-cardano-rule-changes
  - rel: supports
    to: m-cardano-standing-keys
  - rel: supports
    to: m-xrp-ledger-rule-changes
  - rel: supports
    to: m-xrp-ledger-standing-keys
  - rel: derived-from
    to: claim-recorded-governance
created: 2026-11-19
updated: 2026-11-19
---

Cardano's rule changes are votes with thresholds, so the concentration can be read off the chain: ten
delegated representatives hold half of the voting power, fifteen hold the share a hard fork needs, and a
change also needs the stake pools and a committee. Its founding keys were destroyed in 2024.

Bitcoin and Ethereum have no owner and no admin key was found. Their decisions are made in proposals, calls
and what operators choose to run. That may be robust. It cannot be counted.

The XRP Ledger records validator votes on its ledger, and the validators that count come from two published
lists.

This is a difference in kind, not a ranking. A recorded process can be audited, and its weak points can be
seen and worked on. Ten representatives holding half the vote is one of them.
