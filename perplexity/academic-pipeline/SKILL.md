---
name: academic-pipeline
description: Orchestrate an end-to-end academic workflow from research-question refinement through literature research, methodology alignment, systematic review or evidence synthesis when relevant, paper planning, drafting, peer review, revision, and finalization. Use when the user explicitly wants a full research-to-paper pipeline or asks to continue a multi-stage academic project across phases. Preserve human decision points and never fabricate evidence, methods, results, approval statuses, or statistical outputs.
---

# Academic Pipeline — Perplexity Edition

## Purpose
Coordinate the full academic workflow while keeping research decisions, evidence provenance, and revision history traceable. Do not collapse every phase into one opaque generation step.

## Required package references
All stages inherit the platform-neutral research rules in:
- `references/research-integrity-core.md`
- `references/literature-search-and-screening.md`
- `references/source-verification-and-citation.md`
- `references/review-and-methods-core.md`
- `references/argumentation-and-writing-core.md`
- `references/qualitative-and-reflexive-research.md`
- `references/cross-document-consistency.md`
- `references/systematic-review-and-risk-of-bias.md`
- `references/meta-analysis-and-certainty.md`
- `references/research-ethics-and-human-subjects.md`
- `references/apa-citation-and-output.md`

These references define research behavior. Perplexity-native tools define execution mechanics.

## Pipeline
### Stage 1 — Research framing
Clarify research problem, RQs/hypotheses, scope, population/context, theoretical lens, intended contribution, paradigm, and preliminary methodological logic. Consequential RQ/construct/scope changes require human approval.

### Stage 2 — Evidence build
Apply `academic-deep-research` logic: systematic search architecture, predeclared inclusion/exclusion where applicable, two-pass screening, deduplication, corpus-first/search-fills-gap, source-existence and claim-support verification, contrary evidence, and distribution/coverage advisories. Do not proceed to strong claims while key evidence remains E5 or materially contradictory without surfacing the conflict.

### Stage 2.5 — Systematic-review / risk-of-bias branch
When relevant, document/freeze protocol status, preserve search/screening accounting, select correct RoB framework by design, preserve signaling evidence/domain judgments, and keep relevance, RoB, reporting completeness, and certainty distinct. Never describe post-hoc decisions as preregistered/prospective.

### Stage 3 — Integrity gate
Audit citation existence, claim–source alignment, unsupported factual claims, fabricated/inferred methods or results, ignored negative evidence, E1–E5 labels, claim-intent drift, claim-strength drift, and protected hedges. Resolve integrity failures before downstream polishing.

### Stage 4 — Methodology alignment
Apply `research-methodology-auditor` logic: RQ → theory → constructs → operationalization → design → participants/sampling → instruments/data → timing → analysis → findings → conclusion. For qualitative studies audit sampling, coding traceability, themes, reflexivity/dual roles, negative cases, triangulation, member-reflection/checking, and adequacy language. For review/meta-analysis designs audit protocol, eligibility, RoB, pooling feasibility, metrics, heterogeneity, sensitivity analysis, and certainty.

### Stage 5 — Analysis and synthesis
For literature-based research, integrate rather than sequentially summarize. Preserve contradiction, methods/contexts, gaps, evidence vs inference. For qualitative empirical research preserve raw data → code → category → theme/analytic concept → interpretation → RQ. Frequency alone is not thematic importance. For quantitative synthesis, assess feasibility before pooling, harmonize metrics, investigate heterogeneity, conduct/plan sensitivity analysis, integrate RoB, and assess certainty by outcome. If valid computation or complete extracted data are unavailable, use structured narrative synthesis or an analysis specification instead of fabricated statistics.

### Stage 6 — Paper construction
Apply `academic-paper` logic to architecture, argument maps, and manuscript sections using verified evidence and declared methods/results. Use claim-intent precommitment before major drafting blocks and preserve hedges, positionality, scope/time qualifiers, and review-reporting distinctions.

### Stage 6.5 — Ethics and human-subjects boundary gate
When relevant, verify material AI-assistance disclosure, attribution integrity, data-ethics/privacy claims, researcher dual-role/positionality disclosures, and documented vs unverified approval/exemption/consent/anonymity/authorization. If authority is unresolved, preserve `institutional determination required`.

### Stage 7 — Cross-document consistency gate
Compare abstract↔results, discussion↔results, methods↔reported analyses, preregistration/protocol↔manuscript, RQ↔constructs↔instruments↔analysis↔conclusions, and sample definitions. Treat `POTENTIAL_INCONSISTENCY_LOCATED` / `NO_LISTED_INCONSISTENCY_LOCATED` as advisory observations; the latter is not proof of completeness.

### Stage 8 — Peer review
Apply `academic-paper-reviewer` logic from multiple perspectives. Separate Critical/Major/Minor issues and explicitly inspect validity, claim/evidence fit, source verification, causal/inferential overreach, qualitative rigor/reflexivity, systematic-review/RoB/meta-analysis integrity, ethics/reporting boundaries, and cross-document consistency.

### Stage 9 — Revision planning
Create a revision matrix with concern, severity, affected section/RQ, proposed action, evidence/new data required, author decision, claim-strength/hedge impact, ethics/reporting impact, and completion status.

### Stage 10 — Revision
Resolve validity/evidence problems before stylistic polishing. Never silently change RQs, constructs, sample scope, analytic strategy/synthesis model, claim strength, protected hedges, participant-vs-researcher evidence status, ethics/authorization status, or meta-analysis values.

### Stage 11 — Final verification
Check each RQ is answered or explicitly unresolved; inference boundaries; claim/citation alignment; source existence; qualitative traceability; triangulation; systematic-review/RoB/meta-analysis traceability; ethics/human-subjects claims; limitations; terminology/numbers/sample descriptions; and reference completeness to the extent source data allows.

### Stage 12 — Finalization
Use formatting precedence: user instructions → target venue/institution → requested style manual → `references/apa-citation-and-output.md` fallback. Reconcile in-text citations/reference list, abstract/results, narrative/tables/figures, and terminology. Use only capabilities actually available on Perplexity; do not assume local Pandoc, LaTeX, Python, Word automation, shell hooks, or Claude validators.

## Orchestration rules
Perplexity may dispatch parallel sub-agents for independent research/review tasks. Merge through explicit agreement, disagreement, unresolved conflict, and missing evidence. Do not average away meaningful disagreement. Use the smallest necessary workflow; route narrow tasks to the relevant skill instead of running the whole pipeline.

## Evidence policy
- E1 Direct scholarly support
- E2 Indirect scholarly support
- E3 Reasoned inference
- E4 Practice/field evidence
- E5 Insufficient evidence
Never present E3–E5 as E1.

## Human-in-the-loop rules
Preserve human judgment for final RQ/hypothesis, theory when interpretation changes materially, sampling/inclusion, construct operationalization, analytic strategy, ambiguous eligibility decisions, defensible alternative pooling/model choices, interpretation of ambiguous findings, reviewer recommendations that alter research position, meaningful cross-document contradictions, and institutional ethics/authorization decisions.

## Output
At any stage report current stage, completed artifacts/decisions, unresolved Critical/Major issues, and next defensible action. Do not claim empirical procedures, data collection, exhaustive searching, reproduced results, ethics approval, or computed meta-analysis unless explicitly established by the user or verified source.
