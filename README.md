# Tree-Based Models
Conditional Inference Tree and Random Forest classification for graduate admission prediction.

## Overview
This project applies tree-based classification methods to predict graduate admission outcomes. A Conditional Inference Tree provides interpretable decision rules, while the Random Forest and Bagging ensembles did not improve overall test accuracy over the single tree but were much better at identifying non-admits.

## Dataset
- **Source:** Graduate Admission dataset
- **Key variables:** GRE Score, TOEFL Score, University Rating, SOP, LOR, CGPA, Research Experience

## Methods
- Conditional Inference Tree using the `party` package
- Random Forest for ensemble classification
- Bagging (Random Forest with all predictors tried at each split)
- Variable importance ranking
- Model comparison and evaluation with `caret`

## Key Findings
- The Conditional Inference Tree identified CGPA as the primary split variable (threshold at 8.03)
- For applicants with CGPA at or below 8.03 the next split was on LOR (threshold at 2.5); above 8.03 the tree split on CGPA again (threshold at 8.5)
- Random Forest and Bagging did not improve overall test accuracy over the single tree (0.85 and 0.8625 vs 0.8625), but both were much better at identifying non-admits (specificity 0.61 vs 0.39)

## Tools & Libraries
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=R&logoColor=white)
![party](https://img.shields.io/badge/party-276DC3?style=flat-square&logo=r&logoColor=white)
![caret](https://img.shields.io/badge/caret-276DC3?style=flat-square&logo=r&logoColor=white)
![randomForest](https://img.shields.io/badge/randomForest-276DC3?style=flat-square&logo=r&logoColor=white)

## How to Run
1. Clone the repository: `git clone https://github.com/BronsonBagwell/Tree_Based_Models.git`
2. Open the HTML file in a browser, or run the R Markdown file in RStudio
3. Required packages: `party`, `caret`, `randomForest`
