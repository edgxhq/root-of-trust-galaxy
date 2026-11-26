# Contributing

This graph is meant to be argued with. A correction, a better source, a count nobody has made yet, or a fairer
way to count are all welcome. Every network is held to the same test, Cardano included.

## Suggest a change

The easiest way is the form:
**[Suggest a change](https://github.com/edgxhq/root-of-trust-galaxy/issues/new?template=suggest-a-change.yml)**.
You do not need to fork anything or edit a file. Say what should change, and give the source and the passage it
rests on.

If you would rather edit the file, a pull request against one file under `nodes/` is welcome too. The format is
in [SCHEMA.md](SCHEMA.md).

## How a suggestion is decided

A written rule decides, the same for everyone, and each decision is explained.

**A fact**, such as a number, a date, a quote or who did what. The source decides. If a public source says it at
the passage given, it goes in. What is left to decide is how far it has been checked, and the graph shows that
beside it:

| Tag | Shown as | Meaning |
|---|---|---|
| `main` | checked | checked directly against the primary source or the raw data |
| `agent` | first read | a research assistant read the primary source; not yet re-checked |
| `secondary` | reported | rests on a news report, a blog or another secondary source |

So most suggestions are not accepted or refused. They go in with a tag. A suggestion without a source stays open,
labelled `needs a source`, until someone finds one.

**A judgement call**, such as which group a root belongs in, a threshold, or whether a way of counting is fair to
a network. No one person settles it, a steward included.

- You give your answer in the issue, with your reasons. A steward gives theirs, with reasons, against the test in
  [SCHEMA.md](SCHEMA.md), which is the same for every network.
- If the two agree, the change goes in.
- If they do not, both ways of counting are kept. The current one stays on the map, and yours is recorded beside
  it with its reasons, as an open question, until more evidence settles it.
- Where two stewards answer, each writes their answer before seeing the other's, so that neither leads.

## What happens to an issue

1. A steward labels it `needs a source` or `judgement call`, or makes the change straight away.
2. The change is made, and appears here at the next update.
3. The issue is closed with a line or two naming the rule the decision rests on, and one of three labels:
   `in the graph` (with the tag it carries), `two views kept`, or `not taken up` (the source does not say it, or
   it is outside what the graph covers). The node's history names the issue.

Each update of this repository is a fresh snapshot that replaces its history. So a pull request is applied by
hand, named in the node's history, and then closed with a note rather than merged.

## Licence

The graph is shared under the Creative Commons Attribution 4.0 licence ([LICENSE](LICENSE)). Anyone may copy,
share and adapt it, with credit to the Root of Trust Galaxy and a link here. By suggesting a change, you agree
that it may be published under the same licence.

## What the graph keeps to

- Every figure has a source and a date. A source links the passage it is cited for; a repository is linked at a
  fixed commit, not its front page.
- No figure for transactions a second, for any network. A transaction on one ledger is not the same amount of
  work as on another, so how a network is built to carry more is described in words.
- Ideas are put as questions, not as proposals.
