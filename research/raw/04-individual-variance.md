---
date_created: 2026-03-22
topic: "Genetic variants, dietary patterns, and pre-existing conditions affecting prenatal nutrition"
entities:
  - mthfr-c677t
  - mthfr-a1298c
  - hfe-genotype
  - vegan-vegetarian-pattern
  - gestational-diabetes-mellitus
  - preeclampsia
  - thyroid-autoimmunity
research_id: RE-2026-0322-004
source_type: manual
source_ref: "prenatal nutrition first principles research"
depth: deep
triggered_by: on-demand
date: 2026-03-22
queries: 1
models_used: [sonar-deep-research, web-search-supplemental]
cost_estimate: $2.15
cascade_parent: null
---

# Prenatal Nutrition Genetics, Dietary Patterns, and Comorbidity Interactions

## Query 1: MTHFR, VDR, HFE variants; dietary patterns; comorbidities; medication interactions; inter-pregnancy interval
**Timestamp**: 2026-03-22T21:49:45Z
**Raw**: [raw/20260322_214945_mthfr-vdr-hfe-dietary-prenatal-nutrition-genetics.json](raw/20260322_214945_mthfr-vdr-hfe-dietary-prenatal-nutrition-genetics.json)
**Model**: sonar-deep-research | **Tokens**: 11,346 | **Cost**: $2.15
**Supplemental**: 12 WebSearch queries + 6 primary source deep reads via WebFetch

---

## Section 1: MTHFR C677T and A1298C Polymorphisms

### The Debate: What the Evidence Actually Shows

The MTHFR question is one of the most contested areas in prenatal nutrition. The clinical and consumer communities have diverged sharply from the institutional consensus.

#### Enzyme Activity by Genotype

| Genotype | Enzyme Activity Reduction | Population Frequency |
|----------|--------------------------|---------------------|
| C677T heterozygous (CT) | ~30% reduction | ~40% of population carries at least one variant |
| C677T homozygous (TT) | ~65-70% reduction | ~10-15% (varies by ethnicity; higher in Hispanic, Italian, Chinese populations) |
| A1298C heterozygous (AC) | Minimal clinical reduction | ~40% |
| A1298C homozygous (CC) | ~40% reduction (to ~60% normal function) | Variable |
| Compound heterozygous (C677T + A1298C) | ~40-50% reduction | ~15-20% |

Source: NCBI Medical Genetics Summaries; PMC11930790; MedlinePlus Genetics

#### CDC / Institutional Position (Favors Folic Acid)

The CDC states unequivocally: "People with an MTHFR gene variant can process all types of folate, including folic acid." Key evidence they cite:

- People with MTHFR 677 TT genotype have blood folate levels only ~16% lower than CC genotype when consuming identical folic acid amounts
- 400 mcg daily folic acid increases blood folate regardless of MTHFR genotype
- "Folic acid intake is more important than your MTHFR genotype for determining the amount of folate in your blood"
- Folic acid is the ONLY form of folate with RCT evidence for neural tube defect (NTD) prevention
- ACMG recommends against routine MTHFR screening

The CDC position rests on a critical fact: there are zero published clinical trials demonstrating that 5-MTHF (methylfolate) prevents NTDs. All NTD prevention evidence comes from folic acid studies.

