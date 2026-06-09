# Cancer Metabolism: The Warburg Effect and Glucose

## Learning Objectives

After working through this chapter, you should be able to:

1. **Define** the Warburg effect (aerobic glycolysis) and **distinguish** the obsolete "broken mitochondria" explanation from the modern biomass-allocation explanation.
2. **Explain** why a proliferating cell would choose an energetically inefficient pathway, in terms of carbon, nitrogen, and reducing power for biosynthesis.
3. **Trace** the HIF-1α oxygen-sensing pathway and **predict** the consequences of VHL loss.
4. **Describe** the repurposed (not disabled) roles of mitochondria in cancer cells.
5. **Connect** glucose metabolism to a clinical tool (FDG-PET) and to a druggable target (the HIF system).

## Opening Case

A patient with suspected lymphoma is injected with **fluorodeoxyglucose (FDG)** — a radioactive glucose analog — and slid into a **positron emission tomography (PET)** scanner. After an hour, the images come back, and the tumors glow. They have taken up the labeled sugar at rates no normal tissue can match. The brain (always glucose-hungry) lights up, the bladder (where the tracer is excreted) lights up, and then a cluster of lymph nodes lights up that should be dark. The PET scan is, in effect, a glucose-uptake map of the body, and the brightest abnormal spots are cancer.

This is a routine, everyday clinical observation — and it should be puzzling. The tumor is consuming glucose voraciously, but here is the strange part: even with oxygen freely available, it is not burning that glucose all the way down for energy. It ferments most of it to lactate and excretes the lactate as waste, extracting only a fraction of the available ATP. No rational engineer designing for energy efficiency would do this. A cell that could get roughly 30 molecules of ATP per glucose by full oxidation is instead settling for about 2 and throwing the rest away.

Otto Warburg saw this in the 1920s and proposed — incorrectly, as it turned out — that cancer cells must have *broken mitochondria* forcing them to ferment. The mitochondria, we now know, are largely intact. The cell is making a choice. The chapter's question is the one the PET scan forces on us: why would a cell give up most of its energy from glucose, on purpose, when it does not have to?

## Core Concepts

### Glycolysis, briefly, and the two fates of pyruvate

Plain language: **glycolysis** is the universal pathway that splits glucose. Formal definition: glycolysis is a ten-step cytoplasmic pathway converting one glucose (six carbons) into two pyruvate molecules (three carbons each), netting two ATP and two NADH (NCBI Bookshelf, *Molecular Biology of the Cell*).

Two control points matter for cancer. **Hexokinase** phosphorylates glucose at entry, committing it to the pathway; cancer cells often overexpress the isoform **HK2**, which docks on the outer mitochondrial membrane — and, as a bonus, blocks BAX binding there, contributing to apoptosis evasion (a direct link back to Chapters 13–14). **Phosphofructokinase-1 (PFK-1)** catalyzes the irreversible commitment step and is allosterically tuned by the cell's energy state.

What happens to pyruvate depends on conditions. In a normal cell with oxygen, pyruvate enters the mitochondria, is converted by pyruvate dehydrogenase to acetyl-CoA, feeds the **citric acid cycle**, and the resulting electrons drive **oxidative phosphorylation (OXPHOS)** — yielding roughly 30–32 ATP per glucose. In a cell *without* oxygen, the electron transport chain stalls (no oxygen to accept electrons), so pyruvate is instead reduced to **lactate** by lactate dehydrogenase, regenerating the NAD⁺ that glycolysis needs to keep running — at a yield of only 2 ATP per glucose.

The defining oddity of cancer is that it performs lactate fermentation *even when oxygen is available*. This is **aerobic glycolysis**, the **Warburg effect**.

<!-- → [DIAGRAM: glycolysis → pyruvate, with the OXPHOS branch (oxygen present, ~30 ATP) vs the lactate branch (Warburg, ~2 ATP) shown side by side] -->

### The Warburg effect explained — biomass, not ATP

Plain language: the cancer cell is not trying to maximize energy. It is trying to build a second cell.

