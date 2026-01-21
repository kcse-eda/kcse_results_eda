

# KCSE Results Exploratory Data Analysis (EDA)

## Project Overview

This project conducts a structured **Exploratory Data Analysis (EDA)** of the **2025 KCSE Examination Essential Statistics** published by the **Kenya National Examinations Council (KNEC)**.

The objective is to extract, clean, analyze, and visualize official KCSE results data to uncover trends and insights related to:

* Overall grade distribution
* Gender-based performance
* County-level performance
* Other patterns present in the published statistics

This is a **collaborative, time-bound (3 weeks)** data science project involving multiple contributors coordinated via GitHub.

---

## Data Source

**Primary and only official data source:**

📄 *2025 KCSE Examination Essential Statistics*
🔗 [https://knec.ac.ke/wp-content/uploads/2026/01/2025-KCSE-EXAMINATION-ESSENTIAL-STATISTICS.pdf](https://knec.ac.ke/wp-content/uploads/2026/01/2025-KCSE-EXAMINATION-ESSENTIAL-STATISTICS.pdf)

### Notes on Data

* The data is published in **PDF format**.
* No official machine-readable dataset (CSV/Excel) is publicly available.
* The first phase of the project involves **extracting tables from the PDF** into structured formats.
* Any additional granular data would require formal communication with the Ministry of Education and is **out of scope** for this phase.

---

## Project Objectives

1. Extract structured datasets from the official KCSE statistics PDF
2. Clean and standardize the extracted data
3. Perform exploratory data analysis
4. Produce clear visualizations and summary insights
5. Maintain a reproducible, well-documented analysis workflow

---

## Project Timeline (3 Weeks)

### Week 1 – Data Foundation

* PDF table extraction
* Dataset creation (CSV/Excel)
* Initial data cleaning and validation

### Week 2 – Exploratory Analysis

* Descriptive statistics
* Analysis by gender, county, grades
* Visualizations

### Week 3 – Refinement & Reporting

* Insight refinement
* Documentation
* Final notebooks and figures
* Stable merge to `main`

---

## Team Structure

Contributors are organized into **small teams of ~4 people**, each responsible for a specific section of the project.

### Functional Teams

* **Data Extraction & Collection**
* **Data Cleaning & Preparation**
* **Exploratory Data Analysis (EDA)**
* **Reporting & Documentation**

Each team has:

* **Members** → work on feature branches
* **One Group Lead** → reviews and merges team contributions

---

## Repository Structure

```text
.
├── data/
│   ├── raw/          # Extracted data from PDF (unchanged)
│   └── processed/    # Cleaned and ready-for-analysis datasets
│
├── notebooks/
│   ├── extraction/
│   ├── cleaning/
│   └── eda/
│
├── figures/          # Saved plots and visualizations
├── reports/          # Written summaries or markdown reports
├── README.md
└── requirements.txt
```

---

## GitHub Workflow

### Branches

* `main` → Final, stable output (protected)
* `dev` → Integration branch
* Group branches:

  * `data-extraction`
  * `data-cleaning`
  * `eda`
  * `reporting`

### How Contributions Work

1. **Create a feature branch** from your group branch
   Example:

   ```bash
   git checkout eda
   git checkout -b eda-county-analysis
   ```

2. **Work only in your feature branch**

3. **Push changes and open a Pull Request (PR)** to your group branch

4. **Group lead reviews and merges**

5. **Group lead opens PR from group branch → `dev`**

6. **Project lead merges `dev` → `main` at milestones**

⚠️ No direct commits to `main`.

---

## Contribution Guidelines

* Use clear, descriptive commit messages
* Keep notebooks focused and well-commented
* Do not modify raw data once committed
* All changes must go through Pull Requests
* Respect branch ownership and review process

---

## Tools & Stack

* Python
* Pandas, NumPy
* Matplotlib / Seaborn
* Jupyter Notebooks
* Git & GitHub

---

## Expected Outputs

* Clean, structured datasets
* Reproducible analysis notebooks
* Visual summaries and plots
* Clear written insights and documentation

---

## Disclaimer

This project uses **publicly available official statistics** for educational and analytical purposes.
All interpretations are independent and do not represent KNEC or the Ministry of Education.

---

## Contact & Coordination

Project coordination and announcements are handled via the group communication channel.
All technical collaboration happens through GitHub.

---
