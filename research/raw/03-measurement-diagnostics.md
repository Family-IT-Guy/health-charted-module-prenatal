---
date_created: 2026-03-22
topic: "Lab markers and diagnostic interpretation in pregnancy with optimal-vs-standard ranges"
entities:
  - ferritin
  - hemoglobin
  - transferrin-saturation
  - rbc-folate
  - serum-b12
  - methylmalonic-acid
  - holotranscobalamin
  - homocysteine
  - tsh
  - free-t4
  - tpo-antibodies
  - 25-oh-vitamin-d
  - fasting-glucose
  - hba1c
  - urinary-iodine
research_id: RE-2026-0322-003
source_type: manual
source_ref: "prenatal nutrition first principles research"
depth: deep
triggered_by: on-demand
date: 2026-03-22
queries: 1
models_used: [sonar-deep-research]
cost_estimate: $2.14
cascade_parent: null
primary_sources_read: 6
waves_completed: 1
---

# Evidence-Based Pre-Conception Blood Panel for Women Planning Pregnancy

## Query 1: Comprehensive preconception blood panel with optimal pregnancy-specific ranges
**Timestamp**: 2026-03-22T21:49:41Z
**Raw**: [raw/20260322_214941_preconception-blood-panel-pregnancy-optimal-ranges.json](raw/20260322_214941_preconception-blood-panel-pregnancy-optimal-ranges.json)
**Model**: sonar-deep-research | **Tokens**: 15,531 | **Cost**: $2.14 | **Search queries**: 140

---

## Complete Recommended Panel

### Tier 1: Essential (order for every woman planning pregnancy)

| Marker | Test | Optimal Pre-Conception Range | Population Reference Range | Why the Difference Matters |
|--------|------|------------------------------|---------------------------|---------------------------|
| **CBC** | Hemoglobin | >12 g/dL | 12-16 g/dL | Drops ~2 g/dL by T3 from hemodilution; need buffer |
| | MCV | 80-100 fL (investigate if <80 or >95) | 80-100 fL | >95 fL = early B12/folate depletion signal BEFORE anemia |
| | RDW-CV | <14% | <14.5% | Elevated RDW with borderline MCV = mixed cell populations from early deficiency |
| **Iron panel** | Serum ferritin | 50-100 mcg/L (minimum 30) | 15-200 mcg/L | WHO's 15 cutoff misses 66% of iron-depleted pregnant women; 30 mcg/L better predicts transfusion risk |
| | Serum iron | 60-170 mcg/dL | 60-170 mcg/dL | High diurnal variation; interpret with TIBC |
| | TIBC | 250-450 mcg/dL | 250-450 mcg/dL | >450 = iron deficiency driving transferrin synthesis up |
| | Transferrin saturation | >25% (range 20-50%) | 20-50% | <20% = functional iron insufficiency for erythropoiesis even if ferritin looks OK |
| **Folate** | RBC folate | >1000 nmol/L (target 1050-1340) | 140-960 nmol/L | NTD risk reduction is dose-dependent; 1050-1340 nmol/L = maximal prevention (83% risk reduction) |
| | Serum folate | >20 nmol/L (>9 ng/mL) | 11-45 nmol/L | Reflects recent intake only; RBC folate is the real measure of tissue status |
| **B12** | Serum B12 | >400 pg/mL (>295 pmol/L) | 200-900 pg/mL | 200-400 pg/mL is the "gray zone" where 5-10% have functional deficiency masked by normal total B12 |
| | Holotranscobalamin (holoTC) | >30 pmol/L | 20-120 pmol/L | Active B12 fraction; more stable across pregnancy than total B12 |
| | Methylmalonic acid (MMA) | <0.4 mcmol/L (<350 nmol/L) | 0.1-0.4 mcmol/L | Rises before symptoms; elevated MMA + normal B12 = subclinical deficiency needing treatment |
| **Vitamin D** | 25(OH)D | 40-60 ng/mL (100-150 nmol/L) | >30 ng/mL "sufficient" | Continued risk reduction for preterm birth, preeclampsia, GDM documented at 40-60 range; 30 is a skeletal-health floor, not pregnancy optimal |
| **Thyroid** | TSH | <2.5 mIU/mL | 0.4-4.5 mIU/mL | ATA recommends 2.5 cutoff pre-conception; thyroid demand rises 50% in pregnancy, marginal function fails |
| | Free T4 | 0.8-1.8 ng/dL (10-23 pmol/L) | same | Baseline for tracking T1 decline when TBG rises |
| | TPO antibodies | <35 IU/mL (negative) | <35 IU/mL | Euthyroid TPO+ women: OR 1.94 for miscarriage (meta-analysis, 17 studies). LT4 treatment reduces miscarriage RR to 0.59 |
| | Thyroglobulin antibodies | <4 IU/mL (negative) | <1-4 IU/mL | Coexists with TPO Ab in 30-50% of cases; independent miscarriage risk marker |
| **Homocysteine** | Fasting tHcy | <10 mcmol/L (ideal <8) | 5-15 mcmol/L | >10 = functional deficiency in methylation cycle even if B12/folate serum levels look normal; >12 = investigate aggressively |
| **Glucose** | Fasting glucose | <100 mg/dL | 70-100 mg/dL | >100 = impaired fasting glucose; warrants OGTT |
| | HbA1c | <5.7% (ideal <6% if diabetic) | <5.7% normal | Dose-response: HbA1c 6-7% = congenital malformation risk doubles to 4-5%; >7% = 8-10% |
| **Iodine** | Spot urinary iodine | 100-299 mcg/L (median) | 100-299 mcg/L adequate | 7-10% of US reproductive-age women are borderline deficient; most prenatal vitamins have insufficient iodine (<50 mcg vs 150 mcg needed) |

