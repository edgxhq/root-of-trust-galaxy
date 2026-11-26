---
id: m-xrp-ledger-programs
type: measurement
title: "The XRP Ledger offers built-in functions, not general programs"
description: "Its features are built in and arrive by amendment. None of the amendments its servers knew on 19 November 2026 adds general programs."
status: developing
visibility: public
network: net-xrp-ledger
dimension: dim-programs
value: 1
unit: "step on a three-step scale"
threshold: "what the ledger itself can run"
as_of: 2026-11-19
verified: main
tags: [programs, xrp-ledger]
links:
  - rel: derived-from
    to: src-xrpl-rpc
  - rel: derived-from
    to: src-xrpl-amendments
created: 2026-11-19
updated: 2026-11-19
---

The XRP Ledger's functions are built in: payments, an exchange, escrow, automated market makers, tokens,
credentials. Each arrives as an amendment that validators vote on. On 19 November 2026 a public server running
version 3.4.1 listed 107 amendments, 98 of them enabled. None adds general programs that anyone can deploy.
Amendments known but not yet enabled included a lending protocol, a single-asset vault and a cross-chain
bridge.

A fixed set of functions is a design choice. Less can go wrong, and nothing new can be built without an
amendment.
