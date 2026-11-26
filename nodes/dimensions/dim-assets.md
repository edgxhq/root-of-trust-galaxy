---
id: dim-assets
type: dimension
title: "Can it carry other assets"
description: "Whether assets other than the root's own coin can be issued on it, and whether the ledger itself enforces them."
status: developing
visibility: public
group: capability
scale: steps
steps: ["Its own coin only", "By convention, read by outside software", "Enforced by the ledger"]
steps_short: ["own coin only", "by convention", "by the ledger"]
question: "Can it carry other assets?"
short: ASSETS
order: 2
tags: [method, capability]
links:
  - rel: part-of
    to: what-a-root-can-carry
created: 2026-11-19
updated: 2026-11-19
---

Whether assets other than the root's own coin can be issued: stable money, a share, a ticket. Three steps: its
own coin only; by a convention that outside software reads out of transaction data; enforced by the ledger or
by programs the ledger runs.

The middle step matters for a root of trust. If outside software decides who owns a token, the root guarantees
that the data was recorded and in what order. It does not guarantee the token's rules.

In every case the ledger can vouch for the token and not for what stands behind it. A token for a dollar is
still a promise by whoever holds the dollar.
