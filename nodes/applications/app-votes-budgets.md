---
id: app-votes-budgets
type: application
title: "Votes and shared budgets"
description: "A membership voting on its rules and deciding what a common fund pays for."
status: seed
visibility: public
everyday: "A membership voting on its rules and deciding what a common fund pays for."
needs: "Votes counted and money released by the ledger's own rules."
level: root
order: 6
tags: [applications]
links:
  - rel: related
    to: dim-rule-changes
    note: "a root using this on itself"
  - rel: related
    to: dim-funding
    note: "a root paying for its own upkeep"
created: 2026-11-19
updated: 2026-11-19
---

Votes are counted by the ledger and the money moves only if the vote passes. Nobody has to be trusted to tally
or to pay.

A root that sets its own rules and pays for its own upkeep by recorded vote is using this on itself. See
[[dim-rule-changes]] and [[dim-funding]].
