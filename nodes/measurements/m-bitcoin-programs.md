---
id: m-bitcoin-programs
type: measurement
title: "Bitcoin runs limited scripts, by design"
description: "Bitcoin's script language has no loops and keeps no state. Proposals to widen it are written; none is active."
status: developing
visibility: public
network: net-bitcoin
dimension: dim-programs
value: 1
unit: "step on a three-step scale"
threshold: "what the ledger itself can run"
as_of: 2026-11-19
verified: main
tags: [programs, bitcoin]
links:
  - rel: derived-from
    to: src-bitcoin-devguide
  - rel: derived-from
    to: src-bitcoin-bips
created: 2026-11-19
updated: 2026-11-19
---

Bitcoin's developer guide describes its script language as "deliberately designed to be stateless and not
Turing complete", and says the lack of loops "makes the script language less flexible and more predictable,
greatly simplifying the security model". That is a choice, and a sound one for a ledger whose job is money.

Proposals to widen what scripts can do exist as Bitcoin improvement proposals: BIP-119 (status Draft), BIP-347
(Complete, meaning the text is finished) and BIP-348 (Draft), read on 19 November 2026. Each would be a change
to the consensus rules. None is active on the main network, and none would make Bitcoin run general programs,
so no planned figure is shown.
