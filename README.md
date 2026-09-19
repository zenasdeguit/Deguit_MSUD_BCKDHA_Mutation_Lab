# MSUD BCKDHA Mutation Analysis

## Project Overview

This repository contains the sequence-analysis work for the Cell and Molecular Biology Laboratory activity **“From Gene Mutation to Disease: Investigating How DNA Sequence Changes Affect Protein Products and Human Phenotypes.”**

The project focuses on **Maple Syrup Urine Disease (MSUD)** and the **BCKDHA** gene. The analysis examines how a documented nucleotide substitution changes a codon and predicted amino-acid sequence, and compares it with a student-created artificial mutation.

The computational sequence analysis was performed using **Galaxy** and **SeqKit Translate**.

---

## Disease and Gene

### Maple Syrup Urine Disease (MSUD)

MSUD is an inherited metabolic disorder involving impaired breakdown of the branched-chain amino acids **leucine, isoleucine, and valine**. Their metabolites can accumulate and may particularly affect the brain and nervous system.

MSUD is inherited in an **autosomal recessive** pattern.

### BCKDHA

- **Official gene symbol:** BCKDHA
- **Chromosome:** 19q13.2
- **Reference transcript:** NM_000709.4
- **Reference protein:** NP_000700.1
- **Protein:** 2-oxoisovalerate dehydrogenase subunit alpha, mitochondrial isoform 1 precursor

BCKDHA encodes the alpha subunit of the E1 component of the branched-chain alpha-ketoacid dehydrogenase (BCKD) complex. The complex participates in branched-chain amino-acid metabolism in the mitochondria.

---

## Objectives

The analysis was performed to:

1. Obtain the normal BCKDHA coding sequence.
2. Translate the WT coding sequence into a predicted protein sequence.
3. Reproduce a documented BCKDHA mutation.
4. Compare the documented mutant with the WT sequence.
5. Create a student-generated artificial mutation.
6. Translate the artificial mutant sequence.
7. Compare WT, documented mutant, and artificial mutant sequences.
8. Interpret the possible molecular consequences of the mutations.

---

## Reference Sequence

The WT BCKDHA coding sequence was obtained from **NCBI RefSeq**.

| Feature | Result |
|---|---|
| Gene | BCKDHA |
| Reference transcript | NM_000709.4 |
| Reference protein | NP_000700.1 |
| Sequence type | Coding DNA sequence (CDS) |
| CDS length | 1,338 bp |
| Organism | *Homo sapiens* |
| Start codon | ATG |
| Stop codon | TGA |
| Reading frame | Frame 1 |

The original WT CDS was kept unchanged and used as the reference for the mutation analysis.

---

## Galaxy History

**Galaxy History:** `Deguit_MSUD_BCKDHA_Mutation_Lab`

### Final relevant files

| File | Filename | Purpose |
|---|---|---|
| File 1 | `MSUD_CDS.fasta.txt` | WT BCKDHA CDS |
| File 3 | `MSUD_protein.fasta` | Predicted WT protein |
| File 5 | `MSUD_BCKDHA_c929C_G_mutant.fasta` | Documented mutant CDS |
| File 6 | `MSUD_mutant_protein.fasta` | Predicted documented mutant protein |
| File 7 | `MSUD_BCKDHA_artificial_c303G_A.fasta` | Student-created artificial mutant CDS |
| File 8 | `MSUD_artificial_mutant_protein.fasta` | Predicted artificial mutant protein |

File 4 was an intermediate working copy and was deleted after the documented mutant sequence was produced.

---

# Wild-Type Translation

The WT BCKDHA CDS was translated with **SeqKit Translate** in Galaxy.

### Translation settings

- Genetic code: Standard
- Reading frame: Frame 1
- Initial codon translated to M: Yes

### Results

- CDS length: **1,338 bp**
- Predicted protein length: **445 amino acids**
- Start codon: **ATG**
- Stop codon: **TGA**
- First 10 amino acids: `MAVAIAAARV`
- Last 10 amino acids: `EHYPLDHFDK`

**Output:** `MSUD_protein.fasta`

---

# Documented Mutation

The documented BCKDHA variant analyzed was:

**NM_000709.4:c.929C>G (p.Thr310Arg)**

### Mutation details

| Feature | Result |
|---|---|
| Gene | BCKDHA |
| Reference transcript | NM_000709.4 |
| Reference protein | NP_000700.1 |
| Nucleotide change | C → G at c.929 |
| Codon change | ACA → AGA |
| Amino-acid change | Thr310 → Arg310 (T310R) |
| Mutation type | Missense |
| Nucleotides affected | 1 bp |
| CDS length | 1,338 bp |
| Predicted protein length | 445 aa |
| Frameshift | No |
| Premature stop | No |

The documented mutation was introduced into a copy of the WT CDS.

