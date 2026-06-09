# Epigenetics in Cancer: Noncoding RNAs, Reprogramming, and Therapy

## Learning Objectives

By the end of this chapter, you should be able to:

- **Explain** how microRNAs and long noncoding RNAs regulate gene expression, and **classify** a given noncoding RNA as oncogenic or tumor-suppressive by its targets.
- **Describe** the Polycomb–Trithorax system and **explain** how bivalent chromatin connects cellular memory to cancer plasticity.
- **Define** epigenetic reprogramming and the cancer stem cell hypothesis, and **distinguish** the well-supported claims from the contested ones.
- **Survey** the major classes of epigenetic therapy (DNMT, HDAC, EZH2, IDH, BET inhibitors) and **explain** why reversibility is their unifying principle.
- **Evaluate** an epigenetic finding by classifying it as established mechanism, plausible mechanism, or therapeutic speculation.

## Opening Case

In 2002, a research team studying chronic lymphocytic leukemia went looking for the tumor suppressor that ought to sit in a chromosomal region frequently deleted in these patients. They found no protein-coding gene there at all. What they found instead were two **microRNAs** — *miR-15* and *miR-16* — tiny RNA molecules that encode no protein but silence the messenger RNAs of other genes. The deleted region was costing the cell its microRNAs, and that loss released a network of pro-survival genes the microRNAs normally held down (Croce et al., 2002, summarized in archive chapter).

The result reframed a whole layer of biology. The genome was supposed to encode proteins, and for decades the 98 percent that does not was dismissed as filler. But a human has roughly the same number of protein-coding genes as a roundworm — about 20,000. The extra complexity is encoded elsewhere, in the regulatory RNA transcribed from that "non-coding" majority. Cancer, it turns out, deranges this layer extensively.

This chapter picks up where Chapter 7 left off. It covers the noncoding RNAs, the Polycomb–Trithorax system that maintains cell identity, the reprogramming and plasticity that let cancers change their identity under pressure, and the epigenetic drugs that exploit all of it.

## Core Concepts

### MicroRNAs: oncomiRs and tumor-suppressive miRNAs

A **microRNA (miRNA)** is a short RNA, 18–25 nucleotides long, that binds partially complementary sites in the 3′ untranslated regions of target messenger RNAs and silences them — by blocking translation or triggering mRNA degradation. The silencing is done by the miRNA loaded into the **RNA-induced silencing complex (RISC)**. The biogenesis pathway is conserved: a long primary transcript is cleaved by Drosha in the nucleus, exported, cleaved again by Dicer in the cytoplasm, and one strand is loaded into Argonaute to guide RISC (Signal Transduction and Targeted Therapy, 2023). Because the binding is only partial, a single miRNA can target hundreds of mRNAs — its regulatory reach is enormous.

In cancer, miRNAs deregulate in characteristic ways. An **oncomiR** is a miRNA whose overexpression promotes cancer by silencing tumor suppressor mRNAs. *miR-21*, the most-studied oncomiR, is upregulated in nearly every solid cancer and silences the tumor suppressors PTEN and PDCD4, contributing to invasion and metastasis. *miR-17~92*, a six-miRNA cluster and a *MYC* target, is overexpressed in many lymphomas.

Conversely, some miRNAs are tumor suppressors. The *let-7* family targets the oncogenes *RAS* and *MYC*; its loss is common in lung adenocarcinoma. *miR-34a* is a p53 target that helps enact p53's tumor-suppressive program, and its loss is common in p53-mutant cancers. The opening case's *miR-15/miR-16* are tumor-suppressive miRNAs lost by deletion.

Clinically, miRNAs are pursued as biomarkers — they are unusually stable in blood and survive degradation that destroys mRNA — and as therapeutics, by delivering mimics of lost tumor-suppressive miRNAs or inhibitors (anti-miRs) of oncomiRs. The biology is sound; the bottleneck is delivery. MRX34, a *miR-34a* mimic, entered trials in 2013 but was halted in 2016 for immune toxicity. Getting nucleic acids into solid tumors at therapeutic doses remains the hard problem.

