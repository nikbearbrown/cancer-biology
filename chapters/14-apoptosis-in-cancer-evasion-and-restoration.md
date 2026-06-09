# Apoptosis in Cancer: Evasion and Restoration

## Learning Objectives

After working through this chapter, you should be able to:

1. **Explain** the recurrent molecular strategies cancer cells use to evade apoptosis and **classify** each as overexpression, loss, mutation, or signaling-driven survival.
2. **Describe** how a **BH3 mimetic** works at the molecular level, and **explain** why this differs fundamentally from DNA-damaging chemotherapy.
3. **Trace** the venetoclax story from preclinical proof of concept to clinical use, and **identify** the technical problem (BCL-XL toxicity) that selectivity solved.
4. **Evaluate** why an apoptosis-restoring drug works in some cancers and fails in others, using the concept of **apoptotic dependency**.
5. **Compare** BH3 mimetics, TRAIL agonists, IAP antagonists, and MDM2 inhibitors as routes to restoring death signaling.

## Opening Case

A 68-year-old man has chronic lymphocytic leukemia (CLL) that has relapsed after several prior therapies. His leukemic B cells are not dividing especially fast — that is not the problem. The problem is that they will not die. They have accumulated to the point of crowding out his normal blood cells, and conventional cytotoxic drugs, which kill by inflicting DNA damage, have stopped working: each relapse has selected for cells better at surviving damage.

He is started on a single oral drug. Within weeks, his leukemic count plummets and his bone marrow clears to the point where minimal residual disease is undetectable — a depth of response that no prior therapy in his history had produced. The drug did not damage his cells. It did the opposite: it *released* a brake those cells had been holding on their own death program, and they died by their own hand.

The drug is venetoclax. The case captures the conceptual pivot of this chapter. For most of cancer therapy's history, the strategy was to inflict enough damage to kill the tumor before killing the patient — a narrow therapeutic window, because the same damage kills bone marrow, gut, and hair follicles. The newer strategy is to recognize that cancer cells already carry the full apoptotic machinery from the last chapter; they have simply suppressed it. Restore the suppression's release, and the cells die selectively, because normal cells were never suppressing apoptosis to begin with. The chapter's framing: the drug that restores death is the drug that wins.

## Core Concepts

### Apoptosis evasion is active, not passive

Plain language: cancer cells do not merely "fail to die." They are *under constant pressure to die* — they carry DNA damage, oncogene-induced stress, and detachment signals that should all trigger the intrinsic pathway — and they survive only because they have actively acquired counter-measures. Evasion is a selected adaptation, not an empty space where death should be.

