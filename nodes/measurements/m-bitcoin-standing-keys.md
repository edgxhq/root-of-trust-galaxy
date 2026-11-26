---
id: m-bitcoin-standing-keys
type: measurement
title: "No special key over Bitcoin's chain was found"
description: "No special key over Bitcoin's chain was found."
status: developing
visibility: public
network: net-bitcoin
dimension: dim-standing-keys
value: "none"
unit: "standing keys or lists"
threshold: "any standing power over the chain"
as_of: 2026-11-19
verified: agent
tags: [standing-keys, bitcoin]
links:
  - rel: derived-from
    to: src-bitcoin-trusted-keys
created: 2026-11-19
updated: 2026-11-19
---

No layer-one admin key was found. The trusted-keys file governs who may sign merges to the repository, not the
chain.
