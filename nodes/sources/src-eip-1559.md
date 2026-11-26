---
id: src-eip-1559
type: source
title: "EIP-1559, \"Fee market change for ETH 1.0 chain\""
description: "The rule that sets Ethereum's fee and how far the limit on a block may move."
status: developing
visibility: public
url: "https://eips.ethereum.org/EIPS/eip-1559"
publisher: "Ethereum Improvement Proposals"
source_kind: protocol-doc
accessed: 2026-11-19
tags: []
links:
  - rel: related
    to: net-ethereum
    note: "how the limit on a block is moved"
created: 2026-11-19
updated: 2026-11-20
---

The specification of Ethereum's fee market. It also fixes how the limit on work in a block may move: a block
is invalid if its limit differs from its parent's by a 1,024th or more. So the limit drifts, a little with
each block, as the makers of blocks choose.
