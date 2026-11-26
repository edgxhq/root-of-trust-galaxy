---
id: m-midnight-node-software
type: measurement
title: "One implementation makes all of Midnight's blocks"
description: "Midnight's documentation describes one node, built with Substrate and the Partner Chains Toolkit. No second implementation is listed."
status: developing
visibility: public
network: net-midnight
dimension: dim-node-software
value: 1
unit: "implementations"
threshold: "more than half of blocks"
as_of: 2026-11-24
verified: main
tags: [node-software, midnight]
links:
  - rel: derived-from
    to: src-midnight-docs-nodes
  - rel: derived-from
    to: src-partner-chains-readme
created: 2026-11-24
updated: 2026-11-26
---

Midnight's documentation describes one node, the Midnight Node, built with Substrate and the Partner Chains Toolkit,
and no second implementation is listed. With one implementation, one shared fault could reach every node at once.
The count is 1, as on every network here.
