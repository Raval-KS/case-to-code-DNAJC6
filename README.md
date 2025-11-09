# Case-to-Code: Transcriptomic Dissection of DNAJC6-Linked Early-Onset Parkinsonism

# NOTICE: Manuscript in Preparation

This analysis is part of a manuscript currently being prepared for submission:

**Title:** "Integrative Multi-Omic Analysis Reveals Synaptic Vesicle Recycling Failure and Neurodevelopmental Reprogramming in DNAJC6 Developmental Parkinsonism"

**Authors:** Raval KS, et al.

**Status:** Manuscript in preparation for bioRxiv submission

**Key Findings:** This work identifies novel lncRNA regulatory networks, 
including the DLX6-AS1 → DLX6 regulatory module, in DNAJC6 parkinsonism.

**Copyright:** © 2025 Raval Kush. All rights reserved.

**Note:** This work represents original research conducted by Raval Kush. Unauthorized use or reproduction of these findings without 
proper attribution constitutes academic misconduct.

**Contact:** raval.kush.sci@gmail.com

**DOI:** [Will be added upon preprint submission]

Last Updated: 09/11/25




This repository contains the full computational analysis for a "Case-to-Code" project investigating the molecular mechanisms of Infantile Parkinsonism (IPD) linked to *DNAJC6* mutations.

The analysis begins with a clinical case and proceeds to a full transcriptomic re-analysis of a public iPSC-derived neuron dataset (GSE208353), moving from raw data to a complete regulatory hypothesis.

###  viewing the Report

The final, self-contained report can be viewed directly in your browser:
https://raval-ks-case2code-dnajc6.netlify.app/

Alternatively, you can download and open the `code-c2c-ipd.html` file locally.

### Key Findings

This analysis identifies a "Core Signature" of 957 genes that are robustly dysregulated across all patient lines. The key mechanistic conclusions are:

1.  **A Failure of Neurodevelopment:** The Core Signature is dominated by a catastrophic failure of neurodevelopmental and synaptic programs (e.g., `GO:axonogenesis`, `KEGG:Neuroactive ligand-receptor interaction`).
2.  **A Dual Regulatory Collapse:** This failure is driven by a complex, multi-layered regulatory network, including the validated repression of key TFs like **`EGR1`** and the activation of the stress-response TF **`ATF4`**.
3.  **A Novel lncRNA Axis:** The analysis uncovered a novel lncRNA, **`DLX6-AS1`**, as the most significant non-coding gene. Its up-regulation is strongly anti-correlated (r ≈ -0.86) with the down-regulation of the `DLX` family of TFs.
4.  **IPD is Distinct from PD:** The final validation against a post-mortem adult-onset Parkinson's dataset (GSE114517) showed **zero correlation (rho ≈ 0)**. This is a major finding, suggesting IPD is a *developmental* synaptopathy, mechanistically distinct from *degenerative* adult-onset PD.

### Repository Contents

* `code-c2c-ipd.qmd`: The full, commented Quarto source code used to generate the analysis.
* `code-c2c-ipd.html`: The final, self-contained, interactive HTML report.
* `*.csv`: Key outputs from the analysis, such as the list of significant TFs, discovered lncRNAs, and HPA validation hits.
* `AF-O75061-F1-model_v6.pdb`: The AlphaFold protein structure for *DNAJC6* (Auxilin).

### Data Sources

* **Primary Data:** GSE208353
* **Validation Data:** GSE114517
