---
layout: archive
title:
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
**University of Michigan – Ann Arbor**  
*Master of Science in Biostatistics | GPA: 3.860/4.0*

**Colorado State University - Fort Collins**  
*Master of Applied Statistics in Statistical Science | GPA: 3.904/4.0*

**Yanbian University**  
*Bachelor of Science in Statistics | AVG: 81.39/100*

Relevant Coursework
======
* Algebra & Geometry
* Probability & Distribution Theory
* Ordinary Differential Equation
* Stochastic Process
* Multivariate Statistical Analysis
* Machine Learning
* Data Visualization Methods
* Applied Bayesian Statistics
* Quantitative Reasoning
* Computing with Big Data
* Analysis of Categorical Data
* Biostatistics Inference
* Clinical Trials
* Theory and Application of Longitudinal Analysis

Technical Skills
======
**Languages:** English (Advanced), Mandarin (Native)

**Software:** Excel (Advanced), Python (Advanced), R (Advanced), SQL (Intermediate), C++ (Intermediate), Linux (Intermediate), Matlab (Intermediate)

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Work Expreience
======

**Data Analyst (STATCOM Project)**  
_Monroe County Senior Services_ — Ann Arbor, MI (Sep 2025 - Nov 2025)
- Analyzed 464 survey responses focusing on transportation access and relocation intentions, supporting senior mobility planning; engineered a clean 6-variable dataset via Python by handling missingness (12%–40%), harmonizing categorical levels, and removing noise for downstream analysis
- Quantified transportation conditions by developing percentage distributions, missing-rate diagnostics, and grouped comparisons, revealing that 88% reported no driving difficulty, while respondents without vehicle access were 3–5 times more likely to face mobility barriers, identifying transportation-vulnerable subpopulations
- Assessed relocation motivations and found 38% would move only for health reasons, while 45% cited eliminating outside maintenance as the top driver, uncovering core push-factors linked to aging-in-place decisions and environmental burden (e.g., house upkeep, accessibility)
- Built a visual results dashboard with bar charts, stacked 100% transportation comparisons, and relocation-reason ranking plots, enabling stakeholders to connect transportation barriers to relocation risk and prioritize interventions for older adults with limited mobility

**Graduate Research Assistant**  
_Medical School at University of Michigan_ — Ann Arbor, MI (May 2025 - July 2025)

- Conducted large-scale spatial transcriptomic analysis of normal and Alzheimer’s disease mouse brains using SPADE and Seurat, comparing Gaussian process–based spatial variance modeling with cluster-based differential expression. Identified 13,085 significant SV genes via SPADE versus 11,812 via Seurat, demonstrating SPADE’s higher sensitivity (80.4% vs. 36.6%) to localized spatial heterogeneity
- Designed and implemented a multi-stage preprocessing workflow integrating Seurat’s feature selection, log-normalization, and mitochondrial filtering with a custom 250 × 250 µm spatial binning algorithm, reducing data dimensionality from 32,285 × 3,500 to approximately 17000 × 660 while preserving spatial resolution and reducing SPADE runtime by approximately 40%
- Characterized AD-associated spatial dysregulation at both spot and domain scales: SPADE detected confined micro-regional upregulation in genes such as Tuba1c and Wbp1, while Seurat identified domain-level changes including the expansion of Domains 4 and 7 and contraction of Domains 3 and 8, revealing transcriptional reorganization in AD pathology
- Developed reproducible R and Python pipelines on the Great Lakes HPC cluster using Slurm-based modularization of SPADE, Seurat, and BASS components. Implemented automated likelihood-ratio testing, FDR control (BH method), and visualization of conflict genes, achieving scalable cross-validation across > 30000 genes and 7000 spots

**Graduate Research Assistant**  
_Department of Biostatistics at University of Michigan_ — Ann Arbor, MI (May 2025 - Present)
- Designed and implemented elliptical slice sampling algorithms in R for Bayesian parameter estimation, improving computational efficiency in posterior inference by 36% compared to sampling function
- Developed and validated a Multivariate Bayesian Shrinkage Prior (Mt-MBSP) model supporting mixed-type outcomes (continuous, binary, count) with Gibbs sampling  
- Conducted extensive simulation studies comparing Bayesian CRD, Bayesian CRD with imputation, and OLS, evaluating predictive accuracy and convergence via Gelman-Rubin diagnostics
- Applied Bayesian modeling frameworks to real and simulated datasets, generating reproducible analyses and visualizations that supported model validation and interpretation

