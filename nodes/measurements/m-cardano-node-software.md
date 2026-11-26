---
id: m-cardano-node-software
type: measurement
title: "One node implementation still makes most of Cardano's blocks"
description: "Five node implementations have made blocks on Cardano's mainnet, but one still makes nearly all of them, so a bug in it would reach most of block production."
status: developing
visibility: public
network: net-cardano
dimension: dim-node-software
value: 1
unit: "implementation"
threshold: "more than half of block production"
as_of: 2026-11-24
verified: main
tags: [node-software, cardano]
links:
  - rel: derived-from
    to: src-intersect-weekly-update-138
  - rel: derived-from
    to: src-koios
  - rel: derived-from
    to: src-amaru-releases
  - rel: derived-from
    to: src-dingo-readme
  - rel: derived-from
    to: src-acropolis-readme
  - rel: derived-from
    to: src-io-q2-2026-report
created: 2026-11-19
updated: 2026-11-24
---

Five node implementations have now made blocks on Cardano's mainnet: the Haskell cardano-node, Amaru (Rust), Dingo
(Go), cardano-bean and TSUNAGI, by Intersect's count of 22 November 2026. Until November 2026 the Haskell node made
every mainnet block. This is still Cardano's shortest stave.

**Why the count is still 1.** It counts how few implementations, sharing one fault, would reach more than half of
block production. The others are new to mainnet. Amaru's release of 5 November 2026 said "Block forging is no
longer limited to test networks". Dingo passed 100 mainnet blocks in the week to 22 November, while its README,
read again on 24 November, still says it "is not yet ready for mainnet block production use". No counts were
published for Amaru, cardano-bean or TSUNAGI. Cardano made 21,093 blocks in epoch 668 alone, from 15 to 20
November (read from on-chain data on 24 November). For mainnet, Intersect still recommends a release of the
Haskell node. So the Haskell node still makes nearly all of Cardano's blocks, and a bug in it would reach most of
block production.

A block's header does not say which implementation made it, so the split cannot be counted from the chain itself.

A further Rust implementation, **Acropolis**, is not being built any more. Input Output "halted further
development" on 7 April 2026, after it had delivered a node for reading data. Its code remains open.

The count rises when enough stake pool operators run the others that no single implementation carries a majority.
What that would look like is recorded as a planned figure: [[m-cardano-node-software-planned]].

## History

- 19 to 20 November 2026: "One node implementation makes Cardano's blocks today. Two more make blocks on test
  networks." Amaru had opened mainnet block production on 5 November, and no mainnet block by it had been found in
  the chain data used here. The threshold was "all blocks".
