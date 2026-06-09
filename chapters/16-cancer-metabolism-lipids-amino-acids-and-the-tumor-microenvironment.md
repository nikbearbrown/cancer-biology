# Cancer Metabolism: Lipids, Amino Acids, and the Tumor Microenvironment

## Learning Objectives

After working through this chapter, you should be able to:

1. **Explain** why proliferating cancer cells reactivate de novo fatty-acid synthesis and **identify** the targetable enzymes in the pathway.
2. **Describe** glutamine addiction and **analyze** how glutamine serves as carbon, nitrogen, and redox support simultaneously.
3. **Construct** the synthetic-lethality logic linking MTAP deletion to PRMT5 inhibition.
4. **Characterize** the tumor microenvironment as a metabolic ecosystem and **explain** how its features suppress anti-tumor immunity.
5. **Evaluate** the major categories of metabolic cancer therapy and their boundary conditions.

## Opening Case

A child with acute lymphoblastic leukemia (ALL) is treated with a drug that is not a poison aimed at her cancer cells and not a molecule designed to fit any receptor on them. It is a bacterial enzyme, **asparaginase**, and all it does is circulate in her bloodstream chewing up the amino acid **asparagine**. Normal cells shrug — they can synthesize their own asparagine when the supply runs low. Her leukemic cells cannot. They have lost the capacity to make asparagine and depend entirely on what they scavenge from the blood. Starve the blood of asparagine and the leukemic cells, unable to build protein, die. This single metabolic dependency, exploited since the 1960s, helped push pediatric ALL cure rates toward 90 percent [verify — pediatric ALL cure rate].

Hold the case as a template. The previous chapter showed that glucose is reprogrammed in cancer. But glucose is only one input to the factory. A dividing cancer cell also needs **lipids** for membranes, **amino acids** for protein and carbon, and **nucleotide precursors** for DNA — and it rewires all of these. Crucially, each rewiring creates a *dependency*, and a dependency is a target. Asparaginase is the oldest proof: find a metabolic need the cancer cannot meet for itself, then cut off the supply. This chapter surveys the broader metabolic landscape — lipids, glutamine and other amino acids, the elegant MTAP–PRMT5 trick, and the metabolic ecosystem of the tumor — and shows how each becomes a therapeutic opening.

## Core Concepts

### Lipid metabolism: building membranes from scratch

Plain language: a cell about to divide must double its membranes, and many cancer cells, unlike most adult tissue, build their own fatty acids rather than importing them.

A misconception to retire immediately: fat is *not* only an energy store. In cancer biology, lipids are structural (membrane phospholipids and cholesterol), signaling (phosphatidylinositols, ceramide, prostaglandins), and regulatory (lipid modifications that anchor proteins like Ras to membranes). Treating fat metabolism as merely "energy storage" misses most of what it does for a tumor.

Most differentiated cells take up fatty acids from the blood. Cancer cells frequently **reactivate de novo fatty-acid synthesis** (Nature Reviews Cancer, 2011), running this pathway:

1. **Citrate** is exported from mitochondria to the cytoplasm.
2. **ATP-citrate lyase (ACLY)** cleaves it to acetyl-CoA.
3. **Acetyl-CoA carboxylase (ACC)** converts acetyl-CoA to malonyl-CoA.
4. **Fatty acid synthase (FASN)** condenses these into palmitate (a 16-carbon fatty acid).
5. **Elongases and desaturases** (notably **SCD1**) tailor palmitate into the full set of fatty acids the cell needs.

FASN is highly expressed in many cancers (breast, prostate, lung, colon, pancreatic), often essential, and correlates with prognosis; FASN, ACLY, ACC, and SCD1 inhibitors are all in development (Cell Death & Differentiation, 2022). Cholesterol synthesis via the **mevalonate pathway** is likewise upregulated — and because that pathway also makes the isoprenoids that prenylate Ras, **statins** (mevalonate-pathway inhibitors taken by millions for cardiovascular prevention) plausibly affect cancer biology. The epidemiology suggests modestly reduced incidence in statin users, but trial evidence is mixed [contested — see pantry flag; statin anticancer effect not established].

<!-- → [DIAGRAM: de novo fatty-acid synthesis — citrate → ACLY → ACC → FASN → palmitate → SCD1, with targetable enzymes marked] -->

