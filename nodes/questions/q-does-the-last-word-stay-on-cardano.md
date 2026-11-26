---
id: q-does-the-last-word-stay-on-cardano
type: question
title: "If Midnight's validators later come from several places, does the last word stay on Cardano?"
description: "Three questions about which of Midnight's ties to Cardano are meant to last. They are questions, not proposals."
status: developing
visibility: public
tags: [midnight]
links:
  - rel: related
    to: net-midnight
    note: "the ties in question"
  - rel: related
    to: rule-or-setting
    note: "whether a tie can be moved"
  - rel: derived-from
    to: src-mip-0023
  - rel: derived-from
    to: src-mps-0034
  - rel: derived-from
    to: src-partner-chains-readme
  - rel: derived-from
    to: src-midnight-whitepaper
created: 2026-11-20
updated: 2026-11-23
---

Midnight's framework describes a way of choosing validators from more than one network, and says "Version 1 is
exclusive to Cardano". So the share of Midnight's blocks made by Cardano's stake pools may change in time.
That is Midnight's to decide.

What makes a ledger a root for something else is not only who makes the blocks. It is what that ledger can
still guarantee when the parties in between fail: where the asset lives, who witnesses the history, and
whether there is a way back. Those ties could outlast a change of validators. Three questions follow. They are
put as questions because the people who would have to build the answers have not been asked.

1. **Will the bridge stay, whoever sits on the committee?** The committee bridge proposed in Midnight's own
process follows whatever committee is seated; it leaves the choosing of that committee to another part of the
system. If the validators later come from several places, is the bridge to Cardano meant to stay?

2. **Could a change that loosens a tie be made slowly and in the open?** A problem statement in the same
process says the pools' share of block production "needs to be configurable". A setting can be moved. Could a
change to it carry notice, and a vote that Cardano's stake pools and holders of NIGHT can see?

3. **After bootstrapping from Cardano, is Midnight aiming to become a root in its own right?** Midnight's
tokenomics whitepaper describes "the multi-resource consensus system that allows Midnight to tap into Cardano's
robust proof-of-stake layer to secure the network while bootstrapping". It does not say what follows the
bootstrapping. Other chains may connect to Midnight for access and for payment. If the aim is for Midnight to
become a root of its own, could its documents say so plainly, and say where NIGHT's home is and where Midnight's
history is witnessed, so that the answer does not depend on who is asked?
