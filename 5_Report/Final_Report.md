# From Gene Mutation to Disease: BCKDHA and Maple Syrup Urine Disease

## 1. Disease Background

Maple Syrup Urine Disease (MSUD) is an inherited metabolic disorder that affects the body's ability to break down the branched-chain amino acids leucine, isoleucine, and valine. The disorder is associated with reduced activity of the branched-chain alpha-ketoacid dehydrogenase (BCKD) complex. When this pathway is impaired, branched-chain amino acids and their related metabolites can accumulate in the body, particularly affecting the nervous system.

Individuals with MSUD may experience symptoms such as poor feeding, vomiting, lethargy, abnormal muscle tone, neurological problems, seizures, and developmental difficulties. Severe untreated cases can progress to encephalopathy and coma. The severity of the condition can vary depending on the remaining activity of the BCKD complex.

The BCKDHA gene is one of the genes associated with MSUD. It encodes the E1 alpha subunit of the BCKD complex, which participates in the metabolism of branched-chain amino acids. Mutations in BCKDHA can affect the structure or function of the E1 alpha subunit and consequently reduce BCKD complex activity. MSUD follows an autosomal recessive inheritance pattern.

---

## 2. Gene and Protein Background

The gene analyzed in this project was **BCKDHA**, which encodes the E1 alpha subunit of the branched-chain alpha-ketoacid dehydrogenase complex.

### Gene Information

| Feature | Information |
|---|---|
| Gene | BCKDHA |
| Disease | Maple Syrup Urine Disease (MSUD) |
| Reference transcript | NM_000709.4 |
| Reference protein | NP_000700.1 |
| Chromosome | 19q13.2 |
| Protein | 2-oxoisovalerate dehydrogenase subunit alpha, mitochondrial |
| Cellular location | Mitochondrial BCKD complex |

The BCKD complex is involved in the breakdown of the branched-chain amino acids leucine, isoleucine, and valine. The E1 alpha subunit encoded by BCKDHA is therefore important for normal branched-chain amino-acid metabolism.

---

## 3. Reference Sequence

The normal BCKDHA coding sequence (CDS) was obtained from the NCBI RefSeq transcript **NM_000709.4**. The corresponding reference protein is **NP_000700.1**.

The normal CDS was preserved as the wild-type (WT) reference sequence and was not modified during the analysis.

### WT Sequence Information

| Feature | Result |
|---|---|
| Gene | BCKDHA |
| Transcript | NM_000709.4 |
| Protein accession | NP_000700.1 |
| CDS length | 1,338 bp |
| Predicted protein length | 445 aa |
| Start codon | ATG |
| Stop codon | TGA |
| Reading frame | Frame 1 |
| First 10 amino acids | MAVAIAAARV |
| Last 10 amino acids | EHYPLDHFDK |

---

## 4. WT CDS Translation

The WT BCKDHA CDS was translated using SeqKit Translate in Galaxy. The standard genetic code and reading frame 1 were used. The initial codon was translated as methionine.

The 1,338-bp CDS produced a predicted protein sequence of 445 amino acids before the stop codon. The sequence began with **MAVAIAAARV** and ended with **EHYPLDHFDK** before the terminal stop signal.

The resulting protein sequence was used as the WT protein reference for comparison with the documented and artificial mutants.

---

## 5. Documented Mutation

The documented BCKDHA mutation analyzed in this project was:

**NM_000709.4:c.929C>G**

The corresponding protein change is:

**NP_000700.1:p.Thr310Arg (T310R)**

This is a single-nucleotide substitution and is classified as a missense variant.

### Mutation Information

| Feature | Result |
|---|---|
| Gene | BCKDHA |
| Nucleotide change | c.929C>G |
| Original nucleotide | C |
| Mutant nucleotide | G |
| Original codon | ACA |
| Mutant codon | AGA |
| Amino-acid change | Thr (T) → Arg (R) |
| Protein position | 310 |
| Mutation type | Missense |
| Frameshift | No |
| Premature stop | No |

The nucleotide substitution changes the codon from **ACA**, which encodes threonine, to **AGA**, which encodes arginine.

---

## 6. Construction and Translation of the Documented Mutant

The documented mutation was reproduced manually using a copy of the WT BCKDHA CDS. The original WT sequence was preserved unchanged.

The nucleotide at position c.929 was changed from C to G. The resulting mutant CDS was then translated using the same SeqKit Translate settings used for the WT sequence.

The mutant CDS remained **1,338 bp** long and produced a predicted protein of **445 amino acids**. The first sequence difference occurred at amino-acid position 310, where threonine was replaced by arginine.

No reading-frame change or premature stop codon was observed.

### WT vs Documented Mutant

