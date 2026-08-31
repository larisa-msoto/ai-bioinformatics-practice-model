# Model overview

## What 4D-Bio is

**4D-Bio** is a professional practice model for AI-augmented bioinformatics. It is a
community-maintained map of the skills a practicing bioinformatician needs in order
to use generative AI responsibly. It takes the four capabilities of **Anthropic's
4D framework for AI fluency** — Delegation, Description, Discernment, Diligence —
and, under each, enumerates the professional situations ("practice areas") and the
concrete competencies a bioinformatician needs, cross-referencing established
frameworks (primarily the **ISCB Competency Framework v3.0**) wherever a competency
is already catalogued there.

## Purpose

- Give the bioinformatics community a shared vocabulary for AI-related skills.
- Help educators and curriculum designers decide what to teach.
- Help team leads and hiring managers write job descriptions and AI-use guidelines.
- Let individual practitioners self-assess.

## Audience

Practicing bioinformaticians; educators / curriculum designers; team leads and
hiring managers; trainees.

## Origin and format

- The model was **originally authored as a spreadsheet (Excel)**, with columns that
  correspond to the hierarchy levels (see [`hierarchy.md`](hierarchy.md)). The row
  grouping in the spreadsheet (shared/merged cells for a practice area) carried the
  parent–child relationship that the current bulleted Markdown pages lose.
- It is now published as a **MkDocs Material** site on GitHub Pages, with community
  discussion via **giscus** on every page.
- Repo: `github.com/larisa-msoto/ai-bioinformatics-practice-model`
  Site: `https://larisa-msoto.github.io/ai-bioinformatics-practice-model/`

## Status

Early public draft, **v0.1**. Structure, wording, and terminology are all still
open. Community input is invited through GitHub Discussions and page edits.

## The `model-mapper-tool` (future)

The intended tool will represent 4D-Bio as structured data so that mappings to
external frameworks can be authored, validated, versioned, and rendered — both into
the docs site and into a self-assessment view. Nothing is built yet; see
[`proposed-data-model.md`](proposed-data-model.md).