Lipid composition itself matters: cancer cells often shift toward more saturated, rigid membranes, which may resist both MOMP (Chapter 13) and **ferroptosis** (which requires peroxidizable polyunsaturated fatty acids) — a direct metabolic link to the death programs.

### Glutamine addiction

Plain language: many cancers cannot live without a steady supply of glutamine — the most abundant amino acid in blood — even when glucose is plentiful.

A misconception to correct: glucose is not the only metabolic dependency. **Glutamine** is often equally vital, and it does several jobs at once (Frontiers in Oncology, 2022). After import (via transporters such as ASCT2/SLC1A5), **glutaminase** converts glutamine to glutamate, which becomes **α-ketoglutarate** feeding the citric acid cycle. From there glutamine supplies:

- **Carbon for the cycle** — replacing (anaplerotically) the intermediates exported for biosynthesis, the gap created by the Warburg strategy of the last chapter.
- **Nitrogen** for amino-acid and nucleotide synthesis.
- **Glutamate for glutathione**, the major intracellular antioxidant.
- **Reducing power** (NADPH) via malic-enzyme reactions.

Dependence is strongest in **MYC-driven** cancers — MYC raises glutamine transporters and glutaminase — and in some KRAS-mutant cancers. The therapeutic openings: the **glutaminase inhibitor CB-839 (telaglenastat)** (modest clinical activity, often in combination), and the old workhorse **asparaginase** from the Opening Case, which also depletes glutamine. The boundary condition is real: glutamine dependence varies widely across cancers, normal proliferating cells also use glutamine, and the body can partially compensate — so glutamine-targeting is not a universal solution.

<!-- → [FIGURE: glutamine entering the cell → glutaminase → glutamate → α-ketoglutarate feeding the TCA cycle, with branches to glutathione, nucleotides, and NADPH] -->

### Other amino-acid dependencies, and MTAP–PRMT5 synthetic lethality

The asparagine story generalizes. Some cancers depend on **arginine** (hepatocellular carcinoma, some melanomas — targeted by arginine deiminase), some on **methionine**, and many on **cysteine** import (via the xCT antiporter SLC7A11) to sustain glutathione — a dependency whose disruption can trigger ferroptosis. **Tryptophan** degradation by IDO depletes the local environment and suppresses T cells (a theme that returns below).

The most elegant case is **MTAP–PRMT5 synthetic lethality**. Plain language: a gene deletion that is itself harmless creates a hidden weakness a drug can exploit.

Here is the mechanism. **MTAP** (methylthioadenosine phosphorylase) sits on chromosome 9p21, right beside the tumor-suppressor *CDKN2A*. *CDKN2A* is deleted in roughly 30 percent of cancers, and MTAP is often co-deleted as an innocent bystander — making about 15 percent of all human cancers **MTAP-deleted**. MTAP normally clears the metabolite **MTA** (methylthioadenosine). In MTAP-deleted cells, MTA accumulates. Because MTA resembles the methyl donor SAM, it partially inhibits **PRMT5**, an arginine methyltransferase. The deleted cells therefore run with PRMT5 already half-throttled. Add a **PRMT5 inhibitor**, and you push them over the edge — while normal cells, with full PRMT5 activity, tolerate the same dose.

This is **synthetic lethality**: MTAP loss alone is survivable, PRMT5 inhibition alone is survivable, but together they are lethal. PRMT5 inhibitors (MRTX1719, AMG-193, others) are in trials specifically for MTAP-deleted cancers — one of the cleaner examples of metabolism-informed precision oncology.

<!-- → [DIAGRAM: MTAP deletion → MTA accumulation → partial PRMT5 inhibition → added PRMT5 inhibitor tips MTAP-deleted (but not normal) cells into death] -->

### The tumor microenvironment as a metabolic ecosystem

Plain language: a tumor is not a uniform lump of identical cells but an ecosystem — cancer cells, fibroblasts, immune cells, blood vessels, and matrix, all competing for and trading metabolites.

A misconception to retire: the cells in a tumor are *not* metabolically identical. The **tumor microenvironment (TME)** is regionally heterogeneous and metabolically hostile (Hanahan, 2022; Signal Transduction and Targeted Therapy, 2023):

