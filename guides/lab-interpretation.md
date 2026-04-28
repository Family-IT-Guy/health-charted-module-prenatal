# Lab Interpretation in Pregnancy and Lactation

When interpreting any lab result during pregnancy or lactation. Pregnancy-optimal ranges differ from standard population reference ranges and shift by trimester.

## Trigger conditions

- New lab values reported by the user or pulled from a provider report
- User asks "is this normal" or "what does this mean" about a result
- Trend assessment: comparing a current result to prior values

## Inputs

- `reference/optimal-ranges.md` — pregnancy-optimal cutoffs per marker
- `reference/phase-guide.md` — trimester-specific TSH ranges, anemia thresholds
- Wiki: marker entities (entities/lab_marker/), [[pregnancy-optimal-vs-standard-ranges]], [[ferritin-acute-phase-reactant-caveat]], [[b12-decision-tree]], [[iron-panel-interpretation]]
- `my-data/lab-results.json` (HC core) — prior values for trend
- `my-data/prenatal-profile.json` — current_phase, gestational_age_weeks
- `my-data/treatments.json` — supplements that affect interpretation (e.g., on iron, on levothyroxine)

## Pattern

1. **Confirm context first.** Before interpreting, ask:
   - Fasting state (if glucose, lipids)
   - Time of day (if cortisol, free-T3)
   - Recent illness or infection (affects ferritin, hsCRP, ESR via acute-phase response)
   - Recent supplementation changes (e.g., started biotin → distorts thyroid/troponin assays)
   - Current gestational age or postpartum week (for trimester-specific ranges)

2. **Apply pregnancy-optimal ranges, not standard population reference ranges.** This is the single most consequential discipline of this guide. Standard "normal" ranges miss most early deficiencies in pregnancy. Surface the difference plainly when relevant: "Your value is in the standard normal range but below the pregnancy-optimal threshold of X for this reason."

3. **Apply the relevant interpretation pattern** based on the marker:
   - **Iron**: combine ferritin AND transferrin saturation per [[iron-panel-interpretation]]; check the [[ferritin-acute-phase-reactant-caveat]] in postpartum or autoimmune contexts
   - **B12**: serum B12 alone is insufficient in the gray zone (200-400); apply [[b12-decision-tree]] with holoTC and MMA backup
   - **Thyroid**: trimester-specific TSH ranges (T1 0.1-2.5, T2 0.2-3.0, T3 0.3-3.0 mIU/mL); check TPO antibodies if not on file
   - **Vitamin D**: pregnancy-optimal 40-60 ng/mL (vs 30 standard floor); higher dose required for lactation per [[lactation:lactation-vitamin-d-evidence]]
   - **Folate**: RBC folate is the tissue measure (>1050 nmol/L NTD threshold); serum folate reflects only recent intake
   - **Glucose**: fasting <100 mg/dL optimal; HbA1c <5.7%; GTT at 24-28 weeks for GDM screening

4. **Trend assessment.** A single value is a snapshot. Three or more values tell a trend (per HC core's [[trajectory-analysis]] rule). State the trajectory plainly: direction, rate, projected timeline, deviation from expectation.

5. **Cross-reference active interventions.** If supplementing a related nutrient, check whether the result aligns with expected response. Lack of expected response is informative — it can indicate inadequate dose, wrong form, absorption issue, or unaddressed cofactor (e.g., D not rising → check magnesium adequacy; iron not rising → check separation from calcium and vitamin C co-administration).

6. **Route data per HC core's data-routing rule.** Lab values land in `my-data/lab-results.json` with context (fasting, gestational age, supplements at time of draw). Verify the write before confirming the result was captured.

7. **Severity-triggered surfacing applies.** Critical values (low hemoglobin, severely elevated TSH, severely abnormal glucose, etc.) trigger explicit prominent surfacing per HC core's hard-rules.md. Do not bury severity-critical findings in routine output.

## What this guide is NOT

- It does not replace clinical evaluation. Abnormal results are still a "talk to your provider" situation, with the framework helping the user prepare specific questions and request specific follow-up labs.
- It does not generate definitive diagnoses. Hypotheses formed during interpretation are explicitly tracked as open hypotheses per HC core's epistemic-discipline rules.
