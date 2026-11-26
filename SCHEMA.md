# SCHEMA — research graph format

One markdown file per node, in `nodes/<type>/<id>.md`. The graph is the union of all node files; edges live in
frontmatter. Git is the source of truth; everything else (indexes, the site's `graph.json`) is derived and can
be rebuilt.

The format follows the one used for the Wisdom of Data research graph: minimal, Obsidian-compatible (wikilinks
resolve), plain YAML frontmatter, and conformant with the Open Knowledge Format (one concept per file, `type`
always set, `title`, `description`, `tags`, and trust fields). Typed `links:` are a superset extension.

What is different here: this graph carries **measurements**. A measurement is a number about a network, with
its date, its source and how far it has been verified. Numbers are never written into other nodes without a
measurement node behind them.

## Node file

```markdown
---
id: m-bitcoin-block-production     # = filename, kebab-case, globally unique, permanent
type: measurement                  # see Node types
title: Three mining pools make more than half of Bitcoin's blocks
description: One plain sentence. Shown on cards and in the galaxy.
status: developing                 # seed | developing | stable | parked
visibility: public                 # public | internal  (internal never reaches the mirror or the site)
verified: main                     # main | agent | secondary | unverified   (see Verification)
tags: [block-production]
links:
  - rel: derived-from
    to: src-mempool-space
created: 2026-11-19
updated: 2026-11-19
---

Body: 30 to 300 words. The statement first, then what it does and does not show.
Inline [[wikilinks]] are allowed and count as weak `related` edges; typed edges go in frontmatter only.
```

## Node types

| type | directory | id prefix | what it holds |
|---|---|---|---|
| `concept` | nodes/concepts/ | none | a definable idea or thing: root of trust, a level, a kind of system |
| `network` | nodes/networks/ | `net-` | a ledger network. `kind: root` for one that asks to be trusted in its own right, `kind: satellite` for one that hangs off another |
| `dimension` | nodes/dimensions/ | `dim-` | one link in the chain of things that must stay out of one party's hands (also called a stave) |
| `measurement` | nodes/measurements/ | `m-` | one number about one network on one dimension, with date, source and verification |
| `claim` | nodes/claims/ | `claim-` | a falsifiable assertion; must link its evidence |
| `question` | nodes/questions/ | `q-` | an open question or standing challenge; closed by editing status and linking the answer |
| `insight` | nodes/insights/ | `ins-` | a synthesis worth surfacing; must link its provenance |
| `vignette` | nodes/vignettes/ | `v-` | a real event that shows a root of trust failing, holding or adapting |
| `source` | nodes/sources/ | `src-` | one external source: what it is, where it is, when it was read |
| `method` | nodes/methods/ | `method-` | a procedure: the shortest-stave test, how a dimension is counted |
| `application` | nodes/applications/ | `app-` | a kind of everyday use: what people do with a ledger, and what that use takes from a root |

## Type-specific fields

**`network`**

```yaml
kind: root                 # root | satellite
class: class-general       # roots: the type of root it is. The build checks it against the root's own measurements
ownership: tier-public     # roots: tier-public or tier-pseudo-public. The build checks it too (see below)
aim:                       # roots outside tier-public, required: what it says it is for, in its own words
  text: "Peer-to-peer electronic cash"   # the short form shown under its name on the map
  quote: "Bitcoin: A Peer-to-Peer Electronic Cash System"   # the words it rests on, exactly
  sources:
    - to: src-bitcoin-whitepaper
      at: "#page=1"
level: bridged             # satellites and other connected things: root | rooted | anchored | bridged | unrooted
level_fit: rough           # optional: exact (default) | rough. "rough" means nearest fit, a reading and not a verdict
level_note: "..."          # optional: one or two sentences on why it sits there and how firmly
orbits: net-cardano        # satellites: the root it hangs off
paths:                     # optional: where it could move to, and on whose say-so. Drawn as a faint twin on the map
  - level: anchored
    basis: their-proposal  # their-proposal (written in its own process) | spoken (described, not written) | idea (ours)
    label: if its committee bridge is adopted
    note: What would change, in one or two sentences.
    sources:
      - to: src-mip-0023
        at: "#abstract"    # the section of the source the statement rests on
        label: MIP-0023, abstract
ties:                      # satellites: each tie to the root
  - tie: Its token lives on the root
    state: in-place        # in-place | planned | proposed | named | spoken | missing | unspecified
    permanence: unknown    # rule | setting | unknown. Use rule or setting only where a source says which
    ring: anchored         # only on a tie that would move what lives on it nearer: anchored (the root witnesses
                           # its record) or rooted (the root enforces the outcome). Other ties leave it out
    note: NIGHT is a Cardano native asset.
    sources:               # one or more, each pointing at the passage
      - to: src-midnight-whitepaper
        label: Tokenomics whitepaper
```

Tie states: `in-place` (working today), `planned` (in a published plan), `proposed` (a written proposal, not
adopted), `named` (named as a next step, not specified), `spoken` (described in a talk, nothing written),
`missing`, `unspecified`. A `path` with `basis: idea` is this research's own speculation and must say so in its
note; none is made public without the stewards' say.

`level` may also appear on a `concept` node that names a kind of connected system (Hydra heads, wrapped
assets), so the site can place it on a ring.

**`dimension`**: `question` (the plain question, "Who makes the blocks?"), `short` (a one-word label), `order`,
and `group`: `link` (the default: one of the things that must stay out of one party's hands, counted for the
score) or `capability` (something a root can or cannot do; shown beside the score and never part of it).

A link also says which way it gives way, `kind`: `agreement` (a small group acting together), `accident` (one
fault shared across the network, which is what the software link measures) or `outside` (a host or a state that is not
part of the network). The score is the lowest count of all; the lowest of each kind is shown beside it.

A capability also says how its value is drawn:

```yaml
group: capability
scale: steps               # steps | rate
steps: ["Transfers only", "Limited scripts or built-in functions", "General programs"]   # value is the step, from 0
steps_short: ["transfers only", "limited", "general"]                                    # optional, for labels
# or
scale: words               # described in sentences, with no bar and no ranking
facets:                    # the headings every network is described under
  - key: in_root
    label: In the root itself
```

`scale: rate` exists for parked figures only. **No figure for transactions a second is published for any
network.** A transaction on one ledger is not the same amount of work as on another, so the count compares unlike
things. How a root is built to carry more is a described capability (`dim-scaling`). The figures counted in
November 2026 are kept as parked, internal nodes.

**`measurement`**

```yaml
network: net-bitcoin
dimension: dim-block-production
value: 3                   # a number, or "none" (nothing of this kind exists), or null (no count)
value_hi: 56               # optional: the upper figure when two fair ways of counting disagree
unit: mining pools
threshold: more than half of blocks
reason: null               # only when value is null: unmeasured (nobody here has counted it yet)
                           #   or unrecorded (decided off-chain: there is no public record to count)
as_of: 2026-11-19
verified: main
state: planned             # optional: live (default) | planned. See "Planned figures"
stage: Makes blocks on test networks; in beta     # planned only: how far the work has got
expected: no date given                           # planned only: when, in the makers' words
```

A described measurement has words in place of a number:

```yaml
dimension: dim-scaling
summary: Small on purpose; channels beside it          # a few words, for a cell or a label
facets:                                                # one sentence for each heading of the dimension
  in_root: Kept small on purpose. The size of a block is fixed by the consensus rules.
  beside: "Lightning: payments through a network of channels, each opened and closed on Bitcoin."
  building: Not written up here.
```

Each sentence rests on a source the node links. "Not written up here" is this research's gap, said plainly.

A measurement with `scored: false` is **context** for a link: a sourced figure that helps read the count, such as
how many node implementations exist beside how many would have to share a fault. It never feeds a score. The map's
panel lists it under the link, and its `summary`, a few words, is shown under the figure on the scorecard. Give the
same context for every network where a sourced figure exists, not for one network alone.

For a link, the value answers one question: **how few parties, acting together, could control this link?** For a
capability it is the step reached, or the rate counted, with `value_hi` for a ceiling under present rules. State the
threshold used. When a network's own decisive threshold is not one half (a third to halt, two thirds or more
to pass), say so in `threshold` and in the body, so rows are not compared as if they were alike.

