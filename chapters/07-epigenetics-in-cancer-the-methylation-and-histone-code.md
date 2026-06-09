# Epigenetics in Cancer: The Methylation and Histone Code

## Learning Objectives

By the end of this chapter, you should be able to:

- **Define** epigenetics precisely and **explain** why heritable changes in gene expression can occur without any change to DNA sequence.
- **Describe** the paradoxical methylation pattern of cancer — global hypomethylation alongside focal CpG-island hypermethylation — and **explain** how each contributes to the cancer phenotype.
- **Interpret** MGMT promoter methylation in glioblastoma as a predictive biomarker, **tracing** the mechanism from methyl mark to drug response.
- **Distinguish** the writer, eraser, and reader enzymes of the histone code and **identify** how their mutation reshapes the transcriptome in cancer.
- **Evaluate** the claim that epigenetic changes are reversible and therefore easily drugged, naming the conditions under which reversibility helps and where it does not.

## Opening Case

Two patients have the same diagnosis — glioblastoma, the most common and most lethal primary brain cancer — and receive the same treatment: surgery, radiation, and temozolomide, a drug that damages tumor DNA by attaching methyl groups to guanine bases. One patient survives far longer than the other. Their tumors look identical under the microscope and carry overlapping mutations. The difference is a chemical mark on a single gene's promoter.

That gene is *MGMT*. Its protein removes exactly the kind of DNA damage temozolomide causes. In the longer-surviving patient, the *MGMT* promoter is **hypermethylated** — chemically silenced — so the repair protein is not made, the drug's damage accumulates, and tumor cells die. In the other patient, *MGMT* is expressed, the damage is repaired, and the drug is largely wasted. No gene sequence differs between them. The decisive variable is a layer of regulation sitting *on top of* the DNA (Stupp protocol, summarized in NCI, *What Is Cancer?*) [verify].

This is the central fact of cancer epigenetics: cancer is not only a disease of broken genes but of *misread* ones. This chapter explains how that misreading happens through DNA methylation and the histone code, and whether we can reverse it.

## Core Concepts

### What "epigenetics" actually means

A neuron, a liver cell, and a skin cell carry the same ~20,000 protein-coding genes, yet they are different cell types doing different work. What distinguishes them is not DNA sequence but the **epigenome** — the set of chemical marks layered onto DNA and onto the histone proteins that package it, controlling which genes are read and which are silenced.

**Epigenetics** refers to heritable changes in gene expression that do not involve changes to the DNA sequence. The marks are chemical — methyl groups on cytosine bases, acetyl and methyl groups on histone tails, ubiquitin tags — and crucially they **propagate through cell division**. The system has memory because the marks are *enzymatically maintained*: after DNA replicates, the new strand carries no methylation, and the maintenance methyltransferase DNMT1 recognizes this hemimethylated state and methylates the daughter strand to match the parent (Signal Transduction and Targeted Therapy, 2023). A skin cell stays a skin cell across hundreds of divisions because its epigenetic state is faithfully copied.

This memory is what makes epigenetics matter for cancer. Once a tumor suppressor is silenced by methylation, the silencing is inherited by every daughter cell without any new mutation. The lineage drifts from its tissue identity, and the changes accumulate the way mutations do — except that, in principle, they are reversible.

The three pillars of epigenetic regulation are DNA methylation, histone modifications, and noncoding RNAs. This chapter covers the first two; Chapter 8 covers the third and the systems-level picture.

<!-- → [DIAGRAM: same genome, three cell types — identical DNA sequence with different methylation/histone-mark patterns producing neuron, hepatocyte, skin cell] -->

### DNA methylation and its cancer paradox

In mammals, DNA methylation occurs overwhelmingly at **CpG dinucleotides** — a cytosine followed by a guanine — where a methyl group is added to the cytosine (producing 5-methylcytosine). Because CpG is symmetric across the two strands, the mark survives replication: DNMT1 reads the hemimethylated site and restores it.

