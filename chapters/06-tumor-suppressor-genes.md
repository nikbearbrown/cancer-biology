# Tumor Suppressor Genes

## Learning Objectives

By the end of this chapter, you should be able to:

- **Explain** the loss-of-function logic of tumor suppressor genes and **contrast** it with the gain-of-function logic of oncogenes (Chapter 5), including why two hits are usually required.
- **Distinguish** gatekeepers from caretakers, and **classify** TP53, RB1, BRCA1/2, APC, and PTEN by what cellular function their loss removes.
- **Trace** how DNA damage activates p53 and how p53's downstream choices (arrest, repair, senescence, apoptosis) protect the genome.
- **Describe** how tumor suppressors are inactivated — point mutation, loss of heterozygosity, deletion, promoter hypermethylation, viral degradation.
- **Apply** the principle of synthetic lethality to explain why BRCA-mutant cancers are vulnerable to PARP inhibitors.

## Opening Case

A 33-year-old woman has no symptoms but a heavy family history: a mother who died of ovarian cancer at 48, a maternal aunt with breast cancer at 41, a grandmother with breast cancer. Genetic testing finds a pathogenic variant in *BRCA1*. She is healthy. Every cell in her body carries this variant — inherited from her mother — but she does not have cancer.

What she has is one broken copy of a gene whose normal job is to repair a specific kind of DNA damage accurately. The other copy still works, and as long as it does, her cells repair damage correctly. Her elevated risk — a lifetime breast cancer risk of roughly 65–80 percent and ovarian risk of about 40–60 percent — comes from the probability that, somewhere in her breast or ovarian tissue over decades, a single cell will lose its remaining good copy (NCI, *The Genetics of Cancer*) [verify — exact percentages]. In that one cell, the brake fails completely, accurate repair collapses, and mutations begin to accumulate.

This is the inverted logic of tumor suppressor genes. Where oncogenes are accelerators stuck on, tumor suppressors are brakes that must be broken — usually both copies — before the cell runs free. This chapter is about those brakes, how they are lost, and how, paradoxically, their loss can become a therapeutic target.

## Core Concepts

### Loss-of-function genetics and the two-hit rule

Cancer needs two things: an accelerator that is stuck and a brake that is broken. Chapter 5 covered the accelerators. **Tumor suppressor genes** are the brakes — genes whose normal protein products restrain proliferation, repair DNA, maintain genome integrity, or trigger cell death when damage is severe. When they work, they hold cancer at bay; when they fail, cells that should stop do not, and cells that should die survive.

The genetics are inverted relative to oncogenes. Oncogenes are dominant: one mutated allele is enough. Tumor suppressors are typically **recessive at the cellular level** — both functional copies must be inactivated for the brake to fail. This is the **two-hit hypothesis**, reasoned out statistically by Alfred Knudson from the age distribution of retinoblastoma well before the molecular biology was known (Hino, 2017). Inherited retinoblastoma patients carry one defective *RB1* allele in every cell from birth (the first hit) and develop tumors early and often in both eyes, because losing the second copy in any of thousands of retinal cells is nearly certain. Sporadic cases need both hits in the same cell and are rarer and later.

This is why tumor suppressors were harder to find than oncogenes. You cannot identify one by transfecting it into a normal cell and watching for transformation — adding a working brake suppresses cancer rather than causing it. The first proof came from cell-fusion experiments (Harris, 1969): fusing a cancer cell with a normal cell produced hybrids that *could not* form tumors, showing that the normal cell carried something dominant that suppressed the cancer phenotype. *RB1* was the first tumor suppressor cloned (1986); restoring it to retinoblastoma cells suppressed their tumorigenicity — the gold-standard rescue test.

### Gatekeepers and caretakers

Tumor suppressors fall into two functional classes, and the distinction matters because it predicts how their loss promotes cancer.

A **gatekeeper** directly restrains growth or promotes death in a tissue. *RB1* gates entry into S phase; *APC* restrains Wnt signaling in the gut. Lose a gatekeeper and the cell divides when it should not.

