# Postpartum Mood Monitoring

When the user is in the postpartum or lactation phase and any of: mood is mentioned, mental-health concerns surface, the conversation involves recovery, sleep, or support adequacy. Postpartum mood has documented nutritional risk modulators — surface them alongside the standard mental-health framing, not in place of it.

## Trigger conditions

- `current_phase = postpartum` OR `current_phase = lactation`
- User reports mood changes, anxiety, intrusive thoughts, low motivation, persistent fatigue beyond expected sleep deprivation, or scoring concerning on a postpartum mood screen (EPDS, PHQ-9)
- 48-hour postpartum ferritin or recent vitamin D 25-OH-D levels available in `my-data/lab-results.json`
- User asks about postpartum mental health, postpartum depression, or recovery

## Inputs

- `my-data/lab-results.json` — ferritin (especially 48-hour postpartum), 25-OH-D, TSH, TPO antibodies
- `my-data/prenatal-profile.json` — phase_transition_log (delivery date), current_phase
- `my-data/symptoms.json` — mood-related entries, sleep quality, energy
- `my-data/treatments.json` — current supplement stack
- `reference/postpartum-guide.md` — mental-health connection data, lactation-specific dosing
- Wiki: [[postpartum:postpartum-depression]], [[postpartum:postpartum-thyroiditis]], [[ferritin]], [[25-oh-vitamin-d]], [[omega-3-epa]], [[selenium]]

## Pattern

1. **Severity-triggered surfacing applies first.** Per HC core's hard-rules.md, suicidal ideation, severe psychiatric symptoms, intrusive harm thoughts toward self or infant, or acute crisis require explicit prominent surfacing of emergency resources. Do NOT bury this in routine output. Do NOT optimize supplements while a crisis is in motion. The framework's role at this severity is to surface resources and support immediate clinical care, not to replace it.

2. **For non-emergency mood concerns, surface the documented nutritional risk modulators alongside (not instead of) standard mental-health framing:**

   - **Ferritin at 48 hours postpartum**: low (<30 mcg/L) predicts ~4x postpartum-depression risk. The window for this measurement is narrow (first 48 hours before postpartum inflammation distorts ferritin for ~6 weeks). If available and low, surface it as an actionable risk factor.
   - **25-OH-D**: deficiency (<30 ng/mL) is associated with ~2.28x postpartum-depression risk. Optimal range remains 40-60 ng/mL. If lactating, dose escalates to 6,400 IU per [[lactation:lactation-vitamin-d-evidence]].
   - **EPA**: 1-2 g/day shows the largest documented mood-effect size for postpartum depression (SDM ~-0.886 in trials). EPA-specific, not DHA-specific — confirm the user's omega-3 product has adequate EPA content.
   - **Thyroid**: postpartum thyroiditis affects ~8% of postpartum patients with biphasic course; hyperthyroid phase peaks ~14 weeks, hypothyroid ~19 weeks. Both phases can present with mood symptoms. TSH at 3 and 6 months is the screening cadence. Selenium reduces incidence in TPO+ patients.

3. **Encourage clinical evaluation, not in place of it.** Nutritional optimization is one input. A clinical postpartum-mood evaluation (PCP, OB, midwife, or mental-health provider) is the other. Help the user prepare specific questions and identify specific labs to request rather than implying nutrition can substitute for clinical care.

4. **Track over time.** Postpartum mood changes trajectory matters. Three or more data points tell a trend (per HC core's [[trajectory-analysis]] rule). Update `my-data/symptoms.json` with each conversation that touches on mood, with severity, sleep, support level, and any intervention changes.

5. **Sleep-and-support context, not just nutrition.** Sleep deprivation is the largest single confounder of postpartum mood. Acknowledge this honestly: surfacing nutritional risk modulators is not a claim that nutrition is THE driver. It is a claim that nutrition is a measurable, modifiable input that pairs with sleep, support, and clinical care.

## What this guide is NOT

- It does not replace mental-health care. The framework's role is to surface documented nutritional risk modulators and to help the user advocate for adequate clinical support, not to be the support.
- It does not minimize postpartum mood disorders by framing them nutritionally. Mood disorders are real medical conditions with multiple drivers; nutrition is one of them, not the whole story.
- It does not generate definitive risk scores. Effect sizes from observational and trial data inform context; they do not yield individual probability estimates without clinical evaluation.
