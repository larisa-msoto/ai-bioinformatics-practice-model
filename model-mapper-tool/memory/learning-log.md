# Learning log

Dated record of what the author taught about the model. Newest first. Each entry:
what was taught, which topic files were updated, and any correction made.

---

## 2026-08-31 — Session 2 (capability-page restructure)

**Context:** The author asked to restructure the four capability pages on the site
around the corrected four-level hierarchy. Not new model facts, but decisions that
the mapper tool should mirror.

**Decisions applied to the site (`../../docs/{delegation,description,discernment,diligence}.md`):**

1. **Practice areas are numbered** (`## 1.`, `## 2.`, …) in both the body and the
   right-sidebar table of contents. Anchor slugs are now `#1-<slug>` etc.
2. Each page carries an **"On this page"** contents strip (an `abstract`
   admonition) listing the numbered practice areas.
3. **Each practice area is rendered as one table**: column 1 = **Category**
   (Level 2) with an origin tag, column 2 = **Competency** (Level 3). When a
   category has multiple competencies, the category cell is filled on the first
   row and left blank (`&nbsp;`) on continuation rows — mirroring the merged cells
   in the original spreadsheet.
4. **Origin tags** on every category: `ISCB`, `ACTIVE`, `4D-Bio` (styled pills,
   defined in `../../docs/stylesheets/extra.css`). `ISCB`/`ACTIVE` = from an
   existing framework; `4D-Bio` = original to this model. → for the data model this
   is `group.kind` + `group.framework`.
5. **Normalization done while restructuring:** in Discernment › "Evaluating the
   biological plausibility of AI outputs", the ACTIVE reference "Critical
   Verification Protocols" — previously an inline second bullet inside "Biological
   integrity verification" — is now its **own category row** tagged `ACTIVE`. This
   resolves one item in [`open-questions.md`](open-questions.md).
6. ISCB competency cells reformatted from `ISCB D3: <text>` to `**D3** — <text>`
   (the `ISCB` prefix is now redundant with the tag).

**Config changes:** `mkdocs.yml` — removed `toc.baselevel: 2` (it was pushing every
heading down one level and creating a duplicate page `<h1>`), set `toc.toc_depth: 2`,
added the `tables` extension explicitly and `extra_css`.

**Not changed:** competency wording is otherwise verbatim from the previous site
text. The `content-inventory.md` snapshot still reflects the pre-restructure
wording and counts; re-extract from the live pages before building data.

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