### Tier 2: Recommended for specific populations

| Marker | When to Order | Optimal Range |
|--------|--------------|---------------|
| Free T3 | If TSH borderline or investigating thyroid conversion | 2.3-4.2 pg/mL (3.5-6.4 pmol/L) |
| Soluble transferrin receptor (sTfR) | Ferritin normal but MCV low or RDW elevated; inflammation present | 0.9-2.8 mg/L; >3 mg/L = functional iron deficiency despite normal ferritin |
| MTHFR C677T + A1298C | Recurrent pregnancy loss, prior NTD, family history NTD, elevated homocysteine | Wild-type (CC/AA) is normal; TT homozygous = 30% enzyme activity |
| MTRR A66G | Combined with MTHFR testing in high-risk women | 66GG + 677TT = synergistic derangement |

---

## Marker-by-Marker Deep Analysis

### 1. CBC: MCV as Early Warning System

MCV is underutilized when clinicians focus only on hemoglobin. The key insight: **MCV changes precede anemia**.

- **MCV >95 fL**: Investigate for B12/folate depletion even with normal hemoglobin (>12 g/dL). This is macrocytic morphology representing the earliest hematologic sign of functional deficiency.
- **MCV <80 fL**: Iron deficiency until proven otherwise (exclude thalassemia trait, chronic disease).
- **RDW-CV >14%**: Mixed cell populations (normal + abnormal RBCs circulating together) = early deficiency or recovery. Combined elevated RDW + borderline MCV should trigger functional marker workup.

Practical note: Reticulocyte count <2% with low-normal hemoglobin or elevated MCV = inadequate bone marrow response. Suggests absolute micronutrient deficiency rather than recovery.

### 2. Iron Panel: Why Ferritin Is King

**The central problem**: Hemoglobin stays normal until iron stores are completely exhausted. By the time Hb drops, you're months behind.

Ferritin timeline:
- Ferritin drops first (stores depleting)
- Then TSAT drops (functional iron insufficient)
- Then MCV drops (microcytic cells start appearing)
- Finally hemoglobin drops (frank anemia)

**Critical ferritin thresholds**:
- WHO definition of iron deficiency: <15 mcg/L (misses majority of depleted women in pregnancy context)
- Better predictor for pregnancy: <30 mcg/L (at this cutoff, 66.6% of first-trimester women show depleted stores vs only 29% at the WHO cutoff)
- **Optimal pre-conception target**: 50-100 mcg/L (provides buffer for the 3-6 month draw-down during pregnancy)
- Postpartum transfusion risk: ROC analysis identified ferritin 20-25 mcg/L as threshold predicting transfusion need in non-anemic women

