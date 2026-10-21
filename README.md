# Repolex Knowledge Graph of executablebooks/sphinx-remove-toctrees

RDF knowledge graph data for [executablebooks/sphinx-remove-toctrees](https://github.com/executablebooks/sphinx-remove-toctrees), parsed by [repolex](https://repolex.ai).

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
rlex download executablebooks/sphinx-remove-toctrees
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 07a98640c03f767b18c65b7004208b4ae10c7359
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 07a98640c03f767b18c65b7004208b4ae10c7359
│           └── chunk-001.nq.gz
├── blob
│   ├── 0dbae47a76a4e7bf55b8871ee7b7d8cea3b0af1d.nq.gz
│   ├── 32c58fc2a4b4faa80f9ba27c31797c48d62faa81.nq.gz
│   ├── 3c59fc5081b276368d18ad22d09fa18b42222a46.nq.gz
│   ├── 4b92808f785c4f3a10a44279f635d994644d9582.nq.gz
│   ├── 4f9f7f1888ebc7a39842dfb54c2c02be36007fb8.nq.gz
│   ├── 51ced2655e3cbe7ad0c95b17714765134b532728.nq.gz
│   ├── 55a8379008c95f50603d89b4960fa2596b4bb48c.nq.gz
│   ├── 5f023fcae40f9bba1c982efea2da2e0a955e7c8f.nq.gz
│   ├── 6870809431d3489fa08bfb8616dceb27c9bdef13.nq.gz
│   ├── 87f4404677598f8a98af62fd988080dff4e4376f.nq.gz
│   ├── a6c1900d2446675188d1465f104b1485637c2e7e.nq.gz
│   ├── c0be12ace9a4792897400f35574f113e5154e393.nq.gz
│   ├── c6736d4758c487ad00748c40e9da7d2ef0a22262.nq.gz
│   ├── dab6ba48f3dcb26eae65920afb84113b1ebb141f.nq.gz
│   ├── f564d0295ef14a20d28d67d7633f9875a0c092bd.nq.gz
│   ├── f85ad5fc2b2f7840a0eef4b20bcdd77f82b58bd9.nq.gz
│   ├── f88f6e90851fd8ff4246ab12a67b8e8565ce5273.nq.gz
│   ├── fcdb0ec7dc5f38721f8547afb7a5ab691df6e053.nq.gz
│   └── feee9cdbd46428076016ff9339eb2c722992437d.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 07a98640c03f767b18c65b7004208b4ae10c7359.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 27 files
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

[executablebooks/sphinx-remove-toctrees](https://github.com/executablebooks/sphinx-remove-toctrees)

---
*Parsed on 2026-10-21 by [repolex](https://repolex.ai)*
