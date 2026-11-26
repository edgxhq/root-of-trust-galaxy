---
id: v-ethereum-client-bug-2025
type: vignette
title: "One client stumbled. The chain did not."
description: "A bug in one of Ethereum's clients cut participation to three quarters. Finality was not lost."
status: seed
visibility: public
verified: secondary
kind: held
when: "December 2025"
tags: [held]
links:
  - rel: illustrates
    to: dim-node-software
  - rel: derived-from
    to: src-prysm-postmortems
created: 2026-11-19
updated: 2026-11-19
---

In December 2025 a bug in one widely used Ethereum client took its validators out of step. Participation fell to
about 75%. The validators running other clients carried on, and the chain kept finalising. An earlier incident, in
May 2023, delayed finality for four epochs.

**What it shows.** This is what a second implementation is worth. The same bug in a network with one client
would have reached every node.

From a secondary summary of the client team's own post-mortems.