**Interpreting the combined panel**:
| Ferritin | TSAT | Interpretation |
|----------|------|----------------|
| >30, TSAT >20% | Normal | Iron replete |
| <30, TSAT >20% | Depleted stores, functional iron still OK | Supplement now |
| >30, TSAT <20% | Functional deficiency despite stores | Investigate: inflammation, copper deficiency, hemochromatosis |
| <30, TSAT <20% | Combined deficiency | Aggressive supplementation needed |

**Ferritin caveat**: Ferritin is an acute phase reactant. It rises with inflammation independent of iron status. In women with concurrent infection or chronic inflammatory conditions, ferritin may look normal while iron is depleted. This is where sTfR adds value (not affected by inflammation).

### 3. Folate: RBC Folate vs Serum Folate

**Serum folate** = what you ate this week. Changes in days.
**RBC folate** = integrated status over 120-day RBC lifespan. Changes in weeks to months.

For pre-conception, RBC folate is the test that matters. Serum folate is a snapshot; RBC folate is the movie.

**Neural tube defect prevention thresholds**:
- Standard supplementation (400 mcg/day folic acid): reduces NTD risk ~50-70%
- Optimal RBC folate target: **1050-1340 nmol/L** = 83% NTD risk reduction (from randomized trials using 4 mg daily)
- Population reference "normal" (140-960 nmol/L) is inadequate for pregnancy prevention targets
- Time to reach optimal RBC folate on 4 mg/day folic acid: ~20 weeks (5 months)
- Implication: **start folic acid supplementation 5-6 months before intended conception**, not the commonly cited 1-3 months

**The serum-RBC folate discordance problem**:
- Early in supplementation: serum folate rises quickly (days), RBC folate lags (months). Checking only serum folate overestimates tissue repletion.
- Early in deficiency: serum folate drops first, RBC folate preserved temporarily. Checking only serum folate correctly identifies the problem earlier.
- For pre-conception assessment: **check both**. Baseline RBC folate establishes tissue status. Recheck RBC folate 12 weeks after starting supplementation to verify tissue normalization.

### 4. Vitamin B12: The Gray Zone Problem

**The core issue**: Serum B12 has low sensitivity and specificity for functional deficiency. ~5-10% of people with "normal" serum B12 (200-400 pg/mL) have tissue-level insufficiency.

**Why serum B12 misleads**: Total serum B12 measures both active B12 (bound to transcobalamin, delivered to cells) and inactive B12 (bound to haptocorrin, not bioavailable). You can have plenty of haptocorrin-bound B12 inflating the number while cells are starving.

**The decision tree**:
- B12 >400 pg/mL: Replete. No further testing needed.
- B12 200-400 pg/mL (gray zone): Order holoTC + MMA.
  - HoloTC >30 pmol/L AND MMA <0.4 mcmol/L: Functionally adequate despite borderline serum level.
  - HoloTC <25 pmol/L OR MMA elevated: Functional deficiency. Supplement regardless of serum B12.
- B12 <200 pg/mL: Deficient. Supplement immediately.

**Pregnancy-specific B12 dynamics** (from UK cohort of 114 pregnant women):
| Marker | T1 (wk 12) | T2 (wk 20) | T3 (wk 34) |
|--------|------------|------------|------------|
| Serum B12 (pmol/L) | 224 (median) | 205 | 173 |
| HoloTC (pmol/L) | 68 | 63 | 53 |
| MMA (nmol/L) | 143 | 150 | 174 |
| tHcy (mcmol/L) | 4.6 | 4.4 | 5.4 |

Key finding: HoloTC remained more stable across pregnancy than total B12, making it the better tracking marker. Serum B12 declined 23% from T1 to T3 (physiologic, not necessarily deficiency), while MMA rose 22% (potentially concerning -- needs functional interpretation).

**Vegan/vegetarian flag**: MMA elevated in up to 55% of vegans despite preserved serum B12. Dietary assessment is mandatory alongside lab interpretation.

### 5. Vitamin D: Why 30 ng/mL Is Not Enough

**The disconnect**: Population guidelines set 30 ng/mL as "sufficient" based on skeletal health (calcium absorption, bone density). Pregnancy evidence shows continued benefit at higher levels.

