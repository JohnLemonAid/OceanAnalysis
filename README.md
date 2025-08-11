# Statistical Analysis of the OCEAN Personality Model

## Overview
Analysis of **OCEAN** (Big Five) personality traits, focusing on **Openness** differences across racial groups. Conducted using non-parametric methods on Likert-scale survey data from [OpenPsychometrics.org](https://openpsychometrics.org/_rawdata/).
Please notice that some of the calculations belong to the presentation, but do not have a part in the final project.

## Dataset
- **File:** `data.csv` (TSV, 19719 rows, 57 columns)
- **Demographics:** `race`, `age`, `engnat`, `gender`, `hand`, `source`, `country`
- **Traits:** 10 items each for Extraversion (E), Neuroticism (N), Agreeableness (A), Conscientiousness (C), Openness (O)  
  Scale: 1–5 Likert

## Instructions
- **File:** `statistical_theory(M).ipynb`
- **Loading data:** To upload `data.csv` you may update the following line of code, which appears below the imports part:
  ```python
  df_og = pd.read_csv("data.csv", sep='\t')
  ```
