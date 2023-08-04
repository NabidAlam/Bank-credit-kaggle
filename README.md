# Bank-credit-kaggle
 
Developed and implemented highly accurate classification models using Decision Tree, Random Forest, and XGBoost algorithms to predict customer subscription, enabling data-driven marketing strategies and maximizing term deposit conversions.
Dataset: https://www.kaggle.com/datasets/kapturovalexander/bank-credit-scoring

This project's main objective was to build and evaluate classification models to predict whether a customer would subscribe to a term deposit (binary classification) based on various features available in the 'bank.csv' dataset.

The project followed these major steps:

1. Data Preprocessing: The initial step involved loading the dataset using Pandas and performing exploratory data analysis (EDA). EDA included visualizing the distributions of categorical variables using countplots and density plots and box plots for numerical variables to identify potential outliers. The dataset contained categorical features such as job, marital status, education, etc., and numerical features like age, balance, duration, and more.

2. Label Encoding: Since most machine learning algorithms require numerical inputs, the categorical features were converted into a numerical format using Label Encoding. Each unique category in the categorical features was assigned a unique numerical value.

3. Model Building and Evaluation (Part 1): The project explored three classification algorithms: Decision Tree, Random Forest, and XGBoost. For each algorithm, hyperparameters were tuned using GridSearchCV to find the best combination. The models were trained on the preprocessed data and evaluated using performance metrics such as accuracy, F1 score, precision, recall, Jaccard score, and log loss. Confusion matrices were used to visualize the classification results.

4. Feature Importance Analysis: To gain insights into the significance of features in the models, feature importance plots were created using SHAP (SHapley Additive exPlanations) values. SHAP values help interpret the contribution of each feature towards individual predictions.

5. Model Evaluation (Part 2): ROC (Receiver Operating Characteristic) curves were generated to assess the classification performance of the models at different probability thresholds. AUC (Area Under the Curve) values were computed to quantify the models' ability to distinguish between positive and negative instances.

Overall, the project aimed to demonstrate the entire data science pipeline, from data preprocessing and exploratory data analysis to model building, hyperparameter tuning, and model evaluation. The analysis focused on understanding the effectiveness of the three classification models in predicting customer subscription to a term deposit, as well as the impact of different features on the model's decision-making process. The best-performing model was identified based on the evaluation metrics and used to make predictions on the test set.

The final model (XGBoost) achieved an accuracy score of 89.06%, indicating its success in accurately classifying customers likely to subscribe to the term deposit, making it a valuable tool for targeting potential customers for marketing campaigns.
