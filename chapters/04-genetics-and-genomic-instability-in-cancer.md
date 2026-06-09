# Genetics and Genomic Instability in Cancer

## Learning Objectives

By the end of this chapter you should be able to:

- **Distinguish** the major classes of mutation (point, indel, copy-number, translocation, structural, epigenetic) and the gene categories they affect (oncogenes, tumor suppressors, DNA-repair genes).
- **Apply** the driver/passenger distinction to interpret a tumor's mutation list.
- **Explain** Knudson's two-hit hypothesis and reconcile why tumor-suppressor predisposition is dominant at the family level but recessive at the cellular level.
- **Analyze** how DNA-repair failure produces genomic instability, and connect a specific repair defect to a diagnostic biomarker or a therapeutic vulnerability.

## Opening Case

A sequencing report lands on an oncologist's desk for a patient with metastatic colorectal cancer. It lists 187 mutations. The patient's family, reading it later, asks the natural question: which of these 187 caused the cancer, and did the patient inherit them?

Both halves of that question rest on a misunderstanding the report itself invites. The 187 mutations are not 187 causes. The overwhelming majority are **passengers** — incidental changes the cell accumulated while it was evolving, selecting for nothing. A small handful — here, an *APC* truncation, a *KRAS* G12D, and a *TP53* loss — are **drivers**, the changes that actually gave this lineage its growth advantage. And almost all 187 are **somatic** — acquired in the tumor over years, present in no other cell of the body, inheritable by no one. The report looks like an indictment of the genome. It is really a fossil record of a Darwinian process that ran inside one tissue for a decade or more.

