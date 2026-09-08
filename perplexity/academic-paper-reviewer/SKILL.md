---
name: academic-paper-reviewer
description: Perform rigorous structured peer review of academic manuscripts, thesis chapters, conference papers, journal drafts, and systematic reviews. Use when the user asks to review, critique, score, stress-test, or identify revision priorities in a manuscript. Focus on research question clarity, methodological validity, claim–evidence alignment, contribution, structure, citations, limitations, overclaiming, and reporting integrity. Do not use primarily to draft a new paper.
---

# Academic Paper Reviewer — Perplexity Edition

## Purpose

Review the manuscript as a demanding but fair academic reviewer. Diagnose weaknesses, test claims against evidence, and produce actionable revision priorities.

## Required shared references

Apply these platform-neutral rules whenever relevant:
- `../shared/references/research-integrity-core.md`
- `../shared/references/source-verification-and-citation.md`
- `../shared/references/review-and-methods-core.md`
- `../shared/references/argumentation-and-writing-core.md`
- `../shared/references/qualitative-and-reflexive-research.md` for qualitative studies
- `../shared/references/cross-document-consistency.md`
- `../shared/references/systematic-review-and-risk-of-bias.md` for systematic reviews and RoB assessment
- `../shared/references/meta-analysis-and-certainty.md` for pooled/narrative synthesis and certainty claims
- `../shared/references/research-ethics-and-human-subjects.md` for ethics, AI disclosure, data ethics, and human-subjects boundary claims
- `../shared/references/apa-citation-and-output.md` for citation/output-format checks

## Review perspectives

When the manuscript warrants depth, divide review work across complementary perspectives:
- research-question and contribution reviewer
- methodology reviewer
- argument/evidence reviewer
- literature/citation reviewer
- structure/writing reviewer
- devil's-advocate / disconfirming-evidence reviewer
- systematic-review / quantitative-synthesis reviewer when applicable
- ethics / reporting-boundary reviewer when applicable

Perplexity may execute these in parallel. Merge only after reconciling overlaps and contradictions.

## Review dimensions

### 1. Research problem and contribution
Check whether the problem is specific, researchable, and justified. Distinguish genuine contribution from topic importance. Flag novelty claims that are not demonstrated.

### 2. Research-question alignment
Verify that RQs/hypotheses align with theory, design, data, analysis, findings, and conclusions. Where needed, invoke the logic of `research-methodology-auditor` rather than assuming alignment.

### 3. Methodological validity
Assess design fit, sampling, intervention or procedure, measurement/instruments, data collection, analysis, validity/trustworthiness, reflexivity where relevant, and inferential limits.

Do not demand methods merely because they are fashionable. Judge fit to the stated research purpose.

### 4. Claim–evidence alignment
For each central claim, ask:
- what evidence supports it?
- does the cited source or reported result support the exact claim?
- is the claim stronger than the data?
- are alternative explanations addressed?
- has revision silently changed the claim-strength rung or dropped a protected hedge?

Use evidence labels E1–E5 when external literature is involved.

### 5. Literature and citations
Check whether key literature streams are represented, recent work is incorporated where needed, contrary findings are acknowledged, and citations are attached to the claims they actually support.

Distinguish reference existence from claim support. Never invent missing references.

### 6. Results and interpretation
Separate reported findings from interpretation. Flag:
- causal language unsupported by design
- generalization beyond sample/context
- interpretation presented as raw result
- cherry-picking or unaddressed negative cases
- mismatch between tables/figures and narrative

### 7. Qualitative rigor
When applicable, inspect:
- sampling logic and adequacy rationale
- data-generation transparency
- coding traceability
- theme development
- negative cases
- reflexivity and researcher positionality
- triangulation quality
- distinction between participant evidence and researcher interpretation

Do not require every qualitative technique mechanically; assess fit to the declared approach.

### 8. Systematic review, risk of bias, and quantitative synthesis
When applicable, inspect:
- whether protocol and eligibility criteria were set before synthesis;
- search/screening reproducibility and PRISMA-style accounting;
- correct risk-of-bias tool for study design;
- signaling-question evidence behind RoB judgments;
- distinction between relevance and risk of bias;
- whether pooling was justified before meta-analysis;
- effect-size harmonization and model choice;
- heterogeneity investigation;
- sensitivity/subgroup analysis transparency;
- whether certainty claims are outcome-specific and methodologically justified;
- whether narrative synthesis was used appropriately when pooling was not defensible.

Never accept fabricated pooled effects, heterogeneity statistics, forest plots, or certainty ratings when the underlying data/computation are unavailable.

### 9. Ethics and human-subjects boundaries
Check whether the manuscript overstates:
- ethics approval/exemption;
- consent or authorization sufficiency;
- anonymity/de-identification;
- legal/institutional compliance;
- AI disclosure or reproducibility.

The manuscript may describe documented institutional decisions; the reviewer must not manufacture them.

### 10. Cross-document consistency
When the relevant artifacts are available, compare:
- abstract ↔ results
- discussion ↔ results
- methods ↔ reported analyses
- preregistration/protocol ↔ manuscript
- RQ ↔ instrument/data ↔ analysis ↔ conclusion

A no-listed-inconsistency result is advisory, not proof of completeness or perfect agreement.

### 11. Structure, writing, and formatting
Assess logical progression, section function, redundancy, terminology consistency, academic register, and whether headings and transitions reflect the argument rather than merely organizing topics.

When a target venue/style is known, distinguish scientific validity problems from format nonconformance. Verify reference-list/in-text reconciliation and abstract/table/figure consistency where relevant.

### 12. Limitations and integrity
Check whether important limitations are disclosed and whether the manuscript overstates verification, reproducibility, causality, representativeness, novelty, saturation, triangulation, authorization, systematic-review completeness, or certainty of evidence.

## Severity model

Classify findings:
- **Critical** — threatens validity or makes a central conclusion unsupported
- **Major** — materially weakens credibility, interpretation, contribution, or reporting integrity
- **Minor** — improves clarity, completeness, or presentation without changing the core result

Do not inflate stylistic preferences into Major issues.

## Output

Default structure:
1. review recommendation / overall assessment
2. strongest aspects worth preserving
3. Critical issues
4. Major issues
5. Minor issues
6. claim–evidence or RQ alignment concerns
7. systematic-review/meta-analysis concerns when applicable
8. ethics/reporting-boundary concerns when applicable
9. cross-document consistency concerns when applicable
10. prioritized revision sequence
11. optional scorecard if useful

For each Critical/Major issue provide:
- diagnosis
- why it matters
- evidence/location in manuscript when available
- smallest defensible revision
- whether new data are required or textual/methodological clarification is sufficient

## Human checkpoint

Do not rewrite the manuscript unless asked. Separate diagnosis from revision choice. If two defensible revisions imply different research positions, present both and require the author to choose.
