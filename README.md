Transaction Categorization using Logistic Regression
This project uses a trained Logistic Regression model to automatically categorize financial transactions. It's designed to help users analyze and label transaction data efficiently.
```
📁 Project Structure
├── trained_logisticRegressionModel.pkl   # Pre-trained Logistic Regression model
├── trans_categorization.ipynb            # Jupyter Notebook with preprocessing and inference logic
├── README.md 
```

# Project documentation
Load the data from this link: https://drive.google.com/file/d/1qzazL0CYllIVb39aWrK77AXJjdmsYU-M/view?usp=sharing

Features
Load and use a pre-trained LogisticRegression model for classifying transactions.

Preprocessing pipeline likely includes:

Text feature extraction (e.g., from transaction descriptions)

Encoding categorical variables

Normalization/scaling

Example transaction data usage

Inference and prediction


Requirements
Install the dependencies using pip:
pip install pandas numpy scikit-learn joblib
If you're using the notebook:
pip install jupyter


Usage
1. Launch the Notebook
jupyter notebook trans_categorization.ipynb

3. Use the Model

4. Example Code Snippet

import joblib
import pandas as pd

# Load the model
model = joblib.load("trained_logisticRegressionModel.pkl")

# Load your transaction data
df = pd.read_csv("your_transactions.csv")

# Preprocess as shown in the notebook...

# Predict
predictions = model.predict(preprocessed_data)




