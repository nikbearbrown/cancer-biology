# Oncogenes

## Learning Objectives

By the end of this chapter, you should be able to:

- **Distinguish** a proto-oncogene from an oncogene, and **explain** why most oncogenes are normal cellular genes locked in an active state rather than foreign cancer genes.
- **Describe** the three principal mechanisms by which a proto-oncogene becomes an oncogene — point mutation, gene amplification, and chromosomal rearrangement — and **identify** a canonical example of each.
- **Trace** the signaling logic of RAS: how the protein normally switches off, how mutation prevents shutoff, and how the stuck switch drives proliferation.
- **Explain** why oncogenes typically require alteration of only one allele, and **contrast** this gain-of-function logic with the loss-of-function logic of tumor suppressors (Chapter 6).
- **Predict** why oncogene-addicted cancers respond to targeted drugs and why that response is usually temporary.

## Opening Case

A 58-year-old woman is diagnosed with chronic myeloid leukemia (CML). Her white blood cell count is enormous, packed with immature myeloid cells. A karyotype of her marrow shows the telltale lesion: a shortened chromosome 22, the Philadelphia chromosome, produced when a piece of chromosome 9 swaps with a piece of chromosome 22. The swap fuses two genes that should never meet — *BCR* and *ABL1* — into a single hybrid. The fusion protein is an enzyme that never stops firing, and its constant signal is what drives her marrow to overproduce.

Thirty years ago, this diagnosis carried a median survival of a few years. Her oncologist instead prescribes a daily pill. Within weeks her blood counts normalize; within months the Philadelphia chromosome is undetectable. The pill, imatinib, does one thing: it blocks the fused enzyme's active site (Druker et al., as summarized in NCBI Bookshelf, *The Development and Causes of Cancer*). The leukemia, it turns out, had bet everything on that one signal — and the drug called the bet.

This chapter is about why a single jammed gene can drive a cancer, and why blocking it can produce a near-cure. To get there we first have to see what these genes do when they are working normally.

## Core Concepts

### From proto-oncogene to oncogene

Start with the central, counterintuitive fact: **most oncogenes are not cancer genes.** They are normal cellular genes, doing useful work, that have been jammed into the "on" position.

A **proto-oncogene** is a normal gene that promotes cell growth, survival, or signaling as part of healthy tissue function. An **oncogene** is the altered, overactive version of that gene — the same gene after a mutation, amplification, or rearrangement has locked it into excessive or inappropriate activity. The mutation does not give the gene a new job; it removes the controls on the old one. The *KRAS* gene that drives roughly 90 percent of pancreatic cancers is the same *KRAS* required for normal growth-factor signaling in dividing cells throughout the body (NCI, *The Genetics of Cancer*). A single point mutation is what converts the useful gene into the cancer driver.

This was the conceptual revolution. Before the 1970s, cancer was thought to come from outside — a virus, a carcinogen, a foreign "cancer principle." Then Harold Varmus and Michael Bishop, studying the Rous sarcoma retrovirus, discovered that its transforming gene (*v-src*) was a captured, slightly altered copy of a gene already present in normal cells (*c-src*) (NCBI Bookshelf, *The Development and Causes of Cancer*). The implication: cells carry within their own genomes the genes that, when altered, cause cancer. Bishop and Varmus shared the 1989 Nobel Prize for the framework that is now textbook. The first human oncogene, a mutant *HRAS* from a bladder cancer, was identified by transfection assays in 1982.

About 100 human proto-oncogenes are known. They cluster in a few functional categories — growth factors, growth-factor receptors, signaling kinases, GTP-binding switch proteins, transcription factors, cell-cycle and apoptosis regulators. The categories make sense: a cell that grows inappropriately is misfiring the same machinery that controls normal growth.

<!-- → [DIAGRAM: proto-oncogene functional categories arranged along a growth-factor signaling pathway, from secreted growth factor → receptor → cytoplasmic kinase → RAS switch → MAPK cascade → transcription factor → cell-cycle gene] -->

