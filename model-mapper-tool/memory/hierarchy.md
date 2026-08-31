# The 4D-Bio hierarchy (definitive)

> Taught by the author on 2026-08-31, correcting an earlier misreading by the
> assistant. This is the authoritative structure.

The model has **four nesting levels** below the top-level capability. Each level is
a distinct kind of thing — they are not interchangeable, and an earlier draft that
treated them as generic nested bullets was wrong.

```
Capability                      (one of the four D's — one site page)
└── Practice area               LEVEL 1
    └── Category / group        LEVEL 2
        └── Competency          LEVEL 3
```

## Capability (page level)

One of **Delegation, Description, Discernment, Diligence**. Each has:

- an **Anthropic definition** — quoted verbatim from the 4D framework;
- a **bioinformatics definition** — 1–3 sentences written by the 4D-Bio author.

## Level 1 — Practice area

A **professional situation** in which the capability applies. Phrased as a gerund
activity, e.g. *"Framing the biological problem and formulating the solution
roadmap"*, *"Documenting and tracking AI interactions and software parameters for
reproducibility"*. On the site these are the `##` headings. A capability has 3–6 of
them.

## Level 2 — Category / group

A **cluster of related competencies** within a practice area. A group is one of two
kinds:

- **Author-defined group** — a short noun phrase coined for 4D-Bio, e.g.
  *"Hypothesis generation"*, *"High-context prompting"*, *"Provenance logging"*.
- **Framework-derived group** — named after a domain/theme of an external
  framework, e.g. *"Data Science Domain Knowledge (ISCB Competency Framework)"*,
  *"Bioscience domain knowledge (ISCB Competency Framework)"*, *"Awareness and
  Task–AI Alignment (ACTIVE Framework)"*. These exist to attach that framework's
  competencies into the practice area.

## Level 3 — Competency

The **atomic skill**. This is the unit the mapping tool ultimately operates on.
A competency is expressed in one of two forms, and the form encodes whether it
already exists in an external framework:

- **Linked competency** — the competency *exists in an external framework*. It is
  written as a **hyperlink** to that framework's entry, and carries the framework's
  own identifier and wording, e.g.
  `[ISCB D3: Use data science methods suitable for the size and complexity of the
  data.](https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7940)`
- **Plain-text competency** — the competency does *not* exist in any framework
  4D-Bio references. It is written by the 4D-Bio author as a capability statement
  (usually a single sentence, verb-first), with **no link**, e.g.
  *"Leverage domain expertise to formulate novel biological hypotheses and
  questions in research areas where existing data or AI training models are
  limited."*

A single Level-2 group can contain multiple Level-3 competencies, and can mix
linked and plain-text ones.

See [`competency-linking-rules.md`](competency-linking-rules.md) for the full rules
and [`content-inventory.md`](content-inventory.md) for every current instance.

## Mapping back to the original spreadsheet

| Spreadsheet column (approx.) | Model level |
|---|---|
| Capability / "D" | page |
| Practice area | Level 1 |
| Category / group | Level 2 |
| Competency | Level 3 |
| Framework + link (if any) | attribute of the Level-3 competency |