**Ownership.** A root is `tier-public` (publicly owned infrastructure) only when three of its measurements say so:
its rule-changes measurement and its funding measurement both carry `decided_on_ledger: true` (the decision is made
by votes recorded on the ledger) and have a count, and its standing-keys measurement is `none`. Otherwise it is
`tier-pseudo-public`. The build refuses any other label. `decided_on_ledger` is set only where a source shows the
vote is recorded on the ledger.

**`concept` with `kind: ownership-tier`**: a tier of ownership: `rule` and `order`. The first tier is the centre of
the map.

**`concept` with `kind: root-class`**: a type of root, which is a segment of the map. `rule` (the one test that
places a root in it, in words) and `order`. A root's `class` must agree with its measurements: general programs
make it `class-general`; otherwise other assets enforced by the ledger make it `class-built-in`; otherwise
`class-money`. Older roots with an owner are `class-owned`. The build refuses a class the measurements do not
support, so a root cannot be moved to the centre by editing one line.

**`application`**: `everyday` (what it looks like in ordinary life), `needs` (what it takes from a root, in one
sentence), `level` (where it usually sits: a level, or `varies`), `order`. Real cases are vignettes that link to it
with `illustrates`. An application with no such vignette is a description, not evidence, and is listed as a gap.

**`vignette`**: `kind` (`failed`: a weak root gave way; `held`: a strong root under attack or a natural event;
`adapted`: a root that changed itself to meet a new threat; `use`: a root doing ordinary work), `when`,
and `illustrates` edges to the dimensions or concepts it shows.

