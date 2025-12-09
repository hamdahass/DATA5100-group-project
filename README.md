# Breast Cancer Prediction

> The purpose of this project is to identify which cell-level characteristics are most strongly associated with the presence of breast cancer. Using the Breast Cancer Wisconsin dataset, we examine how various features of cell nuclei—such as radius, texture, perimeter, area, smoothness, concavity, and symmetry—differ between benign and malignant diagnoses. By comparing these measurements across the two groups, this analysis aims to determine which variables serve as the strongest indicators of malignancy and therefore may be most useful for predicting breast cancer.

---

## Project Overview

We can use this dataset to investigate the following
    Which features show the biggest differences between benign and malignant tumors?
    Are malignant tumors larger in size?
    Do malignant tumors have more irregular shapes?
    Which features are the BEST predictors of cancer? (ML)
    Which features correlate strongest with the diagnosis?
    Can a single feature predict cancer almost as well as multiple features? (ML)

This project seeks to use machine learning to predict the presence of breast cancer. The data used is the Breast Cancer Wisconsin (Diagnostic) data set available at the UC Irvine Machine Learning Repository. The key finding was that we were able to build an XGBoost model that predicted the presence of breast cancer with over 99% accuracy.

- **Objective:** Predict the presence of breast cancer
- **Domain:** Healthcare
- **Key Techniques:** Logistic Regression, Random Forest, XGBoost

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Source:** https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic 
- **Description:** Brief overview of the dataset features, size, and format
    The data used in the project was the Breast Cancer Wisconsin data set found at the UC Irvine Machine Learning Repository. This data includes 30 numerical features, one ID column, and one diagnosis column. The 30 numerical features are quantitative features extracted from the digitized images of the cell nuclei taken from a fine needle aspiration of the mass. There are ten quantitative characteristics: radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension. The first ten features are the mean of each of these characteristics. The second ten features are the standard deviation of each of these characteristics. The third and final ten features are the worst of each of these characteristics. The diagnosis column is a binary column, either M or B for malignant or benign. There are 569 instances.
  **File Name:** breast_cancer.csv  
- **License:** (if applicable)

---

## Analysis

Python was used to perform the analysis in a Jupyter notebook. Logistic regression, random forest, and XGBoost models were built to predict the diagnosis using the thirty features. The code will reproduce the results if run in order.

---

## Results

All of the models predicted the diagnosis, some better than others. The XGBoost model predicted the diagnosis with over 99% accuracy. This implies that a model can predict the diagnosis using these features.

---

## Authors

- Hamda Hassan - https://github.com/hamdahass/
- Jennifer Poling - https://github.com/jnplng/

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- Tools/libraries used: Python: NumPy, Pandas, Matplotlib, Seaborn, scikit-learn, statsmodels, XGBoost
- Tutorials or papers referenced
- Inspiration or collaborators
