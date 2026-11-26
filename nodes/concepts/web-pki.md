---
id: web-pki
type: concept
title: "The web's certificate roots"
description: "The padlock in a browser rests on about a hundred certificate roots, and any one of them can vouch for any site."
status: developing
visibility: public
class: class-owned
verified: agent
owner: "about a hundred certificate authorities"
tags: [lineage, precursor]
links:
  - rel: instance-of
    to: root-of-trust
  - rel: derived-from
    to: src-fox-it-diginotar
  - rel: derived-from
    to: src-rfc-6962
created: 2026-11-19
updated: 2026-11-20
---

When a browser shows a padlock it has checked the site's certificate against a list of trusted roots. Mozilla's
list held 118 roots in November 2026. Each root can vouch for any site on the web.

That makes the system as strong as its weakest root. In 2011 one of them, DigiNotar, was breached. See
[[v-diginotar-2011]].

The repair did not reduce the number of roots. It added a public, append-only log beneath them, so that every
certificate issued can be seen by anyone. See [[v-certificate-transparency]].
