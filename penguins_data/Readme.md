
# Palmer Penguins Dataset Analysis

## Overview
This project explores the Palmer Penguins dataset using Python libraries such as Pandas, NumPy, Seaborn, and Matplotlib. The analysis includes data exploration, visualization, and a linear regression model to predict penguin body mass based on flipper length. The dataset contains information about penguin species, bill length, bill depth, flipper length, body mass, sex, and island of origin.

## Table of Contents
1. [Requirements](#requirements)
2. [Dataset](#dataset)
3. [Analysis Steps](#analysis-steps)
4. [Key Findings](#key-findings)
5. [Visualizations](#visualizations)
6. [Linear Regression](#linear-regression)
7. [How to Run](#how-to-run)

## Requirements
- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `seaborn`
  - `matplotlib`
  - `scikit-learn`

Install dependencies using:
```bash
pip install numpy pandas seaborn matplotlib scikit-learn
```

## Dataset
The dataset used is the Palmer Penguins dataset, accessible via Seaborn's `load_dataset("penguins")`. It includes:
- **Columns**: `species`, `island`, `bill_length_mm`, `bill_depth_mm`, `flipper_length_mm`, `body_mass_g`, `sex`
- **Species**: Adelie, Chinstrap, Gentoo
- **Rows**: 344

## Analysis Steps
1. **Load Libraries and Dataset**: Import required libraries and load the dataset.
2. **Understand the Data**: Display the first few rows using `penguins.head()`.
3. **Unique Species**: Identify the number of unique species (3: Adelie, Chinstrap, Gentoo).
4. **Average Bill Length**: Calculate the average bill length for each species.
5. **Highest Flipper Length**: Determine the species with the highest average flipper length (Gentoo: 217.19 mm).
6. **Body Mass Distribution**: Visualize body mass distribution across species using a boxplot.
7. **Missing Values**: Check for missing data (e.g., 11 missing values in `sex`).
8. **Correlations**: Analyze correlations between numerical features (e.g., flipper length and body mass: 0.871).
9. **Heaviest Penguins by Island**: Identify the island with the heaviest penguins (Biscoe: 4716.02 g).
10. **Flipper Length by Sex**: (Incomplete in document; analysis not fully shown.)
11. **Most Common Species**: Find the most frequent species (Adelie: 152 occurrences).
12. **Scatter Plot**: Visualize bill length vs. bill depth by species.
13. **Linear Regression**: Predict body mass from flipper length.

## Key Findings
- **Species Count**: 3 unique species (Adelie, Chinstrap, Gentoo).
- **Average Bill Length**:
  - Adelie: 38.79 mm
  - Chinstrap: 48.83 mm
  - Gentoo: 47.50 mm
- **Highest Flipper Length**: Gentoo (217.19 mm).
- **Heaviest Penguins**: Found on Biscoe Island (avg. body mass: 4716.02 g).
- **Correlations**: Strong positive correlation between flipper length and body mass (0.871).
- **Most Common Species**: Adelie (152 instances).

## Visualizations
- **Boxplot**: Distribution of body mass by species.
- **Scatter Plot**: Bill length vs. bill depth, colored by species.
- **Linear Regression Plot**: Flipper length vs. predicted body mass.

## Linear Regression
- **Objective**: Predict `body_mass_g` using `flipper_length_mm`.
- **Steps**:
  1. Handle missing values by filling with column means.
  2. Split data into training (70%) and testing (30%) sets.
  3. Train a `LinearRegression` model.
  4. Evaluate using R² score.
- **Result**: R² = 0.749, indicating ~74.9% of the variance in body mass is explained by flipper length.

## How to Run
1. Ensure all required libraries are installed.
2. Copy the code from the notebook into a Python environment (e.g., Jupyter Notebook).
3. Execute each cell sequentially to reproduce the analysis and visualizations.
