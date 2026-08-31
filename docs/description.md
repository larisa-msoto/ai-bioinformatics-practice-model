# Description

!!! note ""
    According to [Anthropic's 4D Framework for AI fluency](https://www-cdn.anthropic.com/334975cdec18f744b4fa511dc8518bd8d119d29d.pdf?ref=hackshackers.com) Description means _"Effectively describing goals to prompt useful AI behaviors and outputs."_.

In Bioinformatics, description requires effectively communicating goals, context, and assumptions to AI agents in the form of instructions to drive the expected behaviors and make outputs reproducible and interpretable.

!!! abstract "On this page"
    1. [Translating biological knowledge into precise AI instructions](#1-translating-biological-knowledge-into-precise-ai-instructions)
    2. [Structuring raw biological data for AI model context](#2-structuring-raw-biological-data-for-ai-model-context)
    3. [Documenting and tracking AI interactions and software parameters for reproducibility](#3-documenting-and-tracking-ai-interactions-and-software-parameters-for-reproducibility)

In the tables below, the **Category** tag shows where each competency comes from:
<span class="tag tag-iscb">ISCB</span> and <span class="tag tag-active">ACTIVE</span> competencies are drawn from existing frameworks;
<span class="tag tag-4dbio">4D-Bio</span> competencies are original to this practice model.

---

## 1. Translating biological knowledge into precise AI instructions

| Category | Competency |
|---|---|
| **Bioscience domain knowledge** <span class="tag tag-iscb">ISCB</span> | [**A3** — Work at depth in at least one technical area aligned with the life sciences.](https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7950) |
| **Domain knowledge translation** <span class="tag tag-4dbio">4D-Bio</span> | Translate deep domain-specific biological mechanisms, technical terminology, and experimental variables into precise computational instructions for AI execution. |
| **High-context prompting** <span class="tag tag-4dbio">4D-Bio</span> | Write structured, unambiguous prompts using advanced techniques to guide AI analysis. |
| &nbsp; | Handle prompts as one more scientific resource that needs to be tested, documented, reported, reproduced, and cited. |
| **Adaptive instruction** <span class="tag tag-4dbio">4D-Bio</span> | Redirect AI systems dynamically when they drift from the expected analytical path or task boundaries. |

## 2. Structuring raw biological data for AI model context

| Category | Competency |
|---|---|
| **Metadata standardization** <span class="tag tag-4dbio">4D-Bio</span> | Apply highly descriptive system instructions that translate experimental designs and dataset annotations into clear parameters for AI ingestion. |
| **Bioscience domain knowledge** <span class="tag tag-iscb">ISCB</span> | [**B3** — Prepare life science data for computational analysis.](https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7938) |

## 3. Documenting and tracking AI interactions and software parameters for reproducibility

| Category | Competency |
|---|---|
| **Provenance logging** <span class="tag tag-4dbio">4D-Bio</span> | Record every prompt text, system configuration, model version, and seed value used to achieve a computational result. |
| **Automated documentation** <span class="tag tag-4dbio">4D-Bio</span> | Generate exhaustive documentation that describes the functions, parameters, and expected outputs of AI-assisted code. |
| **Version control** <span class="tag tag-4dbio">4D-Bio</span> | Track changes to scripts, prompts, and configurations regularly using version control systems like GitHub. |