### Gain-of-function genetics: why one allele is enough

Here is the genetic signature of an oncogene: a single altered allele is usually sufficient. The problem is too much activity, and one overactive copy provides it. This is **gain of function**, and it makes oncogene mutations behave as **dominant** at the cellular level — one mutated copy overrides the normal one.

Contrast this with tumor suppressors (Chapter 6), where the problem is *loss* of a restraining function and both copies must typically be knocked out before the brake fails — the **two-hit** logic of Knudson (Hino, 2017). Applying two-hit reasoning to oncogenes is a common error: you do not need to mutate both *KRAS* alleles, because one stuck accelerator already pushes the cell forward.

A clean illustration is **HER2** (also called *ERBB2*), a growth-factor receptor. In about 15–20 percent of breast cancers, the *HER2* gene is amplified — present in many extra copies — so the cell displays an overwhelming density of receptor. The protein itself is normal; there is simply too much of it, and the tissue behaves as if drenched in growth signal [verify — specific percentage].

### Three mechanisms of activation

A proto-oncogene becomes an oncogene by one of three main routes.

**Point mutation.** A single base change alters one amino acid and locks the protein active. *KRAS* G12D — glycine to aspartate at codon 12 — is the prototype. *BRAF* V600E, found in roughly half of melanomas, is another (NCBI Bookshelf, *The Development and Causes of Cancer*). What is striking is the *narrowness* of where these mutations land. *KRAS* in pancreatic cancer is almost always mutated at codon 12, rarely elsewhere — because only mutations at the regulatory region produce the constitutively active protein that confers a growth advantage. Selection, not chemistry, explains the hot spots.

**Gene amplification.** Extra copies of the gene raise expression dramatically. *MYCN* is amplified in about 25 percent of neuroblastomas and predicts poor prognosis; *HER2* is amplified in breast and gastric cancers; *EGFR* is amplified in roughly half of glioblastomas. The protein is normal but present at 10 to 100 times the usual level.

**Chromosomal rearrangement.** Translocations either create hybrid proteins or place a gene under inappropriate control. The Philadelphia chromosome from the opening case — *BCR-ABL* — is the canonical fusion: the ABL kinase, normally held in an autoinhibited state, loses its restraint in the fusion and fires continuously. Rearrangements can also drive cancer by **enhancer hijacking**: in Burkitt lymphoma, the t(8;14) translocation moves *MYC* next to immunoglobulin enhancers, forcing the normal MYC protein to extreme expression.

<!-- → [DIAGRAM: three-panel comparison — point mutation (single base → stuck protein), amplification (many gene copies → excess protein), translocation (gene fusion → novel active enzyme)] -->

### RAS: a switch stuck on

RAS deserves a closer look because it is the most commonly mutated oncogene family and because its biology shows the logic cleanly. The three RAS genes — *KRAS*, *HRAS*, *NRAS* — encode small membrane-bound GTPases. A **GTPase** is a molecular switch: **active** when bound to GTP, **inactive** when bound to GDP. Guanine nucleotide exchange factors (GEFs) load GTP and switch RAS on; GTPase-activating proteins (GAPs) accelerate hydrolysis of GTP to GDP and switch it off. Active RAS signals through the RAF→MEK→ERK (MAPK) cascade and the PI3K→AKT pathway, both of which drive proliferation and survival (NCBI Bookshelf, *The Development and Causes of Cancer*).

Mutations at codons 12, 13, or 61 interfere with GTP hydrolysis. RAS can no longer turn itself off — even with GAP help, hydrolysis is roughly 100-fold slower. The switch stays on. The cell keeps receiving the "grow" signal with no growth factor present. The classical analogy is a stuck accelerator, and like all analogies it must be tied back to the molecule: the accelerator is GTP that cannot be hydrolyzed.

