# The Building Blocks of Life: Normal Cell Biology

## Learning Objectives

By the end of this chapter you should be able to:

- **Describe** the architecture of a normal eukaryotic cell — organelles, cytoskeleton, plasma membrane, nucleus — and the specific job each component performs.
- **Explain** the cell cycle as a four-phase decision system gated by cyclin–CDK complexes and policed by checkpoints, naming what p53 and Rb each do.
- **Trace** information flow from DNA to RNA to protein, and connect each major signaling pathway (RAS/MAPK, PI3K/AKT, Wnt) and the apoptosis machinery to a cell behavior.
- **Analyze** how these subsystems compound to maintain tissue homeostasis, and predict, for a given molecular failure, what changes at the level of the cell and the tissue.

## Opening Case

You cut yourself. A thin slice on the edge of a finger — a line of blood, a sting that fades. The bleeding stops within a minute. By next week the skin is fresh again.

Watch what happens underneath. The instant the wound forms, platelets plug the gap and clotting factors crosslink into a scaffold. Then the cells at the wound's edge begin doing something they were not doing five minutes earlier: they divide. Keratinocytes — the cells that make your skin — crawl across the wound, dividing as they go, filling the space. Fibroblasts lay down collagen. Capillaries reroute. White blood cells clear debris.

Now watch the second thing, which is the harder thing to explain. When the gap is filled, the dividing cells *stop dividing*. The crawling stops. The collagen production tapers. The cells know they are done, and they return to maintenance, indistinguishable from their unwounded neighbors.

This is the behavior cancer breaks. In a normal tissue, proliferation switches on when there is work to do and switches off when the work is finished. Roughly thirty trillion cells in your body are coordinating this balance right now (Alberts et al., 2022). About 50 billion of them die each day and about 50 billion are born, and the total stays remarkably constant. To understand cancer, you first have to see the control system that holds that balance — because cancer is what happens when the control fails. That is this chapter.

<!-- → [DIAGRAM: wound healing timeline — clot, proliferation/migration of keratinocytes, then arrest when the gap closes] -->

## Core Concepts

The framing for this entire book is *regulation before failure*: see the normal control system first, then see how cancer breaks it. A normal cell is not a passive blob waiting to misbehave. It is actively, continuously regulated.

### The cell as machinery

A human cell is roughly 10 to 100 micrometers across, and there are more than 200 distinct types (Alberts et al., 2022). Underneath the specialization, every cell shares a common architecture: a **plasma membrane** (the boundary), a **nucleus** (the information vault), and the **cytoplasm** (the working space between them) filled with **organelles** — membrane-bound compartments, each a piece of machinery with a defined job.

The **nucleus** isolates information from work. It holds about two meters of DNA wound around histone proteins into **chromatin**, packaged into 46 **chromosomes** in human somatic cells. When the cell needs a protein, it does not ship the manual; it makes an RNA copy and sends that out through a **nuclear pore**. **Ribosomes** are the protein factories that read the RNA. The **endoplasmic reticulum (ER)** — rough (ribosome-studded, making secreted and membrane proteins) and smooth (lipid synthesis, detoxification) — folds and quality-checks proteins; when misfolded protein accumulates faster than it can be cleared, the cell enters **ER stress**, which can itself trigger cell death. The **Golgi apparatus** tags and sorts proteins. The **mitochondria** generate ATP — and, critically for cancer, they also gatekeep cell death: when a cell commits to dying, mitochondria release **cytochrome c** into the cytoplasm to launch the execution cascade (Letai, 2016). The **cytoskeleton** (actin microfilaments, intermediate filaments, microtubules) gives shape, enables crawling, and separates chromosomes during division.

Hold one correction in mind: the textbook diagram of a labeled blob is misleading. A real cell is in constant motion — vesicles moving along microtubule tracks, mitochondria fusing and fragmenting in minutes. The labels are useful; the controls governing that motion are what cancer breaks.

### The cell cycle as a decision system

A cell does not decide to divide and then divide. It enters the **cell cycle**, and the cycle decides whether to proceed. There are four phases: **G1** (growth, inventory), **S** (DNA synthesis — every chromosome copied once), **G2** (more growth, mitosis prep), and **M** (mitosis — physical division) (NCBI Bookshelf, *Cell Cycle and Programmed Cell Death*). A common misconception is that "cell cycle" means mitosis; in fact mitosis is only a small fraction of the cycle, and most of cancer biology is about what goes wrong in the long interphase (G1, S, G2).