<!-- → [DIAGRAM: miRNA mechanism — oncomiR (miR-21) silencing tumor suppressor PTEN vs tumor-suppressive miRNA (let-7) silencing oncogene RAS, showing opposite phenotypic outcomes] -->

### Long noncoding RNAs

**Long noncoding RNAs (lncRNAs)** are transcripts longer than 200 nucleotides with no protein-coding potential. The genome encodes tens of thousands, and they are functionally heterogeneous: some scaffold protein complexes, some guide chromatin-modifying enzymes to specific loci, some "sponge" miRNAs out of the regulatory pool.

The mechanistic example to hold is *HOTAIR*: a lncRNA that binds Polycomb Repressive Complex 2 (PRC2) and guides it to specific genomic sites, directing the silencing of tumor suppressor genes that would normally be expressed. *HOTAIR* overexpression appears in breast, colorectal, liver, lung, and gastric cancers and correlates with poor prognosis. *MALAT1* (regulating splicing and metastatic behavior) and *NEAT1* (assembling stress-tolerance nuclear bodies) are other widely overexpressed examples. The catalog runs into the hundreds; therapeutic targeting, via antisense oligonucleotides, is still early.

### Polycomb and Trithorax: cellular memory

A cell's identity must survive division — a skin cell's daughters must be skin cells. The transcriptional pattern that defines a cell type is maintained by two opposing, conserved chromatin systems first identified in *Drosophila*: the **Polycomb group**, which maintains *silencing*, and the **Trithorax group**, which maintains *activation*, at the same target genes.

Polycomb works through two complexes. **PRC2** (catalytic subunit EZH2) writes the repressive mark H3K27me3; **PRC1** reads that mark, adds a second repressive mark, and compacts chromatin. Together they keep differentiation genes that should be off, off. The Trithorax group — the KMT2/MLL methyltransferases that write the activating H3K4me3 mark, plus the SWI/SNF remodeling complex — keeps genes that should be on, on.

The concept that links this to cancer is **bivalent chromatin**. In embryonic stem cells, many developmental genes carry *both* the repressive H3K27me3 *and* the activating H3K4me3 simultaneously — they are *poised*, kept low but ready to fire when the cell commits to a lineage. As a cell differentiates, the bivalent state resolves to one or the other. Aggressive cancer cells often *regain* bivalent patterns resembling stem cells: differentiation programs that should be locked stay accessible, and the cell can shift between phenotypes more easily. This is one molecular basis for the **plasticity** that lets cancers de-differentiate and evade targeted therapy by switching identity (Hanahan, 2022).

In cancer, both systems are hit: EZH2 is hyperactivated in lymphomas; MLL1 is rearranged in infant leukemias; SWI/SNF is mutated in ~20 percent of all cancers (carried over from Chapter 7).

### Reprogramming and cancer stem cells — carefully

Here the evidence is genuinely mixed, and the chapter should say so rather than overstate.

**Epigenetic reprogramming** is the claim that some cancers arise when a cell's chromatin landscape is reset to a stem-like state — reactivating stem-cell transcriptional programs — without necessarily the prior mutations the classical model expects. The supporting observation is **DNA methylation drift**: as tissues age, stem-cell methylation patterns drift, the drift correlates with cancer incidence, and epigenetic "clocks" (the Horvath clock) measure it (Hanahan, 2022). This is correlative; whether drift *causes* cancer or merely accompanies it is not settled.

The **cancer stem cell hypothesis** proposes that tumors are hierarchically organized, sustained by a small population of cancer stem cells while the bulk of tumor cells are more differentiated descendants. It is supported by some xenotransplantation experiments (only certain marker-defined cells re-establish the tumor in mice) and contested by others (under permissive conditions, most cells show stem-like potential). The therapeutic stakes are real — if a stem-cell population survives chemotherapy that kills the bulk tumor, it could drive recurrence — but drugs aimed at cancer stem cells (Wnt, Notch, Hedgehog inhibitors) have given mixed clinical results. Present this as active synthesis, not settled dogma (per pantry guidance) [contested — see pantry flag].

### Epigenetic therapy: the unifying principle