- **Hypoxia and acidosis.** Tumors outgrow their blood supply; interior pH often falls to 6.5–6.8 versus 7.4 normally. Hypoxic regions are also more radioresistant, because radiation damage needs oxygen.
- **Nutrient depletion.** Voracious cancer cells lower local glucose, glutamine, and arginine — interstitial glucose can be several-fold below serum.
- **Lactate accumulation and immunosuppression.** Exported Warburg lactate not only acidifies the TME but directly impairs T-cell and NK-cell function, polarizes macrophages toward a tumor-promoting state, and supports regulatory T cells.
- **Immunometabolic competition.** Activated T cells, like cancer cells, need glucose and glutamine to function. Cancer cells outcompete them, contributing to T-cell exhaustion and immune escape — a mechanism of immune evasion grounded in metabolism.

Stromal partners participate too: some **cancer-associated fibroblasts** secrete lactate that cancer cells reuptake (a "reverse Warburg" exchange), and **adipocytes** in breast and ovarian tumors hand off fatty acids — part of why obesity associates with several cancers.

## Worked Example

**Situation.** A patient's tumor is genotyped and found to carry a homozygous deletion at chromosome 9p21. The oncologist's first instinct is that the important loss is the neighboring tumor suppressor. We want to find a drug, and we will take a wrong turn first.

**Process (with a dead end).** The 9p21 deletion removes *CDKN2A* (p16), a cell-cycle brake. The intuitive move is to target the *consequence* of losing p16 — for example, the now-unrestrained CDK4/6 — with a CDK4/6 inhibitor. But this targets a pathway that is deregulated in a huge range of cancers and offers no special selectivity for *this* patient's tumor over countless others; it does not exploit anything unique to the deletion. Worse, it ignores the **passenger** gene that came out with *CDKN2A*. The p16-focused approach is a reasonable dead end: it treats the famous gene and misses the exploitable one.

**Resolution.** Notice that **MTAP** was co-deleted. That changes everything, because MTAP loss is not just an incidental scar — it rewires metabolism. MTA accumulates and partially inhibits PRMT5, leaving the tumor cells running on a half-disabled methyltransferase. That is a *vulnerability normal cells do not share*. A **PRMT5 inhibitor** (or a MAT2A inhibitor, which lowers SAM and deepens the MTA effect) selectively kills the MTAP-deleted cells by synthetic lethality. The deletion that looked like collateral damage is the therapeutic opening.

**The lesson.** The "passenger" of a deletion can be more druggable than the "driver." A metabolic dependency created incidentally by a deletion (MTAP) yields a selective therapy that targeting the famous driver (CDKN2A) never could — because synthetic lethality, not pathway inhibition, supplies the selectivity.

**The limit.** This works only where MTAP is genuinely co-deleted and PRMT5 is the partner; it is not a general tactic for every 9p21 deletion (some retain MTAP), and resistance and on-target toxicity in normal proliferating tissue remain to be fully characterized in the clinic.

## Common Misconceptions

**"Fat metabolism in cancer is just about energy storage."** Lipids in proliferating cancer cells are mainly structural and signaling molecules — membrane phospholipids, cholesterol, and lipid anchors for oncoproteins like Ras. The reactivation of de novo synthesis (ACLY → ACC → FASN → SCD1) exists to *build membranes for the next cell*, which is why FASN inhibition can be lethal to tumors that depend on it. Energy storage is a minor part of the story.

**"Glucose is the only metabolic dependency that matters."** Many cancers are equally or more dependent on glutamine (carbon, nitrogen, redox), and others on asparagine, arginine, methionine, or cysteine. The Opening Case is the proof: depleting asparagine alone can be curative in ALL because the cancer cannot make it. A glucose-only picture of cancer metabolism would have missed the oldest successful metabolic therapy in oncology.

**"All the cells in a tumor are metabolically the same."** The tumor microenvironment is regionally heterogeneous — hypoxic acidic cores beside oxygenated rims, lactate-rich zones that suppress nearby T cells, fibroblasts and adipocytes feeding cancer cells. This heterogeneity is why metabolic immune suppression occurs and why combination strategies (metabolic drug plus checkpoint inhibitor) are being tested. Picturing a uniform lump obscures the competition that lets tumors evade immunity.

