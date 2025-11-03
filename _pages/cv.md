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
- Analyzed 464 senior mobility and relocation surveys from Monroe County, engineering a clean 6-variable dataset in Python through missingness handling (12%–40%), variable harmonization, and categorical level alignment. Produced complete frequency and cross-tab analyses for transportation, health, and planning behaviors
- Quantified transportation accessibility using cross-sectional diagnostics showing that 87.7% reported no driving difficulty, but respondents without vehicle access were twice as likely to face mobility barriers (≈53% moderate/major difficulty vs. 7% with vehicle access), revealing strong associations between transportation independence and quality of life
- Assessed relocation readiness and motivations, finding that 31% plan to move only if health declines, 27% prefer to never relocate, and the top self-reported motivator was eliminating outdoor maintenance (26.9%), followed by downsizing and accessibility upgrades. Integrated qualitative text analysis identified loss of independence and physical decline as major aging concerns
- Built visualization dashboards and summary reports combining percentage distributions, ranked relocation reasons, and cross-domain charts on transportation, planning, and senior engagement. Enabled Monroe County Senior Services to pinpoint high-risk subgroups and prioritize interventions improving mobility access, home maintenance support, and senior independence

**Graduate Research Assistant**  
_Medical School at University of Michigan_ — Ann Arbor, MI (May 2025 - July 2025)

- Conducted large-scale spatial transcriptomic analysis of normal and Alzheimer’s disease mouse brains using SPADE and Seurat, comparing Gaussian process–based spatial variance modeling with cluster-based differential expression. Identified 13,085 significant SV genes via SPADE versus 11,812 via Seurat, demonstrating SPADE’s higher sensitivity (80.4% vs. 36.6%) to localized spatial heterogeneity
- Designed and implemented a multi-stage preprocessing workflow integrating Seurat’s feature selection, log-normalization, and mitochondrial filtering with a custom 250 × 250 µm spatial binning algorithm, reducing data dimensionality from 32,285 × 3,500 to approximately 17000 × 660 while preserving spatial resolution and reducing SPADE runtime by approximately 40%
- Characterized AD-associated spatial dysregulation at both spot and domain scales: SPADE detected confined micro-regional upregulation in genes such as Tuba1c and Wbp1, while Seurat identified domain-level changes including the expansion of Domains 4 and 7 and contraction of Domains 3 and 8, revealing transcriptional reorganization in AD pathology
- Developed reproducible R and Python pipelines on the Great Lakes HPC cluster using Slurm-based modularization of SPADE, Seurat, and BASS components. Implemented automated likelihood-ratio testing, FDR control (BH method), and visualization of conflict genes, achieving scalable cross-validation across > 30000 genes and 7000 spots

**Graduate Research Assistant**  
_Department of Biostatistics at University of Michigan_ — Ann Arbor, MI (May 2025 - Present)
- Designed and implemented elliptical slice sampling algorithms in R for correlated Bayesian regression models, incorporating correlation-aware weight matrices and imputation for missing coefficients. Improved posterior mixing and inference efficiency by 36% compared to standard Metropolis–Hastings sampling through adaptive log-likelihood tuning and acceptance-rate diagnostics
- Developed and validated a Multivariate Bayesian Shrinkage Prior (Mt-MBSP) framework supporting mixed-type outcomes (continuous, binary, count) using Gibbs sampling. Implemented hierarchical shrinkage priors, automatic variance scaling, and posterior predictive sampling to yield stable recovery of sparse β structures across high-dimensional regressors  
- Conducted large-scale simulation studies (n = 50–100, p = 8–10) comparing Bayesian CRD, Bayesian CRD with imputation, and OLS, showing lower mean-squared error (1.12 vs. 1.16) and Gelman–Rubin PSRF ≈ 1.07 under both Spearman and Kendall discrepancies. Validated convergence across 1 000 MCMC iterations using diagnostic chains and trace-plot analyses
- Applied Bayesian frameworks to real and simulated datasets, integrating ROC/PR curve evaluation (AUC = 0.93, AP = 0.91) and residual analysis for predictive validation. Generated reproducible visualizations including posterior density plots, beta-correlation heatmaps, and cumulative mean trajectories to support interpretation of model stability and parameter convergence