**Evidence for 40-60 ng/mL target**:
- Preterm birth: 25(OH)D deficiency (<20 ng/mL) associated with preterm birth rate 6.7% vs 2.3% (adjusted OR 2.56, CI 1.02-6.42)
- Twin pregnancies: hypertensive disorders 27.8% in severely deficient (<10) vs 12.5% in sufficient (>30); p=0.045
- Birth weight: deficient group mean 2850g vs insufficient group 2975g (p=0.041)
- Developmental delay at 1 year: 8.9% in deficient vs 2.0% (OR 3.94)
- NEC risk: 3.3% deficient vs 0.3% (OR 12.5)
- IVF data: vitamin D deficiency significant predictor of clinical pregnancy failure (OR 0.74, p=0.022)

**Supplementation to reach targets**:
- Baseline <20 ng/mL: 4000-6000 IU/day vitamin D3; recheck in 8-12 weeks
- Baseline 20-30 ng/mL: 2000-4000 IU/day; recheck in 8-12 weeks
- Target achievement: 40-60 ng/mL before conception
- Caveat: 71.7% of pregnant women in one large study were deficient (<20 ng/mL). This is extremely common and under-tested.

### 6. Thyroid Panel: The 50% Demand Increase

**Why pregnancy stresses the thyroid**: hCG structurally resembles TSH and stimulates TSH receptors in T1. Estrogen increases TBG (binding protein), reducing free hormone. Renal iodine clearance increases. Fetus relies entirely on maternal thyroid hormone until week 12-14. Net effect: thyroid output must increase ~50%.

**Trimester-specific TSH ranges** (vs non-pregnant 0.4-4.5 mIU/mL):
| Trimester | TSH Range | Why |
|-----------|-----------|-----|
| T1 | 0.1-2.5 mIU/mL | hCG suppresses TSH; this is normal, not hyperthyroid |
| T2 | 0.2-3.0 mIU/mL | hCG declining, TSH normalizing |
| T3 | 0.3-3.0 mIU/mL | Approaching non-pregnant but still lower upper limit |

**Pre-conception TSH interpretation**:
- <2.5 mIU/mL: Optimal for pregnancy planning (ATA recommendation)
- 2.5-4.0 mIU/mL: Subclinical hypothyroidism territory, especially if TPO+. Increased miscarriage risk. Treat with levothyroxine.
- >4.0 mIU/mL: Overt subclinical hypothyroidism. Treat regardless of antibody status.

**The TPO antibody problem**: Euthyroid (normal TSH, normal FT4) women who are TPO-positive have nearly double the miscarriage risk (OR 1.94, 95% CI 1.43-2.64, meta-analysis of 17 studies). Mechanism: autoimmune thyroid inflammation impairs the gland's ability to meet the 50% pregnancy demand increase. It works at baseline but fails under load.

**Treatment evidence for TPO+ women**: Levothyroxine in TPO+ women with recurrent pregnancy loss:
- Miscarriage rate: RR 0.59 (CI 0.44-0.79) -- 41% reduction
- Premature delivery: RR 0.48 (CI 0.32-0.72) -- 52% reduction
- Fetal growth restriction: RR 0.33 (CI 0.12-0.89) -- 67% reduction

Practical recommendation: Screen ALL pre-conception women for TPO antibodies. If positive, even with normal TSH, discuss levothyroxine (25-50 mcg) especially with any history of pregnancy loss.

### 7. Homocysteine: The Methylation Cycle Integrator

Homocysteine is not a single-nutrient marker. It's a system-level readout of whether the one-carbon methylation cycle is functioning.

**What elevated homocysteine tells you**:
- B12 deficient: homocysteine rises (remethylation impaired)
- Folate deficient: homocysteine rises (remethylation impaired)
- B6 deficient: homocysteine rises (transsulfuration impaired)
- MTHFR polymorphism: homocysteine rises (folate conversion impaired)
- Renal dysfunction: homocysteine rises (clearance impaired)
- Hypothyroidism: homocysteine rises

**Pre-conception targets**:
- <10 mcmol/L: Adequate methylation function
- 10-12 mcmol/L: Borderline. Optimize B12, folate, B6.
- >12 mcmol/L: Investigate aggressively. Associated with recurrent pregnancy loss.
- >15 mcmol/L: Hyperhomocysteinemia. Strong association with miscarriage, especially with thrombophilia.