| Feature | WT | Documented Mutant |
|---|---|---|
| CDS length | 1,338 bp | 1,338 bp |
| Protein length | 445 aa | 445 aa |
| Codon at mutation | ACA | AGA |
| Amino acid | Thr (T) | Arg (R) |
| Position | 310 | 310 |
| Frameshift | No | No |
| Premature stop | No | No |

---

## 7. Protein Comparison

Comparison of the WT and documented mutant predicted protein sequences showed one amino-acid difference at position 310.

The WT sequence contains threonine at this position, while the documented mutant contains arginine:

**T310 → R310**

No downstream amino-acid changes were observed. The protein length remained 445 amino acids because the mutation was a single-nucleotide substitution that did not alter the reading frame.

Therefore, the sequence analysis is consistent with a single-nucleotide missense mutation.

---

## 8. Molecular Interpretation of the Documented Mutation

The documented BCKDHA mutation demonstrates the progression from a nucleotide-level change to an amino-acid substitution. In the WT sequence, nucleotide position 929 contains cytosine (C). Changing this nucleotide to guanine (G) changes the codon from **ACA to AGA**.

ACA encodes threonine, whereas AGA encodes arginine. Therefore, the mutation produces the protein change **p.Thr310Arg (T310R)**.

Although the protein length remains unchanged, replacing threonine with arginine changes the chemical properties of the amino acid at this position. Such a substitution can potentially affect protein structure, stability, or interactions with other components of the BCKD complex.

Experimental evidence reported by Wynn et al. (1998) for the corresponding mutation, which was referred to using an earlier numbering designation, showed impaired assembly and reduced stability of the E1 component. The study also reported no detectable enzyme activity for the mutant complex under the conditions examined.

BCKDHA encodes the E1 alpha subunit of the BCKD complex. Reduced BCKD activity can interfere with the normal metabolism of leucine, isoleucine, and valine, resulting in accumulation of branched-chain amino acids and related metabolites. These biochemical changes are associated with the metabolic and neurological manifestations of MSUD.

The computational analysis therefore identifies the DNA, codon, and predicted protein changes, while experimental evidence provides information about the possible functional effects of the documented mutation.

---

## 9. Artificial Mutation

A separate artificial mutation was introduced into the WT BCKDHA CDS to examine how a different type of nucleotide substitution could affect the predicted protein.

The artificial mutation was:

**c.303G>A**

This changed the codon:

**AAG → AAA**

Both AAG and AAA encode lysine (K). Therefore, the artificial mutation was predicted to be a **synonymous mutation**.

### Artificial Mutation Information

| Feature | Result |
|---|---|
| Gene | BCKDHA |
| Nucleotide change | c.303G>A |
| Original codon | AAG |
| Mutant codon | AAA |
| Amino-acid change | K → K |
| Mutation type | Synonymous |
| Frameshift | No |
| Premature stop | No |
| Predicted protein length | 445 aa |

The artificial mutation did not change the predicted amino-acid sequence.

---

## 10. Comparison of WT, Documented, and Artificial Mutants

| Feature | WT | Documented Mutation | Artificial Mutation |
|---|---|---|---|
| CDS length | 1,338 bp | 1,338 bp | 1,338 bp |
| Protein length | 445 aa | 445 aa | 445 aa |
| Mutation | None | c.929C>G | c.303G>A |
| Codon change | ACA | ACA → AGA | AAG → AAA |
| Mutation type | N/A | Missense | Synonymous |
| Reading frame changed? | No | No | No |
| Premature stop? | No | No | No |
| Amino acids affected | None | T310 → R310 | None (K → K) |
| Expected protein sequence effect | None | One amino-acid substitution | No predicted amino-acid change |

Both mutations were single-nucleotide substitutions, but they produced different predicted effects at the protein level. The documented mutation changed threonine to arginine at position 310, whereas the artificial mutation changed one lysine codon to another lysine codon without altering the predicted amino-acid sequence.

---

## 11. Interpretation Questions

### 32. Why does the location of a mutation within a gene matter?

The location of a mutation can determine which codon or part of the protein is affected. A mutation occurring in an important functional or structural region may have a greater effect on protein activity or stability than a change in a region that is less critical.

### 33. Why can a three-base deletion behave differently from a one- or two-base deletion?

A three-base deletion removes one complete codon and can remove a single amino acid without changing the reading frame. In contrast, deletion of one or two nucleotides shifts the reading frame and changes the downstream codons.

### 34. Does every nucleotide mutation change the amino-acid sequence?

No. Some nucleotide substitutions are synonymous and do not change the encoded amino acid. In this project, AAG changed to AAA, but both codons encode lysine.

### 35. Can a nucleotide substitution occur without destroying protein function?

