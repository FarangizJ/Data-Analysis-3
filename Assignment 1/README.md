# Data Analysis 3 – Assignment 1  

**Building a Pricing Model for Airbnb Listings**

## Overview

This project builds and evaluates predictive models for Airbnb listing prices
using InsideAirbnb data. The business case assumes operation of a chain of
Airbnb properties requiring data-driven pricing decisions.

## Data

Data is sourced from <https://insideairbnb.com>.

Datasets used:

- Toronto 2024 Q3 (core training dataset, >10K listings)
- Toronto 2025 Q4 (temporal validity)
- Vancouver 2025 Q4 (cross-city validity)

Raw data files are stored in `data/raw/`.

## Methodology

- Price cleaning and log transformation
- Feature engineering (amenities count, availability, reviews)
- Missing value imputation
- One-hot encoding for categorical variables

## Models

Five models are estimated:

1. OLS
2. LASSO
3. Random Forest
4. Gradient Boosting
5. Extra Trees

Models are trained on Toronto 2024 Q3 and evaluated out-of-sample.

## Structure

```
Data-Analysis-3/
│── Assignment 1/
│ │── data/
│ │ │── raw/
│ │ │── processed/
│ │ │── 01_airbnb_exploration.ipynb
│── README.md


## Reproducibility

To reproduce the results:

1. Clone the repository:
git clone https://github.com/<your-username>/Data-Analysis-3.git


2. Navigate to the Assignment 1 folder and open the notebook:
Assignment 1/01_airbnb_exploration.ipynb


3. Run all cells in the notebook from top to bottom.

All required datasets are included in the repository under `data/raw/`.
Random seeds are fixed where applicable.

## Author
Farangiz Jurakhonova