**Data Analyst Intern**  
_China Everbright Bank, Changchun Branch_ — Changchun, China (Sep 2019 - Nov 2019)
- Collected and processed over 500 monthly economic indicators of Jilin Province and the whole country using SQL, automating data extraction, cleaning, and aggregation, which reduced manual processing time by 40% and enabled timely analysis of GDP drivers from fiscal and monetary policy perspectives
- Analyzed client transaction and portfolio data to identify risk profiles, recommended 3 customized wealth management products, which increased client product adoption by 15% and improved alignment with client investment needs  
- Employed Python to fit generalized and linear regression models on 2,000+ customer records, which improved prediction accuracy of satisfaction and deposit trends by 12%, supporting data-driven decision-making in customer service strategies

Research Experience
======

**Research on Pneumonia Patient Condition Classification Using Diffusion Models and CLIP**  
_Department of Biostatistics at University of Michigan_ — Ann Arbor, MI (Nov 2024 - Dec 2024)
- Deployed the stable Diffusion model and utilized Low-Rank Adaptation of Large Language Models (LoRA) to fine-tune the model to make it generate customized chest X-ray images based on a dataset of 5,856 radiographs
- Utilized the fine-tuned contrastive language-image pre-training (CLIP) model to achieve modest improvements in training accuracy, and the training accuracy improved from 48.94% to 50.51% 
- Collaborated with fellow analysts to process and analyze the graphical data with effective communication

**MLST: Statistical Regression Analysis R Package**  
_Department of Biostatistics at University of Michigan_ — Ann Arbor, MI (Oct 2024 - Nov 2024)
- Independently developed a statistical analysis tool, integrating residual standard error, coefficient of determination `R²`, adjusted coefficient of determination `Adjusted R²`, `F-test`, `T-test`, and 5+ regression diagnostic functions, improving the efficiency of model evaluation for 100+ potential users
- Validated various regression diagnostics and goodness-of-fit indices on simulated datasets of size `n=100`; results were highly consistent with built-in R functions, ensuring accuracy and reproducibility of the data analysis process 
- Authored HTML vignette and Rd documentation to visually demonstrate model evaluation workflows, significantly reducing users’ learning costs and shortening onboarding time by approximately 50%

**Research on Predictive Algorithms for Cardiovascular Disease**  
_Summer Research Seminar, Supervisor: R. Todd Ogden, Columbia University_ — Remote (May 2023 - July 2023)
- Utilized Principal Component Analysis (PCA) to identify relevant predictors and reduce dimensionality in a dataset with more than 4000 observations and 10 plus variables, implemented backward stepwise elimination to refine model features and prevent overfitting
- Developed random forest and logistic regression models on a dataset of 4,239 participants and 16 predictors from the Framingham Heart Study to assess CHD risk factors and support early detection  
- Evaluated models using confusion matrix and AUC-ROC metrics, showing that the optimized random forest achieved 82.1% accuracy, 83.1% sensitivity, 80.9% specificity, and an AUC of 0.82, outperforming logistic regression (67.1% accuracy, AUC 0.737) by 15% in accuracy and 0.083 in AUC for high-dimensional CHD data classification

**Familial Influences on Radiation Effects in Mice**  
_NASA Human Research Program, Weil Lab, Colorado State University_ — Fort Collins, CO (May 2022 – Aug 2022)
- Designed and fitted a generalized linear mixed model on a dataset of 1,200+ mice to analyze the relationship between Modified Merriam-Focht classification and radiation groups, improving model fit by 32% compared to baseline models
- Detected statistically significant differences in radiation effects between γ-rays and HZE nuclei using emmeans command, quantifying radiation-induced ocular damage with odds ratios up to 2.3  
- Conducted regression analysis in R showing that exposure to gamma rays increased the odds of vision impairment by 47%, providing evidence for dose-response effects in familial radiation sensitivity

**Application of Nonlinear Programming to Heat Conduction Model**  
_College of Science at Yanbian University_ — Yanji, China (August 2017 - October 2018)
- Established a nonlinear programming model to determine the optimal thickness (≈13 mm) of the second layer of high-temperature working clothes, given predictors like work hours and ambient temperature (65 °C), ensuring skin temperature ≤ 47 °C for 60 minutes
- Derived the functional relationship between temperature and material thickness using Fourier’s heat conduction law, and validated that simulated annealing reduced model error to less than 0.5% compared with exhaustive search  
- Implemented simulated annealing optimization, which improved solution efficiency by avoiding local optima, and confirmed cost-effective design by reducing unnecessary thickness by ~48% compared to the maximum tested thickness (25 mm)
