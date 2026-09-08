# Perplexity Edition v1 — Migration Inventory

This document records what is being preserved from the original `academic-research-skills` research engine and what is intentionally not migrated into the Perplexity execution shell.

## A. Preserved and adapted

### 1. Claim-strength preservation
Source concept: `shared/references/claim_strength_ladder.md`

Preserved:
- field-sensitive epistemic strength ladder;
- no silent strengthening or weakening;
- causal-language safeguards;
- scope, modality, null-result, and caveat preservation.

Adapted into:
- `perplexity/shared/references/research-integrity-core.md`

### 2. Protected hedging
Source concept: `shared/references/protected_hedging_phrases.md`

Preserved:
- epistemic hedges;
- scope hedges;
- reflexivity/positionality markers;
- temporal bounds;
- word-count pressure must not silently delete truth-conditional hedges.

Adapted into:
- `perplexity/shared/references/research-integrity-core.md`

### 3. Claim-intent precommitment
Source concept: canonical R-CIM rules in `shared/references/firm_rules.md`

Preserved:
- planned claims are declared before drafting;
- drafting and drift-audit roles stay separated;
- unplanned claims are surfaced rather than retroactively hidden;
- claims may not be invented from metadata/frontmatter.

Adapted into:
- `perplexity/shared/references/research-integrity-core.md`

### 4. Evidence-row semantics
Source concept: `shared/references/evidence_row_protocol.md`

Preserved:
- claim/source pairs remain auditable;
- source retrieval/provenance status is distinct from claim-support judgment;
- missing/unperformed/access-failed evidence cannot be promoted to positive evidence;
- bounded excerpts/locators are used for adjudication rather than reproducing full source text.

Adapted into:
- `perplexity/shared/references/research-integrity-core.md`

### 5. Cross-document consistency
Source concept: `shared/references/cross_document_consistency_advisory_protocol.md`

Preserved:
- abstract ↔ results;
- discussion/conclusion ↔ results;
- methods ↔ reported analyses;
- preregistration/protocol ↔ manuscript;
- RQ ↔ instruments/data ↔ analysis ↔ findings;
- absence claims require an explicitly inspected scope;
- `NO_LISTED_INCONSISTENCY_LOCATED` is not proof of a clean document.

Adapted into:
- `perplexity/shared/references/cross-document-consistency.md`

### 6. Review-target separation
Source concept: `shared/references/review_criteria_consumer_protocol.md`

Preserved:
- scientific validity, target fit, and submission readiness remain distinct;
- author-confirmed review target is authoritative;
- conflicting criteria remain parallel;
- major findings require constructive remedies and trade-off disclosure;
- reviewer advice cannot silently change author intent.

Adapted into:
- `perplexity/shared/references/review-and-methods-core.md`

### 7. Psychometric safeguards
Source concept: `shared/references/psychometric_terminology_glossary.md`

Preserved:
- true reverse-coded item vs contrast item distinction;
- construct-equivalence test;
- acquiescence-mitigation caution;
- event-anchored recall-bias mitigation.

Adapted into:
- `perplexity/shared/references/review-and-methods-core.md`

### 8. Human-subjects authority boundary
Source concepts:
- `shared/references/human_subjects_authority_protocol.md`
- `deep-research/references/ethics_checklist.md`

Preserved at principle level:
- do not infer jurisdiction/applicability from locale, affiliation, filename, language, or model memory;
- unknown is not false;
- authority sources are bounded, not complete legal advice;
- no unsupported claims of ethics approval, exemption, consent sufficiency, compliance, or institutional acceptance;
- AI disclosure, attribution, data ethics, COI, fair representation, dual-role reflexivity, and reproducibility remain explicit concerns.

Adapted into:
- `perplexity/shared/references/research-ethics-and-human-subjects.md`
- `perplexity/shared/references/review-and-methods-core.md`

### 9. Literature search and screening
Source concepts:
- `deep-research/agents/bibliography_agent.md`
- associated search/screening references.

Preserved:
- systematic rather than ad-hoc searching;
- predeclared inclusion/exclusion criteria;
- two-pass screening;
- corpus-first/search-fills-gap logic;
- deduplication;
- PRISMA-style accounting;
- distributional coverage/skew advisory;
- search reproducibility and limitations.

Adapted into:
- `perplexity/shared/references/literature-search-and-screening.md`

### 10. Source verification and citation integrity
Source concepts:
- `deep-research/agents/source_verification_agent.md`
- evidence-row and bibliographic integrity mechanisms.

Preserved:
- source existence distinct from claim support;
- DOI/metadata mismatch detection concept;
- retraction/correction/supersession awareness;
- conflict-of-interest/funding context;
- abstract-level vs full-text evidence distinction;
- no fabricated bibliographic completion.

Adapted into:
- `perplexity/shared/references/source-verification-and-citation.md`

### 11. Qualitative and reflexive research
Source concepts:
- methodology and qualitative guidance across deep-research and review logic;
- reflexivity/positionality protection mechanisms.

Preserved:
- RQ-method fit;
- sampling rationale;
- coding traceability;
- raw data → code → category/theme → interpretation chain;
- negative cases;
- reflexivity and researcher dual roles;
- triangulation as distinct evidence perspectives rather than a form count;
- member-checking/reflection and saturation claims kept appropriately bounded.

