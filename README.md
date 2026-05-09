# NADbinder: Identification of NAD Interacting Residues in Proteins

## Overview

NADbinder is a computational platform developed for predicting NAD interacting residues (NIRs) in proteins using amino acid sequence information and machine learning techniques.

The method predicts:

- NAD binding proteins (NADBP)
- NAD interacting residues (NIRs)

without requiring structural information.

---

## Research Paper

**Title:** Identification of NAD interacting residues in proteins

**Authors:** Hifzur R Ansari and Gajendra P. S. Raghava

**Journal:** BMC Bioinformatics (2010)

**DOI:** https://doi.org/10.1186/1471-2105-11-160
https://doi.org/10.5281/zenodo.20092526

---

## Background

Nicotinamide adenine dinucleotide (NAD⁺) is an important cofactor involved in:

- Cellular metabolism
- Energy transfer
- Signal transduction
- Regulatory pathways

NAD binding proteins play critical roles in many biological functions and diseases.

Traditional similarity-based approaches were limited in identifying all NAD binding proteins, especially non-classical proteins lacking Rossmann fold motifs.

NADbinder was developed to overcome these limitations using sequence-based computational prediction.

---

## Dataset Information

The dataset was obtained from:

- Protein Data Bank (PDB)
- SuperSite database
- Ligand Protein Contact (LPC) server

### Dataset Statistics

- 555 NAD binding proteins analyzed
- 1556 protein chains extracted
- 195 non-redundant protein chains selected
- 4772 NAD interacting residues identified

Redundancy reduction was performed using CD-HIT at 40% sequence identity.

---

## Machine Learning Models

### Support Vector Machine (SVM)

Models were developed using:

- Amino acid binary patterns
- Evolutionary information (PSSM profiles)

---

## Binary Pattern Model

### Best Performance

- Window size: 17
- Accuracy: 74.13%
- MCC: 0.47

---

## PSSM-Based Model

### Best Performance

- Window size: 19
- Accuracy: 87.25%
- MCC: 0.75

Evolutionary profiles significantly improved prediction accuracy.

---

## Important Residues

Residues enriched in NAD interacting regions include:

- Glycine (Gly)
- Histidine (His)
- Threonine (Thr)
- Serine (Ser)
- Tyrosine (Tyr)

---

## ROC Analysis

ROC analysis showed:

- Best sequence-based model at window size 17
- Best PSSM model at window size 19

PSSM-based models showed superior prediction performance.

---

## Web Server Features

The NADbinder server allows users to:

- Submit protein sequences in FASTA format
- Predict NAD interacting residues
- Select prediction thresholds
- Analyze unknown proteins

---

## Technologies Used

- SVM_light
- PSI-BLAST
- CD-HIT
- PSSM profiles
- Linux computational environment

---

## Applications

NADbinder can be used for:

- Functional annotation of proteins
- Cofactor binding prediction
- Structure-function studies
- Drug target analysis
- Computational biology research

---

## Availability

The web server is freely available for academic research.

Server URL:

http://www.imtech.res.in/raghava/nadbinder/

---

## Contact

### Prof. Gajendra P. S. Raghava

Department of Computational Biology  
Indraprastha Institute of Information Technology Delhi  
New Delhi, India

Email: raghava@iiitd.ac.in

---

## License

Creative Commons Attribution License

---

Generated from the uploaded NADbinder research paper.
