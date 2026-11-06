# Repolex Knowledge Graph of open-dingtalk/dingtalk-stream-sdk-python

RDF knowledge graph data for [open-dingtalk/dingtalk-stream-sdk-python](https://github.com/open-dingtalk/dingtalk-stream-sdk-python), parsed by [repolex](https://repolex.ai).

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
rlex download open-dingtalk/dingtalk-stream-sdk-python
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 8d8bb1c630848fee1ae8c7bdd11bc1b78097b611
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 8d8bb1c630848fee1ae8c7bdd11bc1b78097b611
│           └── chunk-001.nq.gz
├── blob
│   ├── 0184c33832e0a6e241403aa5e2b8d0be5d2b22dd.nq.gz
│   ├── 065eb32d916ba342a715eb920251734d8045adc6.nq.gz
│   ├── 0692430feaeb25ac36c7eb730edb045321b56cf9.nq.gz
│   ├── 09e3a2725bae3ec2b201fb3d08eb210c1ec5ade1.nq.gz
│   ├── 16a346c89c8d3fd873dc28b14b641d58f5755677.nq.gz
│   ├── 1d57a0ab329554f1a2e2a9e9398c33fd57c7b135.nq.gz
│   ├── 1f26b3efc9d7e2625318b8ec9b3dd627de0078cc.nq.gz
│   ├── 1f95094173290fcd8575273aac507a970a6a0704.nq.gz
│   ├── 20c28ea8f3175dd9f2552f41b6d9eec28df9c8ec.nq.gz
│   ├── 217152c39836f7fef56f9b06284bdbae2e532410.nq.gz
│   ├── 2692997a2d666fa3bad137af8460c527f5f8dea4.nq.gz
│   ├── 2e702b062d45dc784d9c4cab5114247a510c447e.nq.gz
│   ├── 661595f0051937c67c0e39f43715b473a7327cf0.nq.gz
│   ├── 67c31ff98641a70e9f2aa176e3a0c6c9d320c79b.nq.gz
│   ├── 6cb924da29ddbbad1dc391bb0c597bbf8a5df2c4.nq.gz
│   ├── 7e76538a17fbd971274fbc47c36123b2222938fe.nq.gz
│   ├── 7ece288f87ea3d1649b5da0ca4dae2accc8d1028.nq.gz
│   ├── 80c717a87d4e3281df84772690a30cb02c78ae35.nq.gz
│   ├── 855ee85e561a5f142f3e1978039fffeacc61af79.nq.gz
│   ├── 94919c53d17a235c735faa18ff3ff954b587b0bd.nq.gz
│   ├── 99a3c65de9ff718e9cad03338cbd0d53b13b862a.nq.gz
│   ├── a12d0922a13d8aae6470c1d62da496e429b7b52f.nq.gz
│   ├── ad72584bc69944ee741278d5b6ce42a6a85b36fd.nq.gz
│   ├── ae18d5763ca9de3d9f996302439298edf03b380f.nq.gz
│   ├── b6607ed5125ab57ffe8a0566907f3537df202ccc.nq.gz
│   ├── be4d69f10ae6a7ea38d29489545a83a78bd0ee82.nq.gz
│   ├── c50d9e4849b2210d11da5f4a0fd2ad470181acf5.nq.gz
│   ├── dc709741a4e5fffa0560c472dcc7e616b8963421.nq.gz
│   ├── df9559eaed722a0a0a2fd27c22a0a12812fdb992.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── f057ef60b2188a77f4f5244dc69c2ea1800fa155.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 8d8bb1c630848fee1ae8c7bdd11bc1b78097b611.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 39 files
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

[open-dingtalk/dingtalk-stream-sdk-python](https://github.com/open-dingtalk/dingtalk-stream-sdk-python)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