The cycle is driven by **cyclin-dependent kinases (CDKs)** — enzymes that activate other proteins by phosphorylating them. CDKs are inactive alone; they switch on only when bound to **cyclins**, regulatory proteins whose levels rise and fall through the cycle (Ding et al., 2021). Cyclin D–CDK4/6 acts in G1; cyclin E–CDK2 drives the G1/S transition; cyclin A–CDK2 in S; cyclin B–CDK1 in M. After each pair fires, its cyclin is destroyed by the ubiquitin–proteasome system, which makes the cycle one-directional.

Built into the cycle are **checkpoints** — pauses where the cell verifies conditions before proceeding: the G1/S checkpoint (enough nutrients, growth signals, intact DNA?), the G2/M checkpoint (was all DNA copied correctly?), and the spindle-assembly checkpoint within M (are all chromosomes attached to the spindle?). Two proteins dominate the cancer story.

**p53** is "the guardian of the genome." When sensors (ATM, ATR) detect DNA damage, p53 is stabilized and acts as a transcription factor — turning on **p21** (which inhibits CDKs, halting the cycle) or, if damage is severe, pro-death genes like **PUMA**, **NOXA**, and **BAX** (NCI, *DINO and the p53 response*). p53 makes the keep-going-or-die decision. Roughly half of all human cancers carry a *TP53* mutation (Alberts et al., 2022); when p53 is gone, a cell with damaged DNA proceeds through S phase, copies the damage forward, and drifts.

**Rb** (retinoblastoma protein) gates G1/S by binding and inhibiting the transcription factor E2F. When cyclin D–CDK4/6 phosphorylates Rb, E2F is released and S-phase genes switch on. Lose Rb, and E2F is permanently free — the cell enters S phase whether it should or not. The childhood eye cancer retinoblastoma, requiring loss of both *RB1* copies, gave the protein its name and grounded Alfred Knudson's 1971 two-hit hypothesis (Knudson, 1971), which Chapter 4 develops.

<!-- → [FIGURE: cell cycle wheel showing G1/S/G2/M, the three checkpoints, cyclin-CDK pairs at each transition, and where p53 and Rb act] -->

### Information, communication, and death

The **central dogma** — DNA → RNA → protein — gives the cell its instructions and the means to use them. DNA is replicated in S phase with extraordinary fidelity: after polymerase proofreading and mismatch repair, the error rate is about 1 in 10⁹ base pairs, roughly three errors per division across the genome (Alberts et al., 2022). Most uncaught errors are neutral; a rare few create a selective advantage, and those are what matter for cancer. **Transcription** (DNA to messenger RNA) is *regulated* — the same genome produces a liver cell or a neuron depending on which genes are switched on by **transcription factors**. **Translation** reads each three-base **codon** of mRNA into an amino acid. The system is high-fidelity but not perfect, and tightly regulated both in the DNA sequence and in the epigenetic marks layered on top.

**Signaling** lets cells coordinate. A signal binds a receptor and triggers a cascade — typically receptor → adapter → kinase cascade → transcription factor → changed gene expression — that amplifies and integrates inputs. Three pathways recur in cancer: the **RAS/RAF/MEK/ERK (MAPK)** pathway, which drives proliferation and whose *RAS* genes are mutated in roughly 30% of human cancers (Alberts et al., 2022); the **PI3K/AKT/mTOR** pathway, governing growth and survival and restrained by the tumor suppressor PTEN; and the **Wnt/β-catenin** pathway, which loss of *APC* unleashes in colorectal cancer. A targeted therapy, in later chapters, almost always means a drug blocking one node in one of these pathways.

