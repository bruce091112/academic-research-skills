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
Source concept: `shared/references/human_subjects_authority_protocol.md`

Preserved at principle level:
- do not infer jurisdiction/applicability from locale, affiliation, filename, or model memory;
- unknown is not false;
- authority sources are bounded, not complete legal advice;
- no unsupported claims of ethics approval, exemption, compliance, or institutional acceptance.

Adapted into:
- `perplexity/shared/references/review-and-methods-core.md`

## B. Preserved as concepts, but not ported literally

These mechanisms are valuable, but the original implementation is tightly coupled to Claude/Codex/local deterministic runtimes. Perplexity Edition keeps the research principle but not the exact machine contract.

- SHA-256 binding of every intermediate artifact;
- exact JSON schema carriers and passport objects;
- repository-specific `phase_e_claim_verification` carriers;
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
- local formatter pipeline → Perplexity artifact/document output, preserving academic structure
- repo-specific gates → visible human checkpoints and advisory findings

## E. Current v1 skill set

- `academic-deep-research`
- `academic-paper`
- `academic-paper-reviewer`
- `academic-pipeline`
- `research-methodology-auditor`

Shared references:
- `research-integrity-core.md`
- `cross-document-consistency.md`
- `review-and-methods-core.md`

## F. Next migration pass

Before packaging, inspect and selectively port additional reusable content from:
- citation/source-verification protocols;
- literature search and screening guidance;
- argument-building guidance;
- qualitative-research and reflexivity guidance;
- writing-quality and revision rules;
- review rubrics and failure-mode catalogs;
- templates that remain platform-neutral.

Do not package until each skill is self-contained and its required references are copied into that skill's own `references/` folder.