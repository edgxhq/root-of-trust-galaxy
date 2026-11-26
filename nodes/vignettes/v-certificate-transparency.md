---
id: v-certificate-transparency
type: vignette
title: "After the breach, a public log"
description: "The web answered its certificate breaches by adding a public record of every certificate issued."
status: developing
visibility: public
verified: agent
kind: adapted
when: "2013 onwards"
tags: [adapted]
links:
  - rel: illustrates
    to: web-pki
  - rel: illustrates
    to: root-of-trust
  - rel: derived-from
    to: src-rfc-6962
created: 2026-11-19
updated: 2026-11-19
---

Two years after a certificate authority was breached, a standard was published for "publicly logging the
existence of Transport Layer Security (TLS) certificates as they are issued or observed, in a manner that allows
anyone to audit certificate authority (CA) activity and notice the issuance of suspect certificates".

**What it shows.** A system of owned roots repaired itself by adding an append-only record that anyone can
check. It could not remove its owners, so it made them visible. A public ledger starts from that record.