## Exercises

1. **(Understand.)** List the four distinct jobs glutamine performs for a proliferating cancer cell, and name the enzyme that begins its catabolism.

2. **(Apply.)** A solid tumor is found to be MTAP-deleted. Explain, in mechanistic steps, why a PRMT5 inhibitor should be selectively toxic to this tumor but relatively spare the patient's normal cells. Then state one reason the strategy might still fail in practice.

3. **(Apply/Analyze — produce something.)** Draw a metabolic map of a single lactate-rich, hypoxic region of a tumor showing at least three cell types (cancer cell, T cell, cancer-associated fibroblast). Label the nutrients each consumes or secretes, mark where lactate suppresses immune function, and add one arrow showing where a checkpoint inhibitor plus a metabolic drug would intervene. Annotate every arrow with the molecule responsible.

4. **(Analyze.)** Classify each claim as a *definition*, a *mechanism*, an *epidemiological association*, or a *therapeutic implication*: (a) "FASN condenses acetyl-CoA and malonyl-CoA into palmitate." (b) "Statin users show modestly reduced cancer incidence." (c) "Asparaginase depletes blood asparagine, killing ALL cells that cannot synthesize it." (d) "Lactate polarizes macrophages toward a tumor-promoting phenotype." Justify each label in a phrase.

## What Would Change My Mind

The central claim is that cancer's metabolic rewiring of lipids and amino acids creates *selective* dependencies that drugs can exploit with a real therapeutic window. The finding that would most force a revision: well-controlled clinical demonstrations that the headline dependencies do not translate — for example, that MTAP-deleted tumors respond to PRMT5 inhibitors no better than MTAP-intact tumors (collapsing the synthetic-lethality rationale), or that glutaminase and FASN inhibitors show no enrichment of benefit in the biomarker-defined dependent populations across adequately powered trials. If the dependencies identified in cell culture and xenografts consistently failed to predict response in patients, the "dependency as target" framing would have to retreat to asparaginase as a near-unique exception rather than a general principle. The asparaginase precedent and early MTAP-selective PRMT5 data argue the principle is sound, but broad biomarker-negative trial results would be the disconfirming test.

## Still Puzzling

- **How much does dietary metabolic intervention actually do?** Caloric restriction, ketogenic diets, and methionine restriction have strong preclinical signals but weak, hard-to-sustain clinical effects. Whether diet can meaningfully starve tumors in patients is unresolved.
- **Can metabolic–immune combinations be made to work reliably?** The rationale for pairing metabolic drugs with checkpoint inhibitors is clear, but the disappointing IDO-inhibitor trials are a warning that removing one metabolic brake may not be enough. The conditions under which these combinations help remain open.
- **Why do repurposed metabolic drugs (metformin, statins, aspirin) show modest, confounded effects?** Each has plausible mechanism and suggestive epidemiology but inconsistent trials. Whether these are real but small effects, or artifacts of confounding, is a recurring puzzle that bridges metabolism, prevention, and the angiogenesis biology that follows [contested — see pantry flag].

## References

- Nature Reviews Cancer (2021). *Cancer metabolism: looking forward.* https://www.nature.com/articles/s41568-021-00378-6
- Nature Reviews Cancer (2011). *Regulation of cancer cell metabolism.* https://www.nature.com/articles/nrc2981
- Cell Death & Differentiation (2022). *Targeting mitochondrial metabolism for precision medicine in cancer.* https://www.nature.com/articles/s41418-022-01022-y
- Frontiers in Oncology (2022). *Differential glutamine metabolism in the tumor microenvironment.* https://www.frontiersin.org/articles/10.3389/fonc.2022.1011191/full
- Signal Transduction and Targeted Therapy (2023). *Epigenetic regulation in the tumor microenvironment.* https://www.nature.com/articles/s41392-023-01480-x
- Experimental & Molecular Medicine (2023). *Metabolic reprogramming and epigenetic modifications in cancer.* https://www.nature.com/articles/s12276-023-01020-1
- Hanahan, D. (2022). *Hallmarks of Cancer: New Dimensions.* Cancer Discovery, 12(1), 31–46.

## Prompts

*No figures have been generated for this chapter yet.*
