---
id: wrapped-assets
type: concept
title: "Wrapped and bridged assets"
description: "A token on one ledger that stands for an asset held somewhere else. It is worth what the bridge behind it honours."
status: seed
visibility: public
verified: agent
level: bridged
tags: []
links:
  - rel: instance-of
    to: level-bridged
  - rel: derived-from
    to: src-chainalysis-2022-hacks
created: 2026-11-19
updated: 2026-11-19
---

A wrapped asset is a claim on something held by a bridge. If the bridge's operators fail or are compromised,
the ledger the token sits on cannot help: it faithfully records a claim on something that is gone.

Of everything stolen from decentralised finance protocols in 2022, about two thirds was taken from bridges.