Source: CDC MTHFR page (https://www.cdc.gov/folic-acid/data-research/mthfr/index.html)

#### Counter-Evidence (Favors Methylfolate)

A growing body of research raises legitimate concerns about folic acid in MTHFR carriers:

1. **Unmetabolized Folic Acid (UMFA)**: Synthetic folic acid requires conversion by dihydrofolate reductase (DHFR), which has weak activity in humans. One study found 86% of folic acid in the hepatic portal vein is unmetabolized. UMFA accumulation is associated with: decreased NK cell activity, potential DNA damage, cognitive concerns in offspring at high doses (PMC9380836).

2. **The "Folate Trap"**: When B12 is deficient, folate becomes trapped in its methylated form. Post-folic-acid-fortification, the prevalence of insufficient B12 combined with elevated serum folate increased from 0.09% to 0.61%, creating a metabolic imbalance (PMC11435006).

3. **Bioavailability**: 5-MTHF does not require metabolization and is directly absorbed. A study showed 400 mcg of methylfolate with B6 and B12 lowered homocysteine from 21.5 to 10.0 umol/L, outperforming 5 mg/day of folic acid (PMC9380836).

4. **Pregnancy supplementation**: Research demonstrated methylfolate was more efficient at increasing blood 5-MTHF levels than equivalent doses of folic acid through week 24 of pregnancy (PMC9380836).

5. **Fertility outcomes**: A case series of 33 couples with long-standing fertility issues found 800 mcg/day methylfolate led to successful pregnancy for 30 of 33 couples (PMC9380836). Note: case series, not RCT.

#### Clinical Reality Assessment

The debate has a structural asymmetry:

- **Folic acid** has RCT evidence for NTD prevention but no RCTs specifically in MTHFR TT carriers, and theoretical concerns about UMFA accumulation
- **Methylfolate** has mechanistic plausibility, pharmacokinetic superiority data, and case series evidence, but zero RCTs for NTD prevention

A 2024 evidence-based narrative review (PMC11435031) concluded: "Despite the potential value of 5-MTHF as an alternative to FA...clinical studies would be urgently needed" and "randomised controlled trials would have to be conducted to determine effectiveness."

#### Does Homozygous vs. Heterozygous Status Matter Clinically?

The evidence from a study of 102 pregnant women (PMC10787622) found NO significant difference in homocysteine levels across genotypes during mandatory folic acid supplementation (p=0.245 for C677T; p=0.073 for A1298C). The researchers concluded that "mandatory folic acid supplementation during pregnancy may play a crucial role in mitigating the adverse effects" of MTHFR mutations, with homocysteine normalization occurring regardless of genotype.

This is a critical finding: with adequate supplementation (either form), the genotype difference may be clinically irrelevant for homocysteine levels. The concern is specifically about whether folic acid supplementation is always "adequate" in TT homozygotes, and whether UMFA accumulation poses independent risks.

### Bottom Line on MTHFR

**High confidence**: Folic acid at 400+ mcg/day raises blood folate in all MTHFR genotypes. Homocysteine normalizes with adequate B-vitamin supplementation regardless of genotype.

**Moderate confidence**: Methylfolate is at least as bioavailable as folic acid and bypasses the MTHFR bottleneck. UMFA from high-dose folic acid may have adverse effects.

**Unresolved**: Whether methylfolate prevents NTDs (no clinical trial data). Whether the theoretical UMFA risks translate to clinically meaningful outcomes at standard 400-800 mcg doses. Whether TT homozygotes have meaningfully different outcomes with methylfolate vs folic acid when B12 is also adequate.

**Practical synthesis**: The safest evidence-based position is that either form works for most people, but methylfolate eliminates the theoretical UMFA concern without sacrificing efficacy. The risk of recommending methylfolate over folic acid is minimal (same or better bioavailability). The risk of recommending only folic acid to TT homozygotes is probably also minimal at standard doses with adequate B12 -- but carries theoretical concerns about UMFA.

---

## Section 2: VDR (Vitamin D Receptor) Genetic Variants

### Key Variants and Clinical Significance

Four VDR SNPs are most studied: FokI (rs2228570), TaqI (rs731236), BsmI (rs1544410), ApaI (rs7975232).

| VDR Variant | Effect on Vitamin D Response | Evidence Strength |
|-------------|-----------------------------|--------------------|
| FokI (FF genotype) | Better response to supplementation (p<0.001) | Moderate (meta-analysis, 8 studies, 1,038 subjects) |
| TaqI (Tt+tt) | Better response to supplementation (p=0.02) | Moderate |
| BsmI | No significant association (p=0.081) | Weak |
| ApaI | No significant association (p=0.63) | Null |

Source: PMC8780067 (systematic review and meta-analysis)

### Pregnancy-Specific Findings

- VDR ApaI and BsmI polymorphisms may be associated with hypertensive disorders of pregnancy (HDP) susceptibility (PMC10143592)
- FokI variant associated with HDP in Asian populations; BsmI variant associated in Caucasians -- population-specific effects
- VDR variants contribute to variations in vitamin D concentrations and increased prematurity risk

### Clinical Actionability

**Low to moderate**. The meta-analysis could not establish specific dose adjustments by genotype due to small sample sizes and heterogeneous study designs. The FokI and TaqI findings are suggestive but not yet actionable for clinical dosing decisions. No guidelines currently recommend VDR genotyping for vitamin D supplementation dosing in pregnancy.

---

## Section 3: HFE Gene Variants and Iron Absorption

### Variant Overview

| Mutation | Penetrance | Iron Absorption Effect |
|----------|-----------|----------------------|
| C282Y homozygous | Highest risk (clinical hemochromatosis) | Significantly increased |
| C282Y/H63D compound heterozygous | Moderate risk | Moderately increased |
| C282Y heterozygous (carrier) | Low risk | Mildly increased |
| H63D homozygous | Low risk | Mildly increased |
| H63D heterozygous | Minimal risk | Minimal effect |

### Pregnancy Implications

**Key finding**: Hemochromatotic women with elevated preconception ferritin levels probably do not require iron supplementation during pregnancy and breastfeeding (ASH Blood Journal, case study). One case showed maternal ferritin declining from 320+ ng/mL to a nadir of 66 ng/mL at 34 weeks, then rising to 145 ng/mL pre-delivery -- suggesting pregnancy naturally draws down iron stores.

**Contrary to common assumption**: A prospective observational study (PMC5816504) found pregnancy status has no protective impact on progressive iron accumulation in HFE hemochromatosis women -- meaning pregnancy does not "cure" or reliably reduce iron overload.

**Risks of supplementation in HFE carriers**:
- Preeclampsia risk (increased with iron overload)
- Gestational diabetes mellitus
- Offspring neurocognitive deficits
- Increased type 1 diabetes risk in offspring (Norwegian study of 94,209 pregnancies)

### Clinical Guidelines

EASL 2022 guidelines recommend individualized management. For HFE carriers in pregnancy:
- Monitor ferritin and transferrin saturation approximately every 4 weeks
- Do NOT routinely supplement iron if ferritin is elevated at conception
- Standard prenatal vitamins with iron may be contraindicated for C282Y homozygotes or compound heterozygotes with elevated baseline ferritin
- Iron-free prenatal vitamins exist and should be considered

---

## Section 4: Dietary Patterns and Supplementation Needs

### Vegan Pregnancy

**Critical gaps requiring supplementation:**

| Nutrient | Gap Severity | Supplementation Need | Notes |
|----------|-------------|---------------------|-------|
| Vitamin B12 | Critical | 2.6 mcg/day minimum; many sources recommend 250-500 mcg/day | No reliable plant sources. Fortified foods alone may be insufficient. |
| DHA/EPA | High | 200-300 mg DHA/day minimum | Algae-based DHA supplements (not fish oil). ALA conversion to DHA is only 1-10%. |
| Iron | High | 27 mg/day (same as all pregnant women) | Non-heme iron only; absorption enhanced by vitamin C, inhibited by tannins, phytates, calcium |
| Zinc | Moderate-High | 11 mg/day | Phytate in plant foods reduces bioavailability by up to 35% |
| Iodine | Moderate-High | 220 mcg/day in pregnancy | Variable in plant diets; seaweed is unreliable (huge variation) |
| Calcium | Moderate | 1000 mg/day | Achievable through fortified foods + supplements if dairy-free |
| Choline | Moderate | 450 mg/day | Rarely adequate in vegan diets; egg yolk is the richest source |

Source: USDA Dietary Guidelines; JANDONLINE S2212-2672(24)00751-2; NIH ODS Pregnancy Fact Sheet

### Vegetarian Pregnancy (Lacto-Ovo)

**Gaps narrower than vegan but still present:**

- **B12**: Adequate if consuming dairy and eggs regularly; still monitor serum levels
- **Iron**: Heme iron (from meat) is 15-35% absorbed; non-heme iron is 2-20% absorbed. Vegetarians need ~1.8x the iron RDA (48 mg/day) to compensate for lower bioavailability, per IOM
- **DHA**: Still a gap unless consuming eggs from DHA-fed hens (limited) or supplementing
- **Zinc**: Less severe than vegan (dairy provides zinc) but still reduced bioavailability from phytates
- **Iodine**: Dairy provides significant iodine; lacto-vegetarians may be adequate

### Omnivore Pregnancy

**Remaining gaps even with meat consumption:**

- **Folate**: Dietary intake alone rarely meets 600 mcg DFE recommendation; supplementation standard
- **Iron**: 27 mg/day is difficult to meet from food alone even with meat
- **Iodine**: Highly variable in diet; only 58% of top-selling US prenatals contain iodine
- **DHA**: Unless consuming 2+ servings fatty fish/week (which raises mercury concerns), supplementation recommended
- **Choline**: 90-95% of pregnant women do not meet the 450 mg/day adequate intake
- **Vitamin D**: Most women are deficient regardless of diet (see Section 6)

---

## Section 5: Pre-Existing Conditions and Nutrient Metabolism

### Thyroid Disorders (Hypothyroidism / Hashimoto's)

**Iodine**: ATA recommends 150 mcg/day supplement in pregnancy (total intake 250 mcg/day). For Hashimoto's specifically, iodine supplementation at guideline doses appears safe and does not significantly affect TPO antibody levels or thyroid hormones (American Thyroid Association, September 2021).

**Selenium**: L-selenomethionine at 83 mcg/day during pregnancy was safe and effective in lowering autoantibody titers and preventing postpartum thyroiditis relapse (RCT, double-blind). Upper limit: 400 mcg/day. A combined myo-inositol (600 mg) + selenium (83 mcg) supplement maintained normal thyroid levels in 94% of pregnant women vs 69% without (PMC11652148).

**Levothyroxine timing interactions**: Must separate from iron (4 hours), calcium (4 hours), and prenatal vitamins containing either (4 hours). This creates significant practical scheduling challenges for pregnant women on thyroid medication.

### PCOS (Polycystic Ovary Syndrome)

**Insulin resistance** affects 50-75% of PCOS patients and worsens during pregnancy.

| Supplement | Evidence | Effect |
|-----------|----------|--------|
| Myo-inositol | Strong (multiple RCTs) | Improves insulin sensitivity, ovulation, pregnancy rates |
| D-chiro-inositol | Moderate | Synergistic with myo-inositol at 40:1 ratio |
| Vitamin D | Strong | Improves insulin sensitivity, reduces inflammation; 70-85% of PCOS women are deficient |
| Omega-3 | Moderate | Reduces inflammation, improves lipid profile |
| Chromium | Moderate | Improves glucose metabolism |
| NAC (N-acetylcysteine) | Moderate | Antioxidant; comparable to metformin in some outcomes |

Note: These supplements have evidence for PCOS management and fertility, but limitations remain regarding standardized dosing and long-term pregnancy outcomes.

### Celiac Disease

**Malabsorption pattern**: The proximal small intestine is predominantly affected, leading to iron and folate malabsorption even in treated (gluten-free) patients. B12 deficiency prevalence in celiac patients: 8-41%.

**Pregnancy-specific risks**:
- Up to 4x increased preeclampsia risk with B12 deficiency
- 15% increased low birthweight risk
- 21% increased preterm birth risk
- The "folate trap" (B12 deficiency trapping folate in methylated form) is particularly relevant

**Bone health**: Gluten-free diet does not always normalize bone mineral density; vitamin D and calcium supplementation often needed long-term.

**Key recommendation**: Screen for both celiac disease and B12 deficiency in pregnant patients. Supplement B12 alongside folate (not just folate alone). Monitor iron, zinc, calcium, and vitamin D levels.

### Type 1 and Type 2 Diabetes

**Folate**: Higher dose (4-5 mg/day) recommended by most international guidelines (NICE, RCOG, WHO, RANZCOG) for preconception through week 12. However, NO RCTs specifically examine optimal folate dose in pre-existing diabetes. Evidence is consensus-based.

**Caution with high-dose folate**: A U-shaped association exists. Daily FA intake greater than or equal to 800 mcg or prolonged use (>3-6 months) may increase GDM risk. High folate + low B12 is particularly concerning.

**Vitamin D**: Low maternal vitamin D is associated with higher GDM risk. Supplementation improves fasting glucose, HbA1c, and insulin concentrations.

### Obesity (BMI 30+)

**Fat-soluble vitamin sequestration**: Vitamin D is sequestered in adipocyte lipid droplets. Radio-labelling shows 80% of administered vitamin D deposits in adipose tissue and releases very slowly.

**Dosing implications**:
- Standard 400 IU/day is inadequate for overweight/obese pregnant women
- 1000 IU/day achieved sufficient 25OHD (50 nmol/L) in 90% of pregnant women
- 800 IU/day produced 8.7-10.3 nmol/L higher 25OHD than 400 IU/day
- Obese women have lower vitamin D status despite higher dietary intake

Other fat-soluble vitamins (A, E, K) may also be affected by adipose sequestration, but less studied in pregnancy context.

---

## Section 6: Medication Interactions

### Metformin and B12

Metformin depletes B12 through multiple mechanisms: interference with calcium-dependent intrinsic factor binding, altered bile acid metabolism, reduced intrinsic factor secretion, bacterial overgrowth from altered gut motility.

- B12 deficiency is now considered a common side effect, especially with higher doses and longer treatment
- UK MHRA issued guidance: monitor B12 in all patients on metformin with risk factors
- **Combination risk**: Metformin + PPI together produces significantly higher hospitalization rates from B12 deficiency-related complications than either drug alone (PMC12562576)

### PPIs (Proton Pump Inhibitors)

Reduce gastric acid, which is needed to release dietary B12 from food proteins and for iron absorption. Effects:
- Reduced B12 absorption (particularly from food; crystalline B12 supplements less affected)
- Reduced non-heme iron absorption
- May reduce calcium absorption (increased fracture risk with long-term use)

### Levothyroxine

**Timing separation required:**
- Iron supplements: 4 hours apart
- Calcium supplements: 4 hours apart
- Prenatal vitamins (containing iron/calcium): 4 hours apart
- Take levothyroxine on empty stomach, 30-60 minutes before food

**Practical implication**: A pregnant woman on levothyroxine taking a prenatal vitamin with iron and calcium must carefully time doses. Some clinicians recommend bedtime levothyroxine dosing to simplify.

---

## Section 7: Inter-Pregnancy Interval and Nutrient Depletion

### WHO Recommendation

At least 24 months between pregnancies (from live birth to next conception). At least 6 months after miscarriage or abortion.

### Maternal Depletion Hypothesis

The theory: mothers with short interpregnancy intervals lack time to replenish macro- and micronutrients, leading to competition with the fetus for nutrients.

**Evidence status**: A systematic review (PMC6860904) found **no clear evidence** to support the maternal depletion hypothesis directly. Key limitations:
- Most studies scored low on quality scales (2 out of 4)
- Few studies measured micronutrients directly
- One study examining zinc, copper, magnesium, ferritin, folate, and TSH found NO significant relationship with interpregnancy interval
- Most studies failed to control for breastfeeding (a major confounder)

### What IS Established

- Lactation represents a greater nutritional burden than pregnancy itself: energy needs +25%, protein +54%, vitamin/mineral needs +0-93%
- Iron and folate are mobilized from maternal reserves during pregnancy and lactation
- Short intervals (<18 months) are associated with adverse outcomes (preterm birth, low birthweight), but the mechanism may not be nutrient depletion -- could be uterine healing, inflammatory recovery, or psychosocial factors

### Recovery Timeline

**No clear evidence-based timeline exists** for specific nutrient repletion. The systematic review found "no clear answer on recovery duration." The 24-month WHO recommendation is based on epidemiological outcome data (shorter intervals = worse outcomes) rather than measured nutrient recovery curves.

**Practical approach**: Monitor ferritin, B12, folate, vitamin D, and other relevant markers during interpregnancy period. Supplement based on measured deficiency rather than interval-based assumptions.

---

## Synthesis (Updated: 2026-03-22)

### Key Conclusions

1. **MTHFR**: The clinical significance is real but overstated in consumer markets and understated by institutional medicine. Homozygous TT carriers have a meaningful enzyme reduction (~70%), but adequate supplementation normalizes homocysteine regardless of genotype. The folic acid vs. methylfolate debate has a structural asymmetry: folic acid has NTD prevention RCTs; methylfolate has mechanistic and pharmacokinetic superiority data but no NTD prevention trials. Either form appears adequate at standard doses when B12 is also sufficient.

2. **VDR variants**: Clinically interesting but not yet actionable for dosing. FokI and TaqI modify supplementation response, but no guidelines support genotype-based dosing in pregnancy.

3. **HFE carriers**: Genuinely important for pregnancy management. C282Y homozygotes and compound heterozygotes should NOT receive routine iron supplementation without ferritin monitoring. Iron-free prenatals should be considered.

4. **Dietary patterns**: Vegan pregnancy requires supplementation of B12, DHA, and likely iron, zinc, iodine, choline. Vegetarian requires B12 monitoring, DHA supplementation, and higher iron intake. Omnivore still has common gaps in folate, iodine, DHA, choline, and vitamin D.

5. **Comorbidities**: PCOS, thyroid disorders, celiac disease, diabetes, and obesity each alter nutrient metabolism in specific, documented ways that standard prenatal vitamins may not address. Celiac disease malabsorption is particularly underappreciated.

6. **Medication interactions**: Metformin + PPI is a dangerous combination for B12 status. Levothyroxine timing with iron/calcium creates practical challenges. These interactions are well-documented but frequently overlooked in prenatal care.

7. **Inter-pregnancy interval**: The 24-month WHO recommendation is sound but the underlying "maternal depletion" mechanism is not well-evidenced. Monitor and supplement based on measured levels rather than interval-based assumptions.

### Open Questions

- Will any group fund an RCT of methylfolate vs folic acid for NTD prevention? (Unlikely -- folic acid already proven; ethical issues with placebo arm)
- What is the optimal vitamin D dose for obese pregnant women by BMI category?
- Does UMFA accumulation at standard 400-800 mcg folic acid doses produce clinically meaningful effects? (Most UMFA concerns are at high doses)
- What is the actual nutrient recovery timeline after pregnancy + lactation for specific micronutrients?

### Confidence Assessment

- **High confidence**: Folic acid works across MTHFR genotypes at standard doses; HFE carriers need ferritin-guided iron management; dietary pattern determines supplementation needs; medication interactions are well-documented
- **Moderate confidence**: Methylfolate is at least as effective as folic acid for raising blood folate; VDR variants modify vitamin D response; PCOS/thyroid/celiac require condition-specific supplementation
- **Needs verification**: Long-term effects of UMFA at standard doses; optimal inter-pregnancy nutrient recovery timeline; VDR-guided vitamin D dosing; methylfolate for NTD prevention specifically

### Sources

[1] CDC - MTHFR Gene Variant and Folic Acid Facts
    https://www.cdc.gov/folic-acid/data-research/mthfr/index.html
[2] PMC11930790 - Adverse Effects of Excessive Folic Acid and MTHFR C677T
    https://pmc.ncbi.nlm.nih.gov/articles/PMC11930790/
[3] PMC9380836 - Active Folate vs Folic Acid: Role of 5-MTHF in Human Health
    https://pmc.ncbi.nlm.nih.gov/articles/PMC9380836/
[4] PMC11435031 - 5-MTHF Supplementation and NTD Prevention (Narrative Review)
    https://pmc.ncbi.nlm.nih.gov/articles/PMC11435031/
[5] PMC10787622 - MTHFR Polymorphisms, Folic Acid, B12, Homocysteine in Pregnancy
    https://pmc.ncbi.nlm.nih.gov/articles/PMC10787622/
[6] PMC8780067 - VDR Polymorphisms Modify Vitamin D Supplementation Response (Meta-analysis)
    https://pmc.ncbi.nlm.nih.gov/articles/PMC8780067/
[7] PMC10143592 - VDR Polymorphisms and Hypertensive Disorders of Pregnancy (Meta-analysis)
    https://pmc.ncbi.nlm.nih.gov/articles/PMC10143592/
[8] ASH Blood Journal - Iron Studies in Hemochromatosis During Pregnancy
    https://ashpublications.org/blood/article/114/22/5099/77175/
[9] PMC5816504 - Pregnancies and Iron Overload in HFE Hemochromatosis Women
    https://pmc.ncbi.nlm.nih.gov/articles/PMC5816504/
[10] NIH ODS - Dietary Supplements and Pregnancy Fact Sheet
     https://ods.od.nih.gov/factsheets/Pregnancy-HealthProfessional/
[11] JANDONLINE - Vegetarian Diets During Pregnancy USDA Patterns
     https://www.jandonline.org/article/S2212-2672(24)00751-2/fulltext
[12] PMC11435006 - Folic Acid, B12 Deficiency in Pregnant Women with Celiac Disease
     https://pmc.ncbi.nlm.nih.gov/articles/PMC11435006/
[13] PMC10145371 - Folate Supplementation in Women with Pre-Existing Diabetes
     https://pmc.ncbi.nlm.nih.gov/articles/PMC10145371/
[14] PMC10780523 - Vitamin D Supplementation in Overweight/Obese Pregnancy (RCT)
     https://pmc.ncbi.nlm.nih.gov/articles/PMC10780523/
[15] PMC8311483 - Metformin and Vitamin B12 Deficiency
     https://pmc.ncbi.nlm.nih.gov/articles/PMC8311483/
[16] PMC6860904 - Birth Spacing and Maternal Nutritional Status (Systematic Review)
     https://pmc.ncbi.nlm.nih.gov/articles/PMC6860904/
[17] ATA - Iodine Supplementation in Pregnant Women with Hashimoto's
     https://www.thyroid.org/patient-thyroid-information/ct-for-patients/september-2021/vol-14-issue-9-p-13-14/
[18] PMC11652148 - Supplements for Hashimoto's: Systematic Review and Network Meta-Analysis
     https://pmc.ncbi.nlm.nih.gov/articles/PMC11652148/
[19] NCBI Bookshelf - MTHFR Deficiency Medical Genetics Summary
     https://www.ncbi.nlm.nih.gov/books/NBK66131/
[20] PMC12562576 - B12 Deficiency with Metformin and PPI Combinations
     https://pmc.ncbi.nlm.nih.gov/articles/PMC12562576/

### Related Questions (from Perplexity API)
- How do MTHFR polymorphisms affect pregnancy outcomes
- What are the benefits of methylfolate over folic acid for pregnant women
- How does vitamin D receptor status influence pregnancy complications
- Are there specific dietary recommendations for pregnant women with HFE hemochromatosis
- What role does myo-inositol play in managing PCOS-related infertility
