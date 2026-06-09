# Cancer Epidemiology and Risk Factors

## Learning Objectives

By the end of this chapter you should be able to:

- **Distinguish** raw case counts from age-standardized rates, and explain why an aging population raises cancer counts even when individual risk is stable.
- **Explain** how genes and environment jointly determine cancer risk, and why treating them as mutually exclusive is misleading.
- **Apply** causal-inference reasoning (the Bradford Hill criteria) to evaluate whether a risk-factor association is causal.
- **Analyze** how a named exposure produces molecular damage that elevates cancer risk, and identify the prevention point that interrupts it.

## Opening Case

A 65-year-old man arrives with a lung mass on a chest scan. He has a 40 pack-year smoking history and spent two decades around asbestos insulation. The radiologist, the surgeon, and the oncologist all read the same image differently from how they would read it in a lifelong non-smoker with no occupational exposure — not because the shadow looks different, but because the *prior probability* that this shadow is cancer is far higher in this man.

Here is the trap the case sets. It is tempting to convert that elevated risk into blame — to treat the diagnosis as the predictable wage of a personal choice. But two of his biggest risk factors behave very differently. Smoking was, in part, a voluntary exposure; asbestos was a structurally imposed one — a workplace hazard he could not see, did not choose, and was rarely warned about. Both raise risk through the same kind of mechanism: molecules that damage DNA, mutations that accumulate over decades. Epidemiology's job is not to assign blame. It is to give the prior probability — *given these exposures, this age, this history, what is the chance this is cancer?* — and to identify where the chain could have been interrupted.

This chapter builds the tools behind that prior: the global burden of cancer, how genes and environment interact, the major modifiable risk factors, and the rules for deciding when an association is a cause.

## Core Concepts

### Burden and rates

Epidemiology supplies the denominator. **Incidence** is new cases per population per year; **mortality** is deaths; **prevalence** is people living with the disease. The crucial distinction is between raw **counts** and **age-standardized rates** — rates adjusted so that populations with different age structures can be compared. Because cancer is overwhelmingly a disease of age, an aging population produces more cancer *cases* even if each person's age-specific risk is unchanged. Confusing the two is the most common quantitative error in reading cancer statistics.

Globally in 2022, the International Agency for Research on Cancer (IARC) estimated about 20 million new diagnoses and 9.7 million deaths, drawn from the GLOBOCAN database compiling registries from over 185 countries (IARC, 2024). These are the best numbers available — and imperfect: registries are comprehensive in high-income countries and sparse in many low- and middle-income ones, so the latter figures are best-effort extrapolations. The top cancers by incidence were lung, breast, colorectal, prostate, and stomach; lung was the leading killer (about 1.8 million deaths). The U.S. picture, from the American Cancer Society, runs around 2 million new cases and roughly 600,000 deaths annually (ACS, 2026).

Risk rises sharply with age: the probability that any single cell accumulates enough mutations to transform in one year is tiny, but over seventy years the chance that *some* cell does so is substantial. This is also why a "war on cancer" framing oversimplifies — you can shift the curve, but as long as people live long enough, some cells will accumulate the wrong mutations.

### Risk is causal probability, not blame

A **risk factor** is anything that shifts the probability of disease — an exposure, an inherited variant, an infection, a structural condition. The chapter insists on separating biological causation from moral blame, because the slide into "lifestyle blame" is easy and analytically wrong. People do not get cancer because they are bad; cells accumulate mutations, and the accumulation rate depends on exposures — some voluntary, many not. Tobacco is a high-confidence voluntary exposure; occupational asbestos is a structurally mediated one. Both are causes; only one is a choice in any meaningful sense.

How do we decide an association is *causal* and not coincidental? The **Bradford Hill criteria** (Hill, 1965) are the working rules: strength of association, consistency across studies, specificity, correct temporality (cause precedes effect), a biological gradient (dose–response), plausibility, coherence with known biology, experimental evidence, and analogy. Smoking and lung cancer satisfy all of them — a roughly 20-fold relative risk in heavy smokers, replicated across dozens of independent cohorts, with a clean dose–response and a known mechanism (carcinogens binding DNA). That is not an association. It is a cause.

### Genes and environment interact

