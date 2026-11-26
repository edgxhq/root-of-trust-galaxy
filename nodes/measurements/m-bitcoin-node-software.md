---
id: m-bitcoin-node-software
type: measurement
title: "Nearly all Bitcoin nodes run one codebase and its derivative"
description: "Nearly all Bitcoin nodes run one codebase and its derivative."
status: developing
visibility: public
network: net-bitcoin
dimension: dim-node-software
value: 1
unit: "codebase lineage"
threshold: "nearly all reachable nodes"
as_of: 2026-02-23
verified: secondary
tags: [node-software, bitcoin]
links:
  - rel: derived-from
    to: src-bitnodes
created: 2026-11-19
updated: 2026-11-19
---

Bitcoin Core is the reference implementation. Bitcoin Knots, which is derived from it, was at about 10% of
reachable nodes in February 2026. The figure counts reachable nodes, not miners, and was read through a search
result. No later figure was obtained.