Several epigenetic drug classes are now FDA-approved, and what unifies them is that **epigenetic states are reversible while mutations are not** — they can restore a function rather than only block one (Experimental & Molecular Medicine, 2023).

- **DNMT inhibitors** (azacitidine, decitabine): demethylate silenced tumor suppressors and induce differentiation; standard for MDS and elderly AML; combine powerfully with venetoclax in AML. In solid tumors they help most in combination — notably with immune checkpoint inhibitors, where demethylation reactivates dormant immune-recognition genes and makes the tumor more visible to the immune system.
- **HDAC inhibitors** (vorinostat, romidepsin): hyperacetylate histones to reactivate silenced genes; effective mainly in blood cancers, limited by off-target toxicity.
- **EZH2 inhibitors** (tazemetostat, approved 2020): work in EZH2-mutant follicular lymphoma and in *SMARCB1*-deleted epithelioid sarcoma through synthetic-lethal EZH2 dependency.
- **IDH inhibitors** (ivosidenib, enasidenib): suppress the oncometabolite 2-hydroxyglutarate, restoring demethylase function — the cleanest demonstration that epigenetic dysregulation can be pharmacologically reversed.
- **BET inhibitors** (in trials): block bromodomain *readers* that recruit transcription machinery to acetylated chromatin, downregulating MYC-driven programs; modest activity but validating the reader layer as a target.

The clinical impact has been concentrated in blood cancers, where chromatin states are more accessible. Solid tumors resist, partly because their chromatin is more entrenched and partly because the microenvironment supplies survival signals epigenetic drugs alone cannot overcome. Combination strategies are where the next progress is most likely.

## Worked Example

**Situation.** An *EGFR*-mutant lung adenocarcinoma initially shrinks on osimertinib (Chapter 5) but regrows after eighteen months. Sequencing of the resistant tumor shows the original *EGFR* mutation is still present, no new resistance *mutation* in *EGFR*, and — strikingly — the cancer now histologically resembles small-cell lung cancer rather than adenocarcinoma. How did the tumor change identity without a new driver mutation?

**Process.** Start with the expectation from Chapter 5: resistance usually comes from a secondary mutation in the target or a bypass mutation in a parallel pathway. Sequencing was ordered on that assumption.

*A dead end.* No such mutation is found. The *EGFR* driver is unchanged and no bypass-pathway mutation explains the escape. The genetic model predicts a mutation that is not there.

Now bring in this chapter's tools. The transformation to a small-cell phenotype is a **phenotypic switch** — a change in cell identity. Such switches are driven not (or not only) by new mutations but by **epigenetic reprogramming**: the chromatin landscape shifts, bivalent developmental genes that were poised become activated, and the cell adopts a neuroendocrine transcriptional program in which EGFR signaling is no longer the survival driver. The drug still blocks EGFR perfectly — but the cell no longer depends on EGFR.

**Resolution.** Because the resistance is a change of state rather than a change of target, the path forward is not a better EGFR inhibitor but a different therapeutic class matched to the new small-cell phenotype. The reprogramming that defeated the targeted drug is, in principle, an epigenetic process — and that is why epigenetic and combination therapies are an active frontier for exactly this kind of escape.

**The lesson.** Cancer cell identity is not fixed by its founding mutation; under therapeutic pressure a cell can epigenetically reprogram into a different phenotype that no longer needs the original driver — and a genetic-only search for resistance will miss it.

**The limit.** Phenotypic switching is one resistance route among several; many resistances still are simple secondary mutations, and the relative frequency of reprogramming-based escape varies by cancer type and is still being quantified.

<!-- → [DIAGRAM: phenotypic switching under drug pressure — adenocarcinoma cell (EGFR-addicted, drug-sensitive) → epigenetic reprogramming → small-cell phenotype (EGFR-independent, drug-resistant), with bivalent chromatin resolving toward a neuroendocrine program] -->

## Common Misconceptions

**"RNA only matters as mRNA — the messenger between gene and protein."** Most of the genome's RNA output is never translated. miRNAs silence tumor suppressor mRNAs; lncRNAs like HOTAIR guide silencing complexes to specific genes. In the opening case, deleting two non-coding miRNAs — *miR-15/miR-16* — was enough to release a pro-survival network and drive leukemia.

