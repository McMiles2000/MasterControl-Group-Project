# MasterControl-Group-Project
# MasterControl Sales Analytics Project

## Overview

This project was completed as part of a Master of Science in Business Analytics capstone in collaboration with **MasterControl**, a B2B SaaS company specializing in quality and manufacturing software solutions.

The objective was to analyze sales lead data and develop a data-driven approach to improve **lead prioritization, conversion rates, and sales efficiency**, with a specific focus on the underperformance of Manufacturing (Mx) opportunities relative to Quality (Qx).

---

## Business Problem

MasterControl generates a high volume of qualified account leads (QALs) across its product lines. While the Quality (Qx) solution shows strong progression rates, the Manufacturing (Mx) solution lags behind.

This creates a key challenge:

> How can sales teams better identify and prioritize leads most likely to progress, particularly within Mx, to improve overall pipeline performance?

Without a structured approach, sales resources may be spread inefficiently across low-probability opportunities.

---

## Approach

Our analysis followed a structured workflow:

### 1. Exploratory Data Analysis (EDA)
- Evaluated lead progression rates across Qx and Mx
- Analyzed differences by industry, account attributes, and contact roles
- Assessed missingness and data quality considerations

### 2. Predictive Modeling
- Built classification models to estimate likelihood of lead progression
- Leveraged logistic regression and LASSO for interpretability and feature selection
- Evaluated model performance using ROC/AUC and validation techniques

### 3. Threshold & Decision Analysis
- Tested multiple probability thresholds beyond the default 0.50 cutoff
- Analyzed tradeoffs between:
  - Sensitivity (conversion capture)
  - Specificity
  - Precision
- Developed a lead ranking framework to support prioritization

---

## Key Insights

- **Mx leads have significantly lower progression rates than Qx**, confirming a major opportunity for improvement.
- Default classification thresholds are **too conservative** for this business use case and miss a large portion of true conversions.
- A **lead scoring and ranking approach** is more effective than binary classification for sales prioritization.
- Targeting the top-ranked leads can capture a disproportionately high share of progressing opportunities.
- Segment-level analysis highlights meaningful differences across industries and account characteristics.

---

## Business Value

This work enables MasterControl to:

- Prioritize high-probability leads more effectively
- Improve sales team efficiency and focus
- Increase conversion rates within underperforming segments (Mx)
- Make threshold selection a **strategic business decision**, not just a modeling default
- Transition toward a **data-driven sales process**

---

## Deliverables

This repository includes the following materials:

- **Business Problem Statement**
- **Exploratory Data Analysis Notebook**
- **Predictive Modeling Notebook**
- **Final Presentation (PDF)**

---

## Tools & Methods

- R
- Quarto
- tidyverse
- caret
- glmnet (LASSO)
- Classification modeling
- ROC/AUC evaluation
- Threshold optimization
- Data visualization

---

## Data Confidentiality

The data used in this project were provided for academic purposes and are not included in this repository.

---

## Team

- Miles McCunniff (@McMiles2000)
- Sebastian (@username)
- Jeffrey (@username)
