# Repolex Knowledge Graph of scikit-hep/cuda-histogram

RDF knowledge graph data for [scikit-hep/cuda-histogram](https://github.com/scikit-hep/cuda-histogram), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download scikit-hep/cuda-histogram
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 35a3585ddb27ce167483b2f3c415b04f8341f620
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 35a3585ddb27ce167483b2f3c415b04f8341f620
│           └── chunk-001.nq.gz
├── blob
│   ├── 00a7b00c94e08b86c765d47689b6523148c46eec.nq.gz
│   ├── 03a029fc67caadf027db645dd5b952fdacc36fc8.nq.gz
│   ├── 06573ff31dad71122075eea7d24e8d68256d2657.nq.gz
│   ├── 0707de1dcbc8a4693adf76bf5c0e89726d7ac52a.nq.gz
│   ├── 0afbb20a2f7f7b4a17c85d8e2f16012f216f41e5.nq.gz
│   ├── 147e8143370ec8dd70ce31049a0ca54085e9d9a0.nq.gz
│   ├── 2f15b730666220c677c954a7d79dafe612d3a419.nq.gz
│   ├── 40f94d97c027d592f564b8dcfd492b873b5c6056.nq.gz
│   ├── 499d58ac891ab9bd6774487eaf52a7c31fe74ddc.nq.gz
│   ├── 58754f5d372f45fab735ae40df380b8ebe465f7f.nq.gz
│   ├── 5bb2b22f78faec68eeed9a623c15cad2747c9eba.nq.gz
│   ├── 6705b4394f4e5671dc112c07050b26d243955c98.nq.gz
│   ├── 6a3704468b67233accb8ea1e4b9b4c3dcb5f75c2.nq.gz
│   ├── 729cb90b979d3a308a6c9e175688cd81b27f8090.nq.gz
│   ├── 7ac91f0eb3d73288d140f8d17af463e02a0e0d50.nq.gz
│   ├── 7f7b3a4c1c1a171b07b1d1edacf1450fbbf42e08.nq.gz
│   ├── 8da6f6583e832148d00ad5d1a29b96e78c98278b.nq.gz
│   ├── 8fb235d7045be0330d94bcb3abd2ac43badaa197.nq.gz
│   ├── 922152e96a04a242e6fc40f124261d74890617d8.nq.gz
│   ├── 9698af362327991b7c8a00d0187d53336b624ca6.nq.gz
│   ├── aa00841a3f38e45e55b7ae543102d74fb95bb3e6.nq.gz
│   ├── b0657e75f524a7b426b368d70f601a3ce37d3ec9.nq.gz
│   ├── babe7ca4799b86ba14cd602f9ba5faa251e18c9d.nq.gz
│   ├── bd128c56970ccb7bef68716ebf725f10d4f0bfd2.nq.gz
│   ├── c03daf3a81bffcf887a7de03ee790d2dec699c7c.nq.gz
│   ├── c25845b1240ce733307c3f346ad72481f3fd5153.nq.gz
│   ├── cf6f01ae2bb5f58645342f386c725877ad64485e.nq.gz
│   ├── d4bb2cbb9eddb1bb1b4f366623044af8e4830919.nq.gz
│   ├── dbe857f48e49405cd65acaf83b089aa838f3574f.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ea58ef7f460fdabf93e651128b16c0cbddb0568b.nq.gz
│   ├── f046f579618d67e2e7588cdabeca5de151ba2b35.nq.gz
│   └── f36541e3c149ba146faf812d4422530731967b2e.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 35a3585ddb27ce167483b2f3c415b04f8341f620.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 41 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[scikit-hep/cuda-histogram](https://github.com/scikit-hep/cuda-histogram)

---
*Parsed on 2026-10-28 by [repolex](https://repolex.ai)*
