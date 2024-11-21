# Cystic Fibrosis Gene Variant Analysis and Biomarker Discovery

## Project Description
Cystic Fibrosis (CF) is a genetic disorder caused by mutations in the CFTR gene most commonly affecting individuals of European descent, particularly those of Northern European origin. It causes the production of abnormally thick mucus, leading to the blockage of the pancreatic ducts, intestines, and bronchi and often resulting in respiratory infection.It occurs in about 1 in 2,500 to 3,500 live births in the United States. The condition is caused by mutations in the CFTR gene, leading to thick mucus buildup in the lungs and digestive system. Approximately 1 in 25 to 1 in 30 people are carriers of the defective gene. While CF is less prevalent in African, Asian, and Hispanic populations, advancements in treatment have significantly improved life expectancy, with many individuals living into their 30s and 40s.This project explores the genetic variations associated with CF, their annotations, and functional implications. Our ultimate goal is to identify biomarkers that can aid in personalized medicine for CF. Using variant call format (VCF) files, bioinformatics tools, and functional annotation pipelines, we analyze the relationships between genetic mutations, clinical significance, and drug responses.

---

## Biological Background

Cystic Fibrosis is primarily caused by mutations in the *CFTR* gene, which encodes the cystic fibrosis transmembrane conductance regulator protein. This protein is essential for ion transport in epithelial cells. Variants in CFTR disrupt this process, leading to thickened mucus in the lungs, pancreas, and other organs. 

### Key Highlights:
- **Gene of Interest**: *CFTR* (Cystic Fibrosis Transmembrane Conductance Regulator)
- **Common Mutations**:
  - F508del
  - G551D
  - W1282X
  - N1303K
  - G542X
  - R117H
  - P574H
  - 2184delA
  - R334W
  - 3849+10kbC→T
  - S549N
- **Associated Drugs**:
  - Ivacaftor
  - Lumacaftor
  - Tezacaftor
  - Elexacaftor
- **Objective**: Identify biomarkers by analyzing the genetic variants and their impact on CFTR function and drug response.

---

## Project Workflow

### Workflow Steps:
1. **Disease Selection**:
   - Focus on Cystic Fibrosis as the genetic disorder of interest.
2. **Gene and Variant Selection**:
   - Identify CFTR gene mutations from public databases like dbSNP, PharmGKB, and ClinVar.
   - Annotate variants with functional and clinical relevance.
3. **Variant Annotation**:
   - Use tools like ANNOVAR, VEP, and SnpEff to annotate variants with:
     - Functional impact (e.g., missense, nonsense)
     - Clinical significance (e.g., pathogenic, likely benign)
     - Population frequency (e.g., gnomAD, 1000 Genomes)
4. **Biomarker Identification**:
   - Analyze data to identify genetic variants with strong correlations to drug response or disease severity.
5. **Data Visualization**:
   - Generate heatmaps, bar plots, and variant distribution graphs for insights.
   -This graph visualizes the relationship between drug efficacy and toxicity (on the Y-axis) against various CFTR mutations (on the X-axis). The data points represent the efficacy and toxicity values for each drug associated with specific mutations in Cystic Fibrosis patients.

      -**X-axis (Mutations)**: The different CFTR mutations that are associated with Cystic Fibrosis. These may include common mutations such as F508del, G551D, W1282X, N1303K, G542X, and R117H.
      - **Y-axis (Percentage)**: The percentage value representing drug efficacy and toxicity.
      - **Efficacy**: The percentage of how effective the drug is in treating the condition.
      - **Toxicity**: The percentage representing the side effects or toxicity level of the drug.

    -This graph helps visualize how different mutations in the CFTR gene affect the efficacy and toxicity of various drugs. It provides a comparison between drug performance and adverse effects across a range of genetic variations, which can be crucial in personalized medicine.
      - **Efficacy**: Represents the therapeutic     effectiveness of the drug in patients with specific mutations.
      - **Toxicity**: Represents the side effects or toxicity level experienced by patients due to the drug.
      - **Mutations**: Common CFTR gene mutations like F508del, G551D, and others.

6. **Validation**:
   - Compare findings against established biomarkers and clinical data.

---

## Tools and Databases

### Tools Used:
- **Python**: Data analysis and visualization.
- **R**: Statistical analysis and plotting.
- **VCF Tools**: Processing and analyzing VCF files.
- **ANNOVAR**: Functional annotation of genetic variants.
- **Variant Effect Predictor (VEP)**: Predicting the impact of variants.
- **SnpEff**: Variant annotation and effect prediction.

### Databases Used:
- **PharmGKB**: Pharmacogenomics knowledgebase.
- **dbSNP**: Repository of SNPs and genetic variants.
- **ClinVar**: Variants with clinical significance.
- **gnomAD**: Population allele frequency data.

---

## Folder Structure

### Folder Structure:
- **data/**: Contains raw data files (e.g., VCF, TXT, CSV).
- **scripts/**: Python/R scripts for analysis and annotations.
- **results/**: Contains outputs like annotated VCFs, graphs, and heatmaps.
- **docs/**: Documentation and reference materials.
- **README.md**: Project overview and instructions (this file).

---

## How to Run the Project

### Prerequisites:
1. Install Python or R:
   - Python: [Download](https://www.python.org/)
   - R: [Download](https://cran.r-project.org/)
2. Install Required Tools:
   - ANNOVAR: [Installation Guide](https://annovar.openbioinformatics.org/en/latest/)
   - VEP: [Installation Guide](https://www.ensembl.org/info/docs/tools/vep/index.html)
   - SnpEff: [Installation Guide](http://snpeff.sourceforge.net/)

---

### Steps to Run:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/cftr-biomarker-analysis.git
   cd cftr-biomarker-analysis

---

## Future Scope

### Extended Analysis
Expand the analysis to include additional genes and pathways involved in Cystic Fibrosis and other genetic disorders. This will provide a more comprehensive understanding of genetic factors contributing to CF and help identify new therapeutic targets.

### Machine Learning Models
Incorporate machine learning models to predict drug efficacy and disease progression based on genetic variants. This approach can help in making more accurate predictions and personalizing treatment options for patients.

### Clinical Validation
Validate the identified biomarkers using clinical datasets and experimental studies to confirm their potential in real-world applications. This will ensure that the biomarkers identified through the analysis are truly useful for clinical practice.

### Genome-wide Association Studies (GWAS)
Perform Genome-wide Association Studies (GWAS) to uncover novel genetic variants that may be implicated in Cystic Fibrosis or other related diseases. GWAS will help in discovering new genetic factors that contribute to disease susceptibility and treatment response.

### Integration with Electronic Health Records (EHR)
Integrate genetic data with Electronic Health Records (EHR) systems for personalized medicine applications. This integration can enable clinicians to make better-informed decisions based on a patient's genetic profile, improving treatment outcomes.

