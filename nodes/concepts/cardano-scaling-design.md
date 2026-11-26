---
id: cardano-scaling-design
type: concept
title: "How Cardano is designed to carry more: work side by side"
description: "Cardano's design scales by letting work proceed side by side. Part of that is in place, the first step of another part is on a public test network, and the fully concurrent version is research."
status: developing
visibility: public
verified: main
tags: [capability, cardano]
links:
  - rel: related
    to: dim-scaling
    note: "the same described for every network"
  - rel: related
    to: hydra-heads
    note: "work done beside the ledger and settled on it"
  - rel: related
    to: net-cardano
  - rel: derived-from
    to: src-cardano-docs-eutxo
  - rel: derived-from
    to: src-hydra-docs
  - rel: derived-from
    to: src-cip-0164
  - rel: derived-from
    to: src-cardano-org-2026-08-27-leios
  - rel: derived-from
    to: src-cip-0118
created: 2026-11-20
updated: 2026-11-20
---

Cardano's design scales by letting work proceed side by side, in four places. They are at very different
stages, and it matters which is which.

- **In place: transactions that do not touch the same thing do not wait for each other.** Cardano's
  documentation: "Due to the 'local' nature of transaction validation, a high degree of parallelism is
  possible. A node could, in principle, validate transactions in parallel, if those transactions do not try to
  consume the same input." One transaction can also carry many payments and several assets at once, which is
  one reason a count of transactions says little about the work done.

- **In place, beside the ledger: Hydra heads.** A head is "an off-chain mini ledger shared between a small
  group of participants", with "deposits, decommits, and final settlement recorded on the main chain". Each
  head is separate from the others. The root is not carrying their traffic. It is guaranteeing the way out:
  see [[hydra-heads]].

- **Being implemented: Leios, first version.** "Block producers simultaneously create both a standard Praos
  block and a larger secondary block referencing additional transactions." The proposal describes its target
  as "a 30-65x increase" on the present ceiling. Its first public test network "ran for 41 days with 63 pools"
  and at its peak carried "six times Cardano's current mainnet ceiling". This version is "without concurrency
  and linearized processing", by choice, so that nothing existing applications depend on has to change. It is
  not yet approved, and switching it on needs a hard fork passed by on-chain vote.

- **Research: Leios as first designed.** "The Leios research paper describes a highly concurrent protocol"
  with blocks "produced independently across decoupled, pipelined stages". The proposal being implemented
  calls itself "the foundation for subsequent protocol versions with higher throughput capacity".

One more thing is proposed and is not about speed. Nested transactions would let partial transactions from
several parties settle together as one batch, for swaps and for paying another party's fees.

So "massively parallel" is a fair description of where the design is heading, and of part of what exists
today. The present base layer still has, in the proposal's words, "a fixed ceiling". The honest way to speak
of it is as a design, with each part at its stage.

Every network here has a design for carrying more. The same three questions are asked of each in [[dim-scaling]]
.