RAS was considered "undruggable" for decades — the protein has no obvious pocket for a small molecule to grab. That changed when the *KRAS* G12C mutant, common in lung adenocarcinoma, was found to present a reactive surface cysteine that a covalent drug could bind. Sotorasib and adagrasib, both G12C-specific, are now FDA-approved for *KRAS* G12C-mutant lung cancer — modest benefits, but proof that even the hardest targets can yield. The more common G12D mutation (the prototypical pancreatic-cancer driver) lacks that reactive cysteine, which is why a G12D inhibitor was much harder to develop. The boundary condition matters: a strategy that works for one specific RAS variant does not automatically transfer to another.

### MYC: the transcription-factor problem

A second deeply important oncogene category is the **transcription factor** — a protein that binds DNA at specific sequences and turns target genes on or off. The MYC family (*MYC*, *MYCN*, *MYCL*) is the most cancer-relevant; MYC is deregulated in a large fraction of human cancers by amplification, translocation, or upstream pathway activation, and it drives expression of thousands of genes involved in proliferation, metabolism, and ribosome biogenesis (Hanahan, 2022).

MYC also shows how proto-oncogenes are normally controlled. In healthy cells MYC is produced in brief pulses — both the mRNA and the protein have short half-lives — so a growth signal triggers a wave of target-gene expression that then subsides. Cancers that have lost this control (by translocation, amplification, or stabilizing the protein) keep MYC high constantly, locking the cell in proliferation mode. Like RAS, MYC has long been considered undruggable, because a transcription factor has no enzymatic active site to inhibit. The productive strategy has been indirect — drugging what MYC-driven cells depend on (transcriptional cofactors such as the BET reader BRD4, specific metabolic pathways) rather than MYC itself.

## Worked Example

**Situation.** A 55-year-old never-smoker is diagnosed with non-small-cell lung adenocarcinoma. Tumor sequencing is ordered to match her to a targeted therapy.

**Process.** The report shows an *EGFR* exon-19 deletion — a small indel that locks the EGFR receptor tyrosine kinase in an active, ligand-independent state. EGFR signals through RAS/MAPK and PI3K/AKT, the same proliferative pathways RAS feeds. The cell is **oncogene-addicted**: its survival now depends on the continuous EGFR signal. She is started on osimertinib, an EGFR inhibitor, and her tumors shrink dramatically over three months.

*A dead end.* One might predict the response is permanent, because the drug blocks the causal driver. It is not. After about eighteen months her cancer regrows. Resequencing of the resistant tumor shows the original *EGFR* mutation *plus* an amplification of a different gene, *MET*. The cancer has rewired: it now drives the same downstream pathways through MET instead of EGFR — a **bypass track**. Blocking EGFR no longer matters, because the proliferative signal arrives by another route.

**Resolution.** Her therapy is changed to combine EGFR and MET inhibition, restoring control for a further period. Resistance, in oncogene-addicted cancers, is the rule, not the exception. It arises by secondary mutation in the target (the EGFR T790M "gatekeeper" mutation, the BCR-ABL T315I mutation), amplification of the target, bypass activation of a parallel pathway, or phenotypic switching to a different cell state.

**The lesson.** Targeted drugs work because the cancer depends on the oncogene's output, but the same cancer can evolve a new way to produce that output, so durable control requires anticipating and blocking the escape routes.

**The limit.** This logic holds for cancers with a single dominant driver; tumors with many co-equal drivers, or with no druggable driver (most pancreatic *KRAS* cancers, until recently), do not respond to this strategy.

## Common Misconceptions

**"Oncogenes are genes whose normal purpose is to cause cancer."** This inverts the biology. Proto-oncogenes do essential work — signaling growth, transmitting receptor signals, driving normal proliferation. Cancer arises when one is locked active, not when a "cancer gene" is switched on. In the opening case, *ABL1* is a normal kinase needed for healthy cells; the disease comes from fusing it to *BCR* so it cannot turn off.

