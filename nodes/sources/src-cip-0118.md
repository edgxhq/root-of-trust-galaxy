---
id: src-cip-0118
type: source
title: "CIP-0118, \"Nested Transactions\" (Proposed)"
description: "A proposal to let partial transactions from several parties settle together as one batch."
status: developing
visibility: public
url: "https://github.com/cardano-foundation/CIPs/blob/b82f03db55a630ee5d9475d4082ac2e8091b194f/CIP-0118/README.md"
publisher: "Cardano Improvement Proposals"
source_kind: protocol-doc
accessed: 2026-11-20
tags: []
links:
  - rel: related
    to: cardano-scaling-design
    note: "a proposed way to compose transactions"
created: 2026-11-20
updated: 2026-11-20
---

A Cardano improvement proposal, status Proposed when read on 20 November 2026. It proposes "nested
transactions, a construct for composing certain kinds of partially valid transactions, such as unbalanced
transactions, or transactions with missing fees". The parts are gathered into a batch with a top-level
transaction, and "The completed batch must be fully balanced." Its stated uses are swaps without an exchange
and letting one party pay another's fees.
