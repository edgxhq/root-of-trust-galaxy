---
id: m-solana-node-software-planned
type: measurement
title: "An independent client is live on Solana and would lift its count to 2"
description: "Firedancer has releases for the main network and carries a minority of stake. The count rises when no single client carries a majority."
status: developing
visibility: public
network: net-solana
dimension: dim-node-software
state: planned
value: 2
unit: implementations
threshold: "more than half of stake, once no single client lineage carries a majority"
stage: "Released for the main network; a minority of stake"
expected: "no date given"
as_of: 2026-11-19
verified: main
tags: [node-software, solana]
links:
  - rel: derived-from
    to: src-firedancer-releases
  - rel: derived-from
    to: src-solana-compass-fcat
created: 2026-11-19
updated: 2026-11-19
---

Firedancer is a Solana validator client written independently of the main one. Its repository listed
"Firedancer Mainnet Release v26.10.8" on 11 November 2026. A report of a Fidelity study in October 2026 put
Firedancer configurations at about 15% of stake, and noted that some configurations still share code with the
main client.

The count becomes 2 when the independent client carries enough stake that neither lineage has a majority. By
the test for "close" used here this is further along than Cardano's second implementation: it is already
making blocks on the main network.
