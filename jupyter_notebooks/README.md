## 📁 Repository Structure

### 1️⃣ Genome Selection and tRNA Analysis
| Notebook | Description |
|-----------|-------------|
| `1.1_Representative_genome_selection_MASH.ipynb` | Selects representative genomes per genus using **MASH** for distance-based clustering. |
| `1.2_Number_of_tRNAs_AGA_TTA.ipynb` | Counts tRNAs decoding **AGA** and **TTA** codons across genomes. |

---

### 2️⃣ Codon Counting and Localization
| Notebook | Description |
|-----------|-------------|
| `2_Codon_counts_and_positions.ipynb` | Computes codon usage frequencies and positional information per gene. |
| `3_Codon_location_heatmap.ipynb` | Generates heatmaps showing positional distribution of codons across genomes. |
| `4_TTA_codons_genbank.ipynb` | Extracts and annotates genes containing **TTA** codons from GenBank files. |

---

### 3️⃣ Codon Rarity and Correlation Analyses
| Notebook | Description |
|-----------|-------------|
| `5.1_Normalized_rarity_calculation.ipynb` | Calculates normalized codon rarity indices across taxa. |
| `5.2_Correlation_between_rarity_and_position.ipynb` | Tests correlations between codon rarity and positional enrichment within genes. |

---

### 4️⃣ Association of Rare Codons with BGCs
| Notebook | Description |
|-----------|-------------|
| `6.1_antiSMASH_summary_per_genus.ipynb` | Summarizes **antiSMASH** predictions and BGC counts per genus. |
| `6.2_TTA_genes_among_BGCs.ipynb` | Identifies TTA-containing genes located within or near BGCs. |
| `6.3_Analysis_BGC_vs_non_BGC.ipynb` | Compares codon composition between BGC and non-BGC genes. |
| `6.4_TTA_genes_among_BGCs` | Extended analysis of TTA-containing genes within BGC regions. |
| `6.5_Hypergeometric_test_BGCs.ipynb` | Performs hypergeometric enrichment tests for TTA codon overrepresentation in BGCs. |
| `6.6_Fishers_test_gene_categories_BGC_TTA.ipynb` | Applies Fisher’s exact tests to evaluate enrichment of COG categories among BGC-associated TTA genes. |

---

### 5️⃣ Functional Enrichment (COG-Level Analyses)
| Notebook | Description |
|-----------|-------------|
| `7.1_COG_TTA_containing_genes.ipynb` | Maps TTA-containing genes to COG functional categories. |
| `7.2_Hypergeometric_test_COG_TTA.ipynb` | Tests overrepresentation of COG categories among TTA-containing genes. |
| `7.3_COG_TTA_containing_genes_position_0.ipynb` | Analyzes positional patterns of TTA codons in genes across COG categories. |
| `7.4_Hypergeometric_test_COG_TTA_position_0.ipynb` | Statistical tests for positional enrichment of TTA codons within COG functions. |

---

## 📊 Output Summary

The notebooks generate:
- Codon usage matrices and rarity indices per genome.  
- Genome-wide visualizations of codon positions.  
- Lists of TTA-containing genes and their genomic contexts.  
- Enrichment statistics linking rare codons to BGCs and gene functions.  

---

## ⚙️ Requirements

Typical dependencies include:
```bash
python >= 3.8
pandas
numpy
matplotlib
seaborn
biopython
scipy
statsmodels
