# Repolex Knowledge Graph of asimov-modules/asimov-ethereum-module

RDF knowledge graph data for [asimov-modules/asimov-ethereum-module](https://github.com/asimov-modules/asimov-ethereum-module), parsed by [repolex](https://repolex.ai).

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
rlex download asimov-modules/asimov-ethereum-module
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 7f10a8ec82b05f95f1d07be31101c514207c8340
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 7f10a8ec82b05f95f1d07be31101c514207c8340.nq.gz
│   └── repolex
│       └── 7f10a8ec82b05f95f1d07be31101c514207c8340
│           └── chunk-001.nq.gz
├── blob
│   ├── 0ce7e79e0b4754b41a1ee28ef7687b7c0d572637.nq.gz
│   ├── 10b359dd05935c73efb064470f9ecda90f6d28aa.nq.gz
│   ├── 18fbaf73492f25b0c2d2dc5b3b016a7b0a51c17a.nq.gz
│   ├── 29eb3cbe3acebdb63c383c0fcd9f12442f9bbe81.nq.gz
│   ├── 337e6919b0e43cd2eb3bbe95ca63810fd04879af.nq.gz
│   ├── 6b23d61018f43b840f8d2ff3b45a1c02d76df38d.nq.gz
│   ├── 75e3b65f99b29f48ab230e3eab3de8d0b7a9229f.nq.gz
│   ├── 7e0b4f2430d4e97ab1f29270aa4c0944920063d7.nq.gz
│   ├── 8acdd82b765e8e0b8cd8787f7f18c7fe2ec52493.nq.gz
│   ├── 920eafda4f1fd9c8cf3c86108d3b19508570b09c.nq.gz
│   ├── 975ecbd8cc6fb434fad0fe0053e7735de8d3b41d.nq.gz
│   ├── 9fe50de16e59d550235aa6d7d15ee12ddf054414.nq.gz
│   ├── a36fedab8db68b26a76fbbf1de1f549e4a12261b.nq.gz
│   ├── af9908b08f4b33c32a0080af73f53bc0fa0cdce4.nq.gz
│   ├── cf42f6893594e2f8be2b722de51123d65e4d61c4.nq.gz
│   ├── df21de5332feac730d959c76b867d285cf4732b5.nq.gz
│   ├── e3e57a8ce4ccbf74759a6df8fa4a3980ff1c9209.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── efb98088164f5786b17e83ed384971fc3c74f93c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 7f10a8ec82b05f95f1d07be31101c514207c8340.nq.gz
├── filetree
│   └── 7f10a8ec82b05f95f1d07be31101c514207c8340.nq.gz
├── issue
│   └── issue.nq.gz
└── tag
    └── tag.nq.gz

14 directories, 28 files
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

[asimov-modules/asimov-ethereum-module](https://github.com/asimov-modules/asimov-ethereum-module)

---
*Parsed on 2026-09-28 by [repolex](https://repolex.ai)*