Most CpG sites in the genome are methylated — partly to keep repetitive, transposon-derived DNA silent. The exceptions are **CpG islands**: short, CpG-dense regions near the transcription start sites of most genes, normally kept *unmethylated* so transcription can proceed. When a CpG island becomes hypermethylated, the gene downstream is reliably silenced.

In cancer, two opposite things happen to methylation, and this only looks paradoxical at first.

First, **global hypomethylation**. The bulk genome of a cancer cell is *less* methylated than normal, especially at repetitive and intergenic regions. Transposable elements that should be silent reactivate; the genome becomes more fragile and prone to recombination; chromosomal instability rises. This was the first epigenetic abnormality observed in human tumors (Feinberg and Vogelstein, 1983).

Second, **focal hypermethylation of CpG islands** at specific tumor suppressor promoters. *CDKN2A* (p16) is silenced this way in many cancers; *MLH1* is methylated in ~15 percent of sporadic colorectal cancers, phenocopying the germline mismatch-repair loss of Lynch syndrome; *BRCA1* is methylated in some sporadic ovarian and breast cancers, mimicking the inherited mutation from Chapter 6. The two patterns reflect different machinery — failing maintenance on the bulk genome, selected silencing at specific promoters — and both favor the cancer.

What makes promoter methylation therapeutically interesting is that, unlike a mutation, it is **reversible**. The gene sequence is intact; remove the methyl groups and transcription can resume. DNA methyltransferase inhibitors — azacitidine and decitabine — are cytosine analogs that incorporate into DNA, trap DNMT1 in a covalent complex, and let the genome lose methylation over a few divisions, reactivating some silenced genes. Azacitidine, approved for myelodysplastic syndrome in 2004, was the first epigenetic cancer drug; both are now standard for MDS and elderly AML.

### The histone code

The other major layer of marks is on the histones. The structural unit of chromatin is the **nucleosome** — ~147 base pairs of DNA wrapped around a histone octamer (two each of H2A, H2B, H3, H4). The histones are not passive packaging: their N-terminal tails project outward and carry a dense set of chemical marks that are *written* by one set of enzymes, *erased* by another, and *read* by a third. Different marks correlate with different transcriptional states (Signal Transduction and Targeted Therapy, 2023).

The vocabulary you need:

- **Histone acetylation** adds an acetyl group to a lysine (written by histone acetyltransferases/HATs, removed by histone deacetylases/HDACs). It neutralizes the lysine's positive charge, loosens histone–DNA contacts, and opens chromatin. Acetylation is generally *activating*; H3K27ac marks active enhancers.
- **Histone methylation** adds methyl groups to lysines or arginines (written by methyltransferases/KMTs, removed by demethylases/KDMs), and its meaning depends on position and degree. H3K4me3 marks active promoters; H3K27me3 marks Polycomb-repressed regions; H3K9me3 marks heterochromatin (silent, densely packed).

A single nucleosome can carry many marks at once, and **reader** proteins (bromodomains read acetyl-lysines; chromodomains read methyl-lysines) recruit downstream machinery accordingly. Histones are therefore not merely packaging — they are a layered, combinatorial language of regulation, and cancer frequently rewrites it.

### Histone modifications in cancer

The enzymes that write, erase, and read histone marks are mutated at high frequency in cancer. Bladder cancer is the extreme: roughly 80 percent carry mutations in chromatin-modifying genes [verify], including *ARID1A* (a SWI/SNF subunit), *KDM6A*, and *KMT2D*. Most are loss-of-function — the cell loses the ability to maintain a normal mark — and the consequence is a transcriptome shifted toward proliferation or de-differentiation.

Three patterns recur. **Gain-of-function in repressive complexes**: activating mutations in *EZH2* (the catalytic subunit of Polycomb Repressive Complex 2, which writes H3K27me3) deepen the silencing of target tumor suppressors in some lymphomas — and tazemetostat, an EZH2 inhibitor, was approved in 2020 for EZH2-mutant follicular lymphoma. **Loss-of-function in active marks**: *KMT2A* (MLL1), which writes H3K4me3, is rearranged in infant leukemias. **Chromatin-remodeler disruption**: the SWI/SNF complex, which uses ATP to reposition nucleosomes, is mutated in roughly 20 percent of all cancers.

