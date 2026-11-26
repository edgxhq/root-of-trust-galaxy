---
id: m-cardano-node-software-planned
type: measurement
title: "Two more node implementations are close, which would lift Cardano's count to 2"
description: "Amaru and Dingo have both begun making blocks on mainnet. With three implementations sharing stake, any two would have to fail together."
status: developing
visibility: public
network: net-cardano
dimension: dim-node-software
state: planned
work: "Amaru and Dingo"
value: 2
unit: implementations
threshold: "more than half of block production, once no single implementation carries a majority"
stage: "Both have made blocks on mainnet since November 2026, a small share of them; Dingo still says it is not ready for mainnet block production"
expected: "no date given"
as_of: 2026-11-24
verified: main
tags: [node-software, cardano]
links:
  - rel: derived-from
    to: src-intersect-weekly-update-138
  - rel: derived-from
    to: src-amaru-releases
  - rel: derived-from
    to: src-dingo-readme
  - rel: derived-from
    to: src-io-q2-2026-report
created: 2026-11-19
updated: 2026-11-24
---

Two implementations pass the test for "close": built in the open, already running on a network others can
join, and named by their makers as the next step. Amaru (Rust) said on 5 November 2026 that "Block forging is
no longer limited to test networks". Dingo (Go) says it "is not yet ready for mainnet block production use", and
passed 100 mainnet blocks in the week to 22 November. Both are among the five implementations Intersect counted on
mainnet that day. The other two it named are not counted here as close. No public code for cardano-bean was found.
TSUNAGI, written in Zig, has a public repository whose builds were described on 24 November as "not Mainnet-ready
or production-qualified". A further one, Acropolis, was halted in April 2026 and does not count.

**Why the figure is 2 and not 3.** The count is the number of implementations that would have to share a fault
to reach more than half of block production. With three sharing stake evenly, any two together hold more than
half, so the count is 2. It would take four implementations sharing stake before the count could be 3.

**Why it is not yet real.** Software being ready does not raise the count. While one implementation runs on
most stake, a bug in it reaches most of the network and the count is 1. It becomes 2 when enough stake pool
operators run the others that no single implementation carries a majority. That part is in operators' hands.

Ethereum shows the path. It has many implementations in production, and its count here is 1 to 2 because one
of them runs on about half of nodes.
