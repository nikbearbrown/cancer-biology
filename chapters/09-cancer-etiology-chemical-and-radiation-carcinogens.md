# Cancer Etiology: Chemical and Radiation Carcinogens

## Learning Objectives

By the end of this chapter, you should be able to:

- **Explain** how chemical carcinogens that require metabolic activation are converted into DNA-reactive intermediates, and **trace** the path from adduct to mutation to cancer phenotype.
- **Distinguish** the mechanisms of ionizing radiation, ultraviolet radiation, and genotoxic chemicals, and **predict** which kind of DNA damage each produces.
- **Apply** the initiation–promotion–progression framework to explain why a single carcinogen exposure rarely produces immediate cancer.
- **Interpret** an IARC hazard classification correctly, distinguishing carcinogenic hazard from personal risk.
- **Construct** a mechanism map linking a named exposure to a mutational signature, a tumor type, and a public-health intervention.

## Opening Case

A 58-year-old man who smoked about a pack of cigarettes a day for thirty-five years is diagnosed with lung adenocarcinoma. His oncologist orders tumor sequencing. When the report comes back, the *TP53* gene — the most frequently mutated gene in human cancer — carries a guanine-to-thymine change at a familiar position. Across the tumor genome, the same kind of change recurs: G→T, again and again, concentrated at particular sequence contexts.

That pattern is not random. It is a fingerprint. Decades earlier, a molecule from cigarette smoke entered this man's airway cells, was chemically altered by his own enzymes into something reactive, and bound covalently to the DNA. When the cell next copied that DNA, the damaged base was misread. The wrong nucleotide was inserted opposite it. One letter changed. That single substitution, repeated in the right gene in the right cell over thirty-five years of continued exposure, is how the disease began.

The puzzle this chapter solves is mechanistic. *How* does a molecule from smoke change a DNA letter? *How* does a photon of sunlight do something different to a skin cell? And *how* do we know — from the genome of a tumor diagnosed today — what exposure caused it decades ago?

## Core Concepts

A **carcinogen** is any agent that increases the incidence of cancer in an exposed population. The agent may be a chemical, a form of radiation, an infection, or a behavior. This chapter covers the non-biological carcinogens: chemicals and radiation, which damage DNA directly through chemistry or physics. (The biological carcinogens — viruses and bacteria — are covered in the next chapter, because they act indirectly.)

The unifying idea is simple. Most cancer-causing chemicals and radiation share one endpoint: they introduce a **mutation** — a heritable change in the DNA sequence. If that mutation lands in a gene that controls growth, survival, or genome maintenance, the affected cell gains a small selective advantage, and a clonal lineage begins its slow march toward malignancy (NCBI Bookshelf, *The Development and Causes of Cancer*).

### Chemical carcinogenesis and metabolic activation

Most chemical carcinogens are not themselves reactive. They are **procarcinogens** — inert molecules that the cell must first chemically activate. The irony is that the activating enzymes, particularly the **cytochrome P450** family, normally exist to *detoxify* foreign compounds by making them water-soluble and easier to excrete. For some molecules, that same chemistry produces a reactive intermediate instead.

Consider **benzo[a]pyrene**, a **polycyclic aromatic hydrocarbon (PAH)** formed by incomplete combustion of tobacco, charred meat, coal tar, and diesel exhaust. Inert as inhaled, it is converted by cytochrome P450 enzymes (CYP1A1, CYP1B1) into benzo[a]pyrene diol epoxide (BPDE) — the **ultimate carcinogen**, the reactive form that actually does the damage. BPDE binds covalently to guanine, forming a bulky **DNA adduct** (a chemical group attached to a base). If the cell replicates before repair removes the adduct, the polymerase tends to insert adenine opposite the distorted guanine, producing a **G→T transversion** (IARC Monographs; NCBI Bookshelf).

<!-- → [DIAGRAM: metabolic activation of benzo[a]pyrene — procarcinogen → CYP450 → BPDE epoxide → guanine adduct → G→T transversion on replication] -->

The general logic — enter, activate, react, mutate — recurs across most chemical carcinogens. What differs is which adduct forms and therefore which **mutational signature** (the characteristic spectrum of base changes left across a genome) the carcinogen leaves behind.

### Initiation, promotion, progression

A single dose of a carcinogen usually does not produce visible cancer. The dominant framework for why comes from mouse skin-painting experiments of the 1940s–1960s and describes three stages.

**Initiation** is the irreversible step: a carcinogen induces a mutation in a target cell. The initiated cell sits in the tissue, carrying altered DNA but otherwise indistinguishable from its neighbors. **Promotion** is the typically reversible step in which non-mutagenic factors — chronic inflammation, hormonal stimulation, wound healing — cause the initiated cell to proliferate selectively, expanding the clone. **Progression** is the further accumulation of mutations and clonal selection that yields frank malignancy: invasion and metastasis.

