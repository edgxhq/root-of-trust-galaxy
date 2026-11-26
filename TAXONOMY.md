# TAXONOMY — cluster map and classification rules

Read with `SCHEMA.md` (format, edges) and `CLAUDE.md` (voice, process). The site's clusters come from typed
links, so a node's place is decided by what it links to, not by its tags.

## Hubs

| Cluster | Hub | Members |
|---|---|---|
| The idea | `root-of-trust` | `public-root-of-trust`, the older roots (`web-pki`, `dns-root`, `hardware-root-of-trust`, `newspaper-hash`), the lineage sources |
| Distance from the root | `distance-from-the-root` | the five `level-*` concepts, `rule-or-setting`, the connected systems (`hydra-heads`, `reeve-records`, `wrapped-assets`), `net-midnight` and its ties |
| The shortest stave | `method-shortest-stave` | the eight `dim-*` dimensions, every `m-*` measurement, `nakamoto-coefficient`, the Edinburgh index |
| What can be built on a root | `what-a-root-can-carry` | the capability dimensions (`dim-programs`, `dim-assets`, and `dim-scaling`, which is described and not scored), their measurements, and the four types of root (`class-*`) that the first two decide |
| Who owns a root | `tier-public`, `tier-pseudo-public` | the networks, placed by the test in `SCHEMA.md`; the claim that supports the comparison |
| Everyday uses | the `app-*` nodes | each links to the level it usually sits at and the dimension it depends on; vignettes of kind `use` illustrate them |
| The networks | each `net-*` root | its measurements and the vignettes that happened on it |
| What a root is for | `vignettes` by kind | `failed`, `held`, `adapted`, `use` |
| Findings | the `ins-*` insights | each insight links the claims, measurements and sources it rests on |

## Rules of thumb

- A **measurement** links to exactly one network and one dimension (through its fields) and to at least one
  source.
- A **vignette** links with `illustrates` to the dimension it tests. A vignette that illustrates nothing
  measurable is a story, not evidence; park it.
- A **source** links to one to three concepts or networks, most specific first, with a note saying why.
- A **claim** links `supports` or `contradicts` to measurements and sources; an **insight** links to claims.
- A **planned** measurement has a live measurement for the same network and dimension beside it. The build
  refuses one that stands alone.
- An **application** links `instance-of` to the level it usually sits at, or `related` to the dimension it
  depends on.
- A **question** is linked with `raises` from the node that prompted it and `answers` from the node that
  settles it.

## Tags

Tags feed search and the scorecard filters. Use the dimension's slug (`block-production`, `node-software`,
`merge-rights`, `rule-changes`, `funding`, `hosting`, `geography`, `standing-keys`), the network's name, and
`midnight`, `lineage`, `stake-pools`, `method` where they apply.
