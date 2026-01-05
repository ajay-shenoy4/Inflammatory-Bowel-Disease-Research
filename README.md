# The Effects of Inflammatory Bowel Disease on Brain Microstructure

![Research Status](https://img.shields.io/badge/Research-In_Progress-orange)
![Field](https://img.shields.io/badge/Field-Neuroscience-blue)
![Analysis](https://img.shields.io/badge/Analysis-Python_/_Pandas-orange)

## Project Overview
This repository contains the research paper and data analysis pipeline for a study investigating how **Inflammatory Bowel Disease (IBD)** impacts the Central Nervous System (CNS). By utilizing a DSS-induced colitis rodent model and advanced diffusion-weighted MRI techniques (**DTI** and **NODDI**), this project quantifies microstructural changes in psychiatrically relevant brain regions.

**Primary Finding:** IBD-related neuroinflammation is sex-specific. Females exhibit significantly more microstructural alterations, particularly in the amygdala, which may provide a biological explanation for higher rates of IBD-induced anxiety and depression in females.

---

## Research Abstract
IBD is characterized by chronic GI inflammation, but its systemic effects often lead to understudied neurological complications. This study used male and female C57Bl6/J mice to explore the gut-brain axis. Through Diffusion Tensor Imaging (DTI) and Neurite Orientation Dispersion and Density Index (NODDI), we measured:
* **Fractional Anisotropy (FA):** White matter integrity.
* **Mean Diffusivity (MD):** Cellularity and edema.
* **Orientation Dispersion Index (ODI):** Neurite branching and spatial configuration.

Findings indicate that female mice experience unique changes in the **amygdala** and **thalamus**, while both sexes show alterations in the **hippocampus**. These findings suggest that the psychological prognosis of IBD should be treated with sex-specific considerations.



---

## Repository Structure

### Research Paper
* `The_Effects_of_IBD_on_Brain_Microstructure.pdf`: The full paper detailing the autoimmune pathways, cytokine release mechanisms, and the role of sex hormones (Estrogen vs. Testosterone) in neuroprotection. Link: https://docs.google.com/document/d/1p_jaSH9G9YHLq6_-WQvoQrbyt1I3PFAoUrVNd60ANU4/edit?usp=sharing


### Data Analysis (`.ipynb`)
The included Jupyter Notebook performs the following:
1.  **Data Cleaning:** Aggregates mean ROI intensities from CSV datasets.
2.  **Statistical Inference:** Runs independent t-tests to compare DSS (Experimental) vs. Vehicle (Control) groups.
3.  **Sex-Based Filtering:** Separates significant results ($p < 0.05$) for male and female cohorts.
4.  **Visualization:** Generates annotated bar plots with standard deviation error bars.

### Key Data Points
| Brain Region | Measurement | Sex | Observation |
| :--- | :--- | :--- | :--- |
| **Amygdala** | FA | Female | Significant Decrease |
| **Corpus Callosum** | FA | Female | Significant Decrease |
| **Hippocampus** | ODI | Both | Significant Increase |
| **Frontal Cortex** | ODI/MD | Both | Significant Increase |
| **Thalamus** | ODI | Female | Significant Increase |



---

## Technical Setup

### Python Dependencies
To run the analysis notebook, ensure you have the following installed:
```bash
pip install pandas matplotlib scipy numpy
