# Perplexity Packaging Pass

Goal: make each v1 skill directory self-contained and directly packageable as a ZIP whose root contains `SKILL.md` and `references/`.

## Package roots

- `perplexity/academic-deep-research/`
- `perplexity/academic-paper/`
- `perplexity/academic-paper-reviewer/`
- `perplexity/research-methodology-auditor/`
- `perplexity/academic-pipeline/`

## Packaging rules

1. Every package root contains `SKILL.md`.
2. Every reference named by `SKILL.md` must exist under that package's own `references/` folder.
3. No package may require `../shared/`, `.claude/`, Claude hooks, Codex aliases, local shell scripts, Pandoc, LaTeX, or a mandatory Python runtime.
4. Shared reference content is copied byte-for-byte from `perplexity/shared/references/` so the research rules remain synchronized at this packaging snapshot.
5. Package `SKILL.md` files use `references/<file>.md` paths only.
6. A later change to a shared reference does not automatically mutate already-tested package snapshots; packaging should be rerun intentionally and regression-tested.

## Scenario-test order after packaging

1. `academic-deep-research`
2. `research-methodology-auditor`
3. `academic-paper-reviewer`
4. `academic-paper`
5. `academic-pipeline`

Test routing, source verification, RQ-method-data alignment, qualitative/reflexive safeguards, systematic-review/RoB behavior, no-runtime meta-analysis fallback, citation integrity, cross-document consistency, ethics boundaries, and end-to-end orchestration before any merge into `main`.