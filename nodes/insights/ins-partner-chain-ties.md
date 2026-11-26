---
id: ins-partner-chain-ties
type: insight
title: "A partner chain is several ties, not one distance"
description: "The rings describe what lives on a partner chain. The partner chain itself has several ties to the root, and only two move what lives on it closer: the root witnessing its history, and a way back the root enforces."
status: developing
visibility: public
verified: main
confidence: medium
tags: [midnight, method]
links:
  - rel: refines
    to: distance-from-the-root
  - rel: derived-from
    to: src-partner-chains-readme
  - rel: derived-from
    to: src-mip-0023
  - rel: derived-from
    to: src-mps-0033
  - rel: related
    to: rule-or-setting
    note: "each tie can be a rule or a setting"
  - rel: related
    to: level-anchored
    note: "the root witnesses its history"
  - rel: related
    to: level-rooted
    note: "a way back the root enforces"
created: 2026-11-24
updated: 2026-11-26
---

The rings ([[distance-from-the-root]]) answer one question about something a person holds or relies on: if
everyone in between failed or colluded, what could the root still guarantee? A token, an app or a record has one
answer. A partner chain has several ties to the root, and they answer the question differently.

The Partner Chains Toolkit, which Midnight's node is built with, lists them (read at a pinned commit in November
2026): block producers drawn from the root's registered stake pools beside permissioned ones, in "a configurable ratio
of public (registered) versus permissioned validators"; governance by "a set of Governance Authorities with a
configurable threshold"; a token reserve held on the root and observed on the partner chain; rewards for block
producers and delegators; and Minotaur, which could draw validators from more than one network ("Version 1 is
exclusive to Cardano").

Most of these tie a partner chain's operators and economics to the root, and make cheating costlier. The root's
stake pools making its blocks is a tie, not a guarantee: if the producers colluded, the root's ledger could not undo
it. None of these ties, on its own, lets the root guarantee anything to someone on the partner chain. Two ties do.

- **The root witnesses its history** ([[level-anchored]]): commitments to the partner chain's record held on the
  root, so what was signed can be proven. Midnight's proposed committee bridge is one: a light client on Cardano that
  follows the committee and the roots it signs. In the proposal's words it "verifies signatures, not chain validity".
- **A way back the root enforces** ([[level-rooted]]): the root checks proofs of what happened on the partner chain
  before releasing anything, so a person can get out with what is theirs if the operators fail. None is written for a
  partner chain yet.

Neither asks the partner chain to run on the root. Being witnessed costs a small commitment posted now and then.
Being rooted needs proofs the root can check, which is harder engineering. In both, the root checks the partner chain;
it does not run it.

What lives on a partner chain can sit on different rings at once: NIGHT held on Cardano is on the root, and NIGHT
on Midnight is as close as Midnight's ties make it. So a partner chain is placed on the ring of what lives on its own
ledger today. Because each tie can be a setting ([[rule-or-setting]]), a partner chain's distance can change.

Each tie can be a choice, and a partner chain may have good reasons for where it sits. The rings make the choice
plain to state.
