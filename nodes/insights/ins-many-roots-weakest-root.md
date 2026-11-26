---
id: ins-many-roots-weakest-root
type: insight
title: "With many roots, the weakest one sets the level"
description: "The web has about a hundred certificate roots, any of which can vouch for any site. In 2011 one was breached."
status: developing
visibility: public
verified: agent
confidence: medium
tags: [lineage]
links:
  - rel: derived-from
    to: web-pki
  - rel: derived-from
    to: dns-root
  - rel: derived-from
    to: v-diginotar-2011
  - rel: derived-from
    to: v-certificate-transparency
  - rel: supports
    to: claim-one-root
created: 2026-11-19
updated: 2026-11-19
---

The web's padlock rests on about a hundred roots, and each can vouch for any site. In 2011 one of them was
breached and issued 531 fraudulent certificates; about 300,000 addresses, nearly all in Iran, were served a
false certificate for Google.

The repair is instructive. The web did not reduce its roots to one. It added a public, append-only log
beneath them, so anyone can see every certificate issued. It reached for the thing a public ledger starts
with.

The internet's naming system took the other path and has one root by design, with one steward.

A public ledger is the first kind of root that can be single without having an owner. That is the case for
one root, and for holding it to a hard test.
