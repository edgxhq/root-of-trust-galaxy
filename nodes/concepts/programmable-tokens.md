---
id: programmable-tokens
type: concept
title: "Tokens that carry their own rules (CIP-113)"
description: "Assets on the ledger whose rules travel with them, enforced by the ledger."
status: seed
visibility: public
verified: secondary
level: root
tags: []
links:
  - rel: instance-of
    to: level-root
  - rel: illustrates
    to: app-other-assets
  - rel: derived-from
    to: src-cardano-org-2026-10-07-programmable-tokens
created: 2026-11-20
updated: 2026-11-20
---

Live on Cardano's main network from October 2026, by the Cardano Foundation's account: "Programmable tokens
stay native Cardano assets built on the EUTXO model, so wallets, explorers, and applications handle them like
any other token while compliance logic travels with the asset".

The ledger enforces the token's rules, including whatever powers those rules give its issuer. Being on the
root means the rules cannot be changed quietly for one holder. It does not mean the issuer has no powers.
