---
id: src-mip-0023
type: source
title: "MIP-0023, \"Committee Bridge Consensus Integration\" (Proposed, 31 July 2026)"
description: "A proposal in Midnight's own improvement process for a contract on Cardano that follows the signatures of Midnight's committee."
status: developing
visibility: public
url: "https://github.com/midnightntwrk/midnight-improvement-proposals/blob/0de284ef7eb6876579c67b135142b22d55396b00/mips/mip-0023-committee-bridge-consensus.md"
publisher: "Midnight improvement proposals"
source_kind: protocol-doc
accessed: 2026-11-19
tags: [midnight]
links:
  - rel: related
    to: net-midnight
    note: "one of Midnight's ties to Cardano"
created: 2026-11-19
updated: 2026-11-19
---

A proposal in Midnight's own improvement process, status Proposed when read on 18 and 19 November 2026. The
link is to the file as it stood at commit 0de284e.

- Abstract: "The committee bridge lets Cardano contracts verify facts about the Midnight chain."

- Security considerations: "A dishonest two-thirds of seats can sign a root for a chain that honest nodes
  reject; the light client verifies signatures, not chain validity." It adds that corrupting two thirds of
  seats "also breaks GRANDPA itself, so the bridge adds no trust beyond the chain".

- "Why not a succinct (ZK) quorum proof now?": "A quorum of about 100 distinct signers fits one transaction
  today, so direct signature checking ships first." And: "A ZK proof that a threshold of the committee signed,
  verified inside one transaction, replaces the signature list without changing the trust model and lifts the
  cap. That makes it the urgent item after this MIP."

- "Why hold the D-parameter under `signer_cap`?": "The cost is decentralization: a committee under the cap
  seats at most that many distinct pools per session, however many have registered."

A proposal open for comment is not an adopted decision.
