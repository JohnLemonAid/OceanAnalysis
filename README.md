# Statistical Analysis of the OCEAN Personality Model

## Overview
Analysis of **OCEAN** (Big Five) personality traits, focusing on **Openness** differences across racial groups. Conducted using non-parametric methods on Likert-scale survey data from [OpenPsychometrics.org](https://openpsychometrics.org/_rawdata/).

## Dataset
- **File:** `data.csv` (TSV, 19719 rows, 57 columns)
- **Demographics:** `race`, `age`, `engnat`, `gender`, `hand`, `source`, `country`
- **Traits:** 10 items each for Extraversion (E), Neuroticism (N), Agreeableness (A), Conscientiousness (C), Openness (O)  
  Scale: 1–5 Likert

## Notebook
- **File:** `statistical_theory(M).ipynb`
- Loads and cleans data, computes trait scores, performs Kruskal–Wallis and post-hoc tests, and visualizes distributions.
- **Important:** Update this line if `data.csv` is stored elsewhere:
  ```python
  df_og = pd.read_csv("data.csv", sep='\t')