**"You need to knock out both copies of an oncogene, like a tumor suppressor."** This misapplies two-hit logic. Because the problem is excess activity, a single mutant allele is dominant and sufficient (Hino, 2017). The CML patient has one *BCR-ABL* fusion allele and one normal *ABL1*; the fusion alone drives the disease.

**"If the drug hits the causal driver, the response should be permanent."** As the worked example shows, oncogene addiction creates a real vulnerability but not a permanent one. Cancer is an evolving population; secondary mutations and bypass tracks restore pathway output. The CML patient's leukemia can acquire the T315I mutation that prevents imatinib from binding, requiring a different inhibitor.

## Exercises

1. **(Understand)** For each mechanism of activation — point mutation, amplification, translocation — name one oncogene example from this chapter and state in one sentence what the alteration does to the protein.

2. **(Apply)** A tumor carries a *KRAS* G12D mutation. Explain, step by step, why a drug that blocks the RAS GTP-binding pocket the way imatinib blocks ABL has historically been hard to design, and why a G12C-specific covalent inhibitor became possible while a G12D one was harder. Tie your answer to the chemistry of the mutated residue.

3. **(Apply / Produce)** Draw a mechanism map for HER2-amplified breast cancer with four boxes: *normal regulation → cancer alteration → cellular phenotype → therapeutic intervention*. Label the molecule, the mechanism (amplification), the phenotype (excess proliferative signaling), and the drug (trastuzumab). Then add a fifth box for a plausible resistance mechanism.

4. **(Analyze)** Classify each statement as a *definition*, a *mechanism*, an *epidemiological association*, or a *therapeutic implication*: (a) "KRAS is mutated in ~90% of pancreatic cancers." (b) "A codon-12 substitution slows GTP hydrolysis." (c) "An oncogene is an activated proto-oncogene." (d) "BCR-ABL-positive CML responds to imatinib."

## What Would Change My Mind

The chapter's central claim is that oncogene activation is gain-of-function and dominant — one altered allele drives the phenotype. A finding that would force revision: convincing evidence that the canonical oncogenic alterations (KRAS G12, BCR-ABL, HER2 amplification) routinely require *biallelic* inactivation of the normal copy to transform cells, or that single-allele oncogene activation reproducibly fails to confer a growth advantage in well-controlled systems. The transfection assays that found the first human oncogene specifically detected single-allele dominant transformation; a robust failure to replicate that result across modern model systems would undermine the gain-of-function framework.

## Still Puzzling

- Why do some oncogenes (KRAS, MYC) remain so hard to drug directly even though we have known their sequence for decades, while others (BCR-ABL, EGFR) yielded almost immediately? Is "druggability" a property of the protein, the pathway, or our chemistry?
- Why does the same mutation (KRAS G12D) drive aggressive pancreatic cancer but is far less common in other tissues — what tissue context determines whether a stuck accelerator transforms a cell?
- When a cancer escapes targeted therapy by phenotypic switching rather than mutation, is the change genetic, epigenetic, or both? This question hands directly to Chapters 7 and 8 on epigenetic reprogramming.

## References

- National Cancer Institute. *The Genetics of Cancer.* https://www.cancer.gov/about-cancer/causes-prevention/genetics
- National Cancer Institute. *What Is Cancer?* https://www.cancer.gov/about-cancer/understanding/what-is-cancer
- Hino, O., et al. *The two-hit hypothesis, the driver of cancer.* Cancer Science, 2017. https://onlinelibrary.wiley.com/doi/10.1111/cas.13116
- NCBI Bookshelf. *The Development and Causes of Cancer.* https://www.ncbi.nlm.nih.gov/books/NBK9963/
- Hanahan, D. *Hallmarks of Cancer: New Dimensions.* Cancer Discovery, 2022. https://aacrjournals.org/cancerdiscovery/article/12/1/31/675608
- NCBI Bookshelf. *Molecular Biology of the Cell.* https://www.ncbi.nlm.nih.gov/sites/books/n/mboc4/

## Prompts

*No figures have been generated for this chapter yet.*
