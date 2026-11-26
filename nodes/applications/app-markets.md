---
id: app-markets
type: application
title: "Lending, saving and exchange"
description: "A loan, a savings pool or an exchange run by a program instead of a company."
status: seed
visibility: public
everyday: "A loan, a savings pool or an exchange run by a program instead of a company."
needs: "The root runs the program, so its rules hold whoever wrote it."
level: root
order: 2
tags: [applications]
links:
  - rel: related
    to: dim-programs
    note: "needs a root that runs general programs"
  - rel: related
    to: level-bridged
    note: "where it ends up when the root cannot run it"
created: 2026-11-19
updated: 2026-11-19
---

A program holds the money and applies the same rules to everyone. That is only as good as the ledger running
the program.

A root that can run general programs can host these itself: see [[dim-programs]]. Where a root cannot, they
are built on another ledger and reached through a bridge, which puts them at a distance from the root.
