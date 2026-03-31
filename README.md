# Tree-Based Models
Conditional Inference Tree and Random Forest classification for graduate admission prediction.

## Overview
This project applies tree-based classification methods to predict graduate admission outcomes. A Conditional Inference Tree provides interpretable decision rules, while a Random Forest offers improved predictive accuracy through ensemble learning.

## Dataset
- **Source:** Graduate Admission dataset
- **Key variables:** GRE Score, TOEFL Score, University Rating, SOP, LOR, CGPA, Research Experience

## Methods
- Conditional Inference Tree using the `party` package
- Random Forest for ensemble classification
- Variable importance ranking
- Model comparison and evaluation with `caret`

## Key Findings
- The Conditional Inference Tree identified CGPA as the primary split variable (threshold at 8.03)
- LOR served as the secondary splitting criterion
- Random Forest improved accuracy over the single tree model through aggregation

## Tools & Libraries
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=R&logoColor=white)
![party](https://img.shields.io/badge/party-276DC3?style=flat-square&logo=r&logoColor=white)
![caret](https://img.shields.io/badge/caret-276DC3?style=flat-square&logo=r&logoColor=white)
![randomForest](https://img.shields.io/badge/randomForest-276DC3?style=flat-square&logo=r&logoColor=white)

## How to Run
1. Clone the repository: `git clone https://github.com/BronsonBagwell/Tree_Based_Models.git`
2. Open the HTML file in a browser, or run the R Markdown file in RStudio
3. Required packages: `party`, `caret`, `randomForest`
