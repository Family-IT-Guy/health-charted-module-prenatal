# T1 Nausea Management

When the user reports nausea, vomiting, or food aversion during the first trimester. Adherence overrides optimization during this window — a tolerable supplement actually taken outperforms an optimal supplement skipped.

## Trigger conditions

- User in `current_phase = trimester-1` reports nausea, vomiting, food aversion, or supplement intolerance
- User asks "I can't keep my prenatal down — what do I do"
- Symptom severity warranting hyperemesis gravidarum evaluation (separate handling — see below)

## Inputs

- `my-data/prenatal-profile.json` — current_phase, gestational_age_weeks
- `my-data/treatments.json` — current supplement stack
- `my-data/symptoms.json` — nausea severity, frequency, triggers
- Wiki: [[vitamin-b6]], [[folate]], [[trimester-1:neural-tube-closure-window]]

## Pattern

1. **Adherence-first framing.** Surface this explicitly to the user: during T1, the goal is to keep something in. A reduced-dose, easier-to-tolerate prenatal taken consistently outperforms a comprehensive prenatal that gets skipped or vomited. This inverts the usual "optimize the form" framing.

2. **Identify what is currently tolerated.** Ask what the user can keep down right now (any food, any supplement, any beverage). Build outward from there.

3. **Tactics to surface (matched to severity):**
   - **Mild nausea (no vomiting):** split prenatal across the day, take with food, try evening dosing instead of morning
   - **Moderate nausea (occasional vomiting):** vitamin B6 10-25 mg with or without doxylamine succinate (evidence-based first-line for nausea/vomiting in pregnancy); switch to a "prenatal" composed of separate components rather than an all-in-one (allows skipping any specific nutrient that triggers nausea); ginger (mild evidence)
   - **Severe vomiting (multiple times daily, weight loss, dehydration signs):** flag for clinical evaluation — this may be hyperemesis gravidarum (HG) requiring medical care including IV hydration and prescription antiemetics. Do not optimize supplements until clinical evaluation is complete.

4. **Protect the load-bearing nutrient: folate.** The neural-tube-closure window is in days 22-28. If the user can keep down any single supplement, prioritize folate over the prenatal multi during the worst nausea weeks. Methylfolate alone is often better-tolerated than a multi.

5. **Defer optimization explicitly.** Tell the user (in plain language): we will revisit form and timing optimization once the nausea resolves. Form choices that matter at week 24 don't matter at week 9 if the user can't keep them down. Set a follow-up trigger for the symptom resolving.

6. **Update data files** per HC core's data-routing rule:
   - Symptom severity and pattern → `my-data/symptoms.json`
   - Supplement changes (split, paused, swapped form) → `my-data/treatments.json`
   - Decision rationale ("paused full prenatal due to T1 nausea, on folate-only and B6") → `my-data/decisions.json`
   - Recheck trigger ("revisit supplement optimization at trimester-2 transition or sooner if nausea resolves") → `my-data/status.json` `pending_action_items`

7. **Severity-triggered surfacing.** Hyperemesis-level severity (per step 3) triggers explicit prominent surfacing per HC core's hard-rules.md, NOT routine handling.

## What this guide is NOT

- It does not justify dropping supplementation entirely. The folate window matters — keep something in even when much is paused.
- It does not replace clinical care for hyperemesis. HG is a medical condition requiring medical management. The framework helps the user advocate for adequate care, not substitute for it.
