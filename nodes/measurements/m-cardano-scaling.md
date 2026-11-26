---
id: m-cardano-scaling
type: measurement
title: "Cardano is built to do work side by side; part of that is in place and part is being built"
description: "Transactions that do not touch the same thing can be checked side by side, heads run beside the ledger, and a larger second block is being implemented."
status: developing
visibility: public
network: net-cardano
dimension: dim-scaling
summary: "Side by side by design; heads beside it; Leios being implemented"
facets:
  in_root: "Transactions that do not spend the same output can be checked side by side, and one transaction can carry many payments and several assets. The size of a block is fixed, and its own documents say that ceiling cannot be raised much further without a change of design."
  beside: "Hydra heads: a group transacts on a small ledger of its own and settles on Cardano."
  building: "Leios, which adds a larger second block beside each standard one. Being implemented: the first version has run on a public test network. That version works one block at a time; the design in which blocks are made side by side is research."
unit: "a description"
threshold: "the design as its own documents describe it"
as_of: 2026-11-20
verified: main
tags: [scaling, cardano]
links:
  - rel: derived-from
    to: src-cardano-docs-eutxo
  - rel: derived-from
    to: src-cip-0164
  - rel: derived-from
    to: src-hydra-docs
  - rel: derived-from
    to: src-cardano-org-2026-08-27-leios
  - rel: derived-from
    to: src-leios-site
created: 2026-11-20
updated: 2026-11-20
---

In its documents' own words. In the root: "Due to the 'local' nature of transaction validation, a high degree
of parallelism is possible." And on its limit: "there is a fixed ceiling on the network's transaction
throughput that cannot be raised by adjusting protocol parameters alone."

Beside the root: a Hydra head is "an off-chain mini ledger shared between a small group of participants", with
"final settlement recorded on the main chain".

Being built: with Leios, "Block producers simultaneously create both a standard Praos block and a larger
secondary block referencing additional transactions." Its first public test network "ran for 41 days with 63
pools". The proposal is still Proposed, and switching it on needs a hard fork approved by on-chain vote.

The whole design, and which part is at which stage, is in [[cardano-scaling-design]].
