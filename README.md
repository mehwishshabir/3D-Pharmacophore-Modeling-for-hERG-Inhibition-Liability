# 3D Pharmacophore Modeling for hERG Inhibition Liability

[![Software: MOE](https://img.shields.io/badge/Software-MOE%20(CCG)-blue)](https://www.chemcomp.com/)
[![Field: Cheminformatics](https://img.shields.io/badge/Field-Cheminformatics%20%2F%20Toxicology-green)](#)
[![Compliance: FDA Standards](https://img.shields.io/badge/Compliance-FDA%20Safety-orange)](#)

## 📌 Project Overview
This project involves the development and validation of a high-fidelity 3D pharmacophore model designed to identify inhibitors of the **hERG (human Ether-à-go-go-Related Gene)** potassium channel. 

Inhibition of the hERG channel is a critical "anti-target" in drug discovery. Unintended binding can lead to **Long QT Syndrome**, *Torsades de Pointes* (TdP), and sudden cardiac arrest. This model serves as a computational "safety gate" to filter out cardiotoxic leads early in the virtual screening process, ensuring candidates meet **FDA regulatory safety standards**.



---

## 🔬 Computational Methodology
The workflow followed a rigorous medicinal chemistry protocol within the **Molecular Operating Environment (MOE)**:

1.  **Conformational Sampling:** Developed a `db_ConfPack` database to capture the structural flexibility of known hERG ligands.
2.  **Training Template Selection:** Utilized a high-affinity inhibitor ($EC_{50}: 0.0267\text{ nM}$) as the structural anchor for the 3D hypothesis.
3.  **Pharmacophore Mapping:** Identified a multi-feature consensus including:
    * **Hydrogen Bond Donors/Acceptors** (Polar interactions)
    * **Hydrophobic Envelopes** (Lipophilic interactions)
    * **Aromatic Rings** ($\pi-\pi$ stacking interactions)
4.  **Validation:** Evaluated the model against a curated dataset of known actives and inactives to ensure predictive reliability.

---

## 📊 Model Validation & Performance
The model was optimized to prioritize high sensitivity, ensuring that potential cardiotoxins are accurately flagged.

### Statistical Summary
| Metric | Performance |
| :--- | :--- |
| **Accuracy** | 86.67% |
| **Sensitivity (Recall)** | 88.89% |
| **Specificity** | 83.33% |



### Structural Reliability
Validation confirmed that approximately **87% of active compounds** aligned with the 3D hypothesis in a consistent spatial orientation, reinforcing the binding mode hypothesis used for the query.

---

## 🧪 Virtual Screening & Toxicity Prediction
The validated model was deployed to assess the hERG liability of an "Unknown" dataset. 

* **Hit Identification:** Molecules were ranked based on **Root Mean Square Deviation (RMSD)** to the pharmacophore features.
* **Significant Findings:** Two molecules (Mol 1 and Mol 7) showed high structural complementarity to the hERG inhibitory query.
* **Safety Decision:** Based on the high liability scores and predicted interaction with the hERG channel, these molecules were **rejected** from the drug discovery pipeline to mitigate clinical cardiotoxicity risks.



---

## 🛠 Tools & Technical Skills
* **Software:** Molecular Operating Environment (MOE)
* **Core Competencies:** Conformational Search, 3D Pharmacophore Query Construction, Virtual Screening, Database Management, Toxicology Prediction.
* **Scientific Focus:** Structure-Activity Relationship (SAR), Cardiotoxicity, and Pre-clinical Safety Assessment.

---

## 📁 Repository Note
*Detailed inter-feature distances, specific raw datasets, and proprietary chemical structures are withheld to protect intellectual property. For inquiries regarding the full methodology or professional collaboration, please contact the maintainer.*

---
