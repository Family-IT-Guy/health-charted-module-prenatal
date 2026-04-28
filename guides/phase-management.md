# Phase Management

When the user reports a phase change, asks what changes between phases, or current_phase needs evaluation against gestational_age_weeks.

## Trigger conditions

- User reports a positive pregnancy test, conception date, or LMP
- User mentions a phase milestone ("entered second trimester," "delivery," "weaning")
- `gestational_age_weeks` in `my-data/prenatal-profile.json` crosses a phase boundary (13, 27, delivery, postpartum→lactation transition at ~6 weeks)
- User asks "what changes at week X" or "what should I be tracking now"

## Inputs

- `my-data/prenatal-profile.json` — current_phase, gestational_age_weeks, conception_date or lmp_date, due_date, phase_transition_log
- `reference/phase-guide.md` — phase definitions, transition triggers, per-phase measurement schedules
- Wiki: phase-anchored biological windows, phase-specific entities

## Pattern

1. **Confirm the trigger.** If gestational_age_weeks is computed, confirm it against a known anchor (conception_date, LMP, or last ultrasound). If user-reported phase change, ask the date of the trigger event.

2. **Identify the new phase** per `reference/phase-guide.md` phase-definitions table. Surface to the user in plain language ("you're moving into trimester 2") rather than internal logic.

3. **Update `my-data/prenatal-profile.json`:**
   - Set `current_phase` to the new phase
   - Set `phase_set_date` to today (or the user-confirmed trigger date)
   - Update `gestational_age_weeks` if known
   - Append entry to `phase_transition_log` with `from_phase`, `to_phase`, `date`, `trigger`
   - Verify the write per HC core's data-routing rule

4. **Surface what changes in the new phase:**
   - New measurement priorities per `reference/phase-guide.md`
   - Approaching biological windows per the relevant submodule's `covers_entities` (e.g., entering T2 → GDM screening at 24-28 weeks)
   - Supplementation focus shifts (e.g., entering T3 → DHA accretion peak; entering lactation → 6,400 IU vitamin D rationale)
   - Any new intake questions from the now-active submodule's `intake_questions` field

5. **Reassess the existing supplement stack** in `my-data/treatments.json` for phase-appropriateness. Use `reference/supplement-forms.md` and the new submodule's `intake_questions` to identify gaps or overlaps.

6. **Surface upcoming labs** based on the per-phase measurement schedule in `reference/phase-guide.md`. Time windows that are within 4 weeks should be added to `my-data/status.json` `pending_action_items` per HC core's data-routing rule.

7. **Submodule engagement.** The new phase's submodule is now active. Its declared guides may activate when their own triggers fire (e.g., trimester-1's nausea-management guide). Salience hints from the new submodule modulate proactive surfacing.

## Postpartum-specific note

Phase transition to postpartum has additional considerations: ferritin at 48 hours postpartum predicts ~4x postpartum-depression risk; if low, this is a severity-triggered surfacing item (see HC core hard-rules.md).

## Lactation-specific note

Lactation supplementation differs from pregnancy supplementation in non-obvious ways. Vitamin D dose specifically increases (6,400 IU lactation evidence vs 2,000-4,000 IU pregnancy). Surface this on transition rather than inheriting the pregnancy dose.
