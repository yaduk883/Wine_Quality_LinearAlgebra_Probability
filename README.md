# Wine Quality Dataset Analysis: Linear Algebra & Probability

## Overview
This repository contains a Jupyter Notebook (`Wine_Quality_LinearAlgebra_Probability.ipynb`) that demonstrates fundamental concepts of linear algebra and probability using the **Red Wine Quality** dataset. It provides a practical, step-by-step approach to understanding vectors, covariance matrices, eigen decomposition, and probability distributions through exploratory data analysis.

## Dataset
* **Name:** Wine Quality (Red Wine)
* **Shape:** 1599 rows, 12 columns
* **Format:** CSV 

## Key Topics & Concepts Covered
* **Data Preprocessing:** Handling missing values using column means.
* **Vectors & Matrices:** Extracting and analyzing 1D NumPy vectors (e.g., Alcohol, Citric Acid).
* **Covariance Matrices:** Computing and interpreting relationships between features (Alcohol vs. Density).
* **Eigen Decomposition:** Calculating eigenvalues and eigenvectors to understand variance (PCA foundation).
* **Probability:** Analyzing the probability distribution of categorical/discrete outcomes (Wine Quality).

## Project Structure
1. **Q1 - Data Loading & Cleaning:** Imports the dataset and gracefully handles any missing values using mean imputation to maintain data integrity.
2. **Q2 - Vector Extraction:** Extracts `alcohol` and `citric acid` as vectors, computing basic statistics (mean, min, max) and visualizing their distributions.
3. **Q3 - Covariance Analysis:** Generates a covariance matrix for Alcohol and Density, visualized via a Seaborn heatmap, revealing an inverse relationship.
4. **Q4 - Eigen Decomposition:** Performs eigen decomposition on the covariance matrix. Highlights how the primary eigenvalue captures ~99.9% of the variance.
5. **Q5 - Probability Distribution:** Calculates the occurrence probability of each wine quality score, showing a normal distribution centered around scores 5 and 6.

## Key Findings
| Feature | Insight |
| **Covariance** | A negative covariance exists between alcohol and density, indicating that as alcohol content increases, density tends to decrease. |
| **Variance (Eigen)**| Eigenvalue 1 is significantly larger than Eigenvalue 2, meaning the first principal component (driven heavily by alcohol) captures almost all the variance in this feature space. |
| **Probability** | Quality 5 is the most common (~42%). Together, scores 5 and 6 account for roughly 82% of all wines in the dataset. Extreme scores (3 or 8) are very rare (< 2%). |

## libraries used
To run this notebook, you need Python 3 installed along with the following libraries:
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`

google colab file : https://colab.research.google.com/drive/1VFqnG_iue7LkvSp9iY3NBV0noG_b2S2x?usp=sharing
