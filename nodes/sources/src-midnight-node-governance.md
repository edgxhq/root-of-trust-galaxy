---
id: src-midnight-node-governance
type: source
title: "Midnight node, governance in the runtime and the mainnet configuration"
description: "The two governance bodies, their thresholds and powers, and the members listed for mainnet, read in the node repository."
status: developing
visibility: public
url: "https://github.com/midnightntwrk/midnight-node/blob/8fdc8735b846cf6f42988676470a4570440f453f/runtime/src/lib.rs#L784-L940"
publisher: "Midnight node repository"
source_kind: repository
accessed: 2026-11-24
tags: [midnight]
links:
  - rel: related
    to: net-midnight
    note: "a source for Midnight's eight links"
created: 2026-11-24
updated: 2026-11-24
---

The runtime at commit 8fdc873 (18 November 2026) sets two governance bodies, a Council and a Technical Committee,
of up to ten members each (`MAX_MEMBERS = 10`). Each approves a motion with at least two thirds of its members
(`EnsureProportionAtLeast<..., 2, 3>`), and both are required (`MotionApprovalProportion = ...<1, 1>`); an approved
motion runs with the runtime's `Root` privilege. That privilege applies runtime upgrades, sets system parameters,
pauses transactions and forces safe mode (`SafeModeForceDuration = 7 * DAYS`). The mainnet configuration lists six
Council members and nine on the Technical Committee, each with a Cardano key hash, and membership is followed from
Cardano: https://github.com/midnightntwrk/midnight-node/blob/8fdc8735b846cf6f42988676470a4570440f453f/res/mainnet/federated-authority-config.json. Read on 24 November 2026.