Here is the misconception to kill first: students hear "the cell chose an inefficient pathway" and assume the cell is bad at energetics, or that its mitochondria are broken. Neither is right. The cell is optimizing for a *different* quantity — **biomass**, the carbon skeletons, nitrogen, and reducing power needed to construct a daughter cell (Nature Reviews Cancer, 2011).

Consider what dividing requires. New **DNA** needs nucleotides, built from ribose-5-phosphate (off glycolysis, via the pentose phosphate pathway), nitrogen, and carbon. New **membranes** need lipids, built from acetyl-CoA and glycerol-3-phosphate. New **protein** needs amino acids, many synthesized from glycolytic and cycle intermediates (serine from 3-phosphoglycerate, alanine from pyruvate, aspartate from oxaloacetate). And all of this biosynthesis needs **NADPH**, a reducing cofactor.

If the cell oxidized glucose completely to CO₂, it would get maximum ATP — but every carbon would leave as exhaled CO₂, and the cell would have no carbon skeletons to build with. For a quiescent cell, that is fine; it only needs maintenance ATP. For a proliferating cell, complete oxidation is *wasteful of carbon*. By stopping glycolysis at pyruvate (or branching off earlier for the pentose phosphate or serine pathways), the cell preserves carbon for biosynthesis. Excreting lactate dumps the excess reduced carbon and protons without consuming the cycle intermediates the cell needs for building.

So aerobic glycolysis is better understood as **biosynthetic glycolysis**: glucose treated as a carbon source, not an energy source. The high uptake supplies the flux; the lactate is the waste of a carbon-allocation strategy. This reframing — crystallized by Vander Heiden, Cantley, and Thompson in 2009 — replaced Warburg's "broken mitochondria" story and is the current understanding [verify — Vander Heiden, Cantley & Thompson, *Science* 2009].

And ATP? Proliferating cells need *more* ATP, not less. They get it two ways: enough glycolytic flux that even a low per-glucose yield adds up, and mitochondrial oxidation of *other* fuels — glutamine and fatty acids — for the rest. The mitochondria are running; they are just not running primarily on glucose.

<!-- → [FIGURE: glucose carbon fanning out into ribose, serine/glycine, lipid precursors, and lactate — biomass allocation rather than complete oxidation] -->

### Mitochondria in cancer: repurposed, not broken

The "broken mitochondria" idea is the central misconception of this whole topic, so name it plainly: **cancer mitochondria are not universally defective.** In tumor cells they are typically functional and *repurposed* (Cell Death & Differentiation, 2022):

- **Anabolic precursor generation.** The citric acid cycle exports intermediates for biosynthesis — citrate to the cytoplasm for fatty-acid synthesis, α-ketoglutarate and oxaloacetate for amino acids. To replace exported carbon the cycle runs **anaplerotic**, pulling in glutamine (next chapter).
- **Oxidation of alternative substrates.** Glutamine and fatty acids are oxidized in mitochondria for ATP even as glucose is diverted to lactate.
- **ROS signaling.** Mitochondria produce reactive oxygen species that, at controlled levels, support proliferative signaling — balanced against antioxidant defenses.
- **Apoptosis gatekeeping.** Mitochondria remain the hub of intrinsic apoptosis (Chapter 13); the cancer cell needs them functional for energy and biosynthesis but suppressed in their death capacity.

This repurposing is why some mitochondrial-targeted drugs work: complex I inhibitors selectively stress cells with high OXPHOS dependence, and **metformin** (a mild complex I inhibitor used for diabetes) has been associated with reduced cancer incidence in epidemiology — though the data are mixed and suggestive rather than conclusive [contested — see pantry flag; metformin clinical evidence is not settled].

### HIF-1α: the oxygen-sensing switch

Plain language: tumors outgrow their blood supply and develop low-oxygen regions, and the cell has a built-in sensor that reprograms metabolism in response. That sensor is **hypoxia-inducible factor 1α (HIF-1α)**.

