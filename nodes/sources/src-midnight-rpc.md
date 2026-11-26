---
id: src-midnight-rpc
type: source
title: "Midnight's public RPC, mainnet and the Preview test network"
description: "The live committee, the share of seats between permissioned candidates and Cardano's pools, and who is registered, read from Midnight's own public endpoints."
status: developing
visibility: public
url: "https://rpc.mainnet.midnight.network"
publisher: "Midnight"
source_kind: primary-data
accessed: 2026-11-24
tags: [midnight]
links:
  - rel: related
    to: net-midnight
    note: "the live setting behind its block-production figure"
created: 2026-11-24
updated: 2026-11-24
---

Read on 24 November 2026 from https://rpc.mainnet.midnight.network and https://rpc.preview.midnight.network, the
endpoints Midnight's documentation lists, with `systemParameters_getDParameter`, `sidechain_getEpochCommittee` and
`sidechain_getAriadneParameters`. Mainnet: 130 seats for permissioned candidates and none for registered pools; a
committee of 130 seats held by 13 permissioned candidates, ten seats each; no pool registered. Preview: 6 seats for
permissioned candidates and none for pools; six members, one seat each; no pool registered.
