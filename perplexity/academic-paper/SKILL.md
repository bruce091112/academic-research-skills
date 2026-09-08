---
name: academic-paper
description: Plan, outline, draft, revise, and format academic papers, thesis chapters, conference papers, and journal manuscripts using a research-first workflow. Use when the user asks to write or revise an academic paper, create an outline, draft a literature review or methodology section, prepare an abstract, integrate reviewer feedback, or improve argument structure. Preserve claim–evidence traceability and do not fabricate citations or results.
---

# Academic Paper — Perplexity Edition

## Purpose

Turn a defined research problem and evidence base into a defensible academic manuscript. Writing follows evidence; it does not substitute for evidence.

## Required shared references

Apply these platform-neutral rules whenever relevant:
- `../shared/references/research-integrity-core.md`
- `../shared/references/source-verification-and-citation.md`
- `../shared/references/argumentation-and-writing-core.md`
- `../shared/references/qualitative-and-reflexive-research.md` for qualitative studies
- `../shared/references/cross-document-consistency.md` for abstract/results, methods/results, preregistration/manuscript, or multi-artifact consistency
- `../shared/references/review-and-methods-core.md`
- `../shared/references/systematic-review-and-risk-of-bias.md` when drafting or revising systematic reviews
- `../shared/references/meta-analysis-and-certainty.md` when pooled estimates, narrative synthesis, heterogeneity, or certainty of evidence are reported
- `../shared/references/research-ethics-and-human-subjects.md` for ethics, AI disclosure, data governance, human-subjects, and positionality boundaries
- `../shared/references/apa-citation-and-output.md` for APA/citation/output formatting

## Modes

Route the task to the smallest fitting mode:
- **plan** — define paper architecture, contribution, argument, evidence needs
- **outline** — build section structure and claim sequence
- **draft** — write manuscript sections from supplied or verified evidence
- **revision** — revise an existing manuscript while preserving facts and author position
- **revision-coach** — convert reviewer comments into a revision roadmap
- **abstract** — produce an abstract consistent with the manuscript
- **lit-review** — synthesize literature into an argumentative review section
- **citation-check** — inspect claim–citation alignment
- **format** — adapt structure/citations/output to a target venue or style

If the task is primarily evidence discovery, use `academic-deep-research`. If primarily critique, use `academic-paper-reviewer`.

## Core roles

When the task is substantial, Perplexity may distribute work across these roles:
- intake / scope
- literature strategist
- structure architect
- argument builder
- draft writer
- citation compliance checker
- abstract writer
- peer reviewer
- formatter
- revision coach

These are functional roles, not platform-specific agents.

## Workflow

### Phase 0 — Scope and constraints
Identify paper type, discipline, audience/venue if known, language, citation style, word limit, available evidence, and current manuscript stage.

Do not ask for information already supplied. If the user has not chosen a journal or citation style and the choice is not needed yet, proceed with a neutral structure.

### Phase 1 — Evidence readiness
Before drafting substantive claims, determine whether the evidence base is adequate. If not, invoke or recommend `academic-deep-research` logic to fill gaps.

Classify claims using E1–E5. Do not write E3–E5 as established literature fact.

### Phase 2 — Architecture
Build a paper logic map:
research problem → RQ/hypothesis → theoretical frame → argument/analytic path → evidence → findings → discussion → contribution.

Allocate sections by argumentative function, not by topic list alone.

### Phase 3 — Argument construction
For each major section, specify:
- central claim
- evidence
- warrant/reasoning
- qualifier
- counterargument or limitation when material
- transition to next claim

Use claim-intent precommitment before major drafting blocks. Flag unsupported claims before prose drafting.

### Phase 4 — Drafting
Draft section by section. Preserve:
- user-provided facts, numbers, quotations, and findings
- uncertainty and limitation language
- protected hedges
- distinction between result and interpretation
- consistent terminology
- qualitative positionality/reflexivity disclosures when methodologically relevant
- systematic-review protocol, screening, RoB, heterogeneity, and certainty distinctions when relevant

Never invent citations, DOI/page numbers, participant details, methods performed, statistical results, quotations, approval statuses, pooled estimates, or forest-plot values.

### Phase 5 — Citation and integrity check
Check that every substantive sourced claim has an appropriate citation and that the cited source supports the exact nearby claim. Flag citation-by-association, overstatement, source-existence problems, and missing evidence.

### Phase 6 — Internal review
Run a reviewer pass on:
- RQ alignment
- methodological consistency
- claim–evidence fit
- structure
- contribution
- limitations
- writing quality
- qualitative rigor/reflexivity where applicable
- systematic-review/RoB/meta-analysis reporting integrity where applicable
- ethics/human-subjects boundary claims where applicable

For major methodological concerns, apply `research-methodology-auditor` logic.

### Phase 6.5 — Cross-document consistency
When relevant, compare:
- abstract ↔ results
- discussion ↔ results
- methods ↔ reported analyses
- preregistration/protocol ↔ manuscript
- RQs ↔ instruments ↔ analysis ↔ conclusions

Treat `NO_LISTED_INCONSISTENCY_LOCATED` as an advisory result, not proof of perfect agreement.

### Phase 7 — Revision
Prioritize revisions in this order:
1. validity/inference problems
2. RQ/design/evidence alignment
3. argument gaps
4. citation problems
5. ethics/disclosure or reporting-integrity problems
6. structure
7. style and formatting

Do not silently move claims up or down the claim-strength ladder. Do not polish prose before resolving validity problems when both are present.

## Writing quality

Prefer precise academic prose over inflated importance claims, repetitive framing, generic transitions, and unsupported novelty language. Match the user's established academic voice when examples are available. Protect epistemic, scope, reflexive, and temporal qualifiers under word-count pressure.

## Formatting and output

Use this precedence:
1. explicit user instructions;
2. target institution/journal/conference requirements;
3. current requested style manual (e.g., APA 7);
4. fallback rules in `apa-citation-and-output.md`.

Formatting never repairs unsupported claims. Reconcile in-text citations with the reference list, keep abstract and manuscript findings consistent, and verify tables/figures against narrative values.

If the user asks for a document artifact, use Perplexity's actual available document/output capabilities rather than assuming local Pandoc, LaTeX, Word, Python, or shell tools exist.

## Ethics and human-subjects boundary

When applicable, disclose material AI assistance and preserve data-ethics, researcher-role, participant-information, and institutional-authorization boundaries. Do not write that a study is exempt, approved, compliant, or authorized unless explicit current evidence supports that exact status.

## Output

Deliver the requested manuscript content plus, when useful, a concise note of unresolved evidence gaps, consistency issues, ethics/reporting boundaries, or author decisions.

## Human checkpoint

Do not silently change the research question, theoretical stance, sample definition, construct operationalization, analytic strategy, synthesis model, or interpretation of ambiguous findings. Propose the smallest defensible change and let the author decide unless they explicitly authorize revision.
