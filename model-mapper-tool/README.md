# model-mapper-tool

A future tool for working with the **4D-Bio** practice model as structured data:
mapping its competencies to external frameworks (ISCB, ACTIVE, …), validating the
mappings, and rendering them for the docs site and for self-assessment.

**Status:** scaffolding only. No tool code yet. The active work right now is the
knowledge base in [`memory/`](memory/), which is being written so that a future
agent (or contributor) can pick this up with full context.

## Folder layout

| Path | Purpose |
|---|---|
| [`memory/`](memory/) | **Start here.** Everything known about the 4D-Bio model: its structure, source frameworks, linking rules, a full content inventory of the current site, a proposed data model, open questions, and a dated learning log. Written for an agent to consume. |
| `data/raw/` | Original source exports of the model (e.g. the author's spreadsheet). Nothing committed yet. |
| `data/processed/` | Normalized, machine-readable model data produced from `raw/`. |
| `data/schema/` | The schema those files conform to. Draft lives in [`memory/proposed-data-model.md`](memory/proposed-data-model.md). |
| `src/` | Tool source code (none yet). See [`src/README.md`](src/README.md). |
| `docs/` | Design docs and specs for the tool itself (none yet). See [`docs/README.md`](docs/README.md). |
| `tests/` | Tests (none yet). |

## How this folder relates to the rest of the repo

The repo root is the **4D-Bio MkDocs site** (`docs/`, `mkdocs.yml`). This folder is
a self-contained workspace for the tool and is **not** part of the published site
(`docs_dir: docs/` excludes it). Keep site content in `../docs/`; keep model data,
tooling, and agent memory here.