A **caretaker** maintains genome integrity. *BRCA1/2* enable accurate repair of DNA double-strand breaks; the mismatch-repair genes correct replication errors. Losing a caretaker does not directly push the cell to divide — it raises the *supply* of mutations, accelerating the accumulation of changes that eventually hit gatekeepers and oncogenes (NCI, *The Genetics of Cancer*).

A common error is to reduce all tumor suppressors to "brakes on division." *BRCA1* loss does not push a cell to divide; it weakens homologous recombination repair. Some genes blur the categories: *TP53* integrates damage signals and acts as both gatekeeper (triggering arrest and death) and, indirectly, caretaker (mobilizing repair).

<!-- → [DIAGRAM: two-column comparison — gatekeepers (RB1, APC: restrain growth/death directly) vs caretakers (BRCA1/2, MMR: maintain genome, raise mutation supply), with TP53 spanning both columns] -->

### TP53: the decision hub

*TP53* is the most frequently mutated gene in human cancer — altered in roughly half of all tumors, and in over 90 percent of some (high-grade serous ovarian, head and neck squamous) [verify]. It is called *the guardian of the genome* (Lane, 1992), but the phrase hides the mechanism, so trace it.

The protein, p53, is a transcription factor. In healthy cells it is kept at low levels by **MDM2**, an E3 ubiquitin ligase that constantly tags it for degradation. When the cell experiences stress — DNA damage, oncogene activation, hypoxia — sensor kinases (ATM, ATR, CHK1, CHK2) phosphorylate p53 so MDM2 can no longer bind. p53 accumulates and turns on genes that enact a decision:

- *Arrest.* p53 transcribes *CDKN1A* (p21), which inhibits cyclin-CDK complexes and halts the cycle at G1/S so the cell can repair (NCBI Bookshelf, *The Cell Cycle and Programmed Cell Death*).
- *Repair.* p53 activates repair components (GADD45, XPC, DDB2).
- *Senescence.* In some contexts p53 drives a permanent non-dividing state.
- *Apoptosis.* If damage is too severe, p53 transcribes pro-apoptotic genes (PUMA, NOXA, BAX), and the cell dies rather than copy its damage forward.

Lose p53 and the cell loses all of these options at once. It can sustain DNA damage that should have killed it and keep dividing, copying the damage into daughter cells. *TP53* mutations are unusual among tumor suppressors: most are **missense** substitutions in the DNA-binding domain (hot spots R175, R248, R273), not truncations, and many act as **dominant-negative** — because p53 works as a tetramer, mutant subunits poison wild-type ones. Some mutants even gain new oncogenic functions. *Li-Fraumeni syndrome*, inherited *TP53* deficiency, produces multiple primary cancers from childhood, demonstrating how essential p53 is across tissues.

### RB1: the G1/S gate

The *RB1* protein (Rb) controls the gate into DNA replication. In its unphosphorylated state, Rb binds and inhibits the transcription factor **E2F**, which would otherwise turn on the genes needed for S phase. Growth signals activate cyclin D–CDK4/6 complexes, which phosphorylate Rb; phosphorylated Rb releases E2F, and the cell enters S phase (International Journal of Molecular Sciences, 2021). Lose *RB1* and the gate is permanently open — E2F is always free.

This connects to therapy from two directions. Lose Rb and CDK4/6 inhibitors (palbociclib, ribociclib, abemaciclib) have no target to act through; keep Rb intact and these drugs hold the cell in G1 — which is why they work in hormone-receptor-positive breast cancer that retains Rb. Some DNA tumor viruses attack the same gate: human papillomavirus E7 binds and degrades Rb, functionally inactivating it without mutating the gene.

### APC and PTEN: two more functional classes

Two other tumor suppressors round out the functional logic. *APC* is the colorectal-cancer gene — inactivated in roughly 80 percent of colorectal cancers and typically the *earliest* event, appearing in small polyps before other mutations. APC is a scaffold in the **Wnt pathway**: in the absence of a Wnt signal, APC helps form a destruction complex that degrades the transcription factor β-catenin, keeping its level low. Lose APC and the destruction complex fails, β-catenin accumulates and drives proliferation genes (including *MYC* and cyclin D1) regardless of upstream signal — the pathway is permanently on. The inherited form, familial adenomatous polyposis, produces hundreds of polyps and near-certain colorectal cancer without prophylactic surgery, illustrating the gatekeeper logic in a renewing tissue (NCI, *The Genetics of Cancer*).

