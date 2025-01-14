# Baseball Analytics Project

> Written by [Aneesh Sallaram] and [Abigail Mabe].


This project analyzes baseball data to identify trends using statistical methods and data visualization techniques. The analysis focuses on player performance metrics, including bat speed, swing length, and their relationships to run and win expectancies. We used R and R Studio to achieve these effects and illustrate our findings.

## Table of Contents
- [Introduction](#introduction)
- [Data](#data)
- [Key Features](#key-features)
- [Code Explanation](#code-explanation)
- [Installation and Usage](#installation-and-usage)


## Introduction
This project explores the impact of two specific conditions (2 Strikes and Runners on bases, Runner on 3rd with less than 2 Outs) on key performance metrics like bat speed and swing length. It also accounts for variability between different players and shows insights through graphs.

## Data
The dataset used in this project is **`baseball.csv`**, which includes:
- Player performance metrics (e.g., bat speed, swing length)
- Game context (e.g., inning, outs, strikes, runners on base)
- Derived metrics (e.g., deviance from average bat speed, run expectancies)
- The baseball.csv file can be found at https://statds.org/events/csas2025/challenge.html
- It is recommended to rename the csv file to baseball to prevent errors in accessing it.

## Key Features
- Statistical modeling of **bat speed** and **swing length** under the conditions mentioned above.
- Identification and filtering of outliers based on player-specific averages and general game outliers.
- Visualizations:
  - Relationship between bat speed deviance and run expectancy.
  - Hit coordinates colored by bat speed.
- Focused analysis for specific game scenarios (e.g., runners on 3rd with less than 2 outs).

## Code Explanation
- The R code uses linear mixed-effects models to look at the relationship between baseball performance metrics, like bat speed and swing length, and run expectancy, while accounting for player-specific variations.
- It builds two models to quantify how each metric influences game outcomes, incorporating both fixed and random effects. The analysis is complemented by scatterplots to showcase the correlation between metrics and run expectancy, as well as density plots to explore the distribution of bat speeds across different player groups.
- Comments throughout the code offer a deeper explanation to individual parts of the code.

## Installation and Usage
1. Clone the repository:
   git clone https://github.com/asallaram/baseball.git.
2. Ensure that the csv file (baseball.csv) and the R Markdown file used to run the code are in the same directory.
3. Download the following packages in R if not already installed.
   a. install.packages(c("dplyr", "lme4", "ggplot2", "MASS", "Matrix"))
4. Run the code and the visualizations and summaries of the linear models should display below the code.

