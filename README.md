
# Statistical Analysis of the OCEAN Personality Model

## Overview
This repository contains the dataset and Jupyter Notebook used for a statistical analysis project on the **OCEAN** (Big Five) personality traits, with a focus on comparing the trait **Openness** across different racial groups.

The analysis was conducted as part of a statistical theory project, applying non-parametric inference methods to Likert-scale personality data.

## Dataset
- **File:** `data.csv`
- **Source:** [OpenPsychometrics.org](https://openpsychometrics.org/_rawdata/)
- **Rows:** 19719
- **Columns:** 57
- **Format:** Tab-separated values (TSV)
- **Columns:**
  - **Demographics:** `race`, `age`, `engnat` (native English speaker), `gender`, `hand` (handedness), `source`, `country`
  - **Personality Items:** `E1`–`E10` (Extraversion), `N1`–`N10` (Neuroticism), `A1`–`A10` (Agreeableness), `C1`–`C10` (Conscientiousness), `O1`–`O10` (Openness)

Each personality trait is measured using 10 items, rated on a 1–5 Likert scale.

## Notebook
- **File:** `statistical_theory(M).ipynb`
- **Purpose:** Clean, process, and analyze the OCEAN dataset with an emphasis on statistical comparison of Openness across racial groups.
- **Key Steps:**
  1. **Data Loading & Cleaning:**
     - Reads the TSV dataset
     - Filters and processes missing values
  2. **Trait Scoring:**
     - Calculates composite scores for each of the five personality traits by averaging their respective items.
  3. **Exploratory Data Analysis (EDA):**
     - Histograms of Openness for each racial group
     - Sample sizes displayed in plot titles
  4. **Statistical Testing:**
     - Non-parametric omnibus tests (e.g., Kruskal–Wallis)
     - Pairwise post-hoc tests with multiple comparison corrections
  5. **Visualization:**
     - Side-by-side histograms for racial groups
     - Customizable bin counts per plot
  6. **Interpretation:**
     - Identifies which groups differ significantly in Openness
     - Discusses effect sizes and limitations

## Requirements
To run the notebook, install the following Python packages:
```bash
pip install pandas numpy scipy matplotlib seaborn scikit-posthocs pingouin
```

## How to Run
1. Clone the repository:
```bash
git clone <your-repo-url>
cd <your-repo-folder>
```
2. Open the notebook:
```bash
jupyter notebook statistical_theory(M).ipynb
```
3. Ensure `data.csv` is in the same directory as the notebook.
4. Run all cells to reproduce the analysis.

## Output Examples
- **Histograms** of Openness by race
- **Statistical tables** with p-values and significance highlights
- **Effect size estimates** (e.g., epsilon-squared)

## License
This project is for academic and research purposes only. Dataset is from OpenPsychometrics.org under their data usage policy.
