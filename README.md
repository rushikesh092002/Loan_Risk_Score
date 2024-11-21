# **Loan Risk Score Prediction**

This project predicts the loan risk score based on various financial and personal details of loan applicants. The goal is to classify the risk of approving a loan based on features like age, income, credit score, and more. The best performing model in this project is **CatBoost Regressor**, achieving an impressive **99% R² score**.

## Project Overview

- **Dataset**:  
  The dataset contains features such as **Age**, **Annual Income**, **Credit Score**, **Employment Status**, **Education Level**, **Experience**, **Loan Amount**, **Loan Duration**, and more. These features are used to predict the **Risk Score** and determine if a loan will be approved.
- **Objective**:  
  Predict the risk score of a loan approval using machine learning regression techniques.
- **Best Model**:  
  **CatBoost Regressor** achieved the highest R² score of **99%**.

## Project Structure

```plaintext
├── artifacts/  
│   ├── data.csv                        # Full dataset  
│   ├── model.pkl                       # Saved CatBoost model  
│   ├── preprocessor.pkl                # Saved preprocessor  
│   ├── test.csv                        # Testing dataset  
│   ├── train.csv                       # Training dataset  
├── catboost_info/                      # CatBoost training logs  
├── notebook/  
│   └── eda_and_model_training.ipynb    # Jupyter notebook for EDA and training  
├── src/  
│   ├── components/                     # Core components  
│   │   ├── __init__.py  
│   │   ├── data_ingestion.py           # Data ingestion pipeline  
│   │   ├── data_transformation.py      # Data preprocessing and transformation  
│   │   └── model_trainer.py            # Model training pipeline  
│   ├── pipeline/  
│   │   ├── __init__.py  
│   │   ├── predict_pipeline.py         # Prediction pipeline  
│   │   └── train_pipeline.py           # Training pipeline  
│   ├── __init__.py  
│   ├── exception.py                    # Custom exception handling  
│   ├── logger.py                       # Logging setup  
│   └── utils.py                        # Utility functions  
├── templates/                          # HTML templates for web interface  
│   ├── home.html  
│   └── index.html  
├── .gitignore                          # Git ignore file  
├── README.md                           # Project documentation  
├── app.py                              # Flask application for deployment  
├── requirements.txt                    # Python dependencies  
├── setup.py                            # Package setup file  