**Apoptosis** is programmed cell death — orderly, non-inflammatory self-destruction. A family of enzymes called **caspases** sit inactive until triggered, then cleave hundreds of cellular targets within minutes. The **intrinsic pathway** fires from internal signals (irreparable DNA damage, ER stress, loss of matrix contact): signals converge on mitochondria, cytochrome c is released, it assembles the **apoptosome** with Apaf-1, which activates caspase-9, then caspase-3. The **extrinsic pathway** fires from external death signals (FAS ligand, TRAIL) via death receptors and caspase-8. The **Bcl-2 family** sets the threshold: pro-survival members (Bcl-2, Bcl-XL) block mitochondrial permeabilization; pro-death members (BAX, BAK, BIM, PUMA, NOXA) promote it (Letai, 2016). Cancer cells almost universally evade apoptosis — by overexpressing Bcl-2, losing p53, or downregulating death receptors. Drugs that reverse this, such as the **BH3 mimetic** venetoclax that inhibits Bcl-2, work *because* the program was suppressed rather than destroyed (NCI, BH3 mimetic ABT-737; Letai, 2016).

### Integration: tissue homeostasis

Stack these cells into a tissue and the controls compound. In the gut, the lining is replaced every three to five days from **stem cells** at the base of crypts. A stem cell receives signals from its **niche** — Wnt from below, EGF nearby, BMP from above — that tell it whether to divide, differentiate, and migrate. Mutate *APC*, and the cell over-responds to Wnt, proliferates more than it should, and passes the defect to its daughters; over years the lineage accumulates more mutations, and a polyp becomes a carcinoma (NCBI Bookshelf, *Development and Causes of Cancer*). The pattern generalizes: **stem cell + niche + signals = controlled proliferation**, and losing one control lets the system drift. The NCI's working definition of cancer is exactly this — cells that grow uncontrollably, ignore stop and death signals, and spread (NCI, *What Is Cancer?*).

## Worked Example

**Situation.** A keratinocyte in your skin takes a hit of ultraviolet light, creating a **thymine dimer** — two adjacent thymines covalently linked into a structure DNA polymerase cannot read past. What does the cell do?

**Analytical process.** A first, wrong instinct is to say: "The cell is damaged, so it dies." That skips the control logic. Cells do not die on the first lesion — death is the expensive last resort, and treating it as automatic would mean a sunburn killed every exposed cell at once, which plainly does not happen. Track the actual machinery.

The cell enters S phase; polymerase reaches the dimer and stalls. **ATR** detects the stalled fork and phosphorylates **Chk1**, which inactivates Cdc25, keeping cyclin–CDK complexes off — S-phase progression halts. In parallel, ATR phosphorylates p53; phosphorylated p53 escapes its inhibitor MDM2, accumulates, and turns on p21, which blocks cyclin E–CDK2. The G1/S transition is doubly blocked. Now **nucleotide excision repair** excises the damaged segment and resynthesizes the strand. Damage cleared, ATR signaling subsides, p53 and p21 drop, and the cycle resumes (Alberts et al., 2022). Only if the damage is overwhelming does p53 instead switch on BAX, PUMA, and NOXA, committing the cell to apoptosis — and the skin replaces it.

**Resolution.** The cell pauses, repairs, and continues — or, if repair is hopeless, dies cleanly. Now remove p53: none of the p53-dependent steps happen. The cell carries its damage through replication, copies it into daughter strands, and the errors propagate. This, in compressed form, is how cancers start.

**The lesson.** Cancer is rarely one catastrophic event; it is the loss of a control protein that lets ordinary, frequent damage go uncorrected.

**The limit.** This linear story is cleanest for a single well-characterized lesion. Real cells integrate many simultaneous signals, and the same p53 can either arrest or kill depending on damage level, cell type, and context — a threshold behavior this tidy sequence does not fully capture.

## Common Misconceptions

**"Normal cells are passive until something turns them cancerous."** This inverts the biology. Normal cells are actively regulated every moment — receiving signals, checking their DNA, deciding division and death. In the opening case, what stops wound-edge cells from dividing is not the absence of a push but the presence of active controls. Cancer is the *loss* of regulation, not the gain of unusual activity.

**"Cancer is mostly about cells dividing too much."** Cell number depends on both birth and death. A tumor can arise as readily from cells that refuse to die as from cells that divide too fast. Students consistently over-focus on proliferation and underweight death evasion — yet evading apoptosis is one of the most universal features of cancer (Letai, 2016).

**"The cell cycle is basically mitosis."** Mitosis is the dramatic, visible phase, but it is a small slice of the cycle. The decisions that matter — to enter S phase, to halt for repair — are made in interphase, and that is where most cancer-driving failures occur.