**Study data (Georgian women with PCOS)**:
- Controls (no PCOS): mean tHcy 7.3 +/- 2.2 mcmol/L
- PCOS with successful pregnancies: 10.3 +/- 2.6
- PCOS with recurrent pregnancy loss: 13.7 +/- 2.7
- MTHFR C677T carriers had significantly higher levels

**Treatment protocol for elevated homocysteine**:
- High-dose folic acid: 1000+ mcg/day (or methylfolate if MTHFR+)
- B12: 1000 mcg/day
- B6: 50-100 mg/day
- Start in pre-conception period. Recheck homocysteine 8-12 weeks after starting.

### 8. Urinary Iodine: The Forgotten Nutrient

**Why it matters**: Iodine is the rate-limiting substrate for thyroid hormone synthesis. Fetal brain myelination (weeks 10-28) requires thyroid hormone. Iodine deficiency = impaired fetal neurocognitive development independent of maternal thyroid function tests appearing normal.

**WHO categories**:
- <50 mcg/L: Severe deficiency
- 50-99 mcg/L: Inadequate
- 100-299 mcg/L: Adequate
- >300 mcg/L: Excessive

**The gap in prenatal care**: Most prenatal vitamins contain <50 mcg iodine. The recommended supplementation is 150 mcg/day (as potassium iodide). 7-10% of US reproductive-age women are borderline deficient despite salt iodization programs.

**Practical**: Order spot urinary iodine. If <100 mcg/L, supplement with 150 mcg iodine daily in addition to prenatal vitamin. Recheck 4-6 weeks later.

### 9. Glucose and HbA1c: The Teratogenicity Threshold

**Congenital malformation risk by HbA1c** (dose-response, organogenesis weeks 5-10):
| Pre-conception HbA1c | Malformation Risk |
|----------------------|-------------------|
| <6% | ~2% (baseline) |
| 6-7% | 4-5% (doubled) |
| 7-8% | 8-10% |
| >8% | Higher still |

**Pre-conception targets**:
- Non-diabetic: HbA1c <5.7%, fasting glucose <100 mg/dL
- Prediabetic (5.7-6.4%): Intensive lifestyle modification (Mediterranean/DASH diet, 150 min/week exercise, 5-10% weight loss if overweight). Recheck in 8-12 weeks. Consider metformin if persistent.
- Diabetic planning pregnancy: HbA1c <6% before conceiving. This is the single most important pre-conception intervention for diabetic women.

---

## Trimester-Specific Retesting Schedule

| Marker | When to Recheck | Why |
|--------|----------------|-----|
| **TSH** | First prenatal visit (<12 wk), 30 wk if risk factors | T1 hCG suppresses TSH (normal); T3 demand increases, subclinical hypothyroidism can emerge |
| **Hemoglobin + ferritin** | Each trimester | Hemodilution drops Hb ~2 g/dL by T3; ferritin drops from 50-100 to 15-30 by T3 even with adequate stores |
| **Iron panel (full)** | T2 if ferritin was borderline pre-conception | Progressive iron mobilization; hepcidin suppresses to maximize absorption |
| **B12 + holoTC + MMA** | T2 if pre-conception gray zone | Serum B12 declines 23% by T3 (physiologic); MMA may rise; holoTC most stable tracker |
| **RBC folate** | T1 (baseline), T3 if on standard supplementation | New RBCs incorporate diluted folate; T3 RBC folate <5 ng/mL serum = increase supplementation |
| **25(OH)D** | T1 to confirm achievement, T2-T3 if started deficient | Supplementation adequacy; seasonal variation |
| **HbA1c** | T1 if pre-conception elevated; OGTT at 24-28 wk (universal) | GDM screening is standard of care |
| **Urinary iodine** | T1 if pre-conception deficient | Confirm supplementation response |
| **Homocysteine** | T1 if pre-conception elevated | Pregnancy normally lowers it; persistent elevation suggests inadequate supplementation |

---

## Serum vs Functional Markers: Where Serum Misleads