Histone deacetylase (HDAC) inhibitors — vorinostat, romidepsin — were the second epigenetic drug class approved, hyperacetylating histones to reactivate silenced genes. Their clinical activity has been concentrated in blood cancers; solid tumors resist, partly because pan-HDAC inhibitors hit many targets and cause toxicity out of proportion to benefit.

### Metabolic–epigenetic coupling

A consequential subtlety: chromatin-modifying enzymes use small-molecule **metabolites** as cofactors, so the cell's metabolic state shapes its epigenetic state (Experimental & Molecular Medicine, 2023). S-adenosylmethionine is the methyl donor for all methyltransferases; α-ketoglutarate (αKG) is the cosubstrate for the TET DNA demethylases and Jumonji histone demethylases; acetyl-CoA supplies acetyl groups; NAD+ is required by sirtuin deacetylases.

The cleanest case is **IDH1/IDH2** mutation. Normally isocitrate dehydrogenase makes αKG; the cancer-associated mutation creates a neomorphic enzyme that instead makes **2-hydroxyglutarate (2HG)**, a structural mimic of αKG that *inhibits* the αKG-dependent demethylases. DNA and histone methylation accumulate aberrantly, tumor suppressors silence, and differentiation locks up. IDH mutations appear in ~70 percent of low-grade gliomas and ~10 percent of AML, and — remarkably — they are druggable: ivosidenib (IDH1) and enasidenib (IDH2) reduce 2HG, restore demethylase function, and allow differentiation to resume.

## Worked Example

**Situation.** A 60-year-old man is diagnosed with glioblastoma. Before deciding how aggressively to use temozolomide, his oncologist orders an *MGMT* promoter methylation test on the tumor. Why should a methyl mark predict whether a chemotherapy works?

**Process.** Temozolomide is an alkylating agent: it attaches a methyl group to the O6 position of guanine in tumor DNA. During replication, O6-methylguanine mispairs with thymine, introducing mutations that, if numerous, kill the cell.

The *MGMT* gene encodes a repair protein whose only job is to strip that methyl group off guanine — transferring it to its own cysteine residue and then being destroyed (one repair per molecule). So *MGMT* status sets the outcome: in a tumor expressing *MGMT*, the alkylation damage is repaired and the cell survives the drug; in a tumor with a *hypermethylated, silenced MGMT* promoter, the repair protein is absent, damage accumulates, and the cell dies.

*A dead end.* One might assume that *more* DNA repair always protects the patient — repair is good. Here the logic inverts: the tumor's repair capacity protects the *tumor*, not the patient. A patient whose tumor repairs efficiently benefits *less* from the drug. The naive "repair is protective" intuition predicts the wrong direction.

**Resolution.** The test returns *MGMT* promoter hypermethylation. This predicts a better response to temozolomide, and indeed methylated-*MGMT* patients survive significantly longer on temozolomide-based therapy than unmethylated ones (Stupp protocol). The methyl mark on one promoter — read by methylation-specific PCR or bisulfite sequencing — guides the treatment plan.

**The lesson.** A single epigenetic mark, by silencing one repair gene, can determine whether a specific drug works — epigenetic state, not just sequence, is clinically predictive.

**The limit.** This biomarker is specific to *MGMT* and alkylating agents; it does not generalize to other drugs, and methylation status is a probabilistic predictor, not a guarantee of response.

<!-- → [DIAGRAM: MGMT methylation decision tree — methylated promoter → silenced repair → temozolomide damage accumulates → cell death (drug works); unmethylated → MGMT expressed → damage repaired → cell survives (drug wasted)] -->

## Common Misconceptions

