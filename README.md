# ML-Powered Churn Insights for Telka Co.
![Telka Welcome](images/telka_welcome.png)
## Project Overview
Telka, a fictional national telecom provider, has been experiencing significant customer churn, especially among users with flexible contracts and digital payment options. As customer acquisition costs continue to rise, retaining existing users has become more important—and more cost-effective—than ever.

This project leverages machine learning classification techniques to predict which customers are likely to churn. By analyzing behavioral, demographic, and service-related data, we identify the key drivers behind churn and develop a predictive model to flag high-risk customers in advance.

## Objectives
The key objectives of this project is:
1. **Predict Churn** with high accuracy models like Logistic Regression and Decision Trees
2. **Identify key features** influencing customer churn i.e. contract type, tenure or payment method
3. **Support business decisions** with clear, data-driven recommendation for customer retention
4. **Visualise insights** through interpretable, stake-holder friendly charts and dashboards

Customer churn directly affects Telka’s bottom line. With this project, Telka can:
1. Proactively target at-risk customers with personalised retention offers
2. Re-evaluate contract structures and billing methods to reduce churn likelihood
3. Improve long-term customer loyalty and boost lifetime value

## The Dataset
The dataset, `customer_churn.csv`, contains customer information such as their demographics, account details and service usage for a telcom provider. 

The target variable is `Churn` which indicates whether a customer has left the company. The data is located in the `data/` folder.

- **Source:** [Telco Customer Churn on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data)


## Approach

The project follows a structured data science workflow:

1. **Exploratory Data Analysis (EDA):** Data cleaning, handling missing values, and visualizing distributions and relationships to understand key churn drivers.
2. **Feature Engineering:** Encoding categorical variables, scaling numerical features, and creating new features based on domain knowledge.
3. **Modeling:** Multiple supervised learning algorithms are compared, including Logistic Regression, Decision Trees, Random Forests, Gradient Boosting, and CatBoost.
4. **Evaluation:** Models are evaluated using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC. Hyperparameter tuning is performed for optimal results.
5. **Reporting:** Key findings and model comparisons are summarized in the final report.

## Project Structure
- [**data/**](data/): Contains the primary dataset used for analysis and modelling i.e. `customer_churn.csv`.
- [**images/**](images/): This folder stores all static visual assets used throughout the project such as:
    1. Exploratory charts
    2. Feature importance plots
    3. Model evaluation visuals
    4. Presentation-ready graphics
- [**notebooks**](notebooks/): Contains modular notebooks, each dedicated to a specific section of the main workflow i.e. EDA, feature engineering, model training, etc. This is for easier navigation and experimentation.
- [**results**](results/): A storage folder for model perfomance and other table-like outputs.

## Data Explanation
The dataset contains 7403 rows (customers) and 21 features (20 features + 1 target). It is in tabular format, with each row representing a customer and column representing a demographic, service-related or account-related variable.

Among the features:
- 3 are numerical i.e. `tenure`, `MonthlyCharges` `TotalCharges`
- 5 are binary i.e. `Dependents`, `SeniorCitizen`
- 13 are categorical i.e. `gender`, `InternetService`, etc.

The dataset is self-contained and thus does not require any merging of external data. This, coupled with the data being small in size (less than 1MB), making it manageable for EDA and model experimentation.

## License
This project is for environmental purposes.