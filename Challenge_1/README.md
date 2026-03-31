# Challenge 1: Late Refill Risk Prediction 💊

## 🎯 Overview
This directory contains our predictive modeling solution for **Challenge 1** of the Pharmacy2U Hackathon.

The goal of this challenge is to identify and flag patient medication adherence risks before they happen. Specifically, we aim to predict if a patient is at a high risk of a **late refill** on their active prescriptions.

We utilized the CMS `DE-SynPUF` datasets to conduct deep Exploratory Data Analysis (EDA) and built robust predictive features based on explicit patient demographics and detailed historical refill cadence metrics.

---

## 📂 Core Assets
*   **`Pharmacy2U_Project_A.ipynb`**
    *   This master Jupyter Notebook contains the complete end-to-end data science pipeline.
    *   **Phase 1:** `Pre-processing & Data Merging`. Joining Beneficiary and PDE files to establish localized cohorts.
    *   **Phase 2:** `Exploratory Data Analysis`. Visualizing population demographics, top therapeutic classes, and the distribution of refill lead/lag times.
    *   **Phase 3:** `Feature Engineering`. Constructing time-series features (average past refill windows, continuous gap lengths).
    *   **Phase 4:** `Modeling Training`. Baseline execution and final predictions.

---

## 🛠️ Data Infrastructure
*This project strictly uses synthetic data (`DE-SynPUF`), guaranteeing zero real patient data is exposed or analyzed.*

To rerun this pipeline from scratch:
1.  Download the raw `DE-SynPUF Prescription Drug Events, Sample 1` Zip directly from the [CMS Data Source](https://downloads.cms.gov/files/DE1_0_2008_to_2010_Prescription_Drug_Events_Sample_1.zip).
2.  Extract the massive `.csv` files into a `/data` directory at the root level of this repository (Note: `data/` is strictly `.gitignore`'d).
3.  Cross-reference the schemas using the official [CMS Codebook](https://www.cms.gov/files/document/de-10-codebook.pdf).
4.  Execute the Jupyter Notebook sequentially.