# Content inventory (snapshot: 2026-08-31, pre-restructure wording)

> Structure note: as of Session 2 the live pages render each practice area as a
> table (Category | Competency) with numbered practice areas and origin tags, and
> the Discernment "Critical Verification Protocols" ACTIVE item is now its own
> category row. The hierarchy below is unchanged; only presentation and that one
> split differ. Re-extract before building data.


Full extraction of every Level-1 practice area, Level-2 group, and Level-3
competency currently on the site, with linking status. Legend:

- `[L]` linked competency (exists in an external framework)
- `[P]` plain-text competency (authored by 4D-Bio, no link)
- Group kind: `(author)` or `(framework: …)`

This is a **snapshot for reference**; the site is the live source. Re-extract after
any content change. Wording is trimmed for brevity — do not treat as verbatim.

---

## Delegation

*Anthropic:* "Setting goals and deciding whether, when, and how to engage with AI."
*Bioinformatics:* deep understanding of biological context; breaking complex
problems into small independent tasks; deciding which tasks suit generative AI;
choosing the best AI/non-AI tool per task; implementing agentic workflows to best
practice.

### L1: Framing the biological problem and formulating the solution roadmap
- **Hypothesis generation** (author)
  - `[P]` Leverage domain expertise to formulate novel biological hypotheses and questions where existing data or AI training models are limited.
- **Innovative problem solving** (author)
  - `[P]` Devise alternative strategies or creative workarounds when standard computational approaches or AI models fail on a complex biological problem.
- **Workflow architecture selection** (author)
  - `[P]` Select the most effective combination of traditional bioinformatics tools and AI models for a specific biological problem.
- **Cross-disciplinary integration** (author)
  - `[P]` Incorporate multidisciplinary context and biological constraints to define the boundaries of a computational solution.

### L1: Deconstructing the solution roadmap into actionable tasks
- **Modular task decomposition** (author)
  - `[P]` Break down a complex bioinformatics problem into clear, individual tasks that can be performed independently.
- **Technical acceptance criteria definition** (author)
  - `[P]` Define the exact expected outputs, data formats, and quality benchmarks for each task before execution.
- **Awareness and Task–AI Alignment** (framework: ACTIVE)
  - `[P]` Critically assess a task's complexity to determine if AI integration is appropriate or if it risks bypassing essential learning.
- **Data Science Domain Knowledge** (framework: ISCB)
  - `[L]` ISCB **D3** — Use data science methods suitable for the size and complexity of the data. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7940
  - `[L]` ISCB **F3** — Make appropriate use of bioinformatics tools and resources. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7942

### L1: Orchestrating autonomous AI workflows to execute tasks at scale
- **Multi-agent architecture design** (author)
  - `[P]` Architect end-to-end automated workflows that chain AI agents to execute complex, multi-stage bioinformatics analyses.
- **Human-in-the-loop checkpoints** (author)
  - `[P]` Engineer programmatic checkpoints and pause points to surface high-stakes AI decisions for human validation.
- **Computational resource management** (author)
  - `[P]` Manage compute, API limits, and token budgets to keep automated workflows efficient.
- **ISCB Computer Science Domain** (framework: ISCB)
  - `[L]` ISCB **H3** — Make appropriate and efficient use of scripting and programming languages. → https://competency.ebi.ac.uk/framework/iscb/3.0/competencies/H3
- **Transparent integration** (framework: ACTIVE)
  - `[P]` Maintain "human-in-the-loop" governance for all computational conclusions.

---

## Description

*Anthropic:* "Effectively describing goals to prompt useful AI behaviors and outputs."
*Bioinformatics:* communicating goals, context, and assumptions to AI agents as
instructions that drive expected behaviour and make outputs reproducible and
interpretable.

### L1: Translating biological knowledge into precise AI instructions
- **Bioscience domain knowledge** (framework: ISCB)
  - `[L]` ISCB **A3** — Work at depth in at least one technical area aligned with the life sciences. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7950
- **Domain knowledge translation** (author)
  - `[P]` Translate deep domain-specific biological mechanisms, terminology, and experimental variables into precise computational instructions for AI execution.
- **High-context prompting** (author)
  - `[P]` Write structured, unambiguous prompts using advanced techniques to guide AI analysis.
  - `[P]` Handle prompts as a scientific resource to be tested, documented, reported, reproduced, and cited.
- **Adaptive instruction** (author)
  - `[P]` Redirect AI systems dynamically when they drift from the expected analytical path or task boundaries.

### L1: Structuring raw biological data for AI model context
- **Metadata standardization** (author)
  - `[P]` Apply highly descriptive system instructions that translate experimental designs and dataset annotations into clear parameters for AI ingestion.
- **Bioscience domain knowledge** (framework: ISCB)
  - `[L]` ISCB **B3** — Prepare life science data for computational analysis. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7938

### L1: Documenting and tracking AI interactions and software parameters for reproducibility
- **Provenance logging** (author)
  - `[P]` Record every prompt text, system configuration, model version, and seed value used to achieve a computational result.
- **Automated documentation** (author)
  - `[P]` Generate exhaustive documentation of the functions, parameters, and expected outputs of AI-assisted code.
- **Version control** (author)
  - `[P]` Track changes to scripts, prompts, and configurations using version control systems like GitHub.

---

## Discernment

*Anthropic:* "Accurately assessing the usefulness of AI outputs and behaviors."
*Bioinformatics:* using biological intuition to catch mistakes in AI-augmented
analyses; using community standards to assess performance and confidence;
calibrating belief in AI outputs against reference knowledge for biological
plausibility and statistical validity.

