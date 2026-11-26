---
id: m-cardano-merge-rights
type: measurement
title: "Two employers' people merged more than half of the code in Cardano's node over the past year"
description: "Seven people merged more than half of 2,006 changes in a year. By their public profiles they work for two employers or fewer, and Input Output alone accounts for 42.5%."
status: developing
visibility: public
network: net-cardano
dimension: dim-merge-rights
value: 2
value_hi: 7
unit: "parties who merged more than half of the changes: employers by public profile, or people"
threshold: "more than half of the changes merged into the six repositories the node is built from, 20 November 2025 to 19 November 2026"
as_of: 2026-11-20
verified: main
tags: [merge-rights, cardano]
links:
  - rel: derived-from
    to: src-github-intersectmbo-merges
  - rel: derived-from
    to: src-cardano-node-codeowners
  - rel: related
    to: m-cardano-node-software-builders
    note: "who pays the people who merge"
created: 2026-11-19
updated: 2026-11-20
---

Counted from the repositories themselves. In the year to 19 November 2026, 2,006 changes were merged into the
six repositories the node is built from: cardano-node, cardano-ledger, ouroboros-consensus, ouroboros-network,
plutus and cardano-api. Fifty people merged at least one. Seven merged more than half.

By the employers people name on their public profiles, those naming Input Output merged 42.5% of the changes,
and those of one other employer take the total past half. About two in five changes were merged by people who
name no employer, so the true count of employers may be one.

**What it does and does not show.** It counts who did merge, which is close to who can: the repositories'
review rules and team membership are not public. Merging code is not the same as changing the chain. A change
to the rules still needs recorded votes ([[m-cardano-rule-changes]]), and new software runs only where stake
pool operators install it.

**Who pays for the work is decided in the open.** Much of this work is paid from the treasury by recorded
votes, and the same votes have paid two other teams to build separate node implementations: see
[[m-cardano-node-software-builders]]. That does not change how many hands are on the merge button. It does
mean that if those hands were captured, the people who pay for the work could see it and pay others, by a
process recorded on the ledger. No other network here has that.

## History

- 19 November 2026: not counted. The code-owner files name teams, and their members' employers were not resolved.
