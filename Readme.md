# Football League (LaLiga) Data Analysis 

## Table of Contents
- [Introduction](#introduction)
- [About the Dataset](#about-the-dataset)
    - [Context](#context)
    - [Dataset Inspiration](#dataset-inspiration)
    - [Basic Dataset Description](#basic-dataset-description)
- [Usage Scenarios](#usage-scenarios)
- [Analysis Overview](#analysis-overview)
    - [Team Performance Analysis](#team-performance-analysis)
    - [Bayesian Modeling with PyMC](#bayesian-modeling-with-pymc)
    - [Visualization of Results](#visualization-of-results)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction
In this notebook, Bayesian data analysis was performed using the PyMC library. The dataset was explored, data was visualized, and Bayesian modeling was applied to draw inferences and make predictions for the next LaLiga season.

## About the Dataset

### Context
LaLiga, is the top professional football division of the Spanish football league . The dataset used in this analysis contains detailed information on matches played in LaLiga, including team performance metrics such as goals scored at different stages of the match (first half and second half).

### Dataset Inspiration
The dataset allowed us to analyze various aspects of LaLiga matches, such as:
- **Team Performance**: How consistently teams scored during the first half vs. the second half.
- **Bayesian Inference**: Bayesian modeling was applied to estimate team strengths and predict match outcomes.
- **Prediction**: The model was used to predict the likely outcomes for future matches based on historical data.

### Basic Dataset Description
- **Number of Rows**: The dataset contains multiple rows representing individual matches.
- **Number of Columns**: The dataset includes columns such as `Date`, `HomeTeam`, `AwayTeam`, `FTHG` (Full Time Home Goals), `FTAG` (Full Time Away Goals), `HTHG` (Half Time Home Goals), and `HTAG` (Half Time Away Goals).
- **Key Columns**:
    - **Date**: Date of the match.
    - **HomeTeam**: Name of the home team.
    - **AwayTeam**: Name of the away team.
    - **FTHG**: Goals scored by the home team at full time.
    - **FTAG**: Goals scored by the away team at full time.
    - **HTHG**: Goals scored by the home team at half time.
    - **HTAG**: Goals scored by the away team at half time.
- **Dataset Link**
The dataset used in this analysis can be found on Kaggle: [Link](https://www.kaggle.com/datasets/kishan305/la-liga-results-19952020)

## Usage Scenarios

This dataset can be applied in various scenarios:
- **Performance Analysis**: Evaluated team performance trends over different seasons and match conditions (home vs. away).
- **Predictive Modeling**: Models were built to predict match outcomes and assess future team performance.
- **Bayesian Inference**: Bayesian models were used to understand latent variables such as team strengths and match dynamics.
- **Strategy Development**: Assisted teams in strategizing based on historical performance data and Bayesian predictions.

## Analysis Overview

### Team Performance Analysis
- **Team Indexing**: A team index lookup was created to facilitate easy reference to teams within the dataset.
- **Average Goals Analysis**: The top 10 teams with the most average goals scored during both the first half and second half of matches were identified and visualized, separately for home and away games.

### Bayesian Modeling with PyMC
- **Bayesian Model Definition**: A Bayesian model was defined using the PyMC library to estimate team attack and defense strengths. The model incorporated prior distributions, latent variables, and likelihoods to analyze match outcomes.
- **Trace Plot and Posterior Predictive Checks**: Trace plots were generated and posterior predictive checks were performed to validate the model's inferences.

### Visualization of Results
- **Scatter Plots**: Attack and defense strengths for each team were visualized, as well as their actual goals scored and conceded, using scatter plots.
- **Ranking Probability**: The probabilities of teams finishing in various league positions were calculated and visualized based on the Bayesian model's predictions.

## Conclusion
This analysis provided valuable insights into the performance trends of LaLiga teams, leveraging both traditional statistical methods and Bayesian inference. The results can be used to predict future match outcomes, guide team strategies, and enhance our understanding of football dynamics within LaLiga.

## License
This project is licensed under the MIT License. See the LICENSE file for details.