**Data Analyst Intern**  
_China Everbright Bank, Changchun Branch_ — Changchun, China (Sep 2019 - Nov 2019)
- Collected and processed over 500 monthly economic indicators of Jilin Province and the whole country using SQL, automating data extraction, cleaning, and aggregation, which reduced manual processing time by 40% and enabled timely analysis of GDP drivers from fiscal and monetary policy perspectives
- Analyzed client transaction and portfolio data to identify risk profiles, recommended 3 customized wealth management products, which increased client product adoption by 15% and improved alignment with client investment needs  
- Employed Python to fit generalized and linear regression models on 2,000+ customer records, which improved prediction accuracy of satisfaction and deposit trends by 12%, supporting data-driven decision-making in customer service strategies

Research Experience
======

**Research on Pneumonia Patient Condition Classification Using Diffusion Models and CLIP**  
_Department of Biostatistics at University of Michigan_ — Ann Arbor, MI (Nov 2024 - Dec 2024)
- Deployed the Stable Diffusion v2 model integrating an 865 M-parameter U-Net with an OpenCLIP ViT-H/14 encoder to generate synthetic pediatric chest X-rays, addressing class imbalance in a dataset of 5,856 radiographs (1,349 normal / 1,345 viral / 2,538 bacterial). Applied noise-scheduling and forward–reverse diffusion processes to reconstruct high-fidelity 768 × 768 px images for under-represented classes
- Fine-tuned the model using Low-Rank Adaptation (LoRA) on the attention and projection layers of U-Net, freezing pretrained weights while optimizing two low-rank matrices (LoRA_A and LoRA_B). This reduced trainable parameters to ≈ 1% and lowered GPU memory requirements by ≈ 3×, enabling efficient image generation on a single RTX 3090 (24 GB) without compromising quality 
- Optimized and trained a multimodal CLIP ViT-L/14 model with LoRA-based projection fine-tuning using the combined real plus synthetic dataset. Designed structured natural-language prompts (“An image of [Type] chest X-ray”) to improve image–text alignment. Achieved consistent training accuracy gains (48.94 to 50.47 %), F1-score increase (47.25 to 48.91 %), and recall improvement (48.65 to 50.56 %) across three epochs
- Evaluated and interpreted model performance, showing that diffusion-based synthetic augmentation improved feature diversity and class representation, while CLIP’s cosine-similarity-based multimodal learning enhanced interpretability over CNN baselines. Proposed future improvements via consistency models (≈ 50× faster diffusion) and reinforcement fine-tuning (DPO/PPO) for robust radiographic classification under limited data settings

**MLST: Statistical Regression Analysis R Package**  
_Department of Biostatistics at University of Michigan_ — Ann Arbor, MI (Oct 2024 - Nov 2024)
- Designed and implemented the MLST R package to automate statistical evaluation of linear regression models, integrating five diagnostic modules—Residual Standard Error, R², Adjusted R², F-test, and T-test—for model accuracy assessment and performance interpretation across multiple predictors. Packaged functions were optimized for compatibility with matrix-based predictors and numeric responses
- Programmed and tested core computational functions (RSE(), Rsquared(), ADJRS(), Ftest(), Ttest()), each returning structured numeric outputs (estimates, standard errors, F/t statistics, p-values, degrees of freedom) equivalent to results from R’s summary(lm()), while improving reproducibility and user transparency through simplified function syntax and modular code design 
- Validated regression diagnostics and model-fit indices on simulated datasets (n = 100) by replicating canonical linear regression scenarios with varying numbers of predictors. Achieved 1:1 concordance with built-in R analytical routines and verified stability under Monte Carlo simulations, confirming numerical precision and algorithmic efficiency for teaching and applied research contexts
- Authored a comprehensive documentation suite, including HTML vignettes and .Rd help pages, illustrating reproducible code workflows for regression analysis. Integrated GitHub installation (remotes::install_github("Umichyingzhen/MLST")) and vignette browsing (browseVignettes("MLST")), reducing onboarding time by ≈50% and enhancing accessibility for graduate students and applied analysts

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
