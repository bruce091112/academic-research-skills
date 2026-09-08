---
name: academic-pipeline
description: Orchestrate an end-to-end academic workflow from research-question refinement through literature research, methodology alignment, paper planning, drafting, peer review, revision, and finalization. Use when the user explicitly wants a full research-to-paper pipeline or asks to continue a multi-stage academic project across phases. Preserve human decision points and never fabricate evidence, methods, or results.
---

# Academic Pipeline — Perplexity Edition

## Purpose

Coordinate the full academic workflow while keeping research decisions, evidence provenance, and revision history traceable. This skill orchestrates other research functions; it should not collapse every phase into one opaque generation step.

## Required shared references

All stages inherit the platform-neutral research rules in:
- `../shared/references/research-integrity-core.md`
- `../shared/references/literature-search-and-screening.md`
- `../shared/references/source-verification-and-citation.md`
- `../shared/references/review-and-methods-core.md`
- `../shared/references/argumentation-and-writing-core.md`
- `../shared/references/qualitative-and-reflexive-research.md`
- `../shared/references/cross-document-consistency.md`

These references define research behavior. Perplexity-native tools define execution mechanics.

## Pipeline

### Stage 1 — Research framing
Clarify the research problem, RQs/hypotheses, scope, population/context, theoretical lens, intended contribution, paradigm, and preliminary methodological logic.

Checkpoint: consequential RQ, construct, or scope changes require human approval.

### Stage 2 — Evidence build
Apply `academic-deep-research` logic to create a verified evidence base.

Required behaviors:
- systematic search architecture
- predeclared inclusion/exclusion logic where applicable
- two-pass screening
- deduplication
- corpus-first/search-fills-gap when user literature exists
- source-existence and claim-support verification
- supporting, conflicting, and boundary-condition evidence
- distribution/coverage advisories when literature is narrowly concentrated

Checkpoint: do not proceed to strong claims if key evidence is E5 or materially contradictory without surfacing the conflict.

### Stage 2.5 — Integrity gate
Audit:
- citation existence
- claim–source alignment
- unsupported factual claims
- fabricated or inferred methods/results
- negative evidence ignored
- evidence labels E1–E5
- claim-intent drift
- claim-strength drift
- protected hedges

A failed integrity gate blocks downstream polishing until resolved.

### Stage 3 — Methodology alignment
Apply `research-methodology-auditor` logic:
RQ → theory → constructs → operationalization → design → participants/sampling → instruments/data → timing → analysis → findings → conclusion.

For qualitative studies also audit:
- sampling logic
- coding traceability
- theme development
- reflexivity and researcher positionality
- researcher–teacher/practitioner dual role when present
- negative cases
- triangulation logic
- member-reflection/checking claims
- saturation/informational-adequacy language

Checkpoint: if an RQ cannot be answered by the available data or design, surface it before drafting results/discussion.

### Stage 4 — Analysis and synthesis
For literature-based research, synthesize across sources rather than summarize sequentially. Preserve contradiction, compare methods and contexts, identify gaps, and distinguish evidence from inference.

For qualitative empirical research, preserve the audit chain:
raw data → code → category → theme/analytic concept → interpretation → RQ.

Do not use frequency alone as thematic importance.

### Stage 5 — Paper construction
Apply `academic-paper` logic to build architecture, argument maps, and manuscript sections from verified evidence and declared methods/results.

Before drafting major blocks, use claim-intent precommitment. Preserve protected hedges, positionality statements, scope limitations, and temporal qualifiers.

### Stage 5.5 — Cross-document consistency gate
Compare relevant artifacts:
- abstract ↔ results
- discussion ↔ results
- methods ↔ reported analyses
- preregistration/protocol ↔ manuscript
- RQ ↔ constructs ↔ instruments ↔ analysis ↔ conclusions
- participant/sample definitions across documents

Surface `POTENTIAL_INCONSISTENCY_LOCATED` or `NO_LISTED_INCONSISTENCY_LOCATED` as advisory observations only. The latter is never proof of complete consistency.

### Stage 6 — Peer review
Apply `academic-paper-reviewer` logic from multiple perspectives. Separate Critical, Major, and Minor issues.

Require explicit attention to:
- methodological validity
- claim/evidence alignment
- source verification
- causal/inferential overreach
- qualitative rigor and reflexivity where applicable
- cross-document inconsistencies

### Stage 7 — Revision planning
Create a revision matrix:
- reviewer/audit concern
- severity
- affected section/RQ
- proposed action
- evidence or new data required
- author decision required?
- claim-strength/hedge impact
- completion status

### Stage 8 — Revision
Resolve validity and evidence issues before stylistic polishing. Preserve an audit trail of consequential changes.

Never silently:
- change an RQ
- redefine a construct
- alter sample scope
- change analytic strategy
- strengthen or weaken a claim rung
- remove a protected hedge
- convert researcher interpretation into participant evidence

### Stage 9 — Final verification
Check:
- each RQ is answered or explicitly unresolved
- findings and conclusions stay within inferential boundaries
- claims and citations align
- source-existence issues are resolved or disclosed
- qualitative findings remain traceable to data where applicable
- triangulation claims are justified
- limitations are disclosed
- terminology, numbers, and sample descriptions are consistent
- references are complete to the extent source data allows

### Stage 10 — Finalization
Format for the requested venue/output using capabilities available on the platform. Do not assume local Pandoc, LaTeX, Python, shell hooks, or Claude-specific validators.

## Orchestration rules

Perplexity may dispatch parallel sub-agents for independent research or review tasks. Parallel work must be merged through explicit reconciliation:
- agreement
- disagreement
- unresolved conflict
- missing evidence

Do not average away meaningful disagreement.

Use the smallest necessary workflow. If the user asks only for literature research, review, methodology audit, or a single section, route to that function instead of running the entire pipeline.

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
- adjudication of meaningful cross-document contradictions

If the user already decided these, do not reopen them unless a concrete inconsistency or integrity problem appears.

## Output

At any stage, report:
- current stage
- completed artifacts/decisions
- unresolved Critical/Major issues
- next defensible action

Do not claim that an empirical procedure was performed, data were collected, sources were fully searched, or results reproduced unless the user or verified source explicitly establishes that fact.