**"Epigenetic means weak, or not really biological."** The opposite. The *MGMT* mark in the opening case changes survival; IDH mutations silence whole differentiation programs through 2HG. Epigenetic marks are enzymatically written and faithfully inherited through division — they are as biologically consequential as mutations, just reversible in principle.

**"Histones are just packaging."** Histone tails carry a combinatorial code of marks that are written, erased, and read by specific enzymes and that determine whether genes are accessible. When SWI/SNF or EZH2 is mutated, the transcriptome shifts toward proliferation — a change in packaging that drives the disease, not a passive consequence of it.

**"Reversible means easy to fix."** Reversibility makes epigenetic marks attractive drug targets, but because the same enzymes act genome-wide, the effects are broad and context-dependent. DNMT and HDAC inhibitors reactivate many genes at once, work well in blood cancers, and disappoint in solid tumors with entrenched chromatin states — proof of principle and cautionary example at once.

## Exercises

1. **(Understand)** Explain in two or three sentences why a cancer can show *both* global hypomethylation and focal hypermethylation at the same time, and state how each contributes to the cancer phenotype.

2. **(Apply)** A sporadic ovarian cancer has wild-type *BRCA1* sequence but no BRCA1 protein. Propose an epigenetic explanation, and predict whether this tumor might respond to a PARP inhibitor (recall Chapter 6). State what evidence you would need to confirm your prediction.

3. **(Apply / Produce)** Construct a writer/eraser/reader table for these marks: H3K4me3, H3K9me3, H3K27me3, H3K27ac. For each, name the writer enzyme class, the eraser class, an example reader domain, and whether the mark generally indicates active or repressed transcription.

4. **(Analyze)** Trace the IDH→2HG→demethylase chain and explain why an IDH inhibitor *reverses* an epigenetic phenotype even though IDH is a metabolic enzyme, not a chromatin enzyme. Classify each link in the chain as established mechanism or therapeutic implication.

## What Would Change My Mind

The chapter's central claim is that epigenetic dysregulation is a genuine driver of cancer — capable of silencing tumor suppressors and altering phenotype without any sequence change — and that it is, at least sometimes, pharmacologically reversible. Findings that would force revision: convincing evidence that the canonical epigenetic abnormalities (CpG-island hypermethylation of tumor suppressors, IDH-driven hypermethylation) are consistently *downstream consequences* of mutations rather than independent drivers, or that demethylating and IDH-inhibiting drugs produce no durable reactivation of silenced genes and no phenotypic reversal in well-controlled trials. The IDH-inhibitor response — tumors regressing and differentiation resuming as 2HG falls — is the strongest causal evidence; a robust failure to replicate it would undercut the "reversible driver" framing.

## Still Puzzling

- Why do demethylating and HDAC-inhibiting drugs work in blood cancers but largely fail in solid tumors? Is the difference the chromatin state, the microenvironment, drug delivery, or all three?
- Global hypomethylation and focal hypermethylation coexist in the same tumor through different machinery — but is one of them the initiating event, or do they arise independently? Does the order matter for therapy?
- If a tumor suppressor can be silenced by methylation *or* by mutation with the same functional result, what determines which route a given cancer takes in a given tissue? This question carries forward into Chapter 8's account of reprogramming and plasticity.

## References

- Signal Transduction and Targeted Therapy. *Epigenetic regulation in the tumor microenvironment.* 2023. https://www.nature.com/articles/s41392-023-01480-x
- Experimental & Molecular Medicine. *Metabolic reprogramming and epigenetic modifications in cancer.* 2023. https://www.nature.com/articles/s12276-023-01020-1
- National Cancer Institute. *What Is Cancer?* https://www.cancer.gov/about-cancer/understanding/what-is-cancer
- Hanahan, D. *Hallmarks of Cancer: New Dimensions.* Cancer Discovery, 2022. https://aacrjournals.org/cancerdiscovery/article/12/1/31/675608
- NCBI Bookshelf. *Molecular Biology of the Cell.* https://www.ncbi.nlm.nih.gov/sites/books/n/mboc4/

## Prompts

*No figures have been generated for this chapter yet.*