Adapted into:
- `perplexity/shared/references/qualitative-and-reflexive-research.md`

### 12. Argumentation and academic writing
Source concepts:
- `deep-research/references/argumentation_reasoning_framework.md`
- `academic-paper/references/academic_writing_style.md`

Preserved:
- Toulmin claim/evidence/warrant/qualifier/rebuttal logic;
- alternative-explanation testing;
- causal-inference restraint;
- epistemic calibration;
- discipline-sensitive academic register;
- Traditional Chinese academic-writing guidance at principle level.

Adapted into:
- `perplexity/shared/references/argumentation-and-writing-core.md`

### 13. Systematic review and risk of bias
Source concept:
- `deep-research/agents/risk_of_bias_agent.md`

Preserved:
- study-design classification before tool selection;
- RoB 2 / ROBINS-I instrument fidelity;
- signaling questions before judgments;
- evidence for each domain judgment;
- no ad-hoc numeric quality score;
- study-level RoB informs but does not silently determine synthesis inclusion.

Adapted into:
- `perplexity/shared/references/systematic-review-and-risk-of-bias.md`

### 14. Meta-analysis and certainty
Source concept:
- `deep-research/agents/meta_analysis_agent.md`

Preserved:
- feasibility before pooling;
- effect-size harmonization;
- heterogeneity investigation;
- subgroup/sensitivity transparency;
- publication-bias caution;
- outcome-specific certainty assessment;
- structured narrative-synthesis fallback;
- no-runtime/no-data rule against fabricated statistics.

Adapted into:
- `perplexity/shared/references/meta-analysis-and-certainty.md`

### 15. APA, citation, and output rules
Source concepts:
- `academic-paper/references/apa7_extended_guide.md`
- related APA/citation-format references.

Preserved:
- target venue/institution overrides generic style fallback;
- citation integrity precedes formatting;
- APA 7 fallback principles;
- statistics/table/figure consistency;
- abstract must match the manuscript;
- in-text/reference-list reconciliation;
- Traditional Chinese output considerations;
- platform capability boundary for artifact generation.

Adapted into:
- `perplexity/shared/references/apa-citation-and-output.md`

## B. Preserved as concepts, but not ported literally

These mechanisms are valuable, but the original implementation is tightly coupled to Claude/Codex/local deterministic runtimes. Perplexity Edition keeps the research principle but not the exact machine contract.

- SHA-256 binding of every intermediate artifact;
- exact JSON schema carriers and passport objects;
- repository-specific evidence-row carrier schemas;
- exact byte-span replay machinery;
- cache replay contracts;
- deterministic builder scripts;
- command-line validators;
- exact local-path sidecars;
- GitHub issue-number-based protocol identities;
- stage-specific shell gates.

Reason: these are execution-shell mechanisms, not the research engine itself.

## C. Intentionally not migrated in v1

### Claude/Codex execution shell
- `.claude/CLAUDE.md`
- Claude Code slash commands
- hooks / PreToolUse routing
- Claude-specific subagent invocation syntax
- Codex-only aliasing
- local symlink skill loading

### Local-runtime assumptions
- mandatory Pandoc conversion
- mandatory LaTeX runtime
- assumed local Python scripts
- filesystem watchers / persistent local caches
- mandatory local statistical software for meta-analysis

### Repository CI enforcement
- exact mirror-sync linters
- schema/hash CI gates
- held-out repository test harnesses that only validate implementation mechanics

These remain in the original repository and are not deleted.

## D. Perplexity-native replacement strategy

Original execution mechanism → Perplexity Edition replacement:

- Claude subagent call → role/task delegation instructions for Perplexity Computer
- shell routing → skill `description` + explicit workflow classification
- deterministic local web/API scripts → Perplexity search/retrieval with provenance rules
- local formatter pipeline → Perplexity artifact/document output when actually available
- repo-specific gates → visible research-integrity checkpoints and advisory findings
- local meta-analysis runtime → compute only when valid platform computation and complete data are available; otherwise emit analysis specification/narrative synthesis

## E. Current v1 skill set

- `academic-deep-research`
- `academic-paper`
- `academic-paper-reviewer`
- `academic-pipeline`
- `research-methodology-auditor`

Shared references:
- `research-integrity-core.md`
- `literature-search-and-screening.md`
- `source-verification-and-citation.md`
- `qualitative-and-reflexive-research.md`
- `argumentation-and-writing-core.md`
- `cross-document-consistency.md`
- `review-and-methods-core.md`
- `systematic-review-and-risk-of-bias.md`
- `meta-analysis-and-certainty.md`
- `research-ethics-and-human-subjects.md`
- `apa-citation-and-output.md`

## F. Dependency-closure status

Research-engine migration for v1 is now substantially closed at the methodology layer. The five skills explicitly consume the shared references relevant to their roles.

Still required before Perplexity upload testing:
1. copy only the references needed by each skill into that skill's own package directory;
2. ensure every package has `SKILL.md` at ZIP root;
3. remove relative paths that point outside the ZIP;
4. check each package against Perplexity's current upload-size and frontmatter requirements;
5. run scenario tests for routing, literature search, methodology audit, review, systematic review, and end-to-end pipeline behavior;
6. compare outputs against the original engine on a small benchmark set.

Do not merge this branch into `main` merely to test Perplexity packaging. Keep the platform edition isolated until the tests are satisfactory.
