---
id: multi-resource-consensus
type: concept
title: "Multi-resource consensus"
description: "One ledger secured by more than one kind of resource, such as stake and work, so an attacker has to outweigh them all combined."
status: developing
visibility: public
tags: []
links:
  - rel: related
    to: dim-block-production
    note: "who makes the blocks, from more than one kind of resource"
  - rel: related
    to: public-root-of-trust
    note: "one root, secured more than one way"
  - rel: derived-from
    to: src-minotaur-paper
  - rel: derived-from
    to: src-iog-omega-2025-12-10
  - rel: derived-from
    to: src-hoskinson-2025-02-14
  - rel: derived-from
    to: src-hoskinson-2023-08-30
  - rel: related
    to: claim-one-root
    note: "a ledger secured several ways is not the same as facts spread across ledgers"
created: 2026-11-23
updated: 2026-11-23
---

A consensus protocol that takes its security from more than one kind of resource at once: stake and work, and in
principle others, such as useful computation or reputation. Minotaur (2022) combines proof of work and proof of stake
in one chain, secure while the adversary's combined, weighted share stays below a threshold. Cardano's founder said of
it in 2023 that "it's not just two".

Three uses are described in public.

- **For Cardano's own ledger.** On 14 February 2025 the founder named it as a direction after Leios: "engineer
  cardano to have multiple resources". Input Output's account of Ouroboros Omega, the protocol's planned "final form",
  makes "multi-resource security" its second guiding principle, with no date given. Today Cardano's blocks are made by
  stake alone.
- **For partner chains.** In 2023 the founder described Cardano's stake as "a backbone under Minotaur", with another
  network on "another side of it", in a balance the partner chain chooses.
- **For Midnight.** Its whitepaper uses the term for drawing on Cardano's proof of stake while it starts up.

**A distinction this research draws.** A resource the ledger can check by itself, such as work or stake held on the
ledger, keeps it self-contained. A resource that is stake held on another chain makes the ledger depend on reading
that chain, a link of the kind [[claim-one-root]] describes. In one ledger secured by several resources, an attacker
has to outweigh them all, combined; in a root stitched together from several chains, breaking any one link can be
enough.
