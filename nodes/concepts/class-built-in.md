---
id: class-built-in
type: concept
title: "Ledgers with built-in functions"
description: "Offer a fixed set of functions and carry other assets themselves. A new kind of application waits for the ledger to add it."
status: developing
visibility: public
kind: root-class
short: "built-in functions"
rule: "Does not run general programs; other assets are enforced by the ledger."
order: 2
tags: [method, capability]
links:
  - rel: part-of
    to: what-a-root-can-carry
created: 2026-11-20
updated: 2026-11-20
---

A ledger whose functions are built in: payments, an exchange, tokens. Each new function is added to the ledger
itself, by whatever process changes its rules.

A root is placed here when it does not run general programs and its measurement for [[dim-assets]] is
"enforced by the ledger". A fixed set of functions is a design choice: less can go wrong, and nothing new can
be built without the ledger changing.