| Nutrient | Serum Marker (what's measured) | Limitation | Functional Marker (what to add) | What the Functional Marker Catches |
|----------|-------------------------------|------------|--------------------------------|----------------------------------|
| B12 | Serum B12 | 5-10% false normal (haptocorrin-bound B12 inflates total) | HoloTC + MMA | Tissue-level deficiency when serum looks fine |
| Folate | Serum folate | Reflects last few days of intake only | RBC folate | 120-day integrated tissue status |
| Iron | Ferritin | Elevated by inflammation (acute phase reactant) | sTfR, or ferritin/sTfR ratio | Functional iron deficiency despite "normal" ferritin in inflammatory states |
| B12/Folate/B6 | Individual serum levels | Each can appear normal while system is impaired | Homocysteine | Integrated methylation cycle function |

---

## Genetic Testing: MTHFR and Beyond

### MTHFR: What the Evidence Actually Says

**C677T variant** (rs1801133):
- CC (wild-type): 100% enzyme activity
- CT (heterozygous): ~65% activity
- TT (homozygous): ~30% activity (most clinically significant)
- Population frequency: Higher in East Asian and Hispanic populations; lower in African ancestry

**A1298C variant** (rs1801131):
- AA (wild-type): 100% activity
- AC (heterozygous): ~60% activity
- CC (homozygous): ~80% activity (less severe than C677T)

**Compound heterozygosity** (C677T + A1298C): ~60-65% activity. Intermediate phenotype.

**Clinical consequences of reduced MTHFR activity**:
- Impaired conversion of 5,10-methyleneTHF to 5-methylTHF (the active folate form for homocysteine remethylation)
- Elevated homocysteine
- Reduced RBC folate
- Associations: NTD, recurrent miscarriage, preeclampsia, offspring neurodevelopmental conditions
- IVF data: oocyte maturation potential gradually decreases with MTHFR activity reduction (n=1160 IVF/ICSI cycles)

**Should you order it?**

Current professional guidelines (ACOG, ACMG) do NOT recommend routine MTHFR testing for the general population. Rationale: no large RCTs proving MTHFR-guided supplementation improves outcomes vs standard supplementation.

However, the evidence supports testing in **specific populations**:
- Recurrent pregnancy loss (especially unexplained, normal karyotype)
- Personal or family history of NTDs
- Preeclampsia history
- Elevated homocysteine (>10 mcmol/L)
- Ethnic backgrounds with higher polymorphism frequency

**Methylfolate vs folic acid**: Theoretically, methylfolate (5-MTHF) bypasses the MTHFR enzyme defect. Practical evidence: no RCTs showing methylfolate superiority. Current recommendation: MTHFR+ women should take enhanced folic acid (1000+ mcg/day). If homocysteine fails to normalize after 8-12 weeks, consider switching to methylfolate (500-1000 mcg/day).

### MTRR A66G

Methionine synthase reductase variant. GG homozygotes have reduced methionine synthase activity. When combined with MTHFR 677TT, produces synergistic metabolic derangement (markedly elevated homocysteine, reduced RBC folate, elevated MMA). Test when MTHFR results show mutations and homocysteine remains elevated despite supplementation.

### Emerging (Not Standard of Care)

- **VDR polymorphisms** (FokI, BsmI, ApaI, TaqI): Affect vitamin D bioavailability and supplementation response. FokI ff carriers may need lower doses; FF carriers may need higher. Not yet clinically actionable but explains why some women remain deficient despite adequate supplementation.
- **COMT Val158Met**: Affects catecholamine and estrogen metabolism. Theoretical fertility implications. No clinical recommendations exist.
- **Serum hepcidin**: Iron-regulatory hormone. Suppresses below 4 ng/mL when iron-depleted to maximize absorption; >30 ng/mL when replete. ROC analysis shows AUROC 0.86-0.88 for detecting iron deficiency (superior to ferritin alone). Not yet standardized for clinical use but emerging.

---

## Pre-Conception Supplementation Timeline

Based on the evidence, the ideal pre-conception preparation window is **5-6 months** (not the commonly cited 1-3 months):

| Timepoint | Action |
|-----------|--------|
| 6 months pre-conception | Baseline blood panel (full panel above). Start folic acid 400-1000 mcg/day. |
| 5 months | Results back. Start targeted supplementation based on deficiencies. |
| 3 months | Recheck functional markers (RBC folate, homocysteine, MMA if B12 was gray zone, 25(OH)D, ferritin). |
| 2 months | Confirm normalization. Adjust doses if needed. |
| Conception | All markers optimized at tissue level, not just serum level. |

The 5-6 month window is driven by:
- RBC folate requires 8-12 weeks to reach optimal compartmentalization
- At 4 mg/day folic acid, reaching RBC folate 1050-1340 nmol/L takes ~20 weeks
- Ferritin normalization from deficiency: weeks to months depending on severity
- Vitamin D repletion from <20 ng/mL: 8-12 weeks at 4000-6000 IU/day

---

## Primary Source Findings

### Frontiers in Nutrition (2021) - B12 Biomarkers Throughout Pregnancy
- Confirmed trimester-specific B12 marker trajectories in 114 UK women
- HoloTC more stable than total B12 across pregnancy (key finding supporting holoTC as preferred tracker)
- MMA rose from 143 to 174 nmol/L T1-T3 (22% increase)
- "None of the biomarkers could reliably predict any other biomarkers than themselves later in pregnancy"

### Ukrainian Pre-Pregnancy Study - MTHFR and Recurrent Loss
- Women with EPL + adenomyosis: 50% C677T heterozygous, 80% had A1298C polymorphisms
- Homocysteine: 12.8 +/- 2.3 mcmol/L (significantly elevated)
- Folate: 5.0 +/- 0.9 ng/mL (deficient)
- Recommended: methylfolate 400 mcg + methylcobalamin 2.5 mcg + B6 + betaine for 3 months pre-conception

### De Gruyter (2017) - Vitamin D at Term
- 71.7% of 575 pregnant women vitamin D deficient (<20 ng/mL) at term
- Only 7.3% had adequate levels (>30 ng/mL)
- Interestingly: no significant associations with GDM, hypertension, preeclampsia in this study (conflicts with other evidence; may reflect population or power issues)

### Twin Pregnancy Thyroid Study (2025)
- Twin-specific TSH intervals needed (median 0.62 mIU/L vs singleton 1.17 mIU/L)
- Twin-specific FT4 higher (15.40 pmol/L vs 14.80 singleton)
- Low FT4 linked to SGA, LGA, emergency cesarean, fetal distress
- Low TSH associated with preeclampsia

### Leads Followed
- Accessed 6 primary sources via WebFetch; several academic journal paywalls blocked full text retrieval (Karger, Wiley, BMJ, AHA journals returned 403/paywall)
- Evidence base is consistent across sources on core recommendations
- The vitamin D evidence shows some heterogeneity (one null study at term; multiple positive studies earlier in pregnancy), suggesting timing of measurement matters

---

## Sources

[1] Frontiers in Nutrition - "Evaluating the Diagnostic Value of a Combined Indicator of Vitamin B12 Status (cB12) Throughout Pregnancy"
    https://www.frontiersin.org/articles/10.3389/fnut.2021.789357/full

[2] Reproductive Health (Ukraine) - "Pre-pregnancy training of women with early pregnancy loss and adenomyosis, taking into account folate cycle gene polymorphisms"
    https://repro-health.com.ua/article/view/301602

[3] De Gruyter - "Vitamin D deficiency in pregnancy at term: risk factors and pregnancy outcomes"
    https://www.degruyterbrill.com/document/doi/10.1515/hmbci-2017-0005/html

[4] Frontiers in Endocrinology - "First-trimester thyroid reference intervals in twin pregnancy"
    https://www.frontiersin.org/articles/10.3389/fendo.2025.1700641/full

[5] AJJMS - "Role of Haematological Markers Predicting in Vitamin B12, B9 Status in Women"
    https://ajjms.com/article/role-of-haematological-markers-predicting-in-vitamin-b12-b9-status-in-women/

[6] MDPI Nutrients - "Vitamin D: Evidence-Based Health Benefits and Recommendations"
    https://www.mdpi.com/2072-6643/17/2/277

[7] Human Reproduction Open - "MTHFR C677T/A1298C combination polymorphisms and IVF/ICSI outcomes"
    https://academic.oup.com/hropen/article/doi/10.1093/hropen/hoac055/6873744

[8] Elsevier - "Serum Hepcidin Concentrations Decline during Pregnancy and May Identify Iron Deficiency"
    https://linkinghub.elsevier.com/retrieve/pii/S0022316622107728

[9] BMC Pregnancy Childbirth - "Pre-conception blood pressure and evidence of placental malperfusion"
    https://bmcpregnancychildbirth.biomedcentral.com/articles/10.1186/s12884-019-2699-3

[10] BMJ (2022) - Preconception care review
    https://www.bmj.com/lookup/doi/10.1136/bmj-2021-067728

### Related Questions (from Perplexity)
- What are the optimal ranges for thyroid function tests during each trimester of pregnancy
- How does thyroid function change throughout pregnancy and why is it important to monitor it
- What are the key differences in thyroid hormone levels between non-pregnant women and pregnant women
- How do changes in thyroxine-binding globulins affect thyroid function during pregnancy
- What are the implications of untreated thyroid disease during pregnancy on maternal and fetal health

---

## Synthesis (Updated: 2026-03-22)

### Key Conclusions

1. **The standard pre-conception panel is inadequate.** Hemoglobin alone for iron, serum B12 alone for B12, serum folate alone for folate, and non-pregnant TSH ranges for thyroid all produce meaningful rates of missed deficiency. Functional markers (MMA, holoTC, RBC folate, homocysteine) and pregnancy-specific thresholds are required.

2. **Optimal ranges differ substantially from population reference ranges.** Ferritin 50-100 vs WHO's 15. RBC folate >1050 nmol/L vs lab range of 140-960. 25(OH)D 40-60 ng/mL vs 30. TSH <2.5 vs 4.5. These aren't aspirational stretch goals; they're the levels at which adverse outcome rates demonstrably decrease.

3. **The pre-conception window needs to be 5-6 months, not 1-3.** RBC folate compartmentalization at therapeutic doses takes up to 20 weeks. Ferritin normalization takes months. Vitamin D repletion from deficiency takes 8-12 weeks. Starting prenatal vitamins a month before trying to conceive is too late for tissue-level optimization.

4. **TPO antibodies are a miscarriage risk factor independent of thyroid function.** Euthyroid TPO+ women have nearly double the miscarriage risk (OR 1.94). Levothyroxine treatment produces significant reductions in miscarriage (41%), preterm delivery (52%), and fetal growth restriction (67%). This is one of the most actionable findings for women with recurrent loss.

5. **MTHFR testing is not recommended for the general population but is warranted in specific clinical contexts.** The professional society position (no routine testing) is reasonable given no RCTs. The individual clinical position (test if recurrent loss, NTD history, elevated homocysteine) is also evidence-based. These are not contradictory positions.

6. **Homocysteine is the most undervalued marker.** It integrates B12, folate, and B6 status simultaneously. Levels >10 mcmol/L warrant investigation; >12 mcmol/L is associated with recurrent pregnancy loss. It catches functional methylation cycle failure that individual nutrient serum levels can miss.

7. **Iodine is the most under-tested nutrient.** Despite being rate-limiting for thyroid hormone synthesis and critical for fetal neurodevelopment, it's routinely omitted from pre-conception panels. Most prenatal vitamins provide insufficient amounts.

### Open Questions

- Optimal hepcidin cutoffs for pre-conception iron assessment (promising but not standardized)
- Whether VDR genotyping should guide vitamin D supplementation dose
- Whether methylfolate is truly superior to folic acid in MTHFR+ women (no RCTs)
- Optimal B12 supplementation dose and form (cyanocobalamin vs methylcobalamin) in MTHFR/MTRR carriers
- Whether the 40-60 ng/mL vitamin D target applies uniformly or is population-dependent

### Confidence Assessment

- **High confidence**: Iron panel with ferritin 50-100 target; RBC folate >1050 nmol/L for NTD prevention; TSH <2.5 pre-conception; TPO antibodies as miscarriage predictor; HbA1c dose-response for malformations; homocysteine <10 target; 5-6 month pre-conception window
- **Moderate confidence**: Vitamin D 40-60 ng/mL (evidence direction consistent but some heterogeneity in studies); MMA/holoTC decision tree for gray zone B12 (logic sound, not all labs offer holoTC); iodine supplementation protocol (WHO guidance clear, clinical implementation less standardized)
- **Needs verification**: MTHFR-guided methylfolate vs folic acid superiority; hepcidin clinical utility; VDR polymorphism actionability; COMT relevance to fertility
