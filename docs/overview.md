# Overview

4D-Bio maps the day-to-day skills of a practicing bioinformatician onto a single
framework for working with generative AI. This page explains **how the model is
built** and **how to read the four capability pages**.

!!! note "Diagram placeholder"
    A visual of the four capabilities and how the three source frameworks nest
    will go here.

## How the model is built

4D-Bio combines three existing frameworks:

| Framework | What it contributes |
|---|---|
| **[Anthropic's 4D framework for AI fluency](https://www-cdn.anthropic.com/334975cdec18f744b4fa511dc8518bd8d119d29d.pdf?ref=hackshackers.com)** | The top-level structure: four capabilities &mdash; Delegation, Description, Discernment, Diligence &mdash; that together describe fluent, responsible AI use. |
| **[ISCB Competency Framework v3.0](https://competency.ebi.ac.uk/framework/iscb/3.0)** | The established, profession-wide bioinformatics competencies. 4D-Bio links each practice area to the specific ISCB competencies it draws on, so nothing is invented from scratch. |
| **ACTIVE Framework** | AI-specific pedagogy: guidance on task&ndash;AI alignment, verification confidence, and countering cognitive offloading. Referenced where it sharpens a skill. |

The 4D framework gives the shape, ISCB grounds the model in the wider profession,
and ACTIVE adds the teaching-and-learning perspective for AI.

## How to read a capability page

Each of the four pages &mdash; [Delegation](delegation.md), [Description](description.md),
[Discernment](discernment.md), [Diligence](diligence.md) &mdash; is organized the same way:

- A short **definition** of the capability, in general terms and then for bioinformatics.
- A set of **professional practice areas** (the `##` headings). These are the situations
  where the capability shows up in real work.
- Within each practice area, the concrete **skills** it requires, each with a plain-language
  description and, where relevant, a link to the matching **ISCB** competency or **ACTIVE**
  practice.

## The four capabilities at a glance

| Capability | Core question | Focus |
|---|---|---|
| **[Delegation](delegation.md)** | Should AI do this, and how? | Framing the problem, decomposing it into tasks, choosing tools, orchestrating agentic workflows. |
| **[Description](description.md)** | Did I communicate the goal well enough to reproduce it? | Translating biology into precise instructions, structuring data as context, logging provenance. |
| **[Discernment](discernment.md)** | Can I trust this output? | Judging biological plausibility, benchmarking against baselines, catching hallucinations and artifacts. |
| **[Diligence](diligence.md)** | Am I accountable for what this produces? | Governance and compliance, data longevity, preserving manual skill, mentoring and community. |

## Status

4D-Bio is an early public draft (**v0.1**). Content, structure, and terminology are
all still open for discussion. See [How to Contribute](contributing.md).
