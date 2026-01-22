

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

### 2. Update and Switch to `dev`

All feature branches should be created from the latest `dev` branch, **never from group branches**:

```bash
git checkout dev
git pull origin dev
```

---

### 3. Create a Feature Branch

Each task gets its **own personal feature branch**:

```bash
git checkout -b <group>-<short-description>-<your-username>
```

**Branch naming rule:**

```
<group>-<short-description>-<your-username>
```

Examples:

* `eda-gender-analysis-jotham`
* `cleaning-missing-values-jotham`
* `extraction-grade-table-jotham`

> **Important:** One branch per contributor. Do not share branches.

---

### 4. Do Your Work

* Work only on files related to your task
* Do not modify unrelated files
* Do not touch other group branches

---

### 5. Commit Your Changes

```bash
git add .
git commit -m "Add county-level KCSE EDA"
```

Use **clear, descriptive commit messages**.

---

### 6. Push Your Feature Branch

```bash
git push -u origin <group>-<short-description>-<your-username>
```

---

### 7. Open a Pull Request (PR)

On GitHub:

* **Base branch:** your **group branch** (e.g., `eda`)
* **Compare branch:** your **feature branch**
* Add a short, clear description of your work

> **Do not merge your own PR.** Only the team lead merges feature branches.

---

### 8. Review & Merge (Group Lead Only)

* Group lead reviews all PRs for their group branch
* Requests changes if needed
* Merges approved feature branches into the **group branch**

---

### 9. Group Branch → `dev` (Integration)

Once the group branch is stable:

* Group lead opens a PR:

```text
group branch → dev
```

* Project lead reviews and merges

> Only the project lead merges into `dev`.

---

### 10. Final Merge → `main`

When `dev` contains fully tested and approved work:

* Project lead opens a PR:

```text
dev → main
```

* `main` is **protected**; only approved work is merged

---

### ✅ Key Rules to Remember

1. **Never push directly to `dev` or `main`.**
2. **Feature branches are personal.** One person per branch.
3. Always **pull the latest `dev`** before creating a feature branch.
4. Use **clear commit messages** for traceability.
5. Team leads manage merges to group branches; project lead manages merges to `dev` and `main`.
6. Members can request to join multiple teams, but must work on one primary branch per task.


---

Correct Workflow Summary
clone → dev → feature branch → PR → group branch → group lead merges → PR → dev → project lead merges → main

Step-by-Step Explanation

Clone the repository

Update dev (git checkout dev && git pull origin dev)

Create your personal feature branch from dev

Work → commit → push your feature branch

Open a PR to the group branch (e.g., eda)

Group lead reviews & merges your feature branch into the group branch

Once group branch is stable, group lead opens a PR to merge the group branch into dev

Project lead reviews & merges into dev

Finally, project lead merges dev into main (stable, protected)

✅ Key points

Feature branches are always personal

No one pushes directly to dev or main

Teams control reviews and merges to group branches

The PR sequence is: feature → group → dev → main
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