The dichotomy "genes versus environment" is the cleanest place in epidemiology to find a misleading question. The honest answer is *both, interacting*. Roughly 5–10% of cancers are driven primarily by inherited **high-penetrance** mutations — variants that, if you carry one, raise lifetime risk dramatically (NCI, *Risk Factors / Genetics*). *BRCA1* and *BRCA2* are the famous examples: a pathogenic *BRCA1* variant carries a lifetime breast-cancer risk on the order of 65–80% and ovarian risk of about 40–60%, varying by mutation and other factors. *TP53* (Li-Fraumeni), *APC* (familial adenomatous polyposis), the Lynch-syndrome mismatch-repair genes, *RB1*, *VHL*, and *PTEN* are other high-penetrance genes. Below them are **moderate-penetrance** variants (*CHEK2*, *PALB2*, *ATM*) that meaningfully but less dramatically raise risk, and **low-penetrance** common variants identified by genome-wide association studies, each contributing a small effect that aggregates into a **polygenic risk score**.

The other 90–95% of cancers are driven by **somatic** mutations — acquired over a lifetime, usually from environmental exposure. The key insight: environment acts *through* the genome. A carcinogen leaves a **mutational signature** — a recognizable pattern of base changes — that modern genomics can read out of a tumor to reconstruct what the cell was exposed to. The germline mutation sets the stage; the environment fires the gun. A *BRCA1* carrier who drinks heavily and uses estrogen replacement has a different trajectory from one who does not. The opening case's patient layers both: whatever his inherited baseline, tobacco and asbestos supplied decades of DNA-damaging exposure.

### The major modifiable exposures

**Tobacco** is the largest preventable cause of cancer death in history — roughly 22% of cancer deaths worldwide, about 30% in the U.S. (IARC, *European Code Against Cancer: Tobacco*). Smoke contains over 70 known human carcinogens (benzo[a]pyrene, N-nitrosamines, others) that bind DNA, form adducts, and cause replication errors that, over decades, converge on genes like *TP53*, *KRAS*, and *EGFR* in lung cells. The dose–response is steep: heavy smokers carry roughly 20-fold lung-cancer risk, and even secondhand smoke raises risk by about 25%. Quitting before 40 returns risk to nearly never-smoker levels. Vaping's long-term cancer risk is not yet characterized by 30 years of cohort data; the honest summary is "less carcinogenic than smoking, not as safe as breathing air."

**Alcohol** causes about 4% of cancers (mouth, throat, esophagus, liver, breast, colon). Ethanol is metabolized to acetaldehyde, a DNA-binding carcinogen. Even moderate drinking raises breast-cancer risk — roughly 7–10% per daily drink in meta-analysis — which the old "one drink a day for your heart" message badly underweighted.

**Obesity** is causally linked to at least 13 cancers and is now the second-largest modifiable risk factor in high-income countries after tobacco. Adipose tissue is an endocrine organ: excess fat raises circulating estrogen, elevates insulin and IGF-1 (which signal through proliferation-promoting pathways — the PI3K/AKT axis of Chapter 1), and sustains chronic low-grade inflammation. Crucially, obesity is downstream of food access, food economics, and city design, not merely "lifestyle choice."

**Infections** cause about 13% of cancers worldwide and are among the cleanest prevention targets (NCI, *Infectious Agents*). High-risk **HPV** (types 16 and 18) causes essentially all cervical cancer and many oropharyngeal and anal cancers; the HPV vaccine prevents the initiating infection, and Australia is on track to effectively eliminate cervical cancer (NCI, *HPV and Cancer*). **Hepatitis B and C** cause liver cancer (HBV preventable by vaccine, HCV now curable with antivirals). ***Helicobacter pylori*** causes most stomach cancers and gastric MALT lymphoma through chronic inflammation, and is curable with a short antibiotic course (NCI, *H. pylori*). **Epstein-Barr virus** is implicated in Burkitt and Hodgkin lymphoma and nasopharyngeal carcinoma. **HIV** enables cancers indirectly by suppressing immune surveillance.

**Radiation** damages DNA directly: ionizing radiation (X-rays, gamma, particle radiation) breaks strands, with risk rising roughly linearly with dose (the atomic-bomb survivor Life Span Study is the classic source). Radon is the second leading cause of lung cancer after smoking. Non-ionizing **UV** causes pyrimidine dimers (the lesion of Chapter 1) and most skin cancers; tanning beds are IARC Group 1 carcinogens.

