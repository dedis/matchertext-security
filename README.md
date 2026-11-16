# Matchertext injection containment: artifacts

This repository collects the artifacts of the executed containment
experiments. Each one is a submodule pinned at the commit that the paper
measures.

| Path | Content |
|---|---|
| `sqlite/` | SQLite with matchertext holes (`M'(...)'` values, `[...]` names) and the opt-in strict mode. `sqlite/README.md` gives the build modes; `sqlite/changes.diff` shows every change. |
| `parse5/` | parse5 with matchertext holes (`<tag [v]>`, `name=[v]`, `<![MDATA[v]]>`), `composeHtml`, and the guarded serializer. |
| `archive/` | The input snapshots of the CVE corpus, stored as `sha256/<digest>`, so that the corpus can be rebuilt after the upstream sources change. |

Clone with the submodules:

```sh
git clone --recursive <this repository>
```
