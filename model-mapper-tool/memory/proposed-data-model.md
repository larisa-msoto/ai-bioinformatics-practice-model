# Proposed data model (draft)

Not approved by the author. A starting point for representing 4D-Bio as structured
data so the `model-mapper-tool` can validate, version, and render it.

## Shape

```yaml
# one file per capability, e.g. data/processed/delegation.yaml
capability:
  id: delegation                 # delegation | description | discernment | diligence
  name: Delegation
  anthropic_definition: >
    Setting goals and deciding whether, when, and how to engage with AI.
  bioinformatics_definition: >
    ...author's 1-3 sentence framing...
  practice_areas:
    - id: framing-the-biological-problem
      name: Framing the biological problem and formulating the solution roadmap
      groups:
        - id: hypothesis-generation
          name: Hypothesis generation
          kind: author                 # author | framework
          framework: null              # iscb | active | ...  (set when kind: framework)
          competencies:
            - id: delegation.framing.hypothesis-generation.1
              text: >
                Leverage domain expertise to formulate novel biological
                hypotheses and questions where existing data or AI training
                models are limited.
              source: 4d-bio           # 4d-bio | iscb | active
              framework_ref: null      # null for plain-text competencies
        - id: data-science-domain-knowledge
          name: Data Science Domain Knowledge
          kind: framework
          framework: iscb
          competencies:
            - id: iscb.D3
              text: Use data science methods suitable for the size and complexity of the data.
              source: iscb
              framework_ref:
                framework: iscb
                code: D3
                numeric_id: 7940
                url: https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7940
                verbatim: true
```

## Field notes

- **`kind` on a group** is independent of whether its competencies are linked. A
  `framework` group has usually-linked children; an `author` group has plain-text
  children — but exceptions exist (see [`competency-linking-rules.md`](competency-linking-rules.md)).
- **`framework_ref.code`** for ISCB is `<domainLetter><level>` (e.g. `D3`). Keep the
  numeric id too — the site uses two URL forms and the numeric one is more common.
- **`verbatim`** distinguishes framework wording from author paraphrase. Assume ISCB
  entries are verbatim until confirmed otherwise.
- **Stable `id`s** matter — they are how a mapping, a self-assessment answer, or an
  external framework crosswalk will reference a competency. Never renumber; add.
- **Provenance per competency**: consider `added_in` (model version) and
  `sources: []` (list of citation keys from `../../docs/references.md`).

## Open modeling questions

- Should an inline framework mention inside a plain-text competency (e.g.
  Discernment "Critical Verification Protocols (ACTIVE Framework)") be its own
  competency record, or an `annotations: []` field on the parent? → author call.
- Do practice areas need an explicit ordering field, or is file order enough?
- One competency currently maps to one framework entry. Will the tool need
  many-to-many (one 4D-Bio competency ↔ several ISCB codes)? Likely yes for the
  "crosswalk" use case — model `framework_refs` as a list from the start.
