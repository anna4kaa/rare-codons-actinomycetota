## 📁 Repository Structure

### 1️⃣ Genome Selection and tRNA Analysis
| Notebook | Description |
|-----------|-------------|
| `1.1_Representative_genome_selection_MASH.ipynb` | Selects representative genomes per genus based on **MASH** results. |
| `1.2_Number_of_tRNAs_AGA_TTA.ipynb` | Counts tRNAs decoding **AGA** and **TTA** codons across all genomes. |

---

### 2️⃣ Codon Counting and Localization
| Notebook | Description |
|-----------|-------------|
| `2.1_Codon_counts_and_positions.ipynb` | Computes codon usage frequencies and positional information per gene. |
| `2.2_Codon_location_heatmap.ipynb` | Generates heatmaps showing positional distribution of codons across genomes. |
| `2.3_TTA_codons_genbank.ipynb` | Extracts and annotates genes containing **TTA** codons from GenBank files. |

---

### 3️⃣ Codon Rarity and Correlation Analyses
| Notebook | Description |
|-----------|-------------|
| `3.1_Normalized_rarity_calculation.ipynb` | Calculates normalized codon rarity. |
| `3.2_Correlation_between_rarity_and_position.ipynb` | Calculates correlations between codon rarity and position. |

---

### 4️⃣ Association of Rare Codons with BGCs
| Notebook | Description |
|-----------|-------------|
| `4.1_antiSMASH_summary_per_genus.ipynb` | Summarizes **antiSMASH** predictions and BGC counts per genus. |
| `4.2_TTA_genes_among_BGCs.ipynb` | Identifies TTA-containing genes located within BGCs. |
| `4.3_Analysis_BGC_vs_non_BGC.ipynb` | Created dataframes with summaries for TTA genes among BGCs and BGC genes within TTA containing genes. |
| `4.4_TTA_genes_among_BGCs` | Generates summary figures among all genera for BGCs containing TTA genes. |
| `4.5_Hypergeometric_test_BGCs.ipynb` | Performs hypergeometric enrichment tests for TTA codon overrepresentation in BGCs. |
| `4.6_Fishers_test_gene_categories_BGC_TTA.ipynb` | Applies Fisher’s exact tests to evaluate enrichment of TTA genes among BGC gene kinds (biosynthetic, biosynthetic-additional,
transport, regulatory, etc.). |

---

### 5️⃣ Functional Enrichment (COG-Level Analyses)
| Notebook | Description |
|-----------|-------------|
| `5.1_COG_TTA_containing_genes.ipynb` | Maps TTA-containing genes to COG functional categories. |
| `5.2_Hypergeometric_test_COG_TTA.ipynb` | Tests overrepresentation of COG categories among TTA-containing genes. |
| `5.3_COG_TTA_containing_genes_position_0.ipynb` | Analyzes positional patterns of TTA codons in genes across COG categories. |
| `5.4_Hypergeometric_test_COG_TTA_position_0.ipynb` | Statistical tests enrichment in position 0 of TTA codons within COG functions. |

---


## ⚙️ Requirements

Dependencies:
```bash
python >= 3.8
pandas
numpy
matplotlib
seaborn
biopython
scipy
matplotlib.pyplot
glob
os
