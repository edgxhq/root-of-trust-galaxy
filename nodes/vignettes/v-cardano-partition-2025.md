---
id: v-cardano-partition-2025
type: vignette
title: "One implementation, one bug, fourteen and a half hours"
description: "A malformed transaction split Cardano's chain. Funds were safe, and the network converged again without a central switch."
status: developing
visibility: public
verified: agent
kind: held
when: "21 November 2025"
tags: [held]
links:
  - rel: illustrates
    to: dim-node-software
  - rel: derived-from
    to: src-cardano-org-2025-11-incident
created: 2026-11-19
updated: 2026-11-19
---

The public account: "A malformed transaction exploited a deserialization bug" and caused a temporary split; "the
network remained online and funds were safe"; operators "successfully restored full convergence within 14.5 hours"
by upgrading their nodes.

**What it shows.** The root held: there was no switch to turn the network off and on, and hundreds of independent
operators repaired it by acting separately. It also showed the root's short stave. With one node implementation,
one bug reached every node.
