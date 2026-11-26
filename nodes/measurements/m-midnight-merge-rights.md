---
id: m-midnight-merge-rights
type: measurement
title: "Two employers' people merged more than half of the code in Midnight's node over the past year"
description: "Three people merged more than half of 1,838 changes in a year. By their public profiles they work for two employers or fewer, and Shielded Technologies alone accounts for 49.3%."
status: developing
visibility: public
network: net-midnight
dimension: dim-merge-rights
value: 2
value_hi: 3
unit: "parties who merged more than half of the changes: employers by public profile, or people"
threshold: "more than half of the changes merged into the three repositories the node is built from, 24 November 2025 to 23 November 2026"
as_of: 2026-11-24
verified: main
tags: [merge-rights, midnight]
links:
  - rel: derived-from
    to: src-github-midnightntwrk-merges
created: 2026-11-24
updated: 2026-11-24
---

Counted from the repositories themselves, the same way as for Cardano. In the year to 23 November 2026, 1,838 changes
were merged into the three repositories Midnight's node is built from: midnight-node (1,180, including the Partner
Chains Toolkit it carries), midnight-ledger (376) and midnight-zk (282). Forty-three people merged at least one. Three
merged more than half.

By the employers people name on their public profiles, those naming Shielded Technologies merged 49.3% of the
changes, and those of one other employer take the total past half. About 44% were merged by people who name no
employer, so the true count of employers may be one.

**What it does and does not show.** It counts who did merge, which is close to who can. Merging code is not the same
as changing the chain: a new runtime still needs Midnight's two governance bodies ([[m-midnight-rule-changes]]).
