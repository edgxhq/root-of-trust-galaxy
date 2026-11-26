---
id: m-solana-scaling
type: measurement
title: "Solana carries the load in the root itself, running transactions side by side"
description: "Transactions say which accounts they touch, so those that do not collide run at the same time."
status: developing
visibility: public
network: net-solana
dimension: dim-scaling
summary: "Side by side in the root itself"
facets:
  in_root: "The root itself is built to carry heavy traffic. Transactions name the accounts they touch, and those that do not write to the same account are run at the same time."
  beside: "Not written up here."
  building: "Not written up here."
unit: "a description"
threshold: "the design as its own documents describe it"
as_of: 2026-11-20
verified: main
tags: [scaling, solana]
links:
  - rel: derived-from
    to: src-solana-docs-transactions
created: 2026-11-20
updated: 2026-11-20
---

In the root, in its documentation's words: "By specifying all accounts required by an instruction, and whether
each account is writable, transactions can be processed in parallel. For example, two transactions that do not
include any accounts that write to the same state can be executed at the same time."

This is the design that puts most of the work in the root. What it asks of the machines that run a validator
is part of the picture and shows up under hosting; that has not yet been counted here.

Work beside the root, and what is being built, have not been written up here.