**"Apoptosis is a cell giving up — a sign of weakness."** Apoptosis is among the most tightly regulated, energetically expensive behaviors a cell exhibits. It exists because multicellular life requires it. A cell that *will not* die when it should is the one that has broken the contract — and that is cancer.

## Exercises

1. **(Understand/Identify.)** For each function, name the organelle: (a) generates ATP and gatekeeps apoptosis; (b) reads mRNA to build protein; (c) tags and sorts proteins from the ER; (d) holds DNA behind a double membrane; (e) synthesizes lipids and detoxifies drugs.

2. **(Apply.)** A cultured cell completes one 24-hour cycle: G1 = 11 h, S = 8 h, G2 = 4 h, M = 1 h. A synchronized population of 1,000 cells starts in early G1 at *t* = 0. Which phase are the cells in at *t* = 6, 12, 18, and 24 hours? State one assumption your answer depends on.

3. **(Analyze/Produce.)** Draw a mechanism map for the UV-damaged keratinocyte: normal pathway → the specific molecular alteration if *TP53* is lost on both alleles → the resulting cell-level phenotype → one measurement that would let you detect the change in a tissue sample. Label every arrow with the molecule doing the work.

4. **(Apply/Predict.)** For each alteration, predict the cell-level consequence, arguing from the protein's normal job: (a) Bcl-2 overexpression in a B cell; (b) loss of one *APC* allele in a colon stem cell; (c) constitutive PI3K activation; (d) loss of both *RB1* alleles in a retinal cell.

## What Would Change My Mind

The chapter's central claim is that cancer is the failure of *ordinary* cell-regulation systems rather than the introduction of alien machinery. A finding that would force revision: discovery of a recurrent, cancer-specific molecular component with no normal-cell counterpart and no derivation from a normal gene — a true "cancer organelle" or a protein machine present only in tumors and essential to their growth. Decades of genomics have instead found cancer running on mutated versions of normal genes, which is why the regulation-before-failure frame holds. A reproducible exception of that kind would mean cancer is sometimes more than broken normality.

## Still Puzzling

- Why do some tissues — heart muscle, mature neurons — get cancer almost never, even after accumulating mutations across decades, while colon and skin get it often? The correlation with stem-cell division number (Tomasetti & Vogelstein, 2015) is real but [contested — see pantry flag], and does not fully explain the extremes.
- The cell-of-origin question is unsettled for many tumor types: which exact cell in a tissue becomes the cancer-initiating cell? Stem cell, progenitor, or a differentiated cell that de-differentiates?
- How does a single protein like p53 reliably distinguish "pause and repair" from "die now"? The threshold logic is observed but not fully mechanistically resolved.

## References

- Alberts, B., et al. *Molecular Biology of the Cell*, NCBI Bookshelf reference. https://www.ncbi.nlm.nih.gov/sites/books/n/mboc4/
- NCBI Bookshelf. *The Cell Cycle and Programmed Cell Death.* https://www.ncbi.nlm.nih.gov/books/NBK21056/
- NCBI Bookshelf. *The Development and Causes of Cancer.* https://www.ncbi.nlm.nih.gov/books/NBK9963/
- NCI. *What Is Cancer?* https://www.cancer.gov/about-cancer/understanding/what-is-cancer
- NCI Cancer Currents. *DINO RNA and the p53 response.* https://www.cancer.gov/news-events/cancer-currents-blog/2016/dino-p53
- NCI Drug Dictionary. *BH3 mimetic ABT-737.* https://www.cancer.gov/publications/dictionaries/cancer-drug/def/bh3-mimetic-abt-737
- Letai, A. (2016). Mitochondrial apoptosis and BH3 mimetics. https://pmc.ncbi.nlm.nih.gov/articles/PMC5133681/
- Ding, L., et al. (2021). Cyclin-Dependent Kinases and Their Regulation. *Int. J. Mol. Sci.* https://www.mdpi.com/1422-0067/22/6/2935
- Knudson, A. G. (1971). Mutation and Cancer: Statistical Study of Retinoblastoma. *PNAS* 68, 820–823.
- Tomasetti, C., & Vogelstein, B. (2015). Variation in cancer risk among tissues can be explained by the number of stem cell divisions. *Science* 347, 78–81.

---

## Prompts

*No figures have been generated for this chapter yet.*