*PTEN* is a phosphatase that opposes the PI3K pathway — the second most commonly mutated tumor suppressor after *TP53*. PI3K signaling drives growth and survival via AKT; PTEN is the off switch that dephosphorylates the lipid second messenger PIP3 back to PIP2. Lose PTEN and the pathway fires constitutively. *PTEN* is unusual because it is **haploinsufficient**: even partial loss (one allele, or reduced expression) perturbs the pathway, making PTEN a partial exception to the two-hit rule and helping explain why its loss is so common. This is the boundary case students should hold — most tumor suppressors require complete biallelic loss, but not all.

### How tumor suppressors are inactivated

Because the goal is to *lose* function from both copies, tumor suppressors are silenced by several mechanisms beyond simple point mutation. **Loss of heterozygosity (LOH)** is the classic second hit: a cell with one mutated allele loses the wild-type allele through chromosomal deletion, mitotic recombination, or whole-chromosome loss. **Large deletions** can remove a gene entirely (*CDKN2A* at 9p21 is frequently deleted). **Promoter hypermethylation** is the epigenetic equivalent of mutation — a CpG island in the promoter is chemically silenced without any sequence change, as happens to *MLH1* in sporadic microsatellite-unstable colorectal cancers (this connects directly to Chapter 7). **Viral inactivation** removes the protein rather than the gene: HPV E6 degrades p53 and E7 degrades Rb, so HPV-driven cancers functionally lose both tumor suppressors while the genes themselves remain wild-type.

## Worked Example

**Situation.** A 47-year-old woman with a *BRCA1* germline mutation develops high-grade serous ovarian cancer. Her oncologist proposes a PARP inhibitor. Why should a drug against an unrelated repair enzyme kill cells defined by a *BRCA1* defect?

**Process.** Start with normal repair. A double-strand break — both DNA strands severed — is the most dangerous lesion. Cells repair it accurately by **homologous recombination (HR)**, using the sister chromatid as a template; HR requires BRCA1, BRCA2, RAD51, and others. Separately, **PARP1** is an enzyme that repairs single-strand breaks. The cancer cells have lost BRCA1 (germline hit plus loss of the second allele), so HR is broken; they survive by leaning on other repair pathways.

Now give a PARP inhibitor. Single-strand breaks go unrepaired. When a replication fork hits an unrepaired single-strand break, it collapses into a double-strand break. A normal cell repairs that double-strand break by HR and survives. A BRCA1-deficient cell cannot — HR is gone — so the breaks accumulate and the cell dies.

*A dead end.* One might expect a DNA-repair inhibitor to be broadly toxic, harming all dividing cells. It is not selectively lethal to normal tissue, because normal cells retain BRCA function and repair the resulting double-strand breaks. The selectivity comes from the *combination*, not the drug alone.

**Resolution.** This is **synthetic lethality**: two defects, each survivable alone, lethal together. BRCA loss alone is tolerable for the cancer cell; PARP inhibition alone is tolerable for normal cells; both together kill only the BRCA-deficient cancer. Olaparib, the first PARP inhibitor, was approved for BRCA-mutant ovarian cancer and later for BRCA-mutant breast, pancreatic, and prostate cancers.

**The lesson.** Tumor suppressor loss cannot be reversed with a drug, but the dependency it creates can be exploited — the target is not the missing gene but whatever the cell now needs *because* the gene is missing.

**The limit.** Resistance emerges, most often by *reversion mutations* that restore the BRCA reading frame; and the strategy applies only to cancers with a genuine HR defect, not to BRCA-intact tumors.

<!-- → [DIAGRAM: synthetic lethality grid — four cells (BRCA+/PARP active = live, BRCA+/PARP inhibited = live, BRCA-/PARP active = live, BRCA-/PARP inhibited = dead)] -->

## Common Misconceptions

