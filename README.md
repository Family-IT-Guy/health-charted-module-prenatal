# Health Charted — Prenatal Module

Pregnancy and lactation domain knowledge for Health Charted instances. Covers preconception through weaning across six phases: preconception, trimester 1, trimester 2, trimester 3, postpartum, and lactation. Each phase has its own salience triggers, intake questions, and entity coverage.

## What this module adds to a Health Charted instance

- Wiki coverage of nutrients, lab markers, biological windows, supplement forms, genetic variants, and interactions relevant to pregnancy and lactation
- Reference docs for pregnancy-specific lab interpretation, supplement form preferences, timing rules, safety tiers, and postpartum patterns
- Research files (cited primary sources) for developmental timeline, nutrient biochemistry, measurement diagnostics, individual variance (genetics, conditions), safety and dose-response, postpartum and lactation, evidence quality
- Guides for phase management, lab interpretation in pregnancy context, and supplement evaluation
- Schema (`prenatal-profile.schema.json`) and starter template (`prenatal-profile.json`) for tracking pregnancy-specific data the user persists in their Health Charted instance

## What this module does NOT do

- It does not ship behavioral rules. All behavioral discipline (epistemic discipline, communication style, hard rules, behavioral protocol) lives in Health Charted core. This module contributes domain knowledge only.
- It does not replace prenatal care. This is education and research, the same as Health Charted core.
- It does not endorse specific supplement brands or products. Form and dose comparisons reference ingredient profiles, not brand recommendations.

## Installing

Place this module's contents at `<HC-instance>/modules/prenatal/` in a Health Charted v1.9 or newer instance. The instance's session-init module scan will pick it up at the next session start.

## License

CC BY-NC-SA 4.0 — same as Health Charted core. Credit the project, keep it non-commercial, share adaptations under the same license.

## Source

Distilled from a structured prenatal nutrition system originally built for one user, then anonymized and generalized. The system's substantive content (developmental timeline, nutrient biochemistry, optimal range frameworks, biological windows) was always evidence-grounded and survives generalization without loss; the anonymization removed instance-specific data (lab values, dates, providers, supplement brand preferences).
