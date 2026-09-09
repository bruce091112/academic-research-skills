# Cross-document Consistency — Perplexity Edition

This reference preserves the advisory logic of the original cross-document consistency protocol without repository-specific schemas, hashes, or local runtime commands.

## Principle

A consistency check locates potential inconsistencies. It does **not** prove that documents agree, are complete, or are error-free.

Allowed summary outcomes:
- `POTENTIAL_INCONSISTENCY_LOCATED`
- `NO_LISTED_INCONSISTENCY_LOCATED`
- `NOT_CHECKED`

`NO_LISTED_INCONSISTENCY_LOCATED` means only that none of the defined mismatch types were found in the inspected scope.

## Required comparison pairs

When the relevant artifacts exist, inspect at least:

1. **Abstract ↔ Results**
   - numeric mismatch
   - direction mismatch
   - significance mismatch
   - claim-strength mismatch

2. **Discussion/Conclusion ↔ Results**
   - direction mismatch
   - claim-strength mismatch
   - scope or population overreach
   - unsupported generalization

3. **Methods ↔ Reported analyses**
   - declared analysis with no reported counterpart
   - reported analysis not declared in methods
   - conflicting analytic specification

4. **Preregistration/protocol ↔ Manuscript**
   - undisclosed deviation
   - changed outcome/analysis without disclosure
   - scope mismatch

5. **Research questions ↔ Instruments/Data ↔ Analysis ↔ Findings**
   - RQ without corresponding data
   - instrument collecting data not used in analysis
   - finding not traceable to an RQ or planned exploratory aim
   - conclusion using a construct that was never operationalized

## Evidence rule

Every potential inconsistency must cite both sides of the comparison when possible.

For absence claims (for example, "analysis declared in methods but not reported"), explicitly name the inspected counterpart scope. Absence is not evidence unless the relevant scope was actually checked.

If a counterpart source is unavailable, report `NOT_CHECKED` or the specific retrieval/access limitation; do not report agreement.

## Advisory boundary

This check is advisory. It does not automatically:
- rewrite the manuscript;
- change the research question;
- alter the user's interpretation;
- create a PASS/FAIL compliance result;
- infer preregistration intent;
- authorize a methodological change.

Potentially consequential corrections require author review.

## Manuscript revision rule

After a substantive revision, rerun consistency checks that depend on changed sections. Do not assume an earlier clean check remains valid.

## Reporting format

For each finding, report:
- pair checked;
- mismatch type;
- first artifact/section evidence;
- second artifact/section evidence;
- why they may conflict;
- severity for scholarly interpretation (Critical / Major / Minor / Advisory);
- suggested verification or remedy;
- whether author decision is required.
