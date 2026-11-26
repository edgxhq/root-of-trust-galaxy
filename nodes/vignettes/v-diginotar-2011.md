---
id: v-diginotar-2011
type: vignette
title: "One of a hundred roots"
description: "One of the web's certificate authorities was breached and issued 531 false certificates."
status: developing
visibility: public
verified: agent
kind: failed
when: "June to September 2011"
tags: [failed]
links:
  - rel: illustrates
    to: web-pki
  - rel: illustrates
    to: claim-one-root
  - rel: derived-from
    to: src-fox-it-diginotar
created: 2026-11-19
updated: 2026-11-19
---

The investigators' report: "Traces of hacker activity started on June 17th and ended on July 22nd." "In total 531
fraudulent certificates have been issued." One was for Google. "Around 300.000 unique requesting IPs to google.com
have been identified. Of these IPs >99% originated from Iran".

**What it cost what was built on it.** Browsers removed the authority's roots within weeks. Every site that had
bought its certificates there had to replace them, and the company did not survive.

**What it shows.** Each of the web's roots can vouch for any site, so the whole system was as strong as its
weakest root. See [[web-pki]].

The figure of 300,000 is addresses, not people.
