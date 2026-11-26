---
id: hardware-root-of-trust
type: concept
title: "Hardware roots of trust"
description: "The chip a device trusts when it starts. One per platform, with one owner."
status: developing
visibility: public
class: class-owned
verified: agent
owner: "the manufacturer"
tags: [lineage, precursor]
links:
  - rel: instance-of
    to: root-of-trust
  - rel: derived-from
    to: src-globalplatform-rot
  - rel: derived-from
    to: src-nist-roots-of-trust
created: 2026-11-19
updated: 2026-11-20
---

A phone or a computer starts from a small component it has no way to check: the hardware root of trust.
Everything loaded afterwards is verified against it.

The industry's requirements are explicit about ownership: "A Root of Trust SHALL have a single identifiable
owning entity." For a device that is the right design. For a record shared by people who do not trust each
other, an owner is the thing to avoid.
