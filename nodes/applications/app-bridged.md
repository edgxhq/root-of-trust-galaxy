---
id: app-bridged
type: application
title: "Assets brought from another ledger"
description: "A token on one ledger that stands for something held on another."
status: seed
visibility: public
everyday: "A token on one ledger that stands for something held on another."
needs: "Nothing from the root. It is worth what the bridge behind it honours."
level: bridged
order: 9
tags: [applications]
links:
  - rel: instance-of
    to: level-bridged
  - rel: related
    to: wrapped-assets
    note: "what these are"
created: 2026-11-19
updated: 2026-11-19
---

Useful, and widely used. The token is a claim on something a bridge is holding. If the bridge fails, both
ledgers carry on recording faithfully, and the claim is a claim on nothing.
