# Bioinformatics and Aesthetic Medicine  
## Deep Proteomic and microRNA Analysis of Lipedema and Cellulite

 **Bachelor’s Thesis – Bioinformatics**  
 **University of Verona**  
 **Author:** Michael Korsa Parkson Brew  
 **Academic Year:** 2024–2025  
 **Supervisor:** Alessandro Daducci  

---

## Project Overview

This thesis explores how **bioinformatics and computational analysis** can be used to investigate **lipedema**, a chronic adipose tissue disorder, and its molecular similarities with **cellulite**.

By integrating **proteomic data**, **microRNA expression analysis**, and **pathway enrichment**, the project aims to identify **potential biomarkers** and uncover shared and condition-specific biological mechanisms that may support diagnosis and future therapeutic strategies.

---

## Objectives

- Compare **proteomic profiles** of lipedema and cellulite tissues  
- Identify **shared and unique proteins** between the two conditions  
- Perform **pathway enrichment analysis** to uncover key biological processes  
- Analyze **extracellular microRNA expression** data  
- Identify **differentially expressed miRNAs** associated with lipedema  
- Predict **miRNA–mRNA regulatory interactions**  
- Integrate proteomic and miRNA results to propose **candidate biomarkers**

---

## Data Sources

- **Proteomics data**: UniProt protein identifiers derived from mass spectrometry  
- **microRNA dataset**:  
  - GEO accession **GSE138579**  
  - Extracellular miRNA profiles from stromal vascular fraction cells  
- **Databases & Tools**:
  - UniProt
  - GProfiler
  - TargetScan
  - miRDB
  - GEO (NCBI)

---

## Computational Pipeline

### 1. Proteomics Analysis
- Extraction and validation of UniProt protein IDs via API
- Identification of:
  - Lipedema-specific proteins
  - Cellulite-specific proteins
  - Shared proteins
- Visualization using **Venn diagrams**
- Functional enrichment using:
  - Gene Ontology (BP, MF, CC)
  - KEGG pathways

### 2. microRNA Data Processing
- Dataset cleaning and preprocessing
- Batch correction using **ComBat**
- Dimensionality reduction with **PCA**
- Differential expression analysis using **limma (R)** via Python–R integration
- Optimal threshold selection using **KneeLocator**

### 3. miRNA Target Prediction
- Selection of top dysregulated miRNAs:
  - **miR-136-3p** (downregulated)
  - **miR-31-5p** (downregulated)
  - **miR-133a-3p** (upregulated)
- Target prediction using:
  - TargetScan
  - miRDB
- Integration with proteomic results

---

## Key Results

- Significant **protein overlap** between lipedema and cellulite, suggesting shared molecular mechanisms  
- Lipedema-associated pathways enriched in:
  - Protein synthesis
  - Metabolic processes
  - Mitochondrial activity
- Cellulite-associated pathways enriched in:
  - Catabolic processes
  - Oxygen and gas transport
- Shared pathways related to:
  - Stress response
  - Tissue remodeling
  - Wound healing
- Identification of **candidate biomarkers**, including:
  - **FBN1**
  - **EPHX1**
  - **COX5A**
  - **HSPD1**
  - **CCT3**
  - **TMEM43**

---

## Technologies Used

- **Languages**: Python, R  
- **Libraries & Frameworks**:
  - pandas, numpy, matplotlib
  - scanpy, anndata
  - limma (Bioconductor)
  - rpy2
- **Statistical Methods**:
  - PCA
  - Batch correction (ComBat)
  - Differential expression analysis
- **Visualization**:
  - Venn diagrams
  - Bar plots
  - PCA plots

---

## License

This project is for **academic and research purposes**.