**"Once a cell acquires its driver mutation, its identity is fixed."** The worked example shows the opposite: an EGFR-mutant adenocarcinoma can reprogram into a small-cell phenotype that no longer needs EGFR, with no new driver mutation. Plasticity, grounded in bivalent chromatin and epigenetic reprogramming, lets cancer cells change identity under pressure.

**"Early mechanistic findings about RNA modification (m6A, m5C) are settled cancer biology."** The epitranscriptomics field is promising but still emerging. A finding that an RNA modification correlates with a cancer phenotype is not the same as an established causal mechanism or a validated drug target. Classify such claims as plausible mechanism or therapeutic speculation until the causal and clinical evidence is in [contested — see pantry flag].

## Exercises

1. **(Understand)** Explain how a *single* deleted microRNA can disable an entire network of target mRNAs, and why that makes miRNA loss different in scope from losing one protein-coding tumor suppressor.

2. **(Apply)** A lncRNA, *HOTAIR*, is overexpressed in a patient's breast cancer and the tumor shows silencing of several tumor suppressors that lack any mutation or promoter mutation. Propose a mechanism linking the lncRNA to the silencing, naming the complex involved, and state what experiment would test it.

3. **(Apply / Produce)** Draw a mechanism map for therapy-induced phenotypic switching with the boxes *targeted drug applied → selection/induction of a tolerant state → epigenetic reprogramming → new phenotype → clinical consequence*. Label where in this chain a genetic-only resistance assay would fail to detect the escape.

4. **(Evaluate)** For each statement, classify it as *established mechanism*, *plausible mechanism*, or *therapeutic speculation*, and justify in one sentence: (a) "IDH inhibitors reverse hypermethylation by lowering 2HG." (b) "Cancer stem cells are a distinct, drug-resistant population in every solid tumor." (c) "An m6A RNA mark drives metastasis and is a ready drug target." (d) "miR-15/miR-16 loss releases pro-survival genes in CLL."

## What Would Change My Mind

The chapter's central claim is that the noncoding and reprogramming layer of the epigenome is a genuine, sometimes independent driver of cancer behavior — not merely a readout of upstream genetic events — and that epigenetic states' reversibility makes them therapeutically exploitable. Findings that would force revision: convincing evidence that noncoding-RNA changes and phenotypic switches are consistently *downstream* of, and fully explained by, genetic alterations; or that therapy-induced reprogramming (such as adenocarcinoma-to-small-cell transformation) is in every case driven by a selectable pre-existing mutation rather than an epigenetic state change. The cancer stem cell and reprogramming claims are the most contestable here; stronger lineage-tracing evidence either way would substantially revise this chapter.

## Still Puzzling

- Is therapy-induced reprogramming the *selection* of a rare pre-existing drug-tolerant cell or the *induction* of a new state in many cells? The answer changes how we would prevent it, and current evidence supports both in different settings.
- Are cancer stem cells a fixed, distinct population or a transient state any cell can enter? The xenotransplant evidence points one way, the plasticity evidence the other.
- How much of the regulatory noncoding RNA we now detect is functional versus transcriptional noise? As detection improves, distinguishing load-bearing lncRNAs from background remains genuinely hard — and bears on which are worth targeting.

## References

- Signal Transduction and Targeted Therapy. *Epigenetic regulation in the tumor microenvironment.* 2023. https://www.nature.com/articles/s41392-023-01480-x
- Experimental & Molecular Medicine. *Metabolic reprogramming and epigenetic modifications in cancer.* 2023. https://www.nature.com/articles/s12276-023-01020-1
- Hanahan, D. *Hallmarks of Cancer: New Dimensions.* Cancer Discovery, 2022. https://aacrjournals.org/cancerdiscovery/article/12/1/31/675608
- National Cancer Institute. *What Is Cancer?* https://www.cancer.gov/about-cancer/understanding/what-is-cancer
- NCBI Bookshelf. *Molecular Biology of the Cell.* https://www.ncbi.nlm.nih.gov/sites/books/n/mboc4/

## Prompts

*No figures have been generated for this chapter yet.*
