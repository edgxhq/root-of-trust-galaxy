---
id: src-mps-0048
type: source
title: "MPS-0048, \"Enabling Light Clients on Midnight\" (Proposed, 15 October 2026)"
description: "A problem statement in Midnight's own improvement process asking for one compact proof of which committee Midnight seated."
status: developing
visibility: public
url: "https://github.com/midnightntwrk/midnight-improvement-proposals/blob/0de284ef7eb6876579c67b135142b22d55396b00/mps/mps-0048-enabling-light-clients.md"
publisher: "Midnight improvement proposals"
source_kind: protocol-doc
accessed: 2026-11-19
tags: [midnight]
links:
  - rel: related
    to: net-midnight
    note: "what a compact proof of the committee would and would not show"
created: 2026-11-19
updated: 2026-11-19
---

A problem statement in Midnight's own improvement process, status Proposed when read on 19 November 2026. The
link is to the file as it stood at commit 0de284e.

It asks for a single proof of the chain of committee handovers, so that a phone or a contract on any chain can
learn which committee to trust without following Midnight's whole history. Under "Goals": "A single proof of
that induction says what following every handover would say, and a verifier checks it without holding the
chain, without the handovers, and without being on Cardano or anywhere in particular. What it replaces is the
walk, not the trust."

It sets itself apart from the committee bridge proposal: "This MPS does not require cheap verification in
Cardano."

A problem statement open for comment is not an adopted decision.