The experimental proof is clean. A single dose of a genotoxic initiator (such as DMBA) on mouse skin produces no tumors. Repeated application of a non-mutagenic promoter (such as the phorbol ester TPA) afterward produces tumors. TPA without prior initiation produces nothing. The order matters: the promoter acts only on cells already initiated (archive chapter, mouse skin model).

<!-- → [DIAGRAM: initiation–promotion–progression — normal cell → initiated clone (mutation) → expanded clone (promotion) → malignant tumor (progression)] -->

The boundary condition matters too. Real carcinogenesis is rarely this tidy; most carcinogens have both initiating and promoting activity. But the framework tells us something actionable: prevention can target either stage — banning initiators *or* reducing promoters (treating chronic inflammation, reducing obesity).

### Ionizing versus ultraviolet radiation

A frequent confusion is to treat all "radiation" as one mechanism. It is not. **Ionizing radiation** — X-rays, gamma rays, alpha and beta particles, neutrons — carries enough energy to eject electrons from atoms, breaking chemical bonds. In tissue it damages DNA directly (ionizing DNA atoms) and indirectly (ionizing water to produce reactive oxygen species that diffuse to DNA). Its most consequential lesion is the **double-strand break**, because misrepair produces chromosomal rearrangements (NCI, Risk Factors).

**Ultraviolet (UV) radiation** is *non-ionizing* — it cannot eject electrons — but UV-B photons are energetic enough to fuse adjacent pyrimidine bases into a **cyclobutane pyrimidine dimer**, a lesion DNA polymerase cannot read past. Unrepaired dimers cause **C→T transitions** at dipyrimidine sites — the signature of UV exposure. The two kinds of radiation produce different damage, different signatures, and different cancers.

### Hazard versus risk

The **International Agency for Research on Cancer (IARC)**, founded in 1965, runs the *Monographs Programme*, classifying agents by carcinogenicity into Group 1 (carcinogenic to humans), 2A (probably), 2B (possibly), and 3 (not classifiable). Crucially, an IARC group identifies **hazard** — whether an agent *can* cause cancer under *some* exposure conditions — not personal **risk**, which depends on dose, route, and duration (IARC Monographs). Tobacco smoke and processed meat are both Group 1, but their exposure-risk profiles differ by orders of magnitude. A Group 1 label does not mean "equally dangerous at any dose."

## Worked Example

**Situation.** Aflatoxin B1, a toxin produced by *Aspergillus* molds contaminating stored grains and peanuts in humid climates, is one of the most potent natural carcinogens known. A public-health team wants to know why liver cancer rates are so high in a region where both aflatoxin contamination and chronic hepatitis B infection are common — and which intervention to prioritize.

**Process.** Aflatoxin B1 is a procarcinogen. Cytochrome P450 converts it to a reactive epoxide that binds guanine and produces a remarkably specific lesion: a **G→T transversion at codon 249 of *TP53*** (the R249S mutation), one of the most specific mutational signatures known (IARC, Mycotoxins as human carcinogens). So the team's first hypothesis is that aflatoxin alone explains the elevated rates.

*Dead end.* If aflatoxin alone were the driver, you would expect liver cancer wherever aflatoxin contamination occurs, at rates proportional to contamination. But the data don't fit cleanly: regions with aflatoxin but low hepatitis B prevalence show much lower rates than regions with both. Aflatoxin alone underpredicts the burden. The single-cause model fails.

**Resolution.** The resolution is synergy across the initiation–promotion framework. Aflatoxin acts as an **initiator**, introducing the R249S mutation. Chronic hepatitis B infection acts as a **promoter**, driving cycles of liver inflammation, cell death, and regeneration that expand initiated clones and add mutations. Together they produce hepatocellular carcinoma at higher rates and earlier ages than either factor alone (archive chapter). The most cost-effective intervention is therefore *combined*: improve grain storage to cut aflatoxin exposure (remove the initiator) and vaccinate against hepatitis B (remove the promoter).

**The lesson.** A mutational signature can name the initiator precisely, but the cancer rate is set by initiator *and* promoter together. Prevention works at either stage.

**The limit.** This synergy is specific to liver cancer in aflatoxin-and-HBV-endemic regions. It does not generalize to all carcinogens; many tumors lack a clean two-agent structure, and the codon-249 signature is far more specific than most carcinogen fingerprints, which overlap and blur.

## Common Misconceptions

**"Exposure to a carcinogen means you will get cancer."** This collapses the entire initiation–promotion–progression sequence into a single step. Initiation is one mutation in one cell; cancer requires that mutation to be promoted, to accumulate further changes, and to escape repair and immune surveillance over years to decades. The man in the opening case smoked for thirty-five years; the latency from sustained heavy smoking to lung cancer is typically 20–40 years (archive chapter). Carcinogens shift probabilities; they do not flip a switch.

