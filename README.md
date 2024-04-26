# Facebook Page Classification Using Graph-Based Machine Learning Models

This repository contains the implementation and evaluation of various machine learning models to classify Facebook pages based on their content and structural relationships within a Facebook graph dataset.

## Dataset Description

The dataset consists of nodes representing official Facebook pages categorized into four types: politicians, governmental organizations, television shows, and companies. Edges between nodes represent mutual likes among these pages.

### Data Files

- **Node Features:** JSON files with keywords associated with each node, encoded as integers.
- **Edges Data:** CSV file containing mutual likes between pages.
- **Node Labels and Information:** CSV file with node IDs and their respective categories.

## Models Implemented

1. **Support Vector Machine (SVM)**
2. **CatBoost Classifier**
3. **XGBoost Classifier**
4. **Graph Convolution Network (GCN)**

Each model uses a combination of node features and structural information, with detailed evaluations provided in the results section.

## Results and Evaluation
The performance of each model is quantified using metrics like accuracy, confusion matrix, and classification report. Detailed results are as follows:

SVM: Best accuracy of 98.22% with both node features and neighbor information.

CatBoost: Highest accuracy of 95.68% with combined data.

XGBoost: Similar performance to CatBoost with an accuracy of 95.59%.

GCN: Reached an accuracy of 87%, showing effectiveness yet lower than classic models.

## Discussion

Analysis reveals that models combining node attributes and neighbor information generally outperform those using only one type of data, highlighting the complex interplay between content-based and structural characteristics of the nodes. Also, we found that Classical ML methodlogy worked better for this problem.
