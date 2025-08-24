Gut Microbiota Dynamics in Response to Bile
Duct Ligation and FK10 Intervention
Overview
This project explores the impact of bile duct ligation (BDL) and probiotic FK10
treatment on gut microbiota composition and diversity using 16S rRNA sequencing. The
study evaluates microbial community responses, focusing on the abundance of
Prevotellaceae and overall ecological resilience over a 14-day period in murine
models.
Project Structure
gut_microbiota_project/ ├── data/ # Raw and processed sequencing data ├── scripts/ #
Python and shell scripts for analysis │ ├── qiime2_pipeline.qzv │ └──
statistical_analysis.py ├── results/ │ ├── alpha_diversity_plots/ │ ├──
beta_diversity_plots/ │ └── taxonomic_composition/ ├── summary/ │ ├── figures/ #
Summary figures for Prevotellaceae, PCoA plots, etc. │ └── report.pdf # PDF of key
findings └── README.md # Project documentation
Objectives
Assess the gut microbial composition under normal (sham) and BDL-induced
cholestasis conditions.
Examine the effect of FK10 intervention on microbial stability.
Monitor the abundance of Prevotellaceae and diversity metrics over time.
Visualize alpha and beta diversity changes using QIIME 2 plugins.
Statistically compare microbial metrics across experimental groups and time
points.
Methodology
1. Data Processing
QIIME 2 Pipeline:
Imported raw sequence reads.
Demultiplexed and trimmed adapters and low-quality bases.
Denoising and chimera filtering via DADA2 to obtain ASVs.
Taxonomic classification using a pre-trained Naïve Bayes classifier and
Greengenes database.
2. Statistical Analysis
Alpha Diversity: Shannon Entropy, Faith's Phylogenetic Diversity.
Beta Diversity: Jaccard and Bray–Curtis dissimilarity indices with PCoA
visualization.
Statistical Tests:
One-way ANOVA with Tukey’s post hoc test.
Repeated measures ANOVA for within-group changes.
Significance threshold: p < 0.05.

Key Findings
Prevotellaceae Resilience: Relative abundance remained stable or increased
across all experimental groups, even in BDL conditions.
Alpha Diversity: Increased diversity in BDL and FK10_BDL groups, indicating
microbial adaptation rather than dysbiosis.
Beta Diversity: No strong clustering observed, suggesting overlapping microbial
community structure despite specific taxonomic shifts.
Effect of FK10: Modulated microbiota composition subtly but did not prevent
BDL-induced changes.
Limitation: Relative abundance metrics used; absolute quantification is
recommended for follow-up studies.
Figures
Alpha Diversity (Shannon Index, Faith's PD)
Beta Diversity (PCoA plots)
Prevotellaceae Abundance Trends
Group-wise Comparative Taxonomy Charts
Ethics Statement
This research was approved by the Institutional Review Board (IRB) at Theodor Bilharz
Research Institute (TBRI), Cairo, Egypt.

Contact
Student Researcher: Reham Wael
Supervisors:
Dr. Marwa Amer, Lecturer, Department of Bioinformatics and Genomics
Dr. Rehab Abdallah, Lecturer, Department of Bioinformatics and Genomics
Affiliations:
Faculty of Biotechnology, Misr University for Science and Technology (MUST),
Cairo, Egypt
Theodor Bilharz Research Institute (TBRI), Giza, Egypt
Email: rehamwael110@gmail.com
