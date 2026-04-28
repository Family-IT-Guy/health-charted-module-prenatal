# Optimal Ranges in Pregnancy

Pregnancy-specific optimal ranges, distinct from standard population reference ranges. Standard ranges are designed to flag disease in the general population; these ranges are calibrated for pregnancy outcomes based on RCT and meta-analysis evidence. Each range below is a threshold-claim with its own evidence base — apply [[pregnancy-optimal-vs-standard-ranges]] when interpreting.

## Sources

- `research/raw/03-measurement-diagnostics.md` — full per-marker analysis, evidence per cutoff
- `research/raw/02-nutrient-biochemistry.md` — biochemistry behind the markers
- `research/raw/06-postpartum-lactation.md` — postpartum-specific caveats

## Wiki pointers

- Concept: [[pregnancy-optimal-vs-standard-ranges]], [[ferritin-acute-phase-reactant-caveat]], [[iron-panel-interpretation]], [[b12-decision-tree]]
- Lab markers: [[ferritin]], [[hemoglobin]], [[transferrin-saturation]], [[rbc-folate]], [[serum-b12]], [[homocysteine]], [[tsh]], [[25-oh-vitamin-d]], [[hba1c]], [[urinary-iodine]]

## Tier 1: Essential (every person planning pregnancy)

| Marker | Test | Optimal Pre-Conception | Standard "Normal" | Why Different |
|--------|------|------------------------|-------------------|---------------|
| CBC | Hemoglobin | >12 g/dL | 12-16 g/dL | Drops ~2 g/dL by T3 from hemodilution; need buffer |
| CBC | MCV | 80-95 fL (investigate if >95) | 80-100 fL | >95 = early B12/folate depletion BEFORE anemia |
| CBC | RDW-CV | <14% | <14.5% | Elevated RDW = mixed cell populations from early deficiency |
| Iron | Ferritin | 50-100 mcg/L (minimum 30) | 15-200 mcg/L | WHO's 15 cutoff misses ~66% of depleted pregnant patients |
| Iron | Transferrin saturation | >25% (range 20-50%) | 20-50% | <20% = functional iron insufficiency even if ferritin OK |
| Folate | RBC folate | >1050 nmol/L (target 1050-1340) | 140-960 nmol/L | NTD prevention threshold; ~83% risk reduction at 1050+ |
| Folate | Serum folate | >20 nmol/L (>9 ng/mL) | 11-45 nmol/L | Recent intake only; RBC folate is the tissue measure |
| B12 | Serum B12 | >400 pg/mL | 200-900 pg/mL | 200-400 is "gray zone" where 5-10% have masked deficiency |
| B12 | Methylmalonic acid (MMA) | <0.4 mcmol/L | 0.1-0.4 mcmol/L | Catches functional deficiency that serum B12 misses |
| Vitamin D | 25(OH)D | 40-60 ng/mL | >30 ng/mL | 30 is skeletal floor; continued pregnancy benefit at 40-60 |
| Thyroid | TSH | <2.5 mIU/mL | 0.4-4.5 mIU/mL | Thyroid demand increases ~50% in pregnancy; marginal fails |
| Thyroid | Free T4 | 0.8-1.8 ng/dL | same | Baseline for tracking T1 decline |
| Thyroid | TPO antibodies | Negative (<35 IU/mL) | <35 IU/mL | Euthyroid TPO+ = ~2x miscarriage risk; treatable |
| Thyroid | Thyroglobulin Ab | Negative (<4 IU/mL) | <1-4 IU/mL | Independent miscarriage risk marker |
| Methylation | Homocysteine (fasting) | <10 mcmol/L (ideal <8) | 5-15 mcmol/L | >10 = functional methylation impairment; >12 = pregnancy loss risk |
| Glucose | Fasting glucose | <100 mg/dL | 70-100 mg/dL | >100 = impaired fasting glucose |
| Glucose | HbA1c | <5.7% | <5.7% | 6-7% = congenital malformation risk roughly doubles |
| Iodine | Spot urinary iodine | 100-299 mcg/L | 100-299 mcg/L | 7-10% of US women borderline deficient |

## Tier 2: Order if indicated

| Marker | When to Order | Optimal Range |
|--------|--------------|---------------|
| Free T3 | TSH borderline or investigating conversion | 2.3-4.2 pg/mL |
| Soluble transferrin receptor (sTfR) | Ferritin normal but MCV low; inflammation present | <3 mg/L |
| Holotranscobalamin (holoTC) | B12 in gray zone (200-400 pg/mL) | >30 pmol/L |
| MTHFR C677T + A1298C | Elevated homocysteine, prior NTD, recurrent loss | Wild-type is normal; TT = ~30% enzyme activity |
| HFE genotype | High ferritin, family history hemochromatosis | Negative; carriers should avoid routine iron |

## Interpreting Combined Iron Panel

| Ferritin | Transferrin Sat | Interpretation | Action |
|----------|----------------|----------------|--------|
| >50, TSAT >25% | | Iron replete | No supplementation needed |
| 30-50, TSAT >20% | | Adequate but building buffer reasonable | Consider low-dose iron |
| <30, TSAT >20% | | Depleted stores, functional iron still OK | Supplement now |
| >30, TSAT <20% | | Functional deficiency despite stores | Investigate: inflammation, copper, hemochromatosis |
| <30, TSAT <20% | | Combined deficiency | Aggressive supplementation |

## Ferritin Caveat

Ferritin is an acute-phase reactant. It rises with inflammation independent of iron status. In patients with concurrent infection, autoimmune conditions, or in the first ~6 weeks postpartum, ferritin may look normal while iron is depleted. Surface this when interpreting. See [[ferritin-acute-phase-reactant-caveat]].

## B12 Decision Tree

See [[b12-decision-tree]] for the full pattern. Summary:

- B12 >400 pg/mL: Replete. No further testing.
- B12 200-400 pg/mL (gray zone): Order holoTC + MMA.
  - HoloTC >30 AND MMA <0.4: Functionally adequate.
  - HoloTC <25 OR MMA elevated: Functional deficiency. Supplement.
- B12 <200 pg/mL: Deficient. Supplement immediately.
