---
id: method-shortest-stave
type: method
title: "The shortest-stave test"
description: "For each link, ask how few parties, acting together, could control it. The score is the lowest answer."
status: developing
visibility: public
tags: [method]
links:
  - rel: derived-from
    to: src-edi
  - rel: related
    to: nakamoto-coefficient
    note: "the single-subsystem measure it extends"
  - rel: related
    to: src-glassnode-ark-spectrum
    note: "another multi-dimension framework, without a minimum"
  - rel: raises
    to: q-multi-body-threshold
  - rel: raises
    to: q-srinivasan-lee-wording
created: 2026-11-19
updated: 2026-11-26
---

A barrel holds water only up to its shortest stave. A network holds trust the same way: a thousand block
producers do not help if one party can rewrite the rules, or if one bug can reach every node.

**The test.** List every link that has to stay out of one party's hands. For each, count the smallest group
that, acting together, could control it. The score is the lowest count.

**The links.** Eight are counted here: who makes the blocks, whose software they run, who can merge code, who
sets the rules, who pays for upkeep, where it is hosted, which countries, and who holds special keys or lists.

**Counting rules.**

- State the threshold. "More than half" is the default. Where a network's own decisive share is different, such
as a third to halt or four fifths to pass, say so, and do not compare the rows as if they were alike.
- Keep both figures when two fair ways of counting disagree.
- A link nobody has counted yet is a gap, not a zero. A link decided off-chain has no public record to count,
and that is said in so many words.
- Every figure carries its date, its source and how far it has been verified.

**Three ways a link can give way.** The links are not all the same kind of weakness, and each is labelled.

- *By agreement*: a small group acting together, or leaned on together. Who makes the blocks, who can merge code,
who sets the rules, who pays for upkeep, who holds special keys.
- *By accident*: one fault shared across the network. Whose software the nodes run. Many hands write an
implementation, so a count of 1 does not mean one party is in charge. It means one bug could reach most of the
network.
- *From outside*: a party that is not part of the network at all. Where it is hosted, and in which countries.

The score is still the lowest count of all. Beside it the lowest count of each kind is shown, because "one bug from
a stall" and "one company from control" are different things to say about a network, and a single number hides
which is meant.

**Where it comes from.** The Nakamoto coefficient counts the entities needed to control one subsystem. In 2017
Balaji Srinivasan and Leland Lee proposed measuring several subsystems and taking the minimum; their essay has not
yet been opened for this research, so that description rests on secondary accounts. The Edinburgh
Decentralisation Index measures five layers with public data and is the starting point here. It does not yet count
node implementations, merge rights, or who votes.

**Limits.** "Control" can mean passing a change or blocking one, and the two give different counts. A rule that
needs several bodies to agree is harder to capture than the count for any one body suggests. A count says how
few parties are needed, not how likely they are to act together.
