# Research Integrity Core — Perplexity Edition

This reference preserves the platform-neutral integrity logic of the original Academic Research Skills while removing Claude/Codex runtime dependencies.

## 1. Evidence-state discipline

Every substantive claim must be assigned one evidence state:

- **E1 — Direct scholarly support:** the cited source directly supports the claim as written.
- **E2 — Indirect scholarly support:** the source supports only part of the claim or one premise in the reasoning chain.
- **E3 — Reasoned inference:** the claim is a transparent inference from supported premises but is not itself directly stated by the source.
- **E4 — Practice/field evidence:** practitioner experience, classroom observation, craft tradition, local knowledge, or other non-scholarly field evidence.
- **E5 — Insufficient evidence:** available evidence does not justify the claim.

Never present E3, E4, or E5 as E1.

## 2. Claim-intent precommitment

Before drafting a major section or synthesis block, state the intended claims, evidence type, and planned source support. This is a precommitment artifact.

Rules:
- declare intended claims before the first prose draft for that block;
- do not silently rewrite the intent record after drafting begins;
- if a new claim appears later, flag it as newly introduced rather than retroactively pretending it was planned;
- the drafting role emits intended claims; the later audit role checks drift;
- do not use metadata or frontmatter to invent candidate claims that were not present in the supplied corpus or author instructions.

## 3. Claim-strength ladder

Treat epistemic strength as ordered, but field-sensitive:

`may suggest / is consistent with`
< `is associated with / relates to / correlates with`
< `predicts`
< `contributes to`
< `affects / influences / leads to / shapes`
< `causes / determines / demonstrates / proves`

The exact ordering may vary by discipline. The operative rule is: **never move a claim up or down the ladder silently.**

A move includes:
- `associated with` → `causes`;
- removing `may`, `might`, `preliminary`, `exploratory`, or scope limitations;
- deleting a design-based causal caveat;
- changing `predicts` to a weaker or stronger rung without author approval;
- attaching a background citation to a current-study finding it does not support.

Same-rung rewording is allowed if all hedges, scope limits, direction, and evidential meaning remain intact.

## 4. Protected hedges

A hedge is protected when removing it changes the truth-status, scope, positionality, or temporal meaning of a claim.

Protect at least these classes:
- epistemic: may, might, could, tentative, preliminary, exploratory, suggests, indicates, is consistent with;
- scope: in this sample, for this cohort, under the tested conditions;
- reflexivity/positionality: statements that disclose the researcher's role or relationship to the field;
- temporal: former role, explicit study period, historically bounded claims.

Under word-count pressure, cut rhetorical polish before protected hedges. If a required limit cannot be met without changing epistemic meaning, report the conflict instead of silently strengthening the claim.

## 5. Evidence-row concept

For important claim–source pairs, retain an auditable evidence row with:

- claim identifier or exact claim text;
- source identifier;
- locator if available (page, section, quote, paragraph, DOI/URL);
- evidence state (E1–E5);
- bounded excerpt or paraphrase used for adjudication;
- access state: verified, extracted, unconfirmed, not checked, source missing, access failed, retrieval failed, or anchorless;
- a note explaining why the source does or does not support the claim.

A retrieved excerpt proves only that text was found; it does not automatically prove the claim is supported. Claim-support judgment remains separate from excerpt provenance.

Do not treat `source_missing`, `access_failed`, `retrieval_failed`, `not_checked`, or `anchorless` as positive evidence.

## 6. Source integrity and triangulation

Bibliographic or provenance warnings are advisory by default unless the user explicitly adopts a stricter policy.

Do not infer scientific quality, venue type, or eligibility from API metadata alone. Missing metadata is unknown, not negative evidence.

Retraction, correction, supersession, publication status, and source identity should be checked when they materially affect the claim. A source warning does not by itself prove a claim false; it changes the confidence and may require replacement or triangulation.

## 7. Human checkpoint

Require author review before consequential changes to:
- research question or hypothesis;
- construct definition or operationalization;
- sample/population definition;
- primary analytic strategy;
- interpretation of ambiguous or conflicting evidence;
- causal or priority claims;
- conclusions that materially exceed the observed evidence.

If the author has already made a documented decision, audit it rather than reopening it without cause.

## 8. No silent invention

Never invent:
- data, participant characteristics, sample sizes, statistics, effect sizes, quotations, dates, methods, instruments, results, citations, or approvals;
- claims that an experiment, interview, observation, coding pass, or IRB/ethics review occurred when the user has not supplied evidence that it occurred.

When a needed fact is missing, state the gap and continue only with an explicitly labeled assumption, placeholder, or methodological recommendation.