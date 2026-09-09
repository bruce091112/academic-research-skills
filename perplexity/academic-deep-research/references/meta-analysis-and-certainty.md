# Meta-analysis & Certainty Core — Perplexity Edition

This reference preserves the quantitative evidence-synthesis logic of the original Academic Research Skills while avoiding assumptions that the platform always has a statistical runtime.

## 1. Feasibility first

Do not pool studies merely because multiple quantitative results exist.

Meta-analysis is appropriate only when the studies are sufficiently comparable in:
- review question / PICOS;
- population/context;
- intervention/exposure;
- comparator;
- outcome construct and timing;
- study design and effect interpretation.

When these differ too fundamentally, use structured narrative synthesis instead of a misleading pooled estimate.

## 2. Effect-size harmonization

Choose and justify a common effect metric.

Examples:
- continuous, same scale: Mean Difference;
- continuous, different scales measuring the same construct: Standardized Mean Difference / Hedges' g;
- binary outcomes: RR, OR, or RD according to design and interpretive goal;
- time-to-event: HR / log(HR).

Do not convert metrics unless the necessary information is available and the transformation is methodologically justified.

Flag effect sizes that are reconstructed, approximated, or digitized rather than directly reported.

## 3. Model choice and heterogeneity

Report and interpret heterogeneity rather than treating it as nuisance noise.

When statistical synthesis is actually performed, consider:
- Cochran's Q;
- I²;
- tau²;
- prediction intervals when appropriate.

Do not use rigid I² thresholds as automatic decision rules. Interpret magnitude, direction, study design, and substantive diversity together.

If heterogeneity is extreme and unexplained, reconsider pooling.

## 4. Pre-specified subgroup analyses

Prefer subgroup analyses specified before inspecting results.

Potential moderators include:
- study design;
- geography/context;
- intervention type;
- population characteristics;
- publication period;
- risk of bias.

Do not data-dredge subgroups until a desirable significant result appears. If exploratory subgroup analysis is performed, label it exploratory.

## 5. Sensitivity analyses

When feasible, test robustness using approaches such as:
- leave-one-out analysis;
- excluding high-risk-of-bias studies;
- alternative plausible statistical models;
- alternative effect-size assumptions;
- excluding approximated/reconstructed effect sizes.

Report sensitivity analyses that weaken the preferred conclusion as clearly as those that strengthen it.

## 6. Publication-bias assessment

Funnel plots and formal small-study-effect tests are unreliable with very small study counts. Use current methodological guidance and clearly state study-count limitations.

Do not present trim-and-fill or similar methods as proof that publication bias has been corrected.

## 7. GRADE / certainty of evidence

For each important outcome, assess certainty separately.

Common downgrade domains:
- risk of bias;
- inconsistency;
- indirectness;
- imprecision;
- publication bias.

Potential upgrading considerations for eligible observational evidence depend on the current GRADE framework.

Never infer certainty solely from statistical significance.

## 8. No-runtime rule

If Perplexity does not have verified access to the necessary statistical computation capability or complete extracted data:
- do not fabricate pooled effects, CIs, heterogeneity statistics, p-values, or forest plots;
- instead provide the analysis specification, required input table, formulas/metric choice, and a reproducible execution plan;
- label any manually derived value and show enough information for verification.

If computation is available, retain the input data and transformation logic needed to audit the result.

## 9. Narrative synthesis fallback

When pooling is inappropriate, synthesize by pre-declared comparison groups and report:
- grouping logic;
- direction and magnitude where available;
- consistency/inconsistency;
- study quality/risk of bias;
- contextual differences;
- why pooling was not performed.

Avoid simple vote counting by statistical significance.

## 10. Output

When a true meta-analysis is performed, report at minimum:
- included studies and effect data;
- metric and model;
- pooled estimate and CI;
- heterogeneity;
- sensitivity/subgroup results;
- risk-of-bias implications;
- certainty assessment;
- analysis limitations.

When it is not performed, say so explicitly and provide the structured synthesis or analysis plan instead.