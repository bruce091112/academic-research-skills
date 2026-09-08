---
name: academic-pipeline
description: Orchestrate an end-to-end academic workflow from research-question refinement through literature research, methodology alignment, paper planning, drafting, peer review, revision, and finalization. Use when the user explicitly wants a full research-to-paper pipeline or asks to continue a multi-stage academic project across phases. Preserve human decision points and never fabricate evidence, methods, or results.
---

# Academic Pipeline — Perplexity Edition

## Purpose

Coordinate the full academic workflow while keeping research decisions, evidence provenance, and revision history traceable. This skill orchestrates other research functions; it should not collapse every phase into one opaque generation step.

## Pipeline

### Stage 1 — Research framing
Clarify the research problem, RQs/hypotheses, scope, population/context, theoretical lens, and intended contribution.

Checkpoint: consequential RQ or scope changes require human approval.

### Stage 2 — Evidence build
Apply `academic-deep-research` logic to create a verified evidence base. Search for supporting, conflicting, and boundary-condition evidence.

Checkpoint: do not proceed to strong claims if key evidence is E5 or materially contradictory without surfacing the conflict.

### Stage 2.5 — Integrity gate
Audit:
- citation existence
- claim–source alignment
- unsupported factual claims
- fabricated or inferred methods/results
- negative evidence ignored
- evidence labels E1–E5

A failed integrity gate blocks downstream polishing until resolved.

### Stage 3 — Methodology alignment
Apply `research-methodology-auditor` logic:
RQ → theory → constructs → operationalization → design → instruments/data → analysis → findings → conclusion.

Checkpoint: if an RQ cannot be answered by the available data or design, surface it before drafting results/discussion.

### Stage 4 — Paper construction
Apply `academic-paper` logic to build architecture, argument maps, and manuscript sections from the verified evidence and declared methods/results.

### Stage 4.5 — Pre-review integrity gate
Repeat claim–evidence and methodology consistency checks after drafting. Verify that prose has not strengthened claims beyond the evidence.

### Stage 5 — Peer review
Apply `academic-paper-reviewer` logic from multiple perspectives. Separate Critical, Major, and Minor issues.

### Stage 6 — Revision planning
Create a revision matrix:
- reviewer/audit concern
- severity
- affected section/RQ
- proposed action
- evidence or new data required
- author decision required?
- completion status

### Stage 7 — Revision
Resolve validity and evidence issues before stylistic polishing. Preserve an audit trail of consequential changes.

### Stage 8 — Final verification
Check:
- each RQ is answered or explicitly unresolved
- findings and conclusions stay within inferential boundaries
- claims and citations align
- limitations are disclosed
- terminology and numbers are consistent
- references are complete to the extent source data allows

### Stage 9 — Finalization
Format for the requested venue/output using capabilities available on the platform. Do not assume local Pandoc, LaTeX, Python, or shell tools.

## Orchestration rules

Perplexity may dispatch parallel sub-agents for independent research or review tasks. Parallel work must be merged through explicit reconciliation:
- agreement
- disagreement
- unresolved conflict
- missing evidence

Do not average away meaningful disagreement.

Use the smallest necessary workflow. If the user asks only for literature research, review, or a single section, route to that function instead of running the entire pipeline.

## Evidence policy

- E1 Direct scholarly support
- E2 Indirect scholarly support
- E3 Reasoned inference
- E4 Practice/field evidence
- E5 Insufficient evidence

Never present E3–E5 as E1.

## Human-in-the-loop rules

Require or preserve human judgment for:
- final research question/hypothesis
- theory selection when alternatives materially change interpretation
- sampling and participant inclusion decisions
- construct operationalization
- analytic strategy
- interpretation of ambiguous findings
- acceptance/rejection of reviewer recommendations that alter the research position

If the user already decided these, do not reopen them unless a concrete inconsistency or integrity problem appears.

## Output

At any stage, report:
- current stage
- completed artifacts/decisions
- unresolved Critical/Major issues
- next defensible action

Do not claim that an empirical procedure was performed, data were collected, or results reproduced unless the user or verified source explicitly establishes that fact.
