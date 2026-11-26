---
id: m-ethereum-client-implementations
type: measurement
title: "Ethereum has at least six consensus clients and five execution clients in production"
description: "Ethereum has more independent node implementations in production than any other network here, from different teams. How evenly they are used is the count for the link."
status: developing
visibility: public
network: net-ethereum
dimension: dim-node-software
scored: false
value: 6
unit: "consensus clients in production, beside at least five execution clients"
threshold: "in production, from different teams"
summary: "at least 6 consensus and 5 execution clients in production"
as_of: 2026-11-19
verified: main
tags: [node-software, ethereum]
links:
  - rel: derived-from
    to: src-clientdiversity
  - rel: derived-from
    to: src-clientdiversity-data
  - rel: related
    to: m-ethereum-node-software
    note: "the count for the link: how evenly the clients are used"
created: 2026-11-25
updated: 2026-11-25
---

Context for the node-software link, not part of the score. Ethereum runs two layers of software, and each has
several independent clients in production, from different teams: at least six consensus clients and at least five
execution clients, as counted from the same sources as the link, read on 19 November 2026.

This says how many implementations are in use. The link asks how evenly they are used: on 18 November 2026 one
consensus client ran on about half of consensus nodes, which puts the count at 1 if it is above half and 2 if it is
just below.