To read it correctly you need the framework this chapter builds: how mutations arise, which kinds matter, how to tell a driver from a passenger, why some predispositions run in families (Knudson's math), and why the cell's DNA-repair machinery — when it fails — is itself one of the deepest engines of cancer.

## Core Concepts

The chapter's organizing sentence: **cancer is a sequence of mutations selected for in a clonal lineage** — evolution, in real time, inside the body, over decades. Bert Vogelstein's colorectal model was the founding demonstration: biopsying the same lineage at successive stages (normal mucosa → small adenoma → large adenoma → carcinoma), his group read out which mutations appeared at which stage — *APC* first, then *KRAS*, then loss of chromosome 18q, then *TP53* — each conferring a step-change advantage (NCBI Bookshelf, *Development and Causes of Cancer*).

### DNA and the source of mutations

A human cell holds about two meters of DNA — roughly 3 billion base pairs across 46 chromosomes — replicated each S phase by **DNA polymerase**, which reads each parent strand and builds a complement (NCBI Bookshelf, *Molecular Biology of the Cell*). Fidelity is extraordinary: polymerase errs at about 1 in 10⁵, proofreads its own work down to ~1 in 10⁷, and **mismatch repair** afterward brings the final rate to about 1 in 10⁹ — roughly three uncaught errors per division across the genome. Most are silent or neutral. The rare error in the wrong codon of the wrong gene is the substrate cancer evolves from.

### Kinds of mutation

A **point mutation** changes one base. *Missense* changes one amino acid; *nonsense* creates a premature stop, truncating the protein; *silent* changes the DNA but not the protein; *splice-site* disrupts mRNA processing. An **insertion/deletion (indel)** adds or removes bases; if not a multiple of three it causes a *frameshift*, usually producing a truncated, dead protein. A **copy-number variation (CNV)** gains or loses large regions: *amplification* boosts oncogenes (*MYC* in neuroblastoma, *HER2* in breast cancer, *EGFR* in glioblastoma); *deletion* removes tumor suppressors (*CDKN2A* at 9p21). A **chromosomal translocation** joins segments of two chromosomes — the **Philadelphia chromosome**, t(9;22), fuses *BCR* and *ABL1* into a constitutively active tyrosine kinase that drives chronic myeloid leukemia; identified by Nowell and Hungerford in 1960, it later became the target of imatinib, the first truly targeted cancer drug. Other translocations hijack regulatory elements: t(8;14) places *MYC* under immunoglobulin enhancers in Burkitt lymphoma; t(14;18) does the same for *BCL2* in follicular lymphoma. **Structural variants** include *chromothripsis* — a chromosome shattered and reassembled imperfectly, possibly in one catastrophic event. **Epigenetic changes** (DNA methylation, histone modification) alter gene expression without changing sequence and are heritable through divisions; cancers commonly hypermethylate tumor-suppressor promoters to silence them. Chapter 7 develops the epigenetic half.

### Drivers and passengers, and three gene categories

A typical solid tumor carries tens to hundreds of coding mutations, but only **2 to 8 drivers** — the ones conferring selective advantage (NCI, *The Genetics of Cancer*). The rest are **passengers**. Several clues distinguish them: drivers recur across independent patients (recurrence implies selection), land in functionally critical protein regions, and produce specific gain- or loss-of-function changes; passengers are scattered and tumor-unique. The catalogues — COSMIC, The Cancer Genome Atlas — map recurrent drivers across cancer types.

Three functional gene categories matter:

- **Oncogenes** are normal genes whose hyperactivation drives proliferation. Their cancer mutations are **dominant gain-of-function**: a single mutated copy suffices. *KRAS* G12D — one mutant allele locking RAS active — is canonical. *TP53* is mutated in roughly half of cancers; *KRAS* in about 30% (90% of pancreatic, 50% of colorectal, 25% of lung adenocarcinomas). Chapter 5 develops oncogenes.
- **Tumor suppressors** are normal genes whose function restrains proliferation or triggers death. Their cancer mutations are **recessive loss-of-function**: both copies must be inactivated. *TP53*, *RB1*, *APC*, *PTEN*, *BRCA1/2*. Chapter 6 develops them.
- **DNA-repair genes** are technically tumor suppressors, but act one step removed: losing them does not directly drive proliferation, it lets *other* mutations accumulate faster. Mismatch-repair genes (*MLH1*, *MSH2*, *MSH6*, *PMS2*) and homologous-recombination genes (*BRCA1*, *BRCA2*, *PALB2*) sit here.

### Knudson's two-hit hypothesis

Alfred Knudson's 1971 retinoblastoma analysis is the clearest cancer math ever written (Knudson, 1971; reviewed in Hino, 2017). Retinoblastoma is sporadic in ~60% of cases (usually one eye, slightly later) and familial in ~40% (often both eyes, earlier). Knudson reasoned that the cancer requires *two* hits in the same cell. In sporadic cases, both hits must occur de novo in one retinal cell — the probability of a rare event *squared*, hence slow and usually unilateral. In familial cases, the child inherits one hit already present in every retinal cell, so only a single second hit is needed — faster (earlier onset) and likely in both eyes (independent second hits across millions of cells). The model fit the age and laterality data quantitatively, *before any molecular evidence existed*, predicting that both copies of one gene must be lost. Sixteen years later *RB1* was cloned and the prediction held: every tumor carried two inactivated *RB1* alleles — one germline plus one somatic in familial cases, both somatic in sporadic cases.

This resolves the apparent paradox students stumble on: the predisposition is **dominant at the family level** (inheriting one defective allele dramatically raises risk and is passed down) but **recessive at the cellular level** (the cell behaves normally until *both* alleles are gone). A germline carrier already has the first hit in every cell — one somatic event from cancer — which is the entire justification for early, aggressive screening of carriers of *BRCA1/2*, *RB1*, *APC*, *TP53*, *VHL*, and Lynch-syndrome genes. (One nuance: *PTEN* shows *haploinsufficiency* — even one lost allele can matter in some contexts — so the two-hit rule is a strong default, not an absolute law.)

<!-- → [DIAGRAM: two-hit hypothesis — sporadic (two somatic hits, unilateral, later) vs. familial (one germline + one somatic hit, bilateral, earlier), with the probability logic annotated] -->

### DNA repair and genomic instability

Cells suffer tens of thousands of DNA lesions per day from metabolism and exposure; without repair the genome would degrade within days (Alberts et al., *MBoC*). Specialized pathways handle different damage. **Base excision repair (BER)** fixes small single-base modifications. **Nucleotide excision repair (NER)** removes bulky helix-distorting lesions like UV thymine dimers; inherited NER defects cause *xeroderma pigmentosum*, with severe UV sensitivity and childhood skin cancers. **Mismatch repair (MMR)** corrects errors that escape proofreading; inherited MMR defects cause **Lynch syndrome**, and Lynch tumors show **microsatellite instability** — variable repeat lengths — which is a diagnostic biomarker. **Double-strand break repair** uses either **homologous recombination (HR)** — high-fidelity, template-based, requiring RAD51, BRCA1, BRCA2, PALB2 — or **non-homologous end joining (NHEJ)** — faster but error-prone. The 2015 Nobel Prize in Chemistry honored Lindahl (BER), Modrich (MMR), and Sancar (NER) for characterizing these systems.

Inherited HR defects in *BRCA1/2* cause hereditary breast and ovarian cancer: with HR down, breaks are repaired by error-prone routes, accumulating rearrangements. This is also exploited therapeutically through **synthetic lethality**. PARP inhibitors block single-strand-break repair; the resulting lesions become double-strand breaks during replication. HR-competent cells repair them; *BRCA*-mutant cells cannot, and die. Chapter 19 develops synthetic lethality.

Hanahan and Weinberg classed **genomic instability** as an *enabling characteristic*, not a hallmark in itself — a condition that lets the hallmarks be acquired (Hanahan, 2022). The logic is direct: a normal cell mutates ~3 errors per division, making acquisition of 5–10 drivers slow; a cell that has lost a repair pathway or a mitotic checkpoint mutates 10–100× faster, vastly raising the odds it assembles the needed drivers in a human lifetime. This is Loeb's **mutator phenotype** hypothesis. Theodor Boveri anticipated the chromosome-level version in 1914, proposing that abnormal chromosome segregation produces abnormal cells — largely ignored for fifty years, then vindicated: roughly 90% of solid tumors carry chromosomal abnormalities (**aneuploidy**), which perturbs thousands of genes at once. Telomere shortening (the Hayflick limit) drives a pre-cancer "crisis" of chromosome fusions and breaks; cells that emerge with telomerase reactivated and stable chromosomes go on to become cancer.

A counterintuitive payoff: high mutation burden can be therapeutically *useful*. Tumors with many mutations produce many **neoantigens** the immune system can recognize, so microsatellite-instability-high colorectal cancer responds far better to immune checkpoint inhibitors than microsatellite-stable disease — even though it is genetically "worse" (Chapter 18). The same instability that drove the tumor makes it visible to the immune system.

## Worked Example

**Situation.** Interpret the opening-case report: 187 mutations, including *APC* (frameshift truncation), *KRAS* G12D, *TP53* (nonsense), a 9p21 deletion spanning *CDKN2A*, and high microsatellite instability (MSI-high). Which are drivers, what gene categories are they, and what does this report imply for therapy?

**Analytical process.** A first wrong move: rank mutations by how damaging each looks in isolation — a nonsense mutation "looks worse" than a missense one, so call *TP53* the main driver and stop. That conflates molecular severity with selective role and ignores recurrence and gene function.

Sort by function instead. *APC* frameshift → tumor suppressor, loss-of-function, recurrent first hit in colorectal cancer: a driver. *KRAS* G12D → oncogene, recurrent activating point mutation, single allele sufficient: a driver. *TP53* nonsense → tumor suppressor, loss-of-function: a driver. The 9p21/*CDKN2A* deletion → copy-number loss of a tumor suppressor: plausibly a driver. That is four drivers in the recognizable colorectal sequence — the rest of the 187 are overwhelmingly passengers.

Now the MSI-high finding reframes everything. MSI-high means mismatch repair has failed — which both *explains* the unusually high mutation count (a hypermutator phenotype, far more than the usual tens) and predicts the family-screening question: MSI can be sporadic (usually *MLH1* promoter methylation) or germline (Lynch syndrome), so this triggers genetic testing of the patient and relatives. Critically, MSI-high also predicts strong response to immune checkpoint inhibitors, because the high mutation burden generates abundant neoantigens.

**Resolution.** The report describes ~4 drivers riding atop ~180 passengers; the standout actionable feature is not any single driver but the *mismatch-repair failure*, which simultaneously explains the mutation count, flags possible Lynch syndrome, and predicts immunotherapy benefit.

**The lesson.** A long mutation list is read by *function and recurrence*, not length or per-mutation severity — and the most clinically decisive finding can be a repair-pathway failure rather than any individual driver.

**The limit.** Driver/passenger assignment is probabilistic. Rare or private drivers exist that recurrence catalogues miss, and a "passenger" in one context can be a driver in another tissue — the categories are well-supported defaults, not certainties.

## Common Misconceptions

**"Every mutation in a cancer gene list caused the cancer."** Most are passengers. The opening-case report's 187 mutations contain only a handful of drivers; treating the list as 187 causes both overstates the genome's guilt and obscures the few changes that actually matter and might be targetable.

**"Mutation rate and selection are separate topics."** They are coupled. Genomic instability raises the *supply* of variants; selection acts on that supply. A repair defect like the MSI-high finding does not directly drive growth — it speeds the appearance of the drivers that do. Mutation and selection are two halves of one evolutionary process.

**"Autosomal-dominant inheritance and two-hit cellular recessivity contradict each other."** They do not. Knudson's model reconciles them: the inherited single hit is dominant at the *family* level (it is passed down and raises risk), while at the *cellular* level the gene is recessive (the cell needs both copies lost to misbehave). The familial carrier simply starts one hit ahead in every cell.

**"More mutations always means a worse, less treatable cancer."** Genetically worse, sometimes — but a high mutation burden produces neoantigens that make the tumor *more* visible to the immune system, which is why MSI-high tumors respond better to checkpoint inhibitors. The biology gives and takes at once.

## Exercises

1. **(Understand.)** For each, name the mutation class and the gene category most associated with it: (a) *KRAS* G12D; (b) *BRCA1* frameshift; (c) *HER2* amplification; (d) t(9;22) *BCR-ABL1*; (e) *MLH1* promoter hypermethylation.

2. **(Apply.)** Given a tumor with mutations in *APC*, *KRAS*, *TP53*, and 50 scattered missense changes unique to this patient, identify the likely drivers versus passengers and justify each call using recurrence and gene function.

3. **(Analyze/Produce.)** Work Knudson's logic numerically: explain qualitatively why familial retinoblastoma onset is earlier and more often bilateral than sporadic, in terms of the probability of one event versus two. Then draw a two-hit diagram contrasting a germline carrier with a non-carrier, marking where each "hit" occurs.

4. **(Apply.)** A patient's tumor is HR-deficient (*BRCA2* loss). Explain, step by step, why a PARP inhibitor selectively kills the tumor cells but spares normal cells, naming the synthetic-lethal relationship. Then predict one way the tumor might become resistant.

## What Would Change My Mind

The chapter's central claim is that cancer is clonal evolution: drivers selected over time within a lineage, with genomic instability as the enabling accelerant. The strongest finding that would force revision: a common cancer type shown to arise *fully formed* from a single, non-clonal, non-selective event with no preceding driver accumulation and no detectable instability — a tumor that is not the product of sequential selection at all. Chromothripsis hints that some changes happen in one burst, but those still feed a subsequent selective process. A reproducible cancer that skips clonal evolution entirely — same drivers, same instability, but assembled instantaneously and without selection — would mean the evolutionary frame is one route among several rather than the unifying one.

## Still Puzzling

- How many drivers does a given cancer actually *need*, and why does the number vary so widely (a single fusion in some leukemias, many in some carcinomas)?
- Is aneuploidy mostly a *cause* of cancer progression or mostly a *consequence* — and can the same massive chromosomal reshuffling be tolerated by tumor cells that would kill a normal cell? The directionality is still argued.
- For the ~10–15% of cancers maintaining telomeres without telomerase (the ALT pathway), why does that route get selected, and can it be targeted the way telomerase can?

## References

- NCI. *The Genetics of Cancer.* https://www.cancer.gov/about-cancer/causes-prevention/genetics
- NCI. *What Is Cancer?* https://www.cancer.gov/about-cancer/understanding/what-is-cancer
- Knudson, A. G. (1971). Mutation and Cancer: Statistical Study of Retinoblastoma. *PNAS* 68, 820–823.
- Hino, O., & Kobayashi, T. (2017). The two-hit hypothesis. *Cancer Science.* https://onlinelibrary.wiley.com/doi/10.1111/cas.13116
- NCBI Bookshelf. *The Development and Causes of Cancer.* https://www.ncbi.nlm.nih.gov/books/NBK9963/
- NCBI Bookshelf. *Molecular Biology of the Cell.* https://www.ncbi.nlm.nih.gov/sites/books/n/mboc4/
- Hanahan, D. (2022). Hallmarks of Cancer: New Dimensions. *Cancer Discovery* 12, 31–46. https://aacrjournals.org/cancerdiscovery/article/12/1/31/675608

---

## Prompts

*No figures have been generated for this chapter yet.*