**"All radiation damages DNA the same way, so any radiation source is equally a cancer threat."** Ionizing and ultraviolet radiation differ fundamentally. Ionizing radiation breaks DNA strands and produces double-strand breaks and chromosomal rearrangements; UV cannot ionize atoms at all and instead fuses adjacent pyrimidines into dimers (NCI, Risk Factors). A chest X-ray and an afternoon of sunburn injure cells through different chemistry, leave different mutational signatures, and cause different cancers (leukemia and thyroid versus skin). Treating them as one mechanism makes the genomic evidence unreadable.

**"A Group 1 IARC classification means an agent is equally dangerous at any exposure."** Group 1 is a statement about **hazard** — that an agent can cause cancer under some conditions — not a statement about **risk** at a given dose. Tobacco smoke and processed meat share the Group 1 label and almost nothing else about magnitude of risk (IARC Monographs). Reading hazard as dose-independent personal risk is the most common public misreading of the IARC system, and it is exactly the error that lets people dismiss the system as alarmist.

## Exercises

1. **(Understand)** In two or three sentences each, contrast the primary DNA lesion produced by (a) benzo[a]pyrene diol epoxide, (b) ionizing radiation, and (c) UV-B. Name the characteristic mutation each tends to produce.

2. **(Apply)** A non-smoker's lung tumor shows mostly G→A transitions, while a smoker's lung tumor of the same histology shows an excess of G→T transversions at specific *TP53* codons. Explain mechanistically why the two etiologies leave different signatures, and state what this implies about reading a tumor genome as a record of past exposure.

3. **(Produce)** Choose one carcinogen from this chapter (tobacco PAHs, aflatoxin B1, asbestos, benzene, or UV). Draw a mechanism map with five linked boxes: *exposure → molecular damage → mutation/lesion → cancer phenotype → prevention or intervention*. Label each arrow with the mechanism that connects the boxes. Mark one place where the chain could be interrupted.

4. **(Analyze)** A news headline reads: "WHO declares [agent] a carcinogen — same category as tobacco." Using the hazard-versus-risk distinction, write one paragraph explaining what the headline gets right and what it misleads readers about. Reference what an IARC group does and does not tell you about personal risk.

## What Would Change My Mind

The central claim of this chapter is that chemical and radiation carcinogens cause cancer primarily by introducing mutations, and that those mutations leave readable, exposure-specific signatures in tumor genomes. The strongest evidence for this is the convergence of three independent lines — known adduct chemistry, the mutational signatures catalogued across thousands of tumor genomes (Alexandrov et al., *Nature*, 2013), and epidemiology that links exposure to specific cancers. This claim would be seriously weakened if large-scale tumor sequencing showed that the signatures attributed to specific carcinogens (the smoking G→T pattern, the aflatoxin codon-249 mutation, the UV C→T pattern) were in fact *not* enriched in the exposed populations relative to unexposed controls, or if a major carcinogen reliably caused cancer with no detectable mutational footprint and no inflammatory promotion either. A purely non-genotoxic, non-inflammatory mechanism producing a common human cancer would force a substantial revision of the "carcinogen as mutagen" framing.

## Still Puzzling

- **How low is too low?** For genotoxic carcinogens, the regulatory default is a linear, no-threshold dose-response — no exposure is provably safe. But at very low doses the data are noisy, and some studies hint at hormetic (protective) effects of low-dose radiation. Whether a true threshold exists for any genotoxic carcinogen remains genuinely contested.

- **Why these codons?** The tobacco signature concentrates at particular *TP53* codons (157, 248, 273) and aflatoxin at codon 249. How much of this reflects adduct-binding preference versus differential repair versus selection for the resulting protein change is not fully resolved.

- **Mixtures, not molecules.** Tobacco smoke contains more than 70 carcinogens acting together. We catalogue them individually, but how they combine — additively, synergistically, or with one dominating — is poorly characterized for most real-world exposures. This question carries forward into the next chapter, where chemical initiators meet infectious promoters.

## References

- IARC Monographs on the Identification of Carcinogenic Hazards to Humans. International Agency for Research on Cancer. https://monographs.iarc.who.int/
- IARC, European Code Against Cancer: Tobacco and cancer. https://www.iarc.who.int/reference/european-code-against-cancer-4th-edition-tobacco-and-cancer/
- IARC, Mycotoxins as human carcinogens. https://www.iarc.who.int/reference/mycotoxins-as-human-carcinogens-the-iarc-monographs-classification/
- NCI, Risk Factors for Cancer. https://www.cancer.gov/about-cancer/causes-prevention/risk
- NCBI Bookshelf, The Development and Causes of Cancer. https://www.ncbi.nlm.nih.gov/books/NBK9963/
- Alexandrov, L. B., et al. (2013). Signatures of mutational processes in human cancer. *Nature*, 500, 415–421. [verify — citation drawn from archive chapter]

## Prompts

*No figures have been generated for this chapter yet.*
