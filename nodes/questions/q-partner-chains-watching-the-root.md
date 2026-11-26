---
id: q-partner-chains-watching-the-root
type: question
title: "Could partner chains watch the root?"
description: "A suggestion put as a question: a partner chain that chose to, run by parties that do not make the root's blocks, could publish what it sees of the root, with a voice but no veto. By choice, not a duty for every partner chain."
status: developing
visibility: public
tags: []
links:
  - rel: related
    to: v-certificate-transparency
    note: "the precedent: owned roots made visible by a log anyone can check"
  - rel: related
    to: public-root-of-trust
    note: "anyone can check it"
  - rel: related
    to: distance-from-the-root
    note: "the root witnesses its partner chains; this asks the reverse"
  - rel: related
    to: method-shortest-stave
    note: "a weakest-link score, kept in public"
  - rel: related
    to: src-hoskinson-2026-07-27
    note: "the founder on more than one kind of bridge, for checks and balances"
  - rel: derived-from
    to: src-mip-0024
    note: "every Midnight node \"follows and validates Cardano while validating a block\""
created: 2026-11-23
updated: 2026-11-23
---

Partner chains draw their trust from the root. This research asks whether they could also give something back by
watching it.

**What is already there.** Cardano's record is open to anyone who runs a node, and partner chains already check it
as they work. A Midnight proposal describes how: "every node follows and validates Cardano while validating a block,
so Cardano state reaches Midnight with no one carrying it" (MIP-0024, proposed July 2026). The eyes exist.

**What is not.** No partner chain publishes what it sees of the root, and none is proposed to. A partner chain that
chose to could keep the root's weakest-link score in public and up to date, and raise the alarm on censorship, a
fork or a governance anomaly. Nothing in that needs a chain of its own: an index or a public log can keep a score,
and the Edinburgh index already measures some of it. What a partner chain would add is a set of watchers that are
already checking the root, with their own record of what they saw.

**What would decide whether it helps.**

- **A voice, not a veto.** An overseer able to override the root would become a new root above it. Change would stay
  with the root's own recorded votes.
- **Different hands.** It would be run by parties that do not make the root's blocks, and that are independent of
  each other. A watcher run by the same pools would be checking itself.
- **Someone to pay, and someone to answer.** Watching costs money, and the treasury paying for it would put it back
  under the root's own votes. And an alarm changes nothing unless the root's governance is bound to answer it in
  public.
- **By choice.** It is a job some partner chains could take on, beside everyone else who watches the root, not a
  duty for every partner chain.

The precedent is [[v-certificate-transparency]]: after one of the web's certificate roots was breached in 2011, the
repair was not more roots but a public log that anyone can check. A suggestion of this research, put as a question;
nobody who would build it has been asked.