**`source`**: `url`, `publisher`, `source_kind` (`primary-data | protocol-doc | repository | standard | paper |
talk | post | news | blog`), `accessed`, and for video `video_id`. In a video's body, every moment quoted is a
link to that moment: `At [00:01:46](https://www.youtube.com/watch?v=ID&t=106s): "…"`.

## Planned figures

A measurement with `state: planned` says what a figure **would become** once work that is close ships. It never
replaces the live figure: it is a separate node (`m-<network>-<dimension>-planned`) that sits beside it, and the
site draws the two differently in every view.

Work counts as close only if all three hold, for any network:

1. it is built in the open;
2. it already runs on a network other people can join, a public test network or the main network in a small way;
3. its makers name it as their next step.

A proposal that is only written does not qualify; mention it in the body of the live measurement instead. A
planned figure needs a source for each of the three points and cannot be `unverified`. Where the figure depends on
other people's choices, as a second node implementation depends on operators running it, say so in the body.

## Verification

Every `measurement`, `vignette`, `claim` and `insight` carries `verified`:

| value | meaning | where it may appear |
|---|---|---|
| `main` | checked directly against the primary source or raw data | everywhere |
| `agent` | a research agent read the primary source; not yet re-checked | the site, labelled |
| `secondary` | a news report, blog or other secondary source | the site, labelled |
| `unverified` | from memory, a search snippet or an unopened source | the site only in draft mode; never published |

Raising a node's `verified` level is a contribution in its own right. Say in the body what was opened and when.

## Edge relations (`rel`)

Keep to this vocabulary.

- `supports` / `contradicts`: evidence relations (claim or insight with source, measurement or another claim)
- `derived-from`: this node's content came from that node or source
- `measures`: generated by the build from a measurement's `network` and `dimension` fields; do not write by hand
- `illustrates`: a vignette shows this dimension, concept or claim at work
- `refines`: a narrower or improved version of
- `part-of`: composition
- `instance-of`: example of a general category
- `related`: meaningful association; the `note` says why
- `raises` / `answers`: node and question
- `cites`: source cites source

Edges are directional as written but queried both ways; do not add reciprocal duplicates.

## Conventions

- **A dangling link is a to-do, not an error.** The build lists them.
- **A gap is a to-do too.** A network with no measurement on a dimension is drawn as a gap on the site and
  offered as a contribution.
- **One fact-cluster per node.** When two fair ways of counting disagree, keep both: `value` and `value_hi`,
  or two measurement nodes.
- **Insights** must have `supports` or `derived-from` links.
- **Updates**: edit in place and bump `updated`; git history is the change record. When a number changes,
  the old figure and its date stay in the body under `## History`.
- **Hold every network to the same test.** A measurement that flatters Cardano needs the same evidence as one
  that does not.
- **Public nodes name no private files.** Provenance is a `source` node with a URL, never a path in the
  working repository.
- **A source points at the passage.** Link the file at the commit it was read at (not a branch, which moves, and
  not the repository's front page), and give the section on the tie or path that uses it (`at: "#section"`).
  Quote the words the statement rests on. A video's quoted moments are links to the second; a reading of a live
  ledger names the endpoint and says the exact call and the date in the body.
