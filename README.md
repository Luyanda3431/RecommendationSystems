# RecommendationSystems
*Author:Luyanda Cebekhulu*

# Recommender System Analysis

This project is an analysis of various recommender system techniques, including **User-Based Collaborative Filtering (CF)**, **Item-Based CF**, and **Matrix Factorization**. The project implements these techniques in R, builds an ensemble model, and evaluates their performance using the Book-Crossing dataset.

## Project Overview

The aim of the project is to build a recommender system that predicts book ratings based on users' historical ratings and preferences. This analysis uses multiple techniques and combines them into an ensemble model to improve prediction accuracy.

### Key Steps:

1. **Data Preprocessing**: 
    - Clean the dataset, filter out users with fewer than 200 ratings, and handle missing or invalid values.
    - Convert User IDs and ISBNs into integer indices for easier matrix manipulation.

2. **Exploratory Data Analysis (EDA)**: 
    - Visualize the distribution of book ratings, user ratings, and user demographics.
    
3. **Recommender Models**:
    - **User-Based Collaborative Filtering**: Recommend books based on similar users.
    - **Item-Based Collaborative Filtering**: Recommend books based on similar items.
    - **Matrix Factorization**: Use dimensionality reduction to model user-item interactions.

4. **Ensemble Model**: 
    - Combine the predictions from all three methods to improve accuracy.

5. **Model Evaluation**: 
    - Evaluate model performance using Root Mean Squared Error (RMSE) on a test set.

## Files in the Repository

- `CBKLUY001RecommendationSystems.qmd`: Quarto document containing the code for data preprocessing, model building, and analysis.
- `data/`: Contains the input datasets used for the analysis, including user ratings, book information, and user demographics.
- `README.md`: This file, which provides an overview of the project.
- `results/`: Folder containing output files, such as the rendered PDF or Word document of the report.

## How to Run the Project
*Clone the repository:*

```bash
git clone https://github.com/Luyanda3431/RecommendationSystems/edit/main/README.md
```
### Prerequisites

- R (version 4.0 or higher)
- Quarto (for rendering `.qmd` files)
- R packages:
    - `dplyr`
    - `tidyverse`
    - `Matrix`
    - `recosystem`
    - `ggplot2`
    - `DT`
    - `quarto` (for rendering the report)

### Installation of Dependencies

Install the necessary R packages by running the following command in R:

```r

install.packages(c("dplyr", "tidyverse", "Matrix", "recosystem", "ggplot2", "DT"))
