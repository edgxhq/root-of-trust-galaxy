---
id: src-minotaur-paper
type: source
title: "Fitzi, Wang, Kannan, Kiayias, Leonardos, Viswanath and Wang, \"Minotaur: Multi-Resource Blockchain Consensus\" (ACM CCS 2022)"
description: "A protocol that secures one chain with proof of work and proof of stake together."
status: developing
visibility: public
url: "https://arxiv.org/abs/2201.11780"
publisher: "arXiv; ACM CCS 2022"
source_kind: paper
accessed: 2026-11-19
tags: []
links:
  - rel: related
    to: multi-resource-consensus
    note: "the design the term comes from"
created: 2026-11-23
updated: 2026-11-23
---

Combines proof of work and proof of stake in one chain. It works in epochs, "continuously sampling the active
computational power to provide a fair exchange between the two resources, work and stake", and is secure as long as
the adversary's combined, weighted share of the two stays below the threshold. Its authors include researchers at
Input Output and the University of Edinburgh. Read from the arXiv text (version 2, 7 September 2022).