**Mutant CDS:** `MSUD_BCKDHA_c929C_G_mutant.fasta`

---

# Documented Mutant Translation

The documented mutant CDS was translated using the same settings as the WT sequence.

### Results

- Mutant CDS length: **1,338 bp**
- Predicted mutant protein length: **445 aa**
- First amino-acid difference: **position 310, T → R**
- Premature stop codon: **Absent**
- Reading-frame change: **None**
- Approximate amino acids affected: **1**

**Output:** `MSUD_mutant_protein.fasta`

The WT and documented mutant proteins therefore have the same overall length, with the main predicted difference being the **T310R substitution**.

---

# Artificial Mutation

A student-created single-nucleotide substitution was introduced into the WT BCKDHA CDS:

**c.303G>A**

The nucleotide change converted:

**AAG → AAA**

Both codons encode lysine (K), so the mutation was predicted to be **synonymous**.

### Artificial mutation information

| Feature | Result |
|---|---|
| Gene | BCKDHA |
| Reference transcript | NM_000709.4 |
| Mutation type | Single-nucleotide substitution |
| Nucleotide position | c.303 |
| Nucleotide change | G → A |
| Codon change | AAG → AAA |
| Predicted amino-acid change | K → K |
| Predicted mutation type | Synonymous |
| Predicted frameshift | No |
| Predicted premature stop | No |
| Predicted protein length | 445 aa |

**Artificial mutant CDS:** `MSUD_BCKDHA_artificial_c303G_A.fasta`

---

# Artificial Mutant Translation

The artificial mutant CDS was translated using the same SeqKit Translate settings.

**Output:** `MSUD_artificial_mutant_protein.fasta`

### Results

- CDS length: **1,338 bp**
- Predicted protein length: **445 aa**
- Amino-acid substitution: **None**
- Reading-frame change: **None**
- Premature stop codon: **No**

The artificial mutation did not alter the predicted amino-acid sequence because both AAG and AAA encode lysine.

---

# Comparison of the Three Sequences

| Feature | WT | Documented Mutation | Student-Created Mutation |
|---|---|---|---|
| CDS length | 1,338 bp | 1,338 bp | 1,338 bp |
| Protein length | 445 aa | 445 aa | 445 aa |
| Mutation | None | c.929C>G | c.303G>A |
| Codon change | ACA | ACA → AGA | AAG → AAA |
| Mutation type | N/A | Missense | Synonymous |
| Reading frame changed? | No | No | No |
| Premature stop codon? | No | No | No |
| Amino acids affected | None | T310 → R310 | None (K → K) |
| Expected sequence-level consequence | Normal WT sequence | One amino-acid substitution | No predicted amino-acid change |

The documented and artificial mutations are both single-nucleotide substitutions, but they have different predicted protein-level outcomes. The documented mutation changes **ACA to AGA**, producing the **T310R** substitution. The artificial mutation changes **AAG to AAA**, but both codons encode lysine. Therefore, the artificial mutation does not alter the predicted amino-acid sequence.

---

# Molecular Interpretation

The documented **c.929C>G** variant changes one nucleotide in the BCKDHA coding region and produces the predicted **Thr310Arg** substitution. Although the protein remains 445 amino acids long, the replacement of threonine with arginine may influence protein properties such as stability or molecular interactions.

Experimental evidence cited in the laboratory report describes the corresponding historical **T265R** designation and reports effects on E1-alpha stability and assembly with the E1-beta subunit. These published findings provide experimental context for the possible functional effect of the amino-acid substitution.

Because BCKDHA is part of the BCKD complex, changes that reduce normal complex activity can interfere with the metabolism of leucine, isoleucine, and valine. Accumulation of these amino acids and their metabolites is associated with the biochemical and neurological effects of MSUD.

The computational workflow directly establishes the sequence-level relationship:

**DNA substitution → codon change → predicted amino-acid substitution**

Further conclusions about protein stability, enzyme activity, and disease effects require published experimental or clinical evidence.

---

# Interpretation Questions

### 32. Why does the exact location of a mutation matter?

The location of a mutation determines which codon or part of a protein is affected. A change in a functionally important region may influence protein activity more strongly than a change in a less critical region.

### 33. Why can deleting three nucleotides produce a different result from deleting one or two nucleotides?

Deleting three nucleotides removes one complete codon and can leave the reading frame unchanged. Deleting one or two nucleotides shifts the reading frame and changes the way downstream nucleotides are grouped into codons.

### 34. Does every mutation change the amino-acid sequence?

No. Some nucleotide substitutions are synonymous because different codons can specify the same amino acid. In this experiment, **AAG → AAA** still specifies lysine (K), so the predicted amino-acid sequence remained the same.

### 35. Does every amino-acid substitution destroy protein function?

