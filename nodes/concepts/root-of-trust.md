---
id: root-of-trust
type: concept
title: "Root of trust"
description: "The one record you do not have to take on anyone's word. Everything else you trust, you trust because it leads back there."
status: developing
visibility: public
verified: main
tags: [lineage]
links:
  - rel: derived-from
    to: src-nist-roots-of-trust
  - rel: derived-from
    to: src-globalplatform-rot
  - rel: derived-from
    to: src-hoskinson-2021-09-04
created: 2026-11-19
updated: 2026-11-19
---

A root of trust is the point where checking stops. Everything above it can be verified against it; the root
itself has to be relied on.

The term comes from computer security. The United States standards body defines roots of trust as "highly
reliable hardware, firmware, and software components that perform specific, critical security functions". In
hardware a root of trust has an owner: one industry standard requires "a single identifiable owning entity".
On the web the roots are certificate authorities, and there are about a hundred of them.

Charles Hoskinson applied the term to Cardano in 2021: "the point is that you want to establish a stable root
of trust. That's what we've done here". He also said what it costs: "this is the single most expensive thing
to establish".

The older roots all share one property: somebody owns them. See [[public-root-of-trust]] for the kind that
nobody owns.
