# House Credit Default Prediction

This project predicts whether a loan applicant will default using machine learning models trained on the Home Credit Default Risk dataset.

Financial institutions need to estimate credit risk before approving loans. This project builds predictive models using financial and demographic features to identify potential loan defaults.

## Dataset

This project uses the **Home Credit Default Risk dataset**.

Due to file size restrictions, the dataset is not included in this repository.

You can download it from Kaggle:

https://www.kaggle.com/competitions/home-credit-default-risk/data

After downloading, place the file in the project folder:

data/application_train.csv

The dataset contains historical loan application data including:

- Client income
- Credit amount
- Loan annuity
- External credit scores
- Demographic information

Each record represents a loan application.

Target variable:

TARGET  
0 → Loan repaid  
1 → Loan defaulted

## Project Workflow

1. Data preprocessing and cleaning
2. Missing value handling
3. Encoding categorical variables
4. Feature engineering
5. Model training
6. Model comparison
7. Hyperparameter tuning
8. Final model evaluation

## Feature Engineering

Additional features were created based on financial relationships and risk indicators.

Examples:

- credit_income_ratio
- annuity_income_ratio
- credit_annuity_ratio
- ext_source_mean
- ext_source_pred
- ext_diff

These engineered features capture relationships between credit amount, income, and external risk scores.

## Models Used

The following machine learning models were trained and evaluated:

- Logistic Regression
- Random Forest
- Decision Tree
- K-Nearest Neighbors
- Gradient Boosting
- XGBoost
- LightGBM

Model performance was evaluated using cross-validation and ROC-AUC.

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

ROC-AUC was used as the primary evaluation metric due to class imbalance.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib

## Project Structure
HOUSE_CREDIT
│
├ credit_model.ipynb
├ README.md
├ data_description.md
└ requirements.txt

## How to Run

Install dependencies:
pip install -r requirements.txt
Then open the notebook:
credit_model.ipynb

## Author

Vivek  
B.Tech Computer Science and Engineering (AI & ML)  
VIT-AP University