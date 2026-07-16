# Trip_Production_pouyan
Developed machine learning algorithms to predict daily trip rate of households. Implemented supervised learning algorithms
# Trip Production Analysis for Persons With Disabilities

## Overview

This repository contains Python code for analyzing daily travel behavior and trip production among persons with and without disabilities. The analysis uses person-, household-, trip-, and vehicle-level data from the 2022 National Household Travel Survey.

The project compares travel patterns between the two population groups and develops separate trip-production models to identify the household, socioeconomic, and demographic factors associated with daily trip frequency.

## Objectives

The main objectives are to:

- Prepare and merge multiple National Household Travel Survey datasets
- Compare daily travel behavior between persons with and without disabilities
- Examine differences in trip frequency, travel distance, and travel duration
- Analyze trip purposes across age groups
- Identify factors associated with daily trip production
- Develop and evaluate separate count-data models for the two groups

## Data Source

The analysis uses the following public-use files from the 2022 National Household Travel Survey:

- `hhpub.csv`: Household-level data
- `perpub.csv`: Person-level data
- `trippub.csv`: Trip-level data
- `vehpub.csv`: Vehicle-level data

The original datasets are not included in this repository because of their size. They can be obtained from the National Household Travel Survey website.

## Analysis Workflow

The notebook performs the following steps:

1. Loads the household, person, trip, and vehicle datasets
2. Merges household characteristics with person-level records
3. Cleans and recategorizes demographic and socioeconomic variables
4. Calculates total daily trips, travel distance, and travel duration
5. Creates person-level trip-purpose variables
6. Separates respondents into:
   - Persons with disabilities
   - Persons without disabilities
7. Compares travel behavior using descriptive statistics and visualizations
8. Conducts a Mann–Whitney U test for differences in daily trip frequency
9. Examines trip frequency by age and trip purpose using LOESS smoothing
10. Evaluates multicollinearity using correlation analysis and variance inflation factors
11. Estimates separate negative binomial regression models
12. Evaluates model performance using five-fold cross-validation, RMSE, and MAE

## Repository Contents

```text
Trip_Production_pouyan/
├── README.md
└── trip_production_analysis.ipynb