### L1: Evaluating the biological plausibility of AI outputs
- **Biological integrity verification** (author)
  - `[P]` Verify the biological plausibility of AI-generated results against established mechanistic principles and trusted reference sources/databases.
  - `[P]` (inline ACTIVE ref) Critical Verification Protocols — implement structured validation procedures to audit AI-generated code or biological hypotheses.
- **Statistical auditing** (author)
  - `[P]` Assess the statistical assumptions, significance estimates, and error measurements of AI-generated results to verify mathematical rigour.
- **Biological interpretation and contextualization** (author)
  - `[P]` Synthesize AI-generated results with established knowledge to extract meaningful biological insights and draw valid conclusions.

### L1: Benchmarking AI results against standard baselines
- **Algorithmic bias detection** (author)
  - `[P]` Screen AI outputs for population skews, data imbalances, or training-data biases across diverse experimental groups.
- **Automated evaluation design** (author)
  - `[P]` Build programmatic evaluation pipelines that compute error rates and compare AI outputs against gold-standard datasets or software tools.
- **Verification Confidence Calibration** (framework: ACTIVE)
  - `[P]` Close the "proof–belief gap" by aligning one's belief in an AI solution's correctness with objective accuracy outcomes.

### L1: Detecting computational artifacts and hallucinations
- **Hallucination detection** (author)
  - `[P]` Identify fabricated data, non-existent citations, or flawed logical loops in AI text and code outputs.
- **Collaborative code review** (author)
  - `[P]` Use structured peer code review, pull requests, and issue tracking on GitHub to verify AI-generated code iteratively across the project lifecycle.
- **Code auditing and debugging** (author)
  - `[P]` Audit AI-generated scripts line-by-line for syntax errors, silent logical bugs, and hardcoded variables before running them.

---

## Diligence

*Anthropic:* "Taking responsibility for what we do with AI and how we use it."
*Bioinformatics:* accountability for the impact of agentic AI solutions —
adherence to ethical/safe-AI standards, plus keeping the cognitive ability to stay
critical of AI outputs and to do the work manually when agents fail.

### L1: Ensuring pipeline governance and regulatory compliance
- **Professional Conduct** (framework: ISCB)
  - `[L]` ISCB **J3** — Comply with professional, ethical, legal, and social standards. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7946
- **AI regulatory alignment** (author)
  - `[P]` Monitor shifting regional and global AI legal frameworks to align pipeline deployments with local jurisdiction mandates. (site links to github.com/melissawm/open-source-ai-contribution-policies)
- **Ethical evaluation** (author)
  - `[P]` Identify algorithmic bias and ensure AI-driven decisions are calibrated, safe, and legally compliant.
  - `[P]` Formulate institutional/team risk guardrails against algorithmic discrimination, dual-use biological research hazards, and IP infringement.

### L1: Securing digital asset longevity and sustainability
- **Data Science Domain Knowledge** (framework: ISCB)
  - `[L]` ISCB **E3** — Manage own and others' data according to community standards (FAIR principles). → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7941
- **Computer Science Domain Knowledge** (framework: ISCB)
  - `[L]` ISCB **I3** — Construct and maintain bioinformatics computing infrastructure. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7945
  - `[L]` ISCB **G3** — Contribute to the design of user-centric bioinformatics tools. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7943

### L1: Countering mental dependency while preserving technical mastery
- **Iterative skill development** (framework: ACTIVE)
  - `[P]` Counter "cognitive offloading" by intentionally practising the "cognitive musculature" of manual coding and statistical reasoning.
- **Professional Conduct** (framework: ISCB)
  - `[L]` ISCB **M3** — Engage in continuing professional development. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7949

### L1: Nurturing a supportive and responsible scientific community
- **Professional Conduct** (framework: ISCB)
  - `[L]` ISCB **L3** — Work effectively in teams to accomplish common goals. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7948
  - `[L]` ISCB **K3** — Communicate meaningfully with a range of audiences. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7947
- **Bioscience Domain Knowledge** (framework: ISCB)
  - `[L]` ISCB **C3** — Have a positive impact on scientific discovery through bioinformatics. → https://competency.ebi.ac.uk/framework/iscb/3.0/competency/details/7939

### L1: Guiding institutional strategy and cross-sector diplomacy
- **Visionary stewardship** (author)
  - `[P]` Design long-term technical roadmaps, governance models, and sustainability plans for the operational longevity of bioinformatics initiatives.
- **Scientific diplomacy** (author)
  - `[P]` Navigate negotiations and communicate impact across academia, industry, and government to align competing interests and influence decision-makers.

### L1: Elevating workforce capacity and educational legacy
- **Generational mentorship** (author)
  - `[P]` Mentor early-career talent to use generative AI appropriately, critically, and responsibly.
- **Pedagogical dissemination** (author)
  - `[P]` Design open-access learning resources using cloud and AI technologies to democratize access to scientific discoveries and reduce educational inequity.

---

## Tallies (2026-08-31)

| Capability | Practice areas (L1) | Groups (L2) | Competencies (L3) | Linked | Plain |
|---|---|---|---|---|---|
| Delegation | 3 | 13 | 14 | 3 | 11 |
| Description | 3 | 9 | 10 | 2 | 8 |
| Discernment | 3 | 9 | 10 | 0 | 10 |
| Diligence | 6 | 13 | 16 | 8 | 8 |
| **Total** | **15** | **44** | **50** | **13** | **37** |

Counts are approximate — some Level-3 items bundle two sentences, and the inline
ACTIVE reference under Discernment › "Biological integrity verification" is counted
as its own competency. Recount when the content is normalized into data.

## Distinct ISCB codes cited: 13

A3, B3, C3, D3, E3, F3, G3, H3, I3, J3, K3, L3, M3. Each is cited exactly once, so
there are 13 linked-competency instances. No `N3` or higher referenced yet. All
codes end in `3` (the ISCB competency level).
