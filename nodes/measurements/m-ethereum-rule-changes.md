---
id: m-ethereum-rule-changes
type: measurement
title: "Ethereum's rules change by agreement off-chain, with no record to count"
description: "Ethereum's rules change by agreement off-chain, with no record to count."
status: developing
visibility: public
network: net-ethereum
dimension: dim-rule-changes
value: null
unit: parties
threshold: "a change to the consensus rules"
reason: unrecorded
as_of: 2026-11-19
verified: agent
tags: [rule-changes, ethereum]
links:
  - rel: derived-from
    to: src-eip-1
created: 2026-11-19
updated: 2026-11-19
---

A core change needs client teams to implement it: "you will need to either provide an implementation for clients
or convince clients to implement your EIP." Decisions are reached in public proposals and developer calls. Nothing
is recorded on-chain until a fork activates, so the smallest deciding group cannot be counted.
