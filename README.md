# Network Intrusion Detection with SVM on UNSW-NB15

## Overview
This project implements a Network Intrusion Detection System (NIDS) using Support Vector Machine (SVM) on the UNSW-NB15 dataset. It also compares SVM with other machine learning models.

Two tasks are performed:
- Binary classification (Normal vs Attack)
- Multi-class classification (10 attack categories)

Main techniques:
- Log10 scaling and standardization
- GridSearchCV for hyperparameter tuning
- Handling class imbalance using class weights

---

## Dataset
UNSW-NB15 dataset is used.

Download from:
- https://research.unsw.edu.au/projects/unsw-nb15-dataset  
- https://www.kaggle.com/datasets/mrwellsdavid/unsw-nb15  

Files required:
- UNSW_NB15_training-set.csv
- UNSW_NB15_testing-set.csv

Place both files in the project folder.

---

## Project Structure


├── F208_div4.ipynb  
├── UNSW_NB15_training-set.csv  
├── UNSW_NB15_testing-set.csv  
├── model_results.csv  
├── figures (generated images)  
└── README.md  

---

## Setup

Install required libraries:

pip install numpy pandas matplotlib seaborn scikit-learn jupyter

---

## Usage

1. Clone the repository

git clone https://github.com/your-username/repo-name.git  
cd repo-name  

2. Add dataset files

Place:
UNSW_NB15_training-set.csv  
UNSW_NB15_testing-set.csv  

3. Run the notebook

jupyter notebook F208_div4.ipynb  

4. Run all cells in order

- Cell 1: SVM training and testing  
- Cell 2: Other models  
- Cell 3: Graphs and results  

---

## Results

Binary classification:
 - Training Accuracy  : 95.56%   
 - Testing  Accuracy  : 88.18%   
 - DR  (anomaly class): 92.36%   
 - FAR                : 11.82%   

Multi-class classification:
- Accuracy: 65.99%

SVM performs better than most baseline models.

---

## Report Summary

Steps:
1. Data preprocessing (cleaning, encoding, scaling)
2. Hyperparameter tuning using GridSearchCV
3. Model training using SVM
4. Evaluation using accuracy and other metrics

Findings:
- SVM gives strong performance on this dataset
- Random Forest is also competitive
- Proper scaling improves results
- Supervised models perform better than unsupervised methods

---

## Reference

Jing, D., & Chen, H. (2019). SVM based network intrusion detection for the UNSW-NB15 dataset.

---

## Note

This project is for academic use.
