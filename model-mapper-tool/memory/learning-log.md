# Learning log

Dated record of what the author taught about the model. Newest first. Each entry:
what was taught, which topic files were updated, and any correction made.

---

## 2026-08-31 — Session 1 (initial memory build)

**Context:** The author asked for a readability review of the 4D-Bio site, then
asked to stand up this `model-mapper-tool/` folder and start a persistent memory
for a future agent.

**Taught:**

1. **The hierarchy is four levels, not three.** The assistant's first reading —
   *practice area → competency → description + refs* — was **wrong**. Correct
   structure:
   - Level 1: **Practice area**
   - Level 2: **Category / group**
   - Level 3: **Competency**
   Recorded in [`hierarchy.md`](hierarchy.md).

2. **Competency linking rule.** A Level-3 competency that exists in an external
   framework is rendered as a **link** to that framework's entry. One that does not
   exist in any referenced framework is **plain text** authored by 4D-Bio.
   Recorded in [`competency-linking-rules.md`](competency-linking-rules.md).

3. The model was **originally an Excel spreadsheet**; its columns line up with the
   four levels, and merged cells carried the practice-area grouping that the
   bulleted Markdown loses. Recorded in [`model-overview.md`](model-overview.md).

**Also captured (from the site + this conversation, not explicitly taught — verify):**

- Full content inventory of all four capability pages → [`content-inventory.md`](content-inventory.md).
- Roles of the three source frameworks → [`source-frameworks.md`](source-frameworks.md).
- Draft data model → [`proposed-data-model.md`](proposed-data-model.md).
- Open questions and inconsistencies → [`open-questions.md`](open-questions.md).

**Corrections made this session:**

- Reverted the assistant's earlier interpretation of the hierarchy (see item 1).
  The readability suggestions given before this correction (definition lists with
  "competency" as the bold term) were based on the wrong level mapping and must be
  redone against the correct four-level structure.

**Still open:** everything in [`open-questions.md`](open-questions.md) — notably the
ACTIVE framework's expansion and source, the Level-2 term, and whether the original
spreadsheet can be committed to `data/raw/`.
