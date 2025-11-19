Concrete Compressive Strength Prediction
========================================

This project applies various machine learning regression and classification models to predict and analyze the concrete compressive strength based on its ingredient composition.

Dataset
-------

*   **Source**: UCI Machine Learning Repository
    
*   **Features**: Cement, Blast Furnace Slag, Fly Ash, Water, Superplasticizer, Coarse Aggregate, Fine Aggregate, Age, and derived features such as Water/Cement ratio, Total Aggregate, and Binder.
    
*   **Target**: Concrete compressive strength (MPa)
    

Project Structure
-----------------

*   **Data Preprocessing**: Cleaning data (removing Nan, Duplicates etc.) , Feature engineering (Combining features) and splitting the data.
    

**(Took Insights from a civil engineer about the dataset and how to treat each feature)**

**Mentioned everything in the code**

*   **Regression Models**: Linear regression, Polynomial regression, Ridge, Lasso, SVR, CatBoost, tree-based models (Random Forest, Gradient Boosting, XGBoost, LightGBM and CatBoost Regressor).
    
*   **Classification Models**: Binary classification of concrete strength following (Indian Standard IS 456:2000) using Logistic regression, SVM, Decision Trees, CatBoostClassifier, and more.
    
*   **Evaluation**: Used MSE, RMSE, R² for regression; Accuracy, Precision, Recall, F1-score for classification.
    

Requirements
------------

*   Python 3.x
    
*   Libraries: numpy, pandas, scikit-learn, catboost, matplotlib, seaborn,
    

Usage
------------

1.  Open the notebook ML_assignment2.ipynb.
    
2.  Run each cell step-by-step to preprocess data, fit models, and view results.
    

Insights
--------

*   For classification tasks, ensure labels are binary (0/1) before evaluating metrics.
    
*   CatBoost models handle categorical features natively and is the best performing
    
*   Removed L1 reg. in regression due to it diverging for some reason.