A subtle misconception to correct: hypoxia is not merely "the absence of oxygen." It is a *signaling state* — the cell actively detects low oxygen and launches a coordinated transcriptional program. The detection works through oxygen-requiring enzymes called **prolyl hydroxylases (PHDs)**. In normal oxygen, PHDs hydroxylate HIF-1α, marking it for recognition by the **von Hippel–Lindau (VHL)** protein, which targets it for destruction — giving HIF-1α a half-life of about five minutes. When oxygen drops, PHDs stall, HIF-1α escapes hydroxylation and destruction, accumulates, partners with HIF-1β, and activates transcription of an extensive target set: glycolytic enzymes, glucose transporters (GLUT1), the lactate exporter MCT4, the angiogenic factor VEGF, and PDK1 (which inhibits pyruvate's entry to the cycle, reinforcing the lactate route).

This is examined in detail in the Worked Example.

## Worked Example

**Situation.** A clear cell renal cell carcinoma (kidney cancer) behaves as if it is permanently hypoxic — high glycolysis, high VEGF, cytoplasm so lipid-laden it looks "clear" under the microscope — even in well-oxygenated regions of the tumor. We want to explain this, and we will hit a dead end first.

**Process (with a dead end).** The obvious first hypothesis: the tumor is hypoxic, so HIF-1α is stabilized in the usual way. We measure oxygen and find that much of the tumor is *adequately oxygenated*. Under the normal model, well-oxygenated cells should have active PHDs, hydroxylated HIF-1α, VHL-mediated degradation, and therefore *low* HIF activity. That predicts the cells should *not* show the hypoxic program. They do. The hypoxia explanation fails — the oxygen is there but the cells act starved of it. This is the dead end.

**Resolution.** The resolution is to look downstream of oxygen, at VHL itself. Clear cell renal cell carcinoma characteristically *loses VHL function* — it is the gene mutated in von Hippel–Lindau syndrome and is deleted or inactivated in most sporadic clear cell RCC. Without functional VHL, HIF-α is *not degraded even when it is properly hydroxylated*, because the recognition step that VHL performs is missing. HIF accumulates constitutively, regardless of oxygen. The cell runs the full hypoxic program — glycolytic enzymes, VEGF, lipid accumulation — in a state of **pseudohypoxia**: behaving as if oxygen-starved while oxygen is plentiful (Hanahan, 2022, on metabolic reprogramming as a hallmark).

The clinical payoff is direct. In clear cell RCC the dominant driver is often the HIF paralog **HIF-2α**, and **belzutifan**, a HIF-2α inhibitor, was approved by the FDA in 2021 for VHL-disease-associated cancers and advanced clear cell RCC — the first drug to target the HIF system clinically [verify — belzutifan 2021 approval].

**The lesson.** A constitutive metabolic phenotype need not come from the upstream stimulus (hypoxia) at all; it can come from breaking the *off-switch* downstream (VHL). Trace the pathway, not just the input.

**The limit.** VHL loss explains clear cell RCC specifically. Most tumors stabilize HIF through genuine regional hypoxia, oncogenic signaling, or oncometabolites — not VHL deletion. Do not generalize "constitutive HIF" to a single mechanism across all cancers; the route differs by tumor type.

## Common Misconceptions

**"Cancer cells have broken mitochondria — that's why they ferment."** This was Warburg's hypothesis and it is wrong. Tumor mitochondria are usually functional and are repurposed for anabolic precursor generation, alternative-substrate oxidation, and apoptosis gatekeeping. The cell ferments by *choice*, to preserve carbon for biomass — which is why FDG-PET shows high glucose uptake without implying any mitochondrial defect.

**"A cell that picks an inefficient pathway is just bad at energetics — and 'inefficient' must mean it needs less ATP."** Proliferating cancer cells need *more* ATP, not less. Aerobic glycolysis is inefficient *per glucose* but the cell compensates with high uptake and with mitochondrial oxidation of glutamine and fat. The metric the cell optimizes is biomass (carbon, nitrogen, NADPH), not ATP per glucose. Reframing "inefficient" as "carbon-conserving" resolves the apparent paradox of the PET scan.

**"Hypoxia just means low oxygen."** Hypoxia in a tumor is a *signaling state* enacted through HIF, not merely a shortage. And HIF can be constitutively active with *no* low-oxygen at all — as in VHL-deficient kidney cancer, where the off-switch is broken downstream of oxygen sensing. Treating hypoxia as only "lack of O₂" misses both the transcriptional program and the pseudohypoxic cancers.

## Exercises

1. **(Understand.)** State, in one sentence, the modern explanation for why a cancer cell ferments glucose to lactate despite available oxygen, and name the single quantity the cell is optimizing.

2. **(Apply.)** A tumor biopsy shows high HIF-1α target-gene expression in a region you measure to be normoxic. List two distinct mechanisms (other than low oxygen) that could produce constitutive HIF activity, and state which one you would test first if the tumor were a clear cell renal carcinoma.

3. **(Apply/Analyze — produce something.)** Trace one glucose molecule's carbon into four destinations a dividing cell needs: ribose-5-phosphate, serine, a lipid precursor, and lactate. Draw the branch points (name the intermediate at each fork) and label which destination supplies nucleotides, which supplies membrane, and which is waste. End with one sentence explaining why complete oxidation would defeat the purpose.

4. **(Analyze.)** FDG-PET lights up many cancers but not all. Classify each statement as a *definition*, a *mechanism*, or a *clinical implication*: (a) "FDG is a glucose analog trapped after phosphorylation by hexokinase." (b) "Tumors with high glycolytic flux accumulate more FDG." (c) "A tumor with low FDG avidity may be a slowly proliferating or non-glycolytic subtype." Justify each label briefly.

## What Would Change My Mind

The central claim is that aerobic glycolysis reflects a carbon-allocation strategy for biomass, not a defect in mitochondrial respiration. The finding that would most force a revision: rigorous, isotope-tracing evidence across many tumor types showing that cancer cells route the great majority of their glucose carbon to complete CO₂ oxidation while diverting only a trivial fraction to biosynthetic intermediates — i.e., that lactate excretion is *not* accompanied by meaningful preservation of carbon for building blocks. That would reopen the door to an energetics-or-dysfunction explanation. The accumulating ¹³C-flux data showing glucose carbon entering ribose, serine, and lipid pools currently support the biomass model, but a broad negative tracing result would be the disconfirming test.

## Still Puzzling

- **Why lactate excretion specifically?** Even granting biomass optimization, why cells so consistently dump lactate (rather than fully recycling reduced carbon) and what regulates the precise glycolysis-to-OXPHOS ratio across tumor regions is not fully settled.
- **Does metformin actually prevent cancer?** The epidemiological signal is real but confounded, and randomized trial results are mixed. Whether mild complex I inhibition is a genuine, usable prevention strategy remains open [contested — see pantry flag].
- **How metabolically heterogeneous is a single tumor?** Different regions — hypoxic core versus oxygenated rim — likely run different metabolic programs, and how that heterogeneity shapes treatment response seeds the next chapter on the tumor microenvironment.

## References

- Nature Reviews Cancer (2021). *Cancer metabolism: looking forward.* https://www.nature.com/articles/s41568-021-00378-6
- Nature Reviews Cancer (2011). *Regulation of cancer cell metabolism.* https://www.nature.com/articles/nrc2981
- Cell Death & Differentiation (2022). *Targeting mitochondrial metabolism for precision medicine in cancer.* https://www.nature.com/articles/s41418-022-01022-y
- Frontiers in Oncology (2022). *Differential glutamine metabolism in the tumor microenvironment.* https://www.frontiersin.org/articles/10.3389/fonc.2022.1011191/full
- NCI. *What Is Cancer?* https://www.cancer.gov/about-cancer/understanding/what-is-cancer
- Hanahan, D. (2022). *Hallmarks of Cancer: New Dimensions.* Cancer Discovery, 12(1), 31–46. https://aacrjournals.org/cancerdiscovery/article/12/1/31/675608/Hallmarks-of-Cancer-New-Dimensions
- NCBI Bookshelf. *Molecular Biology of the Cell.* https://www.ncbi.nlm.nih.gov/sites/books/n/mboc4/

## Prompts

*No figures have been generated for this chapter yet.*
