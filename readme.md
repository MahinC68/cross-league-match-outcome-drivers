# Which Statistics Drive Winning in European Football?

## Overview

This project uses machine learning to analyze which match statistics drive winning outcomes across top European football leagues (Premier League, Bundesliga, Ligue 1). The focus is on interpreting results and comparing how performance translates to winning across leagues.

---

## Approach

- Engineered **differential features** (home − away) for key match stats  
- Defined a binary target: **home win vs non-home win**  
- Trained **logistic regression** (primary) and **random forest** (comparison) models  
- Evaluated performance using **accuracy** and **ROC-AUC**  
- Analyzed **feature importance** to compare drivers of winning across leagues  

---

## Key Findings

- **Expected goals (xG_diff)** is the strongest predictor across all leagues  
- **Shots on target** is consistently the second most important feature  
- **Ligue 1 is the most predictable**, while **Bundesliga is the least predictable**  
- **Possession and passing have low predictive power** across all leagues  
- Differences in model performance suggest variation in **playstyle and outcome variability**  

---

## Limitations

- Uses in-match statistics, so results are more explanatory than predictive  
- Limited feature set (no team strength, player-level data, etc.)  
- Based on a single season and three leagues  

---

## Tech Stack

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

---

## Structure
├── data/
├── notebooks/
│ ├── 01_data_loading_filtering.ipynb
│ ├── 02_feature_engineering.ipynb
│ ├── 03_modeling_and_evaluation.ipynb
├── README.md
