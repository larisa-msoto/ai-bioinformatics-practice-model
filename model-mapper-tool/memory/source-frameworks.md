# Source frameworks

4D-Bio is assembled from three external frameworks. Each plays a distinct role.

## 1. Anthropic's 4D framework for AI fluency — *the structure*

Provides the four top-level capabilities and their definitions.

| Capability | Anthropic definition (verbatim) |
|---|---|
| **Delegation** | "Setting goals and deciding whether, when, and how to engage with AI." |
| **Description** | "Effectively describing goals to prompt useful AI behaviors and outputs." |
| **Discernment** | "Accurately assessing the usefulness of AI outputs and behaviors." |
| **Diligence** | "Taking responsibility for what we do with AI and how we use it." |

- Authors: Prof. Rick Dakan, Prof. Joseph Feller, and Anthropic.
- Licence: CC BY-NC-SA 4.0 (4D-Bio inherits this licence).
- PDF: `https://www-cdn.anthropic.com/334975cdec18f744b4fa511dc8518bd8d119d29d.pdf`
- Companion site: `https://www.anthropic.com/learn/claude-for-you`

## 2. ISCB Competency Framework v3.0 — *the grounding*

The established, profession-wide competency catalogue for bioinformatics. 4D-Bio
links to it wherever a competency it needs already exists there, so the model is
not invented from scratch.

- Paper: Brooksbank et al. (2024), *The ISCB competency framework v.3*,
  *Bioinformatics Advances* 4(1) vbae166 — `https://doi.org/10.1093/bioadv/vbae166`
- Browsable hub (EMBL-EBI): `https://competency.ebi.ac.uk/framework/iscb/3.0`
- **Competency URL patterns seen on the site (both are in use — normalize later):**
  - `https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/<numericId>`
  - `https://competency.ebi.ac.uk/framework/iscb/3.0/competencies/<code>` (e.g. `.../competencies/H3`)
- **Competency codes** are a domain letter + level number, e.g. `D3`, `F3`, `A3`.
  The trailing `3` appears to denote the framework's competency *level*; every code
  referenced by 4D-Bio so far ends in `3`.
- **ISCB domains referenced so far** (letter → how the site labels it):
  - A, B, C → "Bioscience Domain Knowledge"
  - D, E → "Data Science Domain Knowledge"
  - F → labelled under "Data Science Domain Knowledge" in one place (`F3`), review
  - G, H, I → "Computer Science Domain" / "Computer Science Domain Knowledge"
  - J, K, L, M → "Professional Conduct"

Full list of ISCB codes 4D-Bio currently cites, with URLs, is in
[`content-inventory.md`](content-inventory.md).

## 3. ACTIVE Framework — *the AI pedagogy*

A pedagogical framework for teaching AI use, brought in where it sharpens a skill
(task–AI alignment, verification confidence, countering cognitive offloading).

- Almost certainly the source cited on the site as: *"A pedagogical framework and
  its first classroom implementation in response to automation bias, cognitive
  debt, and the verification paradox"*, EdArXiv — `https://osf.io/preprints/edarxiv/vhwbn_v1`
  (**inferred link — confirm with author**, see [`open-questions.md`](open-questions.md)).
- "ACTIVE" is treated as an acronym but its expansion is **not yet confirmed**.
  Named ACTIVE sub-practices seen in the model:
  - "Awareness and Task–AI Alignment"
  - "Critical Verification Protocols"
  - "Verification Confidence Calibration"
  - "Transparent integration"
  - "Iterative skill development"

## Other references cited on the site (not structural)

- Wen Bin Goh et al. (2026), *Rethinking bioinformatics expertise in the era of
  artificial intelligence*, npj Digital Medicine 9, 398 —
  `https://doi.org/10.1038/s41746-026-02777-1`
- `github.com/melissawm/open-source-ai-contribution-policies` — linked from
  Diligence › "AI regulatory alignment" as a pointer to global AI legal frameworks.
