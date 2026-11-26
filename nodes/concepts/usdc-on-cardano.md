---
id: usdc-on-cardano
type: concept
title: "Dollars from an issuer (USDC)"
description: "A dollar token issued on Cardano. The token is on the root; the dollar behind it is held by its issuer."
status: seed
visibility: public
verified: secondary
level: bridged
tags: []
links:
  - rel: instance-of
    to: level-bridged
  - rel: illustrates
    to: app-other-assets
  - rel: related
    to: wrapped-assets
    note: "the same position: a claim on something held by someone in between"
  - rel: derived-from
    to: src-cardano-org-2026-05-20-integrations
created: 2026-11-20
updated: 2026-11-20
---

A status report of 20 May 2026 lists "Circle's native USDC issuance on Cardano" as live.

The token is held on Cardano, so the ledger says who holds it. The dollar behind it is held by its issuer. If
the issuer failed, the root could not help with the dollar. By the distance test the token is a claim on
something kept by someone in between, which is where a bridged asset sits. That is a statement about where the
trust sits, not about the issuer.
