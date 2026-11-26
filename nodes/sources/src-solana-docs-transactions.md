---
id: src-solana-docs-transactions
type: source
title: "Solana documentation, Transactions and Instructions"
description: "Solana's documentation of how transactions name the accounts they touch."
status: developing
visibility: public
url: "https://github.com/solana-foundation/developer-content/blob/ae78fdb9fa98f1726a48c243e6e4f6137406338d/docs/core/transactions.md"
publisher: "Solana Foundation"
source_kind: protocol-doc
accessed: 2026-11-20
tags: []
links:
  - rel: related
    to: dim-scaling
    note: "how Solana runs transactions side by side"
created: 2026-11-20
updated: 2026-11-20
---

Solana's developer documentation, read in its source repository on 20 November 2026. "By specifying all
accounts required by an instruction, and whether each account is writable, transactions can be processed in
parallel. For example, two transactions that do not include any accounts that write to the same state can be
executed at the same time."
