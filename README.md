![image](https://github.com/user-attachments/assets/c8f408d4-3f11-4c67-a3b6-7c4442f410e3)

# BiotrAIn course: Concepts, approaches and applications of Artificial Intelligence in bioscience

### Pilot Course: June 16-20, 2025 - San José, Costa Rica

## Aditional dataset: TCGA cancer data for Clustering Classification

### Collaborators

Juan Antonio Bizzotto, Universidad de Buenos Aires

# Introduction to The Cancer Genome Atlas (TCGA)

The Cancer Genome Atlas (TCGA) is a landmark project that transformed the landscape of cancer research through large-scale, multi-omic profiling of tumors. Initiated in 2006 as a joint effort between the National Cancer Institute (NCI) and the National Human Genome Research Institute (NHGRI), TCGA was established to catalog the genetic and molecular alterations responsible for cancer. Over its decade-long span, the project generated a comprehensive collection of datasets—including whole-genome and exome sequencing, transcriptomics (RNA-Seq), DNA methylation, copy number variation, and clinical annotations—for over 11,000 tumor samples across 33 distinct cancer types [1,2].

TCGA has profoundly advanced our understanding of molecular heterogeneity both within and across cancer types. Its findings have led to the identification of novel cancer subtypes, the discovery of actionable molecular targets, and a deeper appreciation of the complex genomic landscapes that underlie tumorigenesis and treatment response [3]. The rigorous standardization of data generation, processing, and annotation protocols has established TCGA datasets as a gold standard in cancer genomics, enabling reproducible and comparative analyses across diverse studies.

Beyond its biological insights, TCGA has played a pivotal role in advancing machine learning (ML) and artificial intelligence (AI) in biomedical research. The sheer volume, high dimensionality, and multi-modal nature of TCGA data make it an ideal benchmark for developing, validating, and testing algorithms for unsupervised clustering, supervised classification, feature selection, and survival prediction. These datasets have been instrumental in training AI systems to identify cancer subtypes, predict patient outcomes, and integrate multi-omic data for precision oncology [4,5].

Today, TCGA remains an invaluable resource for the global scientific community. Its impact extends beyond cancer biology, fostering innovation in data science, bioinformatics, and translational medicine. By making these high-quality datasets publicly accessible through platforms like the Genomic Data Commons (GDC), TCGA has democratized cancer research, empowering a global ecosystem of scientists to push the boundaries of ML and AI applications in oncology and beyond.

## References

1.  Tomczak, K., Czerwińska, P., & Wiznerowicz, M. (2015). The Cancer Genome Atlas (TCGA): an immeasurable source of knowledge. *Contemporary Oncology*, 19(1A), A68–A77. https://doi.org/10.5114/wo.2014.47136
2.  Weinstein, J. N., et al. (2013). The Cancer Genome Atlas Pan-Cancer analysis project. *Nature Genetics*, 45(10), 1113–1120. https://doi.org/10.1038/ng.2764
3.  Hoadley, K. A., et al. (2018). Cell-of-Origin Patterns Dominate the Molecular Classification of 10,000 Tumors from 33 Types of Cancer. *Cell*, 173(2), 291–304.e6. https://doi.org/10.1016/j.cell.2018.03.022
4.  Kourou, K., et al. (2015). Machine learning applications in cancer prognosis and prediction. *Computational and Structural Biotechnology Journal*, 13, 8–17. https://doi.org/10.1016/j.csbj.2014.11.005
5.  Huang, C., et al. (2021). Artificial intelligence in cancer diagnosis and prognosis: Opportunities and challenges. *Cancer Letters*, 505, 37–44. https://doi.org/10.1016/j.canlet.2021.01.014

---

# Pan-Cancer Analysis in TCGA

The Pan-Cancer initiative within The Cancer Genome Atlas (TCGA) project represents a paradigm shift in understanding cancer, moving beyond traditional tissue-of-origin classifications. Instead of treating each cancer as a distinct disease, the Pan-Cancer approach integrates multi-omic data across a wide array of tumor types to reveal shared molecular characteristics and unifying biological principles.

A key finding from Pan-Cancer analyses is that tumors from different tissues can share striking molecular similarities, while tumors from the same tissue can exhibit highly distinct molecular subtypes. This insight has profound implications for cancer taxonomy, drug development, and the implementation of personalized treatment strategies [1,2].

A core methodology in these efforts is the application of unsupervised clustering techniques—such as hierarchical clustering, k-means, and non-negative matrix factorization (NMF)—to group tumors based on their molecular profiles. These methods allow researchers to discover latent patterns and structure within high-dimensional data, often revealing novel cancer subtypes or classifying tumors based on fundamental biological processes rather than their anatomical site of origin [3].

For example, while gene expression profiles carry strong tissue-specific signals, they also harbor pan-cancer signatures reflective of processes like cell proliferation, immune infiltration, or metabolic reprogramming. Studies have successfully identified transcriptomic clusters that span multiple tumor types and are associated with prognostically relevant features, such as mesenchymal transformation or immune evasion phenotypes [4].

Pan-Cancer clustering analysis serves not only as a powerful exploratory tool but also as a foundation for dimensionality reduction, feature extraction, and subsequent supervised learning tasks. It is particularly effective for identifying tumors with overlapping molecular features, discovering outlier samples, and building robust multi-class models that respect the biological complexity of the data. This framework is increasingly being leveraged with modern machine learning and deep learning techniques to enhance scalability, interpretability, and predictive power [5].

For students of biology and data science, the TCGA Pan-Cancer datasets offer a compelling case study of how integrative data analysis can reshape our understanding of a complex disease. These datasets, accessible via portals like the Genomic Data Commons, are ideal for hands-on exploration of clustering methods, enabling the visualization and quantification of both inter- and intra-tumor heterogeneity in a biologically meaningful context.

## References

1.  Hoadley, K. A., et al. (2014). Multiplatform analysis of 12 cancer types reveals molecular classification within and across tissues of origin. *Cell*, 158(4), 929–944. https://doi.org/10.1016/j.cell.2014.06.049
2.  Hoadley, K. A., et al. (2018). Cell-of-Origin Patterns Dominate the Molecular Classification of 10,000 Tumors from 33 Types of Cancer. *Cell*, 173(2), 291–304.e6. https://doi.org/10.1016/j.cell.2018.03.022
3.  Ding, L., et al. (2018). Perspective on Oncogenic Processes at the End of the Beginning of Cancer Genomics. *Cell*, 173(2), 305–320.e10. https://doi.org/10.1016/j.cell.2018.03.033
4.  Thorsson, V., et al. (2018). The immune landscape of cancer. *Immunity*, 48(4), 812–830.e14. https://doi.org/10.1016/j.immuni.2018.03.023
5.  Yuan, Y., et al. (2014). Assessing the clinical utility of cancer genomic and proteomic data across tumor types. *Nature Biotechnology*, 32(7), 644–652. https://doi.org/10.1038/nbt.2940

---

# Classification Using the TCGA-PRAD Dataset

Prostate adenocarcinoma (PRAD) is one of the most prevalent cancers in men worldwide and presents a major clinical challenge due to its heterogeneous clinical course, which ranges from indolent, slow-growing tumors to aggressive, metastatic disease. The TCGA-PRAD dataset, part of The Cancer Genome Atlas initiative, provides a comprehensive molecular and clinical characterization of primary prostate tumors. This dataset includes genomic, transcriptomic, epigenomic, and proteomic profiles for nearly 500 patients, enabling deep investigation into the disease's biology.

The TCGA-PRAD project has fueled significant advances in understanding prostate cancer subtypes by identifying key genomic alterations such as *TMPRSS2-ERG* gene fusions, *PTEN* loss, and mutations in *SPOP* and *IDH1*. These molecular features complement traditional clinicopathological parameters and provide critical insights into tumor aggressiveness and progression [1,2].

In terms of clinical variables, TCGA-PRAD includes several features essential for prognostic evaluation. The **Gleason score** is a cornerstone of prostate cancer grading, derived from the histopathological analysis of tumor differentiation. Scores range from 6 to 10, with higher scores indicating more poorly differentiated and aggressive tumors [3].

Another critical clinical measure is **Prostate-Specific Antigen (PSA)**, a serum biomarker widely used for screening and disease monitoring. While elevated PSA levels at diagnosis can indicate disease presence, its utility is limited by a lack of specificity, as levels can also be raised by benign conditions.

The dataset also captures **pathological and clinical staging** (e.g., T2, T3, N0, M0), which describes tumor size, lymph node involvement, and distant metastasis. These variables are essential for determining the extent of the disease and guiding treatment decisions. Finally, **biochemical recurrence (BCR)**—defined as a rising PSA level after definitive local therapy—is a key clinical endpoint available in the dataset. This makes BCR an ideal target for supervised machine learning models designed to predict the risk of relapse [4].

The rich integration of molecular and clinical data in the TCGA-PRAD dataset provides an ideal testbed for classification tasks. Using machine learning, researchers can aim to predict clinical outcomes like recurrence, stratify patients by risk level, or identify molecular subgroups with therapeutic implications, ultimately advancing the goal of personalized medicine in prostate cancer.

## References

1.  Cancer Genome Atlas Research Network. (2015). The Molecular Taxonomy of Primary Prostate Cancer. *Cell*, 163(4), 1011–1025. https://doi.org/10.1016/j.cell.2015.10.025
2.  Armenia, J., et al. (2018). The long tail of oncogenic drivers in prostate cancer. *Nature Genetics*, 50(5), 645–651. https://doi.org/10.1038/s41588-018-0078-z
3.  Epstein, J. I., et al. (2016). The 2014 ISUP Gleason Grading System: Definition and Implications. *European Urology*, 69(3), 428–435. https://doi.org/10.1016/j.eururo.2015.06.046
4.  Ross-Adams, H., et al. (2015). Integration of copy number and transcriptomics provides risk stratification in prostate cancer: A discovery and validation cohort study. *EBioMedicine*, 2(9), 1133–1144. https://doi.org/10.1016/j.ebiom.2015.07.017