No. The effect depends on the amino acids involved and where the substitution occurs. Some substitutions may have little effect, while others can affect protein structure, stability, interactions, or activity.

### 36. Why can a frameshift affect many amino acids even if only one nucleotide was deleted?

A one-nucleotide deletion changes the reading frame from the mutation site onward. This causes downstream codons to be read differently, which can alter many amino acids and may eventually introduce a premature stop codon.

### 37. Why might a premature stop codon produce a nonfunctional protein?

A premature stop codon ends translation before the full protein has been produced. The shortened protein may lack regions required for proper folding, stability, interactions, or biological function.

### 38. Could a mutation affect protein function without greatly changing protein length?

Yes. A mutation can change one amino acid while leaving the total protein length unchanged. If that amino acid is important for protein structure or interactions, the substitution can still affect function. The documented **BCKDHA c.929C>G (p.Thr310Arg)** mutation illustrates this type of sequence change.

### 39. Could a mutation cause disease without changing the protein sequence?

Yes. Mutations can affect gene regulation, RNA splicing, mRNA stability, or the amount of protein produced without changing the amino-acid sequence. A regulatory mutation that reduces BCKDHA expression could decrease the amount of functional BCKD complex.

### 40. What evidence from the analysis supports the proposed molecular mechanism?

The analysis showed that **c.929C>G** changes **ACA to AGA**, producing the predicted **T310R** substitution. The CDS remained 1,338 bp and the predicted protein remained 445 amino acids long, with no frameshift or premature stop codon. Experimental studies are needed to determine the resulting effects on BCKDHA function.

### 41. Which conclusions are supported directly by the computational results, and which require experimental evidence?

The computational results directly support the nucleotide substitution, codon change, predicted amino-acid substitution, unchanged protein length, unchanged reading frame, and absence of a premature stop codon. Effects on protein stability, assembly, enzyme activity, and the clinical manifestations of MSUD require published experimental or clinical evidence.

---

# Reproducibility

The general workflow was:

1. Obtain the BCKDHA WT CDS from NCBI RefSeq.
2. Upload the WT sequence to Galaxy.
3. Translate the WT CDS with SeqKit Translate.
4. Create a copy of the WT sequence for the documented mutation.
5. Introduce the c.929C>G substitution.
6. Translate the documented mutant CDS.
7. Create the artificial c.303G>A mutation from the WT sequence.
8. Translate the artificial mutant CDS.
9. Compare the WT, documented mutant, and artificial mutant proteins.
10. Interpret the sequence findings together with published evidence.

---

# Tools and Databases

- **Galaxy** — sequence analysis workflow
- **SeqKit Translate** — nucleotide-to-protein translation
- **NCBI RefSeq** — reference BCKDHA sequence
- **NCBI ClinVar** — clinical variant information

---

# References

- National Center for Biotechnology Information. **BCKDHA gene**.  
  https://www.ncbi.nlm.nih.gov/gene/593

- National Center for Biotechnology Information. **ClinVar: NM_000709.4(BCKDHA):c.929C>G (p.Thr310Arg)**.  
  https://www.ncbi.nlm.nih.gov/clinvar/RCV002222336.14/

- National Library of Medicine. **BCKDHA gene — MedlinePlus Genetics**.  
  https://medlineplus.gov/genetics/gene/bckdha/

- National Library of Medicine. **Maple syrup urine disease — MedlinePlus Genetics**.  
  https://medlineplus.gov/genetics/condition/maple-syrup-urine-disease/

- Strauss, K. A., Puffenberger, E. G., & Carson, V. J. (2020). **Maple syrup urine disease**. GeneReviews®.  
  https://www.ncbi.nlm.nih.gov/books/NBK1319/

- Chuang, D. T., et al. (2000). Crystal structure of human branched-chain alpha-ketoacid dehydrogenase and the molecular basis of multienzyme complex deficiency in maple syrup urine disease. *Proceedings of the National Academy of Sciences, 97*(10), 5420–5425.  
  https://pubmed.ncbi.nlm.nih.gov/10745006/

- Strauss, K. A., et al. (2017). Maple syrup urine disease: Mechanisms and management. *Molecular Genetics and Metabolism, 120*(1–2), 1–10.  
  https://pubmed.ncbi.nlm.nih.gov/28919799/

- Wynn, R. M., Davie, J. R., Chuang, J. L., Cote, C. D., & Chuang, D. T. (1998). Impaired assembly of E1 decarboxylase of the branched-chain alpha-ketoacid dehydrogenase complex in type IA maple syrup urine disease. *Journal of Biological Chemistry, 273*(21), 13110–13118.  
  https://doi.org/10.1074/jbc.273.21.13110

---

## Galaxy History

Galaxy History used for the analysis:

https://usegalaxy.org/u/zenasdeguit/h/deguit-msud-bckdha-mutation-lab
