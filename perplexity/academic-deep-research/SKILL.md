---
name: academic-deep-research
description: Conduct rigorous academic literature research, source verification, evidence synthesis, claim checking, systematic reviews, and citation-backed research reports. Use when the user asks to investigate a research question, review literature, compare studies, verify scholarly claims, identify evidence gaps, perform a systematic review, assess risk of bias, or build an evidence base. Do not use primarily for drafting a full paper or for peer-reviewing a completed manuscript.
---

# Academic Deep Research — Perplexity Edition

## Purpose

Build a trustworthy evidence base before writing conclusions. Search broadly, verify narrowly, and keep claims traceable to sources.

## Required package references

Apply these platform-neutral rules whenever relevant:
- `references/research-integrity-core.md`
- `references/literature-search-and-screening.md`
- `references/source-verification-and-citation.md`
- `references/argumentation-and-writing-core.md`
- `references/qualitative-and-reflexive-research.md` for qualitative evidence or qualitative synthesis
- `references/cross-document-consistency.md` when comparing manuscripts, preregistrations, protocols, instruments, or multiple research artifacts
- `references/systematic-review-and-risk-of-bias.md` for systematic reviews and study-level bias appraisal
- `references/meta-analysis-and-certainty.md` for quantitative evidence synthesis or structured narrative-synthesis fallback
- `references/research-ethics-and-human-subjects.md` when research ethics, data ethics, AI disclosure, or human-subjects issues arise
- `references/apa-citation-and-output.md` when citation style, report formatting, tables/figures, or APA output is requested

If a package reference conflicts with platform-specific mechanics, preserve the research principle and use Perplexity-native execution.

## Intake

Identify, without unnecessary questioning:
- research topic or question
- population/context if relevant
- date range if stated
- language constraints
- desired depth and output
- inclusion/exclusion constraints
- whether the task is exploratory, structured review, systematic review, fact-check, or quantitative synthesis

If the question is too broad to search coherently, propose a bounded working question and clearly label it as provisional.

## Evidence hierarchy

Use the context-sensitive evidence logic in the package source-verification reference. Do not treat a single universal study-design hierarchy as valid across all disciplines or claim types.

Classify substantive claims:
- E1 Direct scholarly support
- E2 Indirect scholarly support
- E3 Reasoned inference
- E4 Practice/field evidence
- E5 Insufficient evidence

Never present E3–E5 as E1.

## Research workflow

### Phase 1 — Search architecture

Break the question into concepts, synonyms, populations, outcomes, mechanisms, and competing explanations. When useful, dispatch parallel research roles for:
- theoretical literature
- empirical literature
- recent developments
- contrary/negative evidence
- source verification
- risk-of-bias appraisal
- quantitative synthesis feasibility

Search beyond the first result page or first framing when the issue is contested or interdisciplinary. Follow `references/literature-search-and-screening.md` for reproducibility, two-pass screening, corpus-first/search-fills-gap behavior, deduplication, PRISMA-style accounting, and coverage-distribution checks.

### Phase 2 — Source screening and verification

For each important source, assess:
- relevance to the exact claim
- study type and sample
- publication venue/status
- date
- methods and limitations
- whether the source is primary or secondary
- reference existence / identifier consistency
- retraction, correction, or supersession status when material
- conflict-of-interest or funding context when relevant

Do not infer a paper's conclusion from title or abstract wording alone when the full text or sufficient source detail is available.

Separate source existence from claim support. A real paper can still fail to support the claim attributed to it.

### Phase 2.5 — Systematic-review and risk-of-bias branch

When the task is a systematic review or structured evidence review:
- define the protocol and eligibility logic before synthesis;
- select the appropriate risk-of-bias instrument by study design;
- use signaling questions and exact study evidence before domain judgments;
- keep relevance, reporting completeness, and risk of bias distinct;
- preserve study-level judgments for downstream sensitivity/certainty analysis.

Do not invent a custom numeric quality score in place of validated instruments.

### Phase 3 — Claim–evidence matrix

Organize findings around claims rather than around a list of papers. For each major claim record:
- claim
- supporting sources
- contradicting/qualifying sources
- evidence level E1–E5
- verification state
- limitations
- confidence

For consequential claims, maintain an evidence-row-style trace following `references/research-integrity-core.md`.

### Phase 4 — Synthesis

Synthesize agreements, disagreements, mechanisms, boundary conditions, and gaps. Distinguish:
- established findings
- emerging findings
- field/practice knowledge
- plausible inference
- unresolved questions

Integration must go beyond sequential source summaries. Preserve contradiction, compare methods and contexts, and avoid majority-vote logic based only on source count.

For qualitative literature, follow `references/qualitative-and-reflexive-research.md` and avoid treating frequency alone as thematic importance.

### Phase 4.5 — Meta-analysis feasibility and certainty

When quantitative pooling is requested:
- assess comparability before pooling;
- choose and justify the effect metric;
- investigate heterogeneity;
- specify sensitivity/subgroup analyses transparently;
- incorporate risk-of-bias information;
- assess certainty by outcome using the applicable current framework.

If the platform lacks complete data or verified statistical computation capability, do not fabricate pooled estimates, CIs, heterogeneity statistics, p-values, or forest plots. Provide the analysis specification and structured narrative synthesis instead.

### Phase 5 — Verification and ethics gate

Before finalizing:
- confirm that citations exist
- confirm that cited sources support the exact nearby claim
- check dates, sample/context, and direction of findings
- flag citation-by-association or overstatement
- check claim-strength drift and protected hedges
- state when evidence is thin or conflicting
- distinguish abstract-level evidence from full-text evidence
- disclose material AI-assistance, source-access, data-ethics, or human-subjects limitations when relevant
- never imply ethics approval, exemption, legal sufficiency, or institutional authorization without explicit evidence

## Output

Default structure:
1. research question / scope
2. concise answer
3. search and screening summary when relevant
4. evidence synthesis by theme
5. risk-of-bias / certainty summary when relevant
6. conflicting or limiting evidence
7. evidence gaps
8. claim–evidence summary
9. verification and ethics limitations
10. references/citations supplied by the platform

When systematic-review reporting is requested, apply the current applicable reporting guideline and make clear whether the actual workflow satisfies it.

Do not fabricate DOI, page numbers, quotations, statistics, bibliographic details, effect sizes, approval statuses, or analytical results.

## Human checkpoint

Request a human decision only when a consequential choice cannot be resolved from the request or evidence, such as changing the research question, excluding a major evidence stream, choosing a synthesis model, or choosing between materially different interpretations. Preserve decisions the user already made unless evidence exposes a conflict that must be surfaced.
