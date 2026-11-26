---
id: src-partner-chains-ariadne-v2
type: source
title: "Partner Chains Toolkit, committee selection (Ariadne v2)"
description: "The rule that fills a partner chain's committee: each candidate's whole number of expected seats guaranteed, the rest drawn by weight."
status: developing
visibility: public
url: "https://github.com/midnightntwrk/midnight-node/blob/8fdc8735b846cf6f42988676470a4570440f453f/partner-chains/toolkit/committee-selection/selection/src/ariadne_v2.rs"
publisher: "Midnight node repository"
source_kind: repository
accessed: 2026-11-24
tags: [midnight]
links:
  - rel: related
    to: net-midnight
    note: "how its seats would be filled from Cardano's pools"
created: 2026-11-24
updated: 2026-11-24
---

"Let `E_i` be the expected number of places in the resulting committee of candidate `i` calculated from D-parameter
and its weight relative to other candidates. Then candidate `i` is guaranteed to get at least `floor[E_i]` seats." The
remaining seats are drawn at random, weighted by what is left of each candidate's expectation. Read at commit 8fdc873
(18 November 2026).
