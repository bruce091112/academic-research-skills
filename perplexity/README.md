# Academic Research Skills — Perplexity Edition v1

This directory ports the research engine of `academic-research-skills` to Perplexity Computer.

## Design principle

Keep the research engine; replace the execution shell.

Preserved:
- research-question clarification and convergence
- literature strategy and evidence synthesis
- claim–evidence alignment
- citation/source verification
- human-in-the-loop checkpoints
- academic integrity gates
- paper planning and drafting workflow
- structured peer review and revision loops
- cross-stage consistency checks

Removed or rewritten:
- Claude Code slash commands
- `.claude/CLAUDE.md` routing dependencies
- Claude hooks and PreToolUse machinery
- Claude-specific subagent invocation syntax
- assumptions about local Pandoc/LaTeX/Python runtimes
- symlink-based skill loading

Perplexity Computer decides when to dispatch sub-agents. These skills specify roles, evidence rules, checkpoints, and merge criteria rather than platform-specific agent calls.

## Skills

1. `academic-deep-research` — rigorous literature search, evidence synthesis, claim verification, and research reports.
2. `academic-paper` — plan, outline, draft, revise, and format academic papers while preserving claim–evidence traceability.
3. `academic-paper-reviewer` — structured multi-perspective peer review and revision priorities.
4. `academic-pipeline` — end-to-end research → writing → review → revision → finalization orchestration.
5. `research-methodology-auditor` — audit alignment among RQs, theory, constructs, instruments, data, analysis, findings, and conclusions.

## Perplexity upload format

Each skill should be packaged separately so that `SKILL.md` is at the ZIP root:

```text
academic-paper.zip
├── SKILL.md
├── references/       # optional
└── templates/        # optional
```

Perplexity Computer currently requires:
- `.zip` with `SKILL.md` at root, or a direct `.md` upload
- YAML frontmatter containing `name` and `description`
- lowercase hyphenated skill names
- maximum upload size 10 MB

## Recommended installation order

1. `academic-deep-research`
2. `research-methodology-auditor`
3. `academic-paper-reviewer`
4. `academic-paper`
5. `academic-pipeline`

The first four are useful independently. Install `academic-pipeline` after them because it assumes a complete research workflow and may invoke complementary skills when Perplexity deems them relevant.

## Shared evidence policy

All five skills follow the same evidence labels:

- **E1 — Direct scholarly support**: the cited source directly supports the claim.
- **E2 — Indirect scholarly support**: the source supports part of the reasoning but not the full claim.
- **E3 — Reasoned inference**: a transparent inference from supported premises; must be labeled as inference.
- **E4 — Practice/field evidence**: practitioner experience, classroom observation, craft tradition, or local knowledge; not interchangeable with scholarly evidence.
- **E5 — Insufficient evidence**: the available evidence does not justify the claim.

Never present E3–E5 as E1.

## Human checkpoint rule

Do not silently lock in consequential research decisions. Pause for a human decision when the task requires selecting or changing:
- the research question or hypothesis
- population/sample definition
- construct operationalization
- primary analytic strategy
- interpretation of ambiguous or conflicting evidence
- claims that exceed the evidence base

When the user has already made the decision, preserve it and audit it rather than reopening it without cause.
