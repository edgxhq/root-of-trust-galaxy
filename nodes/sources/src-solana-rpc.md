---
id: src-solana-rpc
type: source
title: "Solana mainnet RPC"
description: "The network's own records: its validators and the stake on each, what each validator publishes about itself, and who holds that stake."
status: developing
visibility: public
url: "https://api.mainnet-beta.solana.com"
publisher: "Solana Foundation"
source_kind: primary-data
accessed: 2026-11-21
tags: []
links:
  - rel: related
    to: net-solana
    note: "stake by validator, read from the chain"
created: 2026-11-19
updated: 2026-11-21
---

The network's own records, read through its public endpoint.

- `getVoteAccounts`: every validator and the stake active on it. Read on 19 November 2026 (659 validators, 426
  million SOL) and on 21 November 2026 (685 validators, 429 million SOL).
- Validator info, held by the Config program: the name, website and Keybase name each validator publishes about
  itself. Read on 21 November 2026.
- Vote accounts (`getMultipleAccounts`): each validator's withdraw authority, the key that controls its earnings.
  Read for the largest 100 on 21 November 2026.
- Stake accounts (Stake program, by validator): who holds the stake on a validator. Read on 21 November 2026 for
  the validators among the largest 80 that keep all their rewards.

The vote list names validators, not the operators behind them. The other three records are how validators under
one operator can be found and counted once.