**Occupational and environmental exposures** were largely identified through occupational epidemiology — workers in specific industries developing specific cancers at elevated rates. Asbestos and mesothelioma is the canonical case, with a 30–40 year latency; benzene and acute myeloid leukemia is another; fine particulate air pollution (PM2.5) is now an IARC Group 1 carcinogen. **Aflatoxins** — mycotoxins contaminating stored grains — are Group 1 carcinogens compounding liver-cancer risk in parts of Africa and East Asia (IARC, *Mycotoxins*).

### Disparities

Cancer outcomes are unequal within and between countries, and most of the gap is structural, not biological. In the U.S., Black Americans have higher cancer mortality than white Americans for most cancer types — driven largely by access: less screening, later-stage diagnosis, less guideline-concordant treatment, less specialty referral. Some biological differences are real (more aggressive triple-negative breast cancer and lethal prostate cancer in people of African ancestry), but the dominant signal is the healthcare system delivering different care to different people. Globally the gap is starker: low- and middle-income countries account for about 70% of cancer deaths but a fraction of research funding; childhood cancer survival is around 20% there versus over 80% in high-income countries — identical biology, unequal access.

## Worked Example

**Situation.** Two newspaper claims cross your desk on the same day: (a) "Processed meat causes cancer — IARC Group 1, same category as tobacco." (b) "Coffee causes cancer." You have to advise a public-health committee which to act on.

**Analytical process.** The tempting wrong move is to rank by category label: both processed meat and (historically) coffee have appeared on IARC lists, so treat them as equivalent threats. This conflates *strength of evidence for causation* with *magnitude of risk* — two different things the Group 1/2A/2B system does not separate. IARC categories rate how *confident* we are that something can cause cancer, not how *much* it raises your risk.

Apply Bradford Hill. Processed meat (Group 1, colorectal cancer): the relative-risk increase is modest — about 17% per 50 g/day — but the evidence is consistent across many studies, has a plausible mechanism (N-nitroso compounds, heterocyclic amines, heme iron), shows a dose gradient, and has the right temporality. Strong causal confidence, small per-person effect. Coffee: earlier observational associations were confounded (coffee drinkers smoked more), and once smoking was controlled, the association largely dissolved; IARC ultimately moved coffee off the "possibly carcinogenic" list and even noted a possible protective association for some cancers. The association failed consistency and, on closer look, temporality and specificity.

A second dead end worth naming: the beta-carotene story. Observational data in the 1980s suggested it was protective against lung cancer. But randomized trials (ATBC, CARET) found supplementation *increased* lung-cancer risk in smokers — the observational signal had reversed under experiment. The Bradford Hill "experiment" criterion exists precisely to catch this.

**Resolution.** Act on processed meat as a genuine but modest contributor (population-level messaging, not panic); do not treat coffee as a carcinogen. The Group 1 label means "we are confident it can cause cancer," not "it is as dangerous as tobacco."

**The lesson.** Causal confidence and effect size are independent axes; sound risk advice requires both, and the Bradford Hill criteria — especially the experiment criterion — separate real causes from confounded associations.

**The limit.** Bradford Hill is a guide, not an algorithm. For exposures where randomized trials are impossible (you cannot assign people to smoke), causal inference rests on observational evidence weighted across all criteria, and reasonable experts can disagree at the margins.

## Common Misconceptions

**"More cancer cases means higher individual risk."** Rising case *counts* can come entirely from a growing, aging population while age-standardized *rates* hold steady or fall. The opening case's patient is high-risk because of his exposures and age, not because national case counts are up. Always check whether a "cancer is rising" claim cites counts or rates.

**"Cancer risk is mostly genetic" / "mostly bad luck."** Both overgeneralize. Only 5–10% of cancers are driven primarily by inherited high-penetrance mutations; most are somatic mutations shaped by age and exposure. And "bad luck" (random replication error) is real but is not a substitute for the large, modifiable contributions of tobacco, obesity, infection, and radiation [contested — see pantry flag on the bad-luck debate].