**"Tumor suppressors are all just brakes on cell division."** This misses the caretakers. *BRCA1/2* do not restrain division — they enable accurate double-strand-break repair (homologous recombination). The opening-case patient's risk comes from failed repair raising her mutation supply over decades, not from a released brake on her cell cycle.

**"All tumor suppressors work in the same pathway."** They cover different functions: RB1 gates S-phase entry, APC controls Wnt signaling, PTEN opposes PI3K, BRCA1/2 repair DNA, TP53 integrates stress signals. Treating them as one pathway predicts the wrong vulnerabilities — PARP inhibitors exploit HR-defective cancers specifically, not tumor suppressor loss in general.

**"'Guardian of the genome' is the explanation for what p53 does."** The phrase is a label, not a mechanism. p53 guards by accumulating under stress and then *choosing* among arrest, repair, senescence, and apoptosis through specific transcriptional targets. Without the decision logic, you cannot predict why losing p53 lets a damaged cell keep dividing — the actual cause of its danger.

## Exercises

1. **(Understand)** State the two-hit hypothesis in one sentence, then explain why inherited retinoblastoma appears earlier and more often bilateral than sporadic retinoblastoma.

2. **(Apply)** A sporadic colorectal cancer is found to have silenced *MLH1* by promoter hypermethylation rather than mutation. Explain why this produces a Lynch-syndrome-like phenotype (microsatellite instability, hypermutation) even though no gene sequence has changed, and classify *MLH1* as a gatekeeper or caretaker.

3. **(Apply / Produce)** Build a mechanism map for *APC* loss in colorectal cancer with the boxes *normal Wnt regulation → APC inactivation → β-catenin behavior → cellular phenotype → therapeutic challenge*. Then add one sentence on why restoring the brake pharmacologically has been difficult.

4. **(Analyze)** A claim states: "Because PARP inhibitors exploit a DNA-repair defect, they should work in any cancer with a high mutation burden." Identify what is wrong with this overgeneralization and repair it into a correct, bounded statement.

## What Would Change My Mind

The chapter's central claim is that most tumor suppressors follow loss-of-function, two-hit logic — both alleles must be inactivated for the brake to fail. Findings that would force revision: convincing evidence that single-allele loss is routinely sufficient to drive cancer across many tumor suppressors (not just the known haploinsufficient exception, *PTEN*), or that restoring a single working allele fails to suppress tumorigenicity in the gene-transfer rescue experiments that defined the category. The rescue experiments are load-bearing; a robust failure to reverse the cancer phenotype by reintroducing a wild-type tumor suppressor would undermine the loss-of-function model.

## Still Puzzling

- Why is *PTEN* haploinsufficient — dose-sensitive, so that partial loss matters — when most tumor suppressors require complete biallelic loss? What determines whether a brake fails gradually or only when fully removed?
- Why are *TP53* mutations overwhelmingly missense (dominant-negative) when most other tumor suppressors are inactivated by truncation? Does the tetramer architecture fully explain this, or is gain-of-function selection driving it?
- Promoter hypermethylation silences tumor suppressors without changing sequence, and is in principle reversible. Why have demethylating drugs worked well in blood cancers but poorly in solid tumors? This question opens directly into Chapters 7 and 8 on cancer epigenetics.

## References

- National Cancer Institute. *The Genetics of Cancer.* https://www.cancer.gov/about-cancer/causes-prevention/genetics
- Hino, O., et al. *The two-hit hypothesis, the driver of cancer.* Cancer Science, 2017. https://onlinelibrary.wiley.com/doi/10.1111/cas.13116
- NCBI Bookshelf. *The Development and Causes of Cancer.* https://www.ncbi.nlm.nih.gov/books/NBK9963/
- NCBI Bookshelf. *The Cell Cycle and Programmed Cell Death.* https://www.ncbi.nlm.nih.gov/books/NBK21056/
- International Journal of Molecular Sciences. *Cyclin-Dependent Kinases and Their Regulation in Cancer.* 2021. https://www.mdpi.com/1422-0067/22/6/2935

## Prompts

*No figures have been generated for this chapter yet.*
