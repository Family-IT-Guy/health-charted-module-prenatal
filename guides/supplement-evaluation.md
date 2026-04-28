# Supplement Evaluation in Pregnancy and Lactation

When evaluating a supplement (form, dose, timing, interactions) for pregnancy or lactation context.

## Trigger conditions

- User asks about a specific supplement product (prenatal multivitamin, standalone iron, choline, fish oil, etc.)
- User mentions a new supplement they are considering or have started
- Form question ("methyl- vs cyano- B12," "ferrous bisglycinate vs sulfate," "D3 vs D2")
- Dose question ("is this too much," "is this enough")
- Interaction question ("can I take iron with my prenatal")

## Inputs

- `reference/supplement-forms.md` — preferred forms per nutrient with rationale
- `reference/safety-rules.md` — pregnancy-specific ULs, three-tier safety classification
- `reference/timing-rules.md` — clinically meaningful interactions
- Wiki: supplement entities (entities/supplement/), [[supplement-form-bioavailability]], [[pregnancy-upper-limits]]
- `my-data/treatments.json` — current supplement stack
- `my-data/prenatal-profile.json` — current_phase (lactation has different dosing for some nutrients)
- `my-data/lab-results.json` — recent values that may calibrate dose (especially iron via ferritin/TSAT, vitamin D via 25-OH-D)

## Pattern

1. **Identify the form first.** Many supplements with the same nominal dose perform very differently based on chemical form. Apply [[supplement-form-bioavailability]]:
   - Folate: methylfolate or folinic acid > folic acid
   - Iron: ferrous bisglycinate > ferrous sulfate (better absorbed, fewer GI effects)
   - B12: methylcobalamin > cyanocobalamin
   - Vitamin D: D3 (cholecalciferol) > D2 (ergocalciferol)
   - Vitamin A: beta-carotene safe; retinol teratogenic >10,000 IU per [[vitamin-a-teratogenicity-mechanism]]
   - Magnesium: glycinate or malate > oxide (~4% bioavailable)
   - Omega-3: triglyceride form > ethyl ester
   - Calcium: citrate (low stomach acid) > carbonate
   - Iodine: potassium iodide > kelp (variable potency)

2. **Check dose against pregnancy ULs.** Apply `reference/safety-rules.md` Tier 1/2/3 classification and the UL table:
   - Tier 1 (broadly safe without testing): methylfolate 800-1000 mcg, vitamin D3 2000-4000 IU, DHA 300+ mg, choline 450-550 mg
   - Tier 2 (test first): iron, B12 (especially if omnivore), iodine, calcium
   - Tier 3 (serious care): retinol-form vitamin A, high-dose iron without deficiency, high-dose iodine, B6 above 100 mg

3. **Check the user's current stack** for overlap and gaps:
   - Overlap: vitamin D, K2, B12, B6 commonly stack across multiple products and can exceed safe levels
   - Gaps: choline is the most commonly under-dosed or omitted nutrient in commercial prenatal multivitamins
   - Phase-specific: lactation requires 6,400 IU vitamin D per [[lactation:lactation-vitamin-d-evidence]] — higher than pregnancy. Surface this when transitioning to lactation.

4. **Check interactions** per `reference/timing-rules.md`:
   - [[iron-calcium-interaction]]: separate by 2+ hours
   - [[iron-vitamin-c-synergy]]: take iron with vitamin C source
   - Levothyroxine: 30-60 minutes before food, 4 hours from iron and calcium

5. **Calibrate dose to labs when applicable.** Some doses are not "one-size-fits-all":
   - Iron dose calibrated to ferritin and TSAT per [[iron-panel-interpretation]]
   - Vitamin D dose calibrated to 25-OH-D
   - Iodine confirmed against urinary iodine where uncertainty exists

6. **Evaluate the product itself** when assessing a specific brand:
   - Forms (per step 1)
   - Doses (per step 2)
   - Missing nutrients (per step 3)
   - Third-party testing (USP, NSF, ConsumerLab) — verifies label accuracy and purity but does NOT verify bioavailability or efficacy
   - Delivery format (capsule count, liquid, powder) — match adherence reality

7. **Route updates to data files** per HC core's data-routing rule. Treatment changes land in `my-data/treatments.json` with form, dose, timing, and reason. Surface monitoring cadence (e.g., recheck ferritin in 8-12 weeks after starting iron).

## What this guide is NOT

- It does not endorse specific brands. Brand recommendations create implicit authority; ingredient-level analysis is the framework's contribution.
- It does not replace prescribing decisions. Anything requiring a prescription (levothyroxine, prenatal-targeted medications, retinoids) routes to the user's clinician with framework-prepared questions.
