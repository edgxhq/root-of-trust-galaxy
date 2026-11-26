---
id: m-xrp-ledger-rule-changes
type: measurement
title: "An XRP Ledger rule change needs four fifths of listed validators for two weeks"
description: "An XRP Ledger rule change needs four fifths of listed validators for two weeks."
status: developing
visibility: public
network: net-xrp-ledger
dimension: dim-rule-changes
value: 25
unit: "listed validators"
threshold: "more than 80% of trusted validators for two weeks; the threshold stood at 25 in October 2026"
as_of: 2026-10-09
verified: agent
decided_on_ledger: true
tags: [rule-changes, xrp-ledger]
links:
  - rel: derived-from
    to: src-xrpl-amendments
created: 2026-11-19
updated: 2026-11-20
---

"If an amendment receives more than 80% support for two weeks, the amendment passes", and the result is recorded
on the ledger. An amendment enabled on 9 October 2026 had 32 validations against a threshold of 25.

The validators that count are the ones on the trusted lists, so this stave rests on the one beside it.