This is the single most important misconception to correct up front. Students often picture apoptosis evasion as a passive absence (the death signal simply isn't there). It is better understood as an arms race the cancer cell is *winning*: the death signals are present and strong, and the cell has built defenses against them. That reframing is what makes the next idea — a drug that strips the defense — make sense.

Cancers evade apoptosis through a small set of recurrent strategies (NCBI Bookshelf, NBK9963):

- **Overexpression of anti-apoptotic BCL-2 family proteins.** The canonical case is BCL-2 itself, discovered at the t(14;18) translocation of **follicular lymphoma**, which fuses the *BCL2* gene to the immunoglobulin heavy-chain enhancer and drives extremely high BCL-2 expression. The lymphoma cells aren't dividing faster — they simply refuse to die. BCL-XL and **MCL-1** overexpression are common across many cancers, and MCL-1 is often the factor that limits the response to BCL-2 inhibition.
- **Loss of pro-apoptotic proteins.** Loss or mutation of BAX, BAK, or the BH3-only sensors (PUMA, NOXA, BIM) lowers the cell's apoptotic capacity. BAX is mutated in some microsatellite-instability-high cancers.
- **Mutation of *TP53*.** Present in roughly half of all cancers, this removes the upstream sensor that links DNA damage to death (Chapter 13).
- **Overexpression of Inhibitor of Apoptosis Proteins (IAPs)** — XIAP, c-IAP1/2, and **survivin**, which inhibit caspases directly. Survivin is overexpressed in most cancers and nearly absent from normal adult tissue.
- **Downregulation of death receptors** (FAS, DR4, DR5) or loss of caspase-8 (sometimes by promoter hypermethylation, as in some neuroblastomas).
- **Active survival signaling.** PI3K–AKT phosphorylates and inactivates the BH3-only protein BAD, raises MCL-1, and suppresses p53; NF-κB raises BCL-XL and IAPs; MAPK destabilizes BIM. Survival is the net output of many converging signals.

These are not mutually exclusive. A single cancer cell may overexpress BCL-2, lose BAX, mutate *TP53*, and run hyperactive PI3K–AKT all at once — layered, redundant defenses. That redundancy is exactly why single-target apoptosis-restoring drugs sometimes fail and why combinations are often required.

<!-- → [DIAGRAM: the evasion strategies mapped onto the Chapter 13 pathway — where each alteration (overexpression, loss, TP53 mutation, IAP, survival signaling) breaks the death circuit] -->

### BH3 mimetics and the logic of dependency

Plain language: a **BH3 mimetic** is a small molecule shaped to imitate the business end of a natural BH3-only protein. It slips into the binding groove of an anti-apoptotic guardian (such as BCL-2) and pries it loose from the pro-apoptotic effectors it was sequestering — freeing BAX and BAK to permeabilize mitochondria.

Formal definition: a **BH3 mimetic** is a compound that binds the hydrophobic BH3-binding groove of an anti-apoptotic BCL-2-family protein, displacing bound pro-apoptotic partners and thereby promoting MOMP (NCI Drug Dictionary; Letai, 2016).

The crucial distinction — and a misconception worth naming — is that **BH3 mimetics do not kill by causing DNA damage** the way chemotherapy does. They cause no new lesions. They simply remove a brake the cancer cell was already straining against. This is why their selectivity can be better: a normal cell that was not leaning on BCL-2 to stay alive is largely unaffected when BCL-2 is inhibited.

Whether a BH3 mimetic kills depends on **apoptotic dependency** — also called being "primed for death." A cell that has loaded its mitochondria with pro-apoptotic pressure and is surviving *only* because one specific guardian (say, BCL-2) is holding the line is exquisitely vulnerable to a drug against that guardian. A cell whose survival is spread across multiple guardians, or that has lost its effectors entirely, is not. CLL cells are heavily BCL-2-dependent; many solid tumors depend on multiple survival pathways at once. This is the boundary condition: the drug works where the dependency is concentrated, and a single death-restoring drug should *not* be expected to work across all cancers.

<!-- → [FIGURE: BCL-2 holding BAX/BAK in check, then a BH3-mimetic molecule occupying the groove and releasing the effectors → MOMP] -->

### Restoring death: the therapeutic families

The same logic — find the brake, release it selectively — generates several drug classes. They differ in *which* brake they target:

- **BH3 mimetics** release anti-apoptotic guardians (the venetoclax family).
- **TRAIL agonists** push the extrinsic pathway by engaging death receptors.
- **IAP antagonists** mimic SMAC/DIABLO to release caspases from IAP inhibition.
- **MDM2 inhibitors** restore p53 levels in cancers that have wild-type *TP53* but suppress it.

We examine each in the Worked Example and the survey that follows.

## Worked Example

**Situation.** Take the CLL cell from the Opening Case. We want to understand, mechanistically, why one drug (venetoclax) succeeds where another reasonable design failed — and we will let the field's own history supply the dead end.

**Process (including a real dead end).** The structural biology of the 1990s revealed that anti-apoptotic guardians have a hydrophobic groove that binds the BH3 helix of pro-apoptotic proteins. If a small molecule could occupy that groove, it would mimic a BH3 protein and disrupt the protective complex. **ABT-737** (2005) proved this in principle, binding BCL-2, BCL-XL, and BCL-W with nanomolar affinity and killing BCL-2-dependent tumors in the lab.

Its orally available successor, **navitoclax (ABT-263)**, went into CLL and small-cell lung cancer trials and showed activity — but here is the dead end. Navitoclax inhibits BCL-XL as well as BCL-2, and **platelets depend on BCL-XL for survival**. Inhibiting BCL-XL drove platelet apoptosis, producing dose-limiting **thrombocytopenia** (low platelet count). The very breadth that made the drug potent against tumors made it toxic to a normal cell type that happened to share the dependency. The biology was elegant; the drug was limited.

**Resolution.** The fix was selectivity. **Venetoclax (ABT-199)** was engineered by structure-guided medicinal chemistry to retain potent BCL-2 binding while *avoiding* the BCL-XL pocket — sparing platelets. It was approved by the FDA in 2016 for CLL (Letai, 2016). In heavily pretreated CLL, single-agent response rates exceed 70 percent, with a substantial fraction reaching undetectable minimal residual disease; in combination with anti-CD20 antibodies (the MURANO and CLL14 regimens) responses are deeper still [verify — trial response figures]. In acute myeloid leukemia (AML), venetoclax plus a hypomethylating agent (azacitidine) became standard of care for elderly patients, roughly doubling response rates over the hypomethylating agent alone [verify — VIALE-A].

**The lesson.** The decisive variable was not raw potency against the tumor but *which normal cell shared the dependency*. BCL-2 selectivity converted a toxic compound into a transformative drug. Mechanism on the page: same groove, narrower target, better therapeutic window.

**The limit.** Venetoclax is not universal. Resistance emerges through *BCL2* mutations that block binding (G101V is the most common), through upregulation of MCL-1 or BCL-XL as the cell switches its dependency, and through changes in BAX/BAK levels. And in multiple myeloma, venetoclax works mainly in the t(11;14) subgroup, which is BCL-2-dependent — outside it, activity is limited. The drug works exactly as far as the dependency extends, and no further.

## Common Misconceptions

**"Apoptosis evasion is just the absence of a death signal."** The death signals are present and strong in cancer cells — that is why they are *primed*. Evasion is an actively acquired set of defenses (overexpressed guardians, lost effectors, mutated *TP53*, IAPs, survival signaling). The Opening Case patient's cells were straining against death the whole time; venetoclax worked by removing one defense, not by adding a new signal.

**"BH3 mimetics kill cells the way chemotherapy does."** They do not. Chemotherapy inflicts DNA damage and lets the cell die from it; a BH3 mimetic inflicts no damage and simply releases the cell's own pre-loaded death program. This is why a normal cell not leaning on BCL-2 is largely spared — and why the toxicity profile and resistance mechanisms are completely different from those of cytotoxic drugs.

**"One death-restoring drug should work across all cancers."** Apoptosis-restoring therapy works only where the cancer is *dependent* on the brake the drug releases. Venetoclax is dramatic in BCL-2-dependent CLL and modest-to-absent in tumors whose survival is spread across MCL-1, BCL-XL, and multiple signaling pathways. Expecting one BH3 mimetic to cover all cancers ignores the dependency boundary that governs every drug in this class.

## Exercises

1. **(Understand.)** In your own words, explain why a BH3 mimetic can have a better therapeutic window than DNA-damaging chemotherapy, referring explicitly to what each does (or does not do) to a normal, non-primed cell.

2. **(Apply.)** A patient with CLL responds beautifully to venetoclax, then relapses. Sequencing reveals upregulated MCL-1. Explain mechanistically why MCL-1 upregulation confers resistance to a BCL-2-selective drug, and name the class of agent you would add to overcome it.

3. **(Apply/Analyze — produce something.)** Build a decision table. Columns: BCL-2, MCL-1, BCL-XL. Rows: the targeting drug class, the cancers known to depend on it, and the dose-limiting toxicity (recall the platelet/BCL-XL story; MCL-1 is required by cardiomyocytes). Then write one sentence recommending which guardian you would target in a *new* program and why.

4. **(Analyze.)** TRAIL agonists had striking preclinical selectivity for cancer cells but modest clinical activity. List two specific drug-design reasons for the gap (consider receptor clustering and ligand half-life), and explain why this is a cautionary tale about translating elegant biology into effective drugs.

## What Would Change My Mind

The central claim is that selectively *releasing* a cancer cell's suppressed death program is a clinically powerful, mechanistically distinct strategy from inflicting damage. The finding that would most force a revision: a rigorous demonstration that venetoclax's clinical benefit in BCL-2-dependent cancers is actually driven by an off-target or DNA-damage-like mechanism rather than by on-target BCL-2 displacement — for instance, if BCL-2-mutant cells that cannot bind the drug still died at the same rate, or if biomarkers of apoptotic priming failed entirely to predict response in adequately powered cohorts. That would collapse the "restore death, selectively" framing back into ordinary cytotoxicity. The G101V resistance mutation, which maps precisely to the drug-binding groove and abolishes response, currently argues strongly for the on-target mechanism — but a clean dissociation between target engagement and killing would be the disconfirming test.

## Still Puzzling

- **Why does TRAIL biology fail to translate?** The preclinical selectivity of TRAIL for cancer cells is striking, yet first-generation agonists were disappointing. Whether newer multivalent constructs (hexavalent TRAIL receptor agonists) close the gap, or whether the extrinsic pathway is simply too easily bypassed in vivo, is unresolved.
- **Can MCL-1 ever be safely drugged?** MCL-1 is the most common limiting dependency, but it is also required by cardiomyocytes and hepatocytes, making selective inhibition treacherous. Whether a viable therapeutic window exists is an open clinical question.
- **Is mutant-p53 reactivation achievable at all?** Restoring DNA-binding function to a misfolded mutant p53 protein (as APR-246 attempted) is a far harder problem than raising wild-type p53 levels, and the clinical record so far is mixed. This seeds the metabolism chapters, where p53's *non*-canonical roles reappear.

## References

- NCI Drug Dictionary. *BH3 mimetic ABT-737.* National Cancer Institute. https://www.cancer.gov/publications/dictionaries/cancer-drug/def/bh3-mimetic-abt-737
- Letai, A. (2016). *Mitochondrial apoptosis and BH3 mimetics.* PMC5133681. https://pmc.ncbi.nlm.nih.gov/articles/PMC5133681/
- NCI Cancer Currents (2016). *DINO RNA and the p53 response.* https://www.cancer.gov/news-events/cancer-currents-blog/2016/dino-p53
- NCI. *The Genetics of Cancer.* https://www.cancer.gov/about-cancer/causes-prevention/genetics
- Hino, O., et al. (2017). *The two-hit hypothesis.* Cancer Science. https://onlinelibrary.wiley.com/doi/10.1111/cas.13116
- NCBI Bookshelf. *The Development and Causes of Cancer.* NBK9963. https://www.ncbi.nlm.nih.gov/books/NBK9963/

## Prompts

*No figures have been generated for this chapter yet.*
