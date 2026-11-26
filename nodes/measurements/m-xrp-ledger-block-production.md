---
id: m-xrp-ledger-block-production
type: measurement
title: "The XRP Ledger's default list holds 35 validators under 35 different domains"
description: "The default list holds 35 validators, each under a different domain. Four fifths of them have to agree."
status: developing
visibility: public
network: net-xrp-ledger
dimension: dim-block-production
value: 28
unit: validators
threshold: "80% of the 35 validators on the default list"
as_of: 2026-11-19
verified: agent
tags: [block-production, xrp-ledger]
links:
  - rel: derived-from
    to: src-vl-ripple
  - rel: derived-from
    to: src-xrpl-validators-data
created: 2026-11-19
updated: 2026-11-19
---

The default list held 35 validators on 19 November 2026, each registered under a different domain: exchanges,
universities, infrastructure firms, individuals, and one under Ripple's own domain.

The ledger's consensus needs four fifths of trusted validators to agree, which is 28 of them. The domains were
read directly; the quorum is from the ledger's documentation as read by a research assistant.

The validators are many and varied. Which ones count is decided by the published lists, which is the stave to
look at for this network.
