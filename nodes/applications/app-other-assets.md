---
id: app-other-assets
type: application
title: "Stable money, shares and tickets"
description: "A token that stands for a dollar, a share or a seat."
status: seed
visibility: public
everyday: "A token that stands for a dollar, a share or a seat at a concert."
needs: "The ledger enforces who holds the token."
level: root
order: 3
tags: [applications]
links:
  - rel: related
    to: dim-assets
    note: "needs a root that carries other assets"
created: 2026-11-19
updated: 2026-11-19
---

The ledger keeps track of who holds the token, and on a root that enforces its own assets nobody can quietly
change that: see [[dim-assets]].

What the ledger cannot vouch for is what stands behind the token. A token for a dollar is still a promise by
whoever holds the dollar.