Yes. The effect depends on the amino acid involved and its location within the protein. Some substitutions may have little effect, while others can alter protein structure, stability, interactions, or activity.

### 36. Why can a one-base deletion have a major effect on a protein?

A one-base deletion changes the reading frame. This can alter many downstream codons and may eventually introduce a premature stop codon, producing a substantially altered or shortened protein.

### 37. What is the effect of a premature stop codon?

A premature stop codon causes translation to terminate earlier than expected. The resulting protein may be shortened and may lack regions required for its normal structure or function.

### 38. Can a mutation change one amino acid without changing protein length?

Yes. The documented BCKDHA c.929C>G mutation is an example. It changes threonine to arginine at position 310 while the predicted protein remains 445 amino acids long.

### 39. Can a mutation cause disease without changing the protein sequence?

Yes. Mutations can affect regulatory regions, RNA splicing, mRNA stability, or gene expression. These changes can alter how much functional protein is produced even when the amino-acid sequence itself is unchanged.

### 40. What did the BCKDHA mutation analysis show?

The analysis showed that c.929C>G changes the codon from ACA to AGA and produces a Thr310Arg substitution. The CDS remained 1,338 bp and the predicted protein remained 445 amino acids long, with no frameshift or premature stop codon.

### 41. Which conclusions are directly supported by the computational analysis, and which require experimental evidence?

The computational analysis directly supports the nucleotide substitution, codon change, amino-acid substitution, protein length, and absence of a frameshift or premature stop codon. Effects on protein stability, complex assembly, enzyme activity, and clinical manifestations require experimental or clinical evidence.

---

## 12. Conclusion

This project demonstrated how a nucleotide change in the BCKDHA gene can be traced from the DNA sequence to a predicted protein change and then interpreted in relation to Maple Syrup Urine Disease.

The documented mutation, **c.929C>G**, changed the codon from ACA to AGA and resulted in a **Thr310Arg (T310R)** substitution. The predicted protein remained 445 amino acids long, indicating that the mutation did not cause a frameshift or premature stop codon. Published experimental evidence provides additional support that the corresponding mutation can affect the stability and assembly of the BCKD complex.

The artificial mutation, **c.303G>A**, produced a synonymous codon change from AAG to AAA. Because both codons encode lysine, the predicted protein sequence was unchanged.

Overall, the comparison illustrates that mutations affecting the same gene can have different consequences at the protein level. Sequence analysis can identify nucleotide and predicted amino-acid changes, while experimental evidence is needed to establish their effects on protein function and disease mechanisms.

---

## 13. Galaxy Analysis

The sequence analysis was performed using Galaxy and SeqKit Translate.

### Galaxy History

**History name:**  
`Deguit_MSUD_BCKDHA_Mutation_Lab`

### Main datasets used

- WT BCKDHA CDS
- WT BCKDHA predicted protein
- Documented BCKDHA mutant CDS
- Documented BCKDHA mutant predicted protein
- Artificial BCKDHA mutant CDS
- Artificial BCKDHA mutant predicted protein

---

## 14. Scientific References

1. NCBI. BCKDHA Gene. NCBI Gene.  
   https://www.ncbi.nlm.nih.gov/gene/593

2. MedlinePlus Genetics. BCKDHA gene. U.S. National Library of Medicine.  
   https://medlineplus.gov/genetics/gene/bckdha/

3. Strauss, K. A., et al. (2017). Maple syrup urine disease: mechanisms and management. *Molecular Genetics and Metabolism, 120*(1–2), 1–10.  
   https://pubmed.ncbi.nlm.nih.gov/28919799/

4. Wynn, R. M., Davie, J. R., Chuang, J. L., Cote, C. D., & Chuang, D. T. (1998). Impaired assembly of E1 decarboxylase of the branched-chain α-ketoacid dehydrogenase complex in type IA maple syrup urine disease. *Journal of Biological Chemistry, 273*(21), 13110–13118.  
   https://pubmed.ncbi.nlm.nih.gov/9582350/

5. Chuang, D. T., Chuang, J. L., & Wynn, R. M. (2000). Crystal structure of human branched-chain α-ketoacid dehydrogenase and the molecular basis of multienzyme complex deficiency in maple syrup urine disease. *Proceedings of the National Academy of Sciences, 97*(10), 5420–5425.  
   https://pubmed.ncbi.nlm.nih.gov/10745006/

6. NCBI ClinVar. NM_000709.4(BCKDHA):c.929C>G (p.Thr310Arg).  
   https://www.ncbi.nlm.nih.gov/clinvar/RCV002222336.14/

7. NCBI RefSeq. NM_000709.4 BCKDHA transcript.  
   https://www.ncbi.nlm.nih.gov/nuccore/NM_000709.4
