---
id: programs-on-cardano
type: concept
title: "Programs on the root: exchanges, lending, a stablecoin"
description: "Applications whose rules are programs the ledger itself runs, so what they promise is what the root enforces."
status: seed
visibility: public
verified: secondary
level: root
tags: []
links:
  - rel: instance-of
    to: level-root
  - rel: illustrates
    to: app-markets
  - rel: derived-from
    to: src-defillama-cardano
  - rel: related
    to: oracle-price-feeds
    note: "what many of them take from outside"
created: 2026-11-20
updated: 2026-11-20
---

Applications whose rules are programs that Cardano's ledger runs. Among those that run on Cardano alone, the
largest by value held, as listed by DefiLlama on 20 November 2026, include Minswap, Dano Finance and
SundaeSwap (exchanges), Liqwid and Surf Lending (lending) and Djed (a stablecoin).

Because the ledger runs the program, the program's rules are the root's rules: nobody in between can change
them for one user. What such an application takes from outside, such as a price, sits at the distance of
whatever brings it in ([[oracle-price-feeds]]), and some rely on operators to put orders together. The root
guarantees the program, not everything around it.
