# Breast Cancer Prediction

Breast cancer is the leading type of cancer in women worldwide, and it also affects men. The purpose of this project is to build a model that will predict the presence of breast cancer. We ask the following questions: Can we build a machine learning model to accurately predict whether a tumor is malignant or benign? Which features are the strongest indicators of malignancy? 

---

## Project Overview

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
- **Description:** 
    The data used in the project was the Breast Cancer Wisconsin data set found at the UC Irvine Machine Learning Repository. This data includes 30 numerical features, one ID column, and one diagnosis column. The 30 numerical features are quantitative features extracted from the digitized images of the cell nuclei taken from a fine needle aspiration of the mass. There are ten quantitative characteristics: radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension. The first ten features are the mean of each of these characteristics. The second ten features are the standard deviation of each of these characteristics. The third and final ten features are the worst of each of these characteristics. The diagnosis column is a binary column, either M or B for malignant or benign. There are 569 instances.
  **File Name:** breast_cancer.csv  
- **License:** (if applicable)

---

## Analysis

Python was used to perform the analysis in a Jupyter notebook. Logistic regression, random forest, and XGBoost models were built to predict the diagnosis using the thirty features. The code will reproduce the results if run in order.

---

## Results

We analyzed the Breast Cancer Wisconsin Diagnostic dataset to determine how well different machine learning models could predict whether a tumor is malignant or benign based on 30 numerical features extracted from biopsy images. We tested several modeling approaches, including single-feature logistic regression, multiple-feature models, Random Forest, and XGBoost.

Our single-input models showed that individual features like radius and concave points hold strong predictive power, but they also revealed limitations, especially in correctly identifying malignant tumors. Adding multiple features improved performance, demonstrating that cancer diagnosis cannot rely on one measurement alone.

Tree-based models produced the strongest results. Random Forest achieved over 91% accuracy and demonstrated the value of combining predictors. Our most successful approach, XGBoost, reached 99.12% accuracy and an AUC of 99.31%, misclassifying only one benign case and correctly identifying every malignant tumor in the test set. These results show that machine learning, especially advanced ensemble models can effectively support breast cancer detection by recognizing structural patterns in tumor cell features.

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
- https://www.cancercenter.com/community/blog/2023/01/whats-the-difference-benign-vs-malignant-tumors
- https://pmc.ncbi.nlm.nih.gov/articles/PMC7237065/ 
- https://pmc.ncbi.nlm.nih.gov/articles/PMC8184621/
- https://www.analyticsvidhya.com/blog/2018/09/an-end-to-end-guide-to-understand-the-math-behind-xgboost/
