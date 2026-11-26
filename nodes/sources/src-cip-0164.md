---
id: src-cip-0164
type: source
title: "CIP-0164, \"Ouroboros Linear Leios: Greater transaction throughput\" (Proposed)"
description: "The proposal to raise Cardano's throughput, with its targets and what remains before it is active."
status: developing
visibility: public
url: "https://github.com/cardano-foundation/CIPs/blob/a2cac18039d7bab6c0dc1a806ad8a96b8b0546fc/CIP-0164/README.md#how-leios-addresses-cps-18"
publisher: "Cardano Improvement Proposals"
source_kind: protocol-doc
accessed: 2026-11-19
tags: []
links:
  - rel: related
    to: dim-scaling
    note: "what Leios changes and what it leaves for later"
created: 2026-11-19
updated: 2026-11-20
---

A Cardano improvement proposal, status Proposed when read on 19 and 20 November 2026. The link is to the file
as it stood at commit a2cac18 (15 September 2026).

- On today's ceiling: "there is a fixed ceiling on the network's transaction throughput that cannot be raised
  by adjusting protocol parameters alone."

- On what it changes: "Block producers simultaneously create both a standard Praos block and a larger
  secondary block referencing additional transactions." It describes its target as "a 30-65x increase".

- On counting transactions: "TPS is not an appropriate metric", because it "does not account for transaction
  size or computational complexity, making systems with smaller transactions appear 'faster' while providing
  less utility".

- On what it leaves for later: "The Leios research paper describes a highly concurrent protocol", with blocks
  "produced independently across decoupled, pipelined stages". This proposal is "the proposed variant without
  concurrency and linearized processing", and calls itself "the foundation for subsequent protocol versions
  with higher throughput capacity".

- Under "Path to Active", the steps not yet ticked include "Successful operation with open participation in
  testnet environments over several months" and "Hard-fork enabling Leios is successfully executed on
  mainnet."
