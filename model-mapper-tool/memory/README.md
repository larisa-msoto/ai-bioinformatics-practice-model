# 4D-Bio model memory

This directory is a persistent knowledge base about the **4D-Bio practice model**.
It is written for a **future agent** that will build the `model-mapper-tool`. Treat
it as the source of truth for *what the model is and how it is structured*; the
prose on the live site (`../../docs/`) is the source of truth for *wording*.

## Read in this order

1. [`model-overview.md`](model-overview.md) — what 4D-Bio is, who it's for, current status.
2. [`hierarchy.md`](hierarchy.md) — **the definitive 4-level structure.** Read carefully; an earlier draft got this wrong.
3. [`source-frameworks.md`](source-frameworks.md) — Anthropic 4D, ISCB v3.0, ACTIVE: what each is and how the model references it.
4. [`competency-linking-rules.md`](competency-linking-rules.md) — when a competency is a link vs. plain text.
5. [`content-inventory.md`](content-inventory.md) — full dump of every practice area / group / competency currently on the site.
6. [`proposed-data-model.md`](proposed-data-model.md) — a draft schema for representing the model as data.
7. [`open-questions.md`](open-questions.md) — known inconsistencies and decisions still owned by the author.
8. [`glossary.md`](glossary.md) — terms.
9. [`learning-log.md`](learning-log.md) — dated record of what the author taught, newest first.

## How to maintain this memory

- When the author teaches something new, **add it to the relevant topic file** and
  **append a dated entry to `learning-log.md`**. Don't only log it — fold it into
  the topic file so a reader never has to reconstruct state from the log.
- When something here is contradicted, **correct the topic file** and note the
  correction (with date) in `learning-log.md`. Keep superseded claims out of the
  topic files.
- Keep claims that are *taught* separate from claims that are *inferred*. Mark
  inferences explicitly and move them to `open-questions.md` if unconfirmed.
- Every ISCB/ACTIVE reference should carry its exact URL and identifier. Never
  paraphrase an identifier.

## Provenance

Authoritative source: **Larisa M. Soto** (larisamsoto@bioinfopro.org), author of the
4D-Bio model. Anything not attributable to her or to the site content is an
inference and must be labeled as such.
