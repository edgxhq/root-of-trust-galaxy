---
id: distance-from-the-root
type: concept
title: "Distance from the root"
description: "If everyone in between failed or colluded, what could the root still guarantee for you?"
status: developing
visibility: public
tags: [method]
links:
  - rel: related
    to: public-root-of-trust
    note: "what the distance is measured from"
  - rel: derived-from
    to: src-l2beat-stages
created: 2026-11-19
updated: 2026-11-26
---

Anything connected to a root of trust is at most as trustworthy as the root, less whatever sits in between.
So the useful question about a connected system is not whether it is "built on" the root. It is this:

**If everyone in between failed or colluded, what could the root still guarantee for you?**

The answer is a distance, and it belongs to the thing a person holds or relies on: a token, an app or a record,
wherever it runs, whether on the root, on a layer two, on a partner chain or on another chain. Here is one way to
think about that distance, in five rings, from nearest to furthest: [[level-root]], [[level-rooted]],
[[level-anchored]], [[level-bridged]], [[level-unrooted]].

A second marker sits beside the ring: is the tie a rule or a setting? See [[rule-or-setting]].

This is a way of describing, not a ranking of worth, and not an argument against bridges or other chains. People
will use them, and some will be very good. The rings say plainly how much of the root's trust reaches you when you
do. Grading systems by how far their own operators can override the chain beneath them is established practice for
layer-two networks.

**Partner chains are a special case.** The distance matters for everything that relies on the root. A partner
chain, though, is several ties rather than one: who makes its blocks, whether the root witnesses its history, and
whether there is a way back the root enforces. Only the last two bring what lives on it closer, so a partner chain
sits on the ring of what lives on it today ([[ins-partner-chain-ties]]).

The five rings are this research's first attempt, open to correction; nobody has yet checked that they cover every
kind of tie.
