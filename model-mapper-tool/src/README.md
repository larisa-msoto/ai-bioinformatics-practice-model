# src/

Source code for the `model-mapper-tool`. **Nothing here yet.**

## Intended responsibilities (not yet designed)

- **Parse** the 4D-Bio model from `../data/` (and/or extract it from the site under
  `../../docs/`) into the schema in [`../memory/proposed-data-model.md`](../memory/proposed-data-model.md).
- **Validate** — check every linked competency resolves, every id is unique and
  stable, every group's `kind` is consistent with its children.
- **Map / crosswalk** — relate 4D-Bio competencies to external frameworks (ISCB,
  ACTIVE, …) in either direction, and surface coverage gaps.
- **Render** — emit Markdown for the docs site and/or a self-assessment view.

Before writing code, read all of [`../memory/`](../memory/) and resolve the
relevant items in [`../memory/open-questions.md`](../memory/open-questions.md) with
the author.