**"Genetic and environmental causes are mutually exclusive."** They interact through the same molecular substrate. Environment acts by causing somatic mutations; an inherited DNA-repair defect amplifies the damage from any given exposure. A *BRCA* carrier plus a DNA-damaging exposure is layered risk, not an either/or — exactly the layering in the opening case.

**"A risk factor means the patient is at fault."** Risk is causal probability, not blame. Many of the largest exposures — asbestos, air pollution, food environments — are structurally imposed. Reading the opening case as "he did this to himself" both misattributes the asbestos exposure and obscures where prevention policy should act.

## Exercises

1. **(Understand.)** Define incidence, mortality, prevalence, and age-standardized rate. Then explain in two sentences why a country's cancer counts can rise while its age-standardized rate falls.

2. **(Apply.)** A claim states: "Drinking sugary soda causes pancreatic cancer." Evaluate it against at least five Bradford Hill criteria. For each, state what evidence you would need and whether the claim is likely to meet it. Conclude with a calibrated verdict.

3. **(Analyze/Produce.)** Draw a mechanism-to-prevention map for one infection-driven cancer (HPV-cervical, HBV-liver, or *H. pylori*-gastric): exposure → molecular damage / chronic inflammation → cell-level consequence → the specific intervention (vaccine, antiviral, antibiotic, screening) that interrupts the chain. Label what stage each intervention acts at.

4. **(Evaluate.)** Take the disparity finding that Black Americans have higher cancer mortality than white Americans for most cancers. Separate the plausible biological contributors from the structural ones, and propose the single intervention you think would close the largest share of the gap. Defend the choice.

## What Would Change My Mind

The chapter's central claim is that most cancer is not "bad luck" but reflects exposures acting through the genome, with a large modifiable fraction. The strongest finding that would force revision: rigorous evidence that the modifiable fraction is much smaller than current estimates — that, after fully accounting for age and stem-cell division number, the great majority of cancer variation is irreducible stochastic replication error not meaningfully alterable by prevention. Tomasetti and Vogelstein's stem-cell-division argument pushes in that direction and is genuinely contested [contested — see pantry flag]; a convincing demonstration that interventions on tobacco, obesity, and infection fail to move incidence at the population level — contradicting the natural experiments of declining smoking and HPV vaccination — would undercut the prevention-centered frame this chapter is built on.

## Still Puzzling

- How large *is* the irreducible "bad luck" fraction of cancer? The stem-cell-division debate remains open and consequential for how much we invest in prevention versus early detection.
- Why do some carcinogens have apparent thresholds while others (ionizing radiation, on the standard model) act linearly from zero dose? The shape of low-dose risk curves is hard to measure and still argued.
- How much of racial and geographic disparity is biological versus structural, and can the two even be cleanly separated when chronic stress and environment themselves alter tumor biology?

## References

- IARC. *Global cancer burden in 2022.* https://www.iarc.who.int/news-events/new-report-on-global-cancer-burden-in-2022-by-world-region-and-human-development-level/
- American Cancer Society. *Cancer Facts & Figures 2026.* https://www.cancer.org/research/cancer-facts-statistics/all-cancer-facts-figures/2026-cancer-facts-figures.html
- NCI. *Risk Factors for Cancer.* https://www.cancer.gov/about-cancer/causes-prevention/risk
- NCI. *HPV and Cancer.* https://www.cancer.gov/about-cancer/causes-prevention/risk/infectious-agents/hpv-and-cancer
- NCI. *Risk Factors: Infectious Agents.* https://www.cancer.gov/about-cancer/causes-prevention/risk/infectious-agents
- NCI. *H. pylori and Cancer.* https://www.cancer.gov/about-cancer/causes-prevention/risk/infectious-agents/h-pylori-fact-sheet
- IARC. *European Code Against Cancer: Tobacco and Cancer.* https://www.iarc.who.int/reference/european-code-against-cancer-4th-edition-tobacco-and-cancer/
- IARC. *Mycotoxins as Human Carcinogens.* https://www.iarc.who.int/reference/mycotoxins-as-human-carcinogens-the-iarc-monographs-classification/
- Hill, A. B. (1965). The Environment and Disease: Association or Causation? *Proc. R. Soc. Med.* 58, 295–300. [verify — Bradford Hill criteria, cited from archive chapter; not in pantry source bank]

---

## Prompts

*No figures have been generated for this chapter yet.*
