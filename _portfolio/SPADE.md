---
title: "Research on gene expression in the mouse brain using SPADE for Alzheimer’s disease"
excerpt: " Investigated differential gene expression in Alzheimer’s disease mouse brains using spatial transcriptomics. By applying SPADE and Seurat, we identify spatially variable genes, compare detection sensitivity, and reveal complementary insights into disease-associated spatial expression patterns."
collection: portfolio
date: 2025-07-05
---

This study applies spatial transcriptomics to analyze gene expression in Alzheimer’s disease mouse brains. SPADE and Seurat are used to identify spatially variable genes and to evaluate their relative sensitivity. The analysis highlights both overlapping and method-specific detections, showing that the two approaches provide complementary perspectives on spatial gene expression relevant to Alzheimer’s pathology.

---

### 🧠 Project Summary

- **Dataset**: The dataset contains spatial transcriptomics profiles from Alzheimer’s disease and normal mouse brain sections, with 3541 spatial spots and 32285 gene expression counts measured.
- **Key Methods**: SPADE for normalization and spatially variable gene detection; Seurat for preprocessing, clustering, and differential expression; BASS for multi-sample spatial domain alignment; visualization of spatial gene expression patterns using ggplot2; Capping algorithm for reducing computational burden.  
- **Main Finding**: SPADE showed higher sensitivity for detecting localized spatial expression differences, while the Seurat+BASS framework captured broader domain-specific gene expression. About 37% of significant genes differed between methods, reflecting their complementary strengths and methodological differences.

---

### 🧾 Dataset Results Overview

[`Binned Alzheimer’s disease coordinate information`](/files/ad_binned_coords.csv)

[`Binned normal brain tissue coordinate information`](/files/normal_binned_coords.csv)

[`Alzheimer’s disease and normal brain tissue gene expression information`](/files/binned_expr_matrix.zip)

[`Spatial variance (SV) genes detection results (Likelihood Ratio Tests)`](/files/LRT_results.csv)

---

### 🔁 Data Visualization Results

<img src="/files/Spatial_Domain_Facet.png" alt="Comparison of Spatial Domain Distributions in AD versus Normal mouse brain" style="width:100%;"/>
  
> - Domain 4 and Domain 7 expanded in AD compared to WT (p < 0.05)  
> - Domain 3 and Domain 8 showed shrinkage or relocation (p < 0.05)  
> - Spatial reorganization indicates potential degeneration in AD pathology

<img src="/files/Domain_Size_vs_R.png" alt="" style="width:100%;"/>
  
> -  
> -  
> - 

---

### 📎 Full Report

👉 [Download Full Report (PDF)](/files/Application of SPADE and Seurat to Between Group Expression.pdf)

---
 
