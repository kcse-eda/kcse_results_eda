

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


---

## Contributor Workflow (From Clone to Merge)

### 1. Clone the Repository

```bash
git clone https://github.com/kcse-eda/kcse_results_eda.git
cd kcse_results_eda
```

---

### 2. Switch to Your Group Branch

Each contributor works under **one group branch** only.

Examples:

```bash
git checkout eda
# or
git checkout data-cleaning
# or
git checkout data-extraction
```

Always confirm:

```bash
git branch
```

---

### 3. Create a Feature Branch

Every task gets its **own feature branch**.

```bash
git checkout -b eda-county-analysis
```

**Branch naming rule:**

```
<group>-<short-description>
```

Examples:

* `eda-gender-analysis`
* `cleaning-missing-values`
* `extraction-grade-table`

---

### 4. Do Your Work

* Make changes only related to your task
* Do not modify unrelated files
* Do not touch other group branches

---

### 5. Commit Your Changes

```bash
git add .
git commit -m "Add county-level KCSE EDA"
```

Use clear, meaningful messages.

---

### 6. Push Your Feature Branch

```bash
git push -u origin eda-county-analysis
```

---

### 7. Open a Pull Request (PR)

On GitHub:

* Base branch: **your group branch** (e.g. `eda`)
* Compare branch: **your feature branch**
* Add a short description of what you did

---

### 8. Review & Merge (Group Lead Only)

* Group lead reviews the PR
* Requests changes if needed
* Merges into the **group branch**

Members **do not merge their own PRs**.

---

### 9. Group Lead → Integration

When the group branch is stable:

* Group lead opens a PR:

  ```
  group branch → dev
  ```
* Project lead reviews and merges

---

### 10. Final Merge

* Project lead merges:

  ```
  dev → main
  ```
* This marks a milestone or release

---

## What You Must NOT Do

* ❌ Push directly to `main` or `dev`
* ❌ Work directly on group branches
* ❌ Mix multiple tasks in one feature branch
* ❌ Merge your own PR

---

## Workflow Summary

```text
clone → group branch → feature branch → PR → group branch → dev → main
```

---

## If You Get Stuck

* Pull latest changes:

```bash
git pull origin <your-group-branch>
```

* Ask your group lead before rebasing or resolving conflicts

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
