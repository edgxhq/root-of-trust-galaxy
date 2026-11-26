---
id: net-midnight
type: network
title: Midnight
description: "A privacy-focused partner chain launched with its token on Cardano. What ties it to Cardano today, what is proposed, and roughly where that places it."
status: developing
visibility: public
kind: satellite
level: bridged
level_fit: rough
level_note: "A reading of public documents on 18 and 19 November 2026, not a verdict. NIGHT held on Cardano is on the root itself. Midnight's own ledger is reached by a link that runs one way and is operated by Midnight's validators, which is nearest to this ring."
orbits: net-cardano
paths:
  - level: anchored
    basis: their-proposal
    label: "if its committee bridge is adopted"
    note: "A proposal in Midnight's own process would let contracts on Cardano check what Midnight's committee signed. In its words, the contract \"verifies signatures, not chain validity\"."
    sources:
      - to: src-mip-0023
        at: "#abstract"
        label: "MIP-0023, abstract"
ties:
  - tie: "Its token launched on the root"
    state: in-place
    permanence: unknown
    note: "NIGHT was launched as a Cardano native asset, and most of the supply is on Cardano today. Nothing written says it will stay there: Midnight's protocol includes a bridge that moves NIGHT to Midnight, and a problem statement would make the form on Midnight the one that is staked."
    sources:
      - to: src-midnight-whitepaper
        label: "Tokenomics whitepaper"
      - to: src-mps-0034
        at: "#success-criteria"
        label: "MPS-0034, success criteria"
      - to: src-mps-0033
        at: "#problem"
        label: "MPS-0033, problem"
  - tie: "It reads the root"
    state: in-place
    permanence: unknown
    note: "Every Midnight node runs a Cardano node. A draft calls this \"the largest single item in a Midnight node's operating envelope\" and asks for a lighter way to do it, not for removing it."
    sources:
      - to: src-mps-0038
        at: "#abstract"
        label: "MPS-0038, abstract"
  - tie: "The root's stake pools produce its blocks"
    state: planned
    permanence: setting
    note: "Planned in the whitepaper with no date. Live on 24 November 2026, its committee had 130 seats, all for permissioned candidates, and no pool was registered, on mainnet or on its Preview test network. A problem statement says the pools' share \"needs to be configurable\"."
    sources:
      - to: src-midnight-rpc
        label: "Live committee, read from Midnight's RPC"
      - to: src-midnight-node-config
        label: "Mainnet setting in the repository"
      - to: src-mps-0034
        at: "#success-criteria"
        label: "MPS-0034, success criteria"
  - tie: "Rewards reach pools and delegators on the root"
    state: proposed
    permanence: unknown
    note: "Proposed: rewards for making blocks paid in NIGHT on Cardano, split between a pool's operator and its delegators as Cardano staking rewards are."
    sources:
      - to: src-mip-0024
        at: "#abstract"
        label: "MIP-0024, abstract"
  - tie: "A way back to the root"
    state: proposed
    permanence: unknown
    note: "Not there yet: \"NIGHT can move from Cardano to Midnight, but not back.\" Proposed in Midnight's own process: a problem statement (status Proposed, 21 August 2026) sets out what a way back must guarantee, with each release on Cardano authorised by the Midnight committee through the committee bridge of MIP-0023. Each release would rest on the committee's word, not on a check the root makes, so this way back does not by itself bring what lives on Midnight closer."
    sources:
      - to: src-mps-0033
        at: "#problem"
        label: "MPS-0033, problem"
      - to: src-mps-0033
        at: "#goals"
        label: "MPS-0033, goals"
  - tie: "The root can check what its committee signed"
    state: proposed
    permanence: unknown
    ring: anchored
    note: "Proposed: a contract on Cardano that follows the signatures of Midnight's committee. It shows what the committee signed. In the proposal's words it \"verifies signatures, not chain validity\"."
    sources:
      - to: src-mip-0023
        at: "#abstract"
        label: "MIP-0023, abstract"
      - to: src-mip-0023
        at: "#security-considerations"
        label: "security considerations"
  - tie: "A compact proof of those signatures"
    state: named
    permanence: unknown
    ring: anchored
    note: "Named as \"the urgent item after\" the committee bridge: a zero-knowledge proof that enough of the committee signed. It \"replaces the signature list without changing the trust model\" and lifts a cap of about 100 signers, so more pools could sit on the committee."
    sources:
      - to: src-mip-0023
        at: "#why-not-a-succinct-zk-quorum-proof-now"
        label: "MIP-0023, why not a succinct proof now"
      - to: src-mps-0048
        at: "#goals"
        label: "MPS-0048, goals"
  - tie: "The root checks that its ledger kept its rules"
    state: spoken
    permanence: unknown
    ring: rooted
    note: "Charles Hoskinson has described bridging by zero-knowledge proofs checked on both sides, once later upgrades are in place on each chain. No written proposal for it was found in Midnight's process on 19 November 2026. How far it would move Midnight depends on what the proofs cover, and that is not yet written down."
    sources:
      - to: src-hoskinson-2026-07-27
        label: "AMA, 27 July 2026, from 00:35:14"
tags: [midnight]
links:
  - rel: related
    to: net-cardano
    note: "the root it is built on"
  - rel: instance-of
    to: level-bridged
    note: "the nearest fit for its own ledger on the documents read in November 2026"
  - rel: derived-from
    to: src-midnight-whitepaper
  - rel: derived-from
    to: src-partner-chains-readme
  - rel: raises
    to: q-does-the-last-word-stay-on-cardano
    note: "which ties are meant to last"
created: 2026-11-19
updated: 2026-11-26
---

Midnight is a separate ledger for private computation, launched with its token on Cardano. This entry lists what
is known about its ties to Cardano, each with a link to the passage it rests on, and says roughly where those
ties place it. It is a reading of public documents, made on 18 and 19 November 2026. The documents are moving
quickly, and some of this will be out of date soon.

**Where it roughly fits.** NIGHT launched on Cardano, and while it is held there it is on the root itself. Nothing
written says it must stay. Midnight's own ledger is reached by a link
that runs one way and is operated by Midnight's validators. By the distance test that is nearest to "bridged":
if the parties in between failed, Cardano could not yet help with what is on Midnight.

**What would change that.** Two things are written down in Midnight's own process. A committee bridge would let
contracts on Cardano check what Midnight's committee signed, which is the kind of tie called "anchored" here.
After it, a compact proof of those signatures would do the same job for a larger committee; by the proposal's own
account it does not change what is trusted.

A third thing has been described and not yet written: bridging by zero-knowledge proofs checked on both chains.
Whether that would let the root enforce an outcome, and not only witness one, depends on what the proofs cover.

**What is not known here.** Which of these ties are meant to be permanent. One of them, the share of blocks made
by Cardano's stake pools, is described in Midnight's process as something that "needs to be configurable".

A new network is entitled to choose how it is secured. Nothing here is a proposal for what Midnight should do.
