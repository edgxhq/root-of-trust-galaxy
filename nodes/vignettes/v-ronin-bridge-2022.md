---
id: v-ronin-bridge-2022
type: vignette
title: "Five keys out of nine"
description: "A game's bridge was controlled by nine keys, five of them enough. An attacker obtained five."
status: seed
visibility: public
verified: unverified
kind: failed
when: "March 2022"
tags: [failed]
links:
  - rel: illustrates
    to: dim-standing-keys
  - rel: illustrates
    to: level-bridged
  - rel: illustrates
    to: app-bridged
created: 2026-11-19
updated: 2026-11-19
---

A popular game moved its players' assets across a bridge controlled by nine validator keys, any five of which
could approve a withdrawal. In March 2022 an attacker obtained five, four of them held by the game's own
developer, and withdrew about US$620 million.

**What it cost what was built on it.** Players could not withdraw for months. Neither ledger on either side did
anything wrong; each faithfully recorded what the bridge approved.

**What it shows.** The application's real root of trust was five keys, held in practice by two parties. Its
shortest stave was the one nobody was looking at.

From memory of public reporting. The amount and the key counts need a primary source before use.
