---
id: m-bitcoin-merge-rights
type: measurement
title: "Five keys can sign merges to Bitcoin Core"
description: "Five keys can sign merges to Bitcoin Core."
status: developing
visibility: public
network: net-bitcoin
dimension: dim-merge-rights
value: 5
unit: "maintainer keys"
threshold: "all merges to the reference implementation"
as_of: 2026-11-19
verified: agent
tags: [merge-rights, bitcoin]
links:
  - rel: derived-from
    to: src-bitcoin-trusted-keys
created: 2026-11-19
updated: 2026-11-19
---

The repository's trusted-keys file held five fingerprints on 19 November 2026. Press reports say a sixth
maintainer was added in January 2026; the file did not show it, and the difference is unresolved.

The maintainers are funded by several organisations, not one. A merge matters only if node operators choose to
run the release, and the file governs the repository, not the chain.
