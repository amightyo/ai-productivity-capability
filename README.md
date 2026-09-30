# AI-Assisted Performance and Independent Capability

Open and reproducible secondary-analysis project investigating when AI-assisted performance translates into later independent capability.

## Research focus

The project distinguishes immediate AI-assisted performance from subsequent performance after AI is removed. It examines whether patterns of human-AI interaction—such as delegation, scaffolding, verification, revision, and iterative reasoning—help explain divergence between assisted output and independent capability.

## Reproducibility principles

- Reproduce the source study before novel analysis.
- Keep reproduction and secondary analysis pipelines separate.
- Preserve task-level Part 2 → Part 3 linkage.
- Treat post-treatment interaction behavior carefully; association is not automatically causal.
- Predefine and validate the cognitive-engagement coding scheme before scaling classification.
- Report falsification and sensitivity analyses.

## Repository structure

- `reproduction/` — independent reproduction of published results
- `analysis/` — novel secondary analyses
- `code/` — reusable processing/classification utilities
- `docs/` — codebooks, provenance, analytic decisions
- `data/raw/` — not tracked; obtain from original source
- `data/derived/` — derived analysis files, subject to source-license review
- `outputs/` — reproducible tables and figures

## Source data

Primary source: Bastani et al., *Generative AI Can Harm Learning*.

Upstream repository: https://github.com/obastani/GenAICanHarmLearning

Raw source data are intentionally not redistributed here. See `data/raw/README.md` and `docs/data_provenance.md`.

## Manuscript policy

The manuscript is intentionally maintained outside this public research repository and is excluded via `.gitignore`.
