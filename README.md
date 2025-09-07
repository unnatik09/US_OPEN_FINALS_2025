# Tennis Match Outcome Prediction using XGBoost

This repository contains a predictive model for ATP tennis matches, built using **XGBoost**. The model predicts the probability of a player winning a match based on player stats, match context, and synthetic Elo ratings.

---

## Overview

Due to limited availability of historical match data, this model represents the best predictive performance achievable with the current dataset. We also created **synthetic Elo ratings** because date-wise Elo data was not available.

We first trained a **baseline Logistic Regression** model as a reference:

- **Accuracy:** 0.6692  
- **ROC AUC:** 0.7389  

The XGBoost model significantly improves upon this baseline:

- **Accuracy:** 0.685  
- **ROC AUC:** 0.7585  

---

## Features Used

The final model uses the following features:

- `Best of`
- `Rank_1`, `Rank_2`
- `Pts_1`, `Pts_2`
- `Odd_1`, `Odd_2`
- `rank_diff`, `pts_diff`
- `surface_encoded`, `court_encoded`
- `round_encoded`, `series_encoded`
- `wins_1_last5`, `wins_2_last5`
- `winperc_1`, `winperc_2`
- `h2h_1_vs_2`, `h2h_2_vs_1`
- `surface_winperc_1`, `surface_winperc_2`
- `streak_1`, `streak_2`
- `ELO_1`, `ELO_2`, `ELO_diff`
- `Surface_ELO_1`, `Surface_ELO_2`, `Surface_ELO_diff`

---

