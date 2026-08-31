# Open questions

Ambiguities and decisions owned by the author (Larisa M. Soto). Resolve by asking,
not by guessing. Move resolved items into the relevant topic file with a date.

## Structure & terminology

- **Level-2 naming.** Author-defined groups are short noun phrases
  ("Hypothesis generation"); framework-derived groups are framework domain names
  ("Data Science Domain Knowledge (ISCB Competency Framework)"). Is "group" /
  "category" the settled term for Level 2? The site currently gives Level 2 no
  label at all (just a bullet).
- **Level-3 wording for author competencies.** Plain-text competencies are full
  capability sentences, not short names. Should they also get a short handle for
  display / linking, or stay sentence-only?
- **Framework-named group, plain-text child.** e.g. Delegation › "Awareness and
  Task–AI Alignment (ACTIVE Framework)" has a plain-text child with no link. Is
  the group "framework-derived" (named after ACTIVE) or "author" (the competency
  is authored)? Affects `kind` in the data model.
- **Inline framework references.** Discernment › "Biological integrity
  verification" folds "Critical Verification Protocols (ACTIVE Framework)" into the
  description text instead of making it a discrete Level-3 item. Normalize how?

## Frameworks

- **ACTIVE — expansion and canonical source.** Is the EdArXiv preprint
  `https://osf.io/preprints/edarxiv/vhwbn_v1` the ACTIVE framework? What does
  ACTIVE stand for? Is there a canonical list of its practices/letters?
- **ISCB URL form.** Site uses both `/competency/details/<numericId>` and
  `/competencies/<code>` (H3). Standardize on one for the data model.
- **ISCB domain letters.** Confirm the letter→domain map, especially `F`
  (site files `F3` under "Data Science Domain Knowledge").
- **ISCB level.** Every code cited ends in `3`. Confirm `3` = competency level and
  whether 4D-Bio will ever reference other levels.

## Model governance

- **Versioning.** Site says v0.1. How are model versions cut, and does each
  competency need an `added_in` marker?
- **The original spreadsheet.** Can a copy go in `data/raw/`? It is the cleanest
  source for the parent–child relationships.
- **Mapping direction.** Is the tool's job (a) 4D-Bio → external frameworks,
  (b) external frameworks → 4D-Bio (coverage gaps), (c) practitioner self-
  assessment against 4D-Bio, or all three?
- **Many-to-many.** Can one 4D-Bio competency map to several ISCB codes?

## Content issues spotted (site, not model)

- `discernment.md` — "Critical Verification Protocols" reads as a run-on inside a
  bullet; candidate for its own competency.
- Some Level-3 items bundle two distinct competencies in one bullet
  (e.g. Description › "High-context prompting"). Split when moving to data.
