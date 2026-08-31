# Competency linking rules

> Taught by the author on 2026-08-31.

Every **Level-3 competency** is either *linked* or *plain text*. The distinction is
semantic, not cosmetic — it records whether the competency already exists in an
external framework.

## Rule

- **The competency exists in an external framework** → render it as a **link** to
  that framework's entry. Use the framework's own identifier and wording.
- **The competency does not exist in any referenced framework** → render it as
  **plain text**, authored by 4D-Bio. No link.

## Consequences for the data model

Each competency record needs:

- `text` — the wording shown to the reader.
- `framework_ref` — `null` for plain-text competencies; otherwise:
  - `framework` — `iscb` | `active` | (future: others)
  - `id` — e.g. `D3` (ISCB code) or an ACTIVE practice name
  - `url` — the exact link
  - `verbatim` — `true` if `text` is the framework's own wording, `false` if the
    author paraphrased (currently ISCB entries appear verbatim; confirm).
- `source` — who authored this competency line: `iscb` / `active` / `4d-bio`.
  For linked competencies this equals the framework; for plain-text it is `4d-bio`.

## Edge cases observed (see `open-questions.md`)

- Some **Level-2 groups** are named after a framework (e.g. *"Awareness and Task–AI
  Alignment (ACTIVE Framework)"*) but their **Level-3 child is plain text with no
  link**. So a framework-named group does *not* guarantee linked children.
- A few ACTIVE references appear **inline inside a plain-text competency's
  description** rather than as their own Level-3 item (e.g. Discernment ›
  "Biological integrity verification" mentions "Critical Verification Protocols
  (ACTIVE Framework)" mid-text). These need to be normalized into discrete
  competency records or explicit annotations.
- One ISCB group (`F3`) is filed under "Data Science Domain Knowledge" on the site;
  verify F is a Data Science domain letter in ISCB v3.0.
