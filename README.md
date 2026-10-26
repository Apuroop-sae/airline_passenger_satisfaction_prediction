# ✈️ Airline Passenger Satisfaction Prediction Using Logistic Regression

A machine learning project that predicts airline passenger satisfaction using **Logistic Regression**. This project explores passenger data, performs data preprocessing and exploratory data analysis, trains a classification model, and uses the saved model to make predictions.

## 📌 Project Overview

Passenger satisfaction is an important factor in the airline industry. Understanding passengers' experiences can help identify areas where airline services may be improved.

The objective of this project is to build a machine learning model that predicts whether an airline passenger is **satisfied** or **neutral/dissatisfied** based on information about their flight experience, service ratings, and travel details.

The project uses Python and Scikit-learn to implement the machine learning workflow, from data analysis and preprocessing to model training and prediction.

## 🎯 Project Objectives

- Explore and understand airline passenger satisfaction data.
- Perform exploratory data analysis (EDA) using data visualization.
- Clean the dataset and handle missing values.
- Encode categorical variables and scale numerical features.
- Train a Logistic Regression classification model.
- Evaluate model performance using classification metrics.
- Save the trained model for reuse.
- Predict passenger satisfaction using new input data.

## 📊 Dataset

The project uses an airline passenger satisfaction dataset containing information about passengers, their journeys, and their ratings of airline services.

### Important features

| Category | Examples |
|---|---|
| Passenger information | Gender, Age, Customer Type |
| Travel information | Type of Travel, Class, Flight Distance |
| Service ratings | Seat Comfort, Food and Drink, Inflight Wi-Fi Service |
| Other service features | Online Boarding, Baggage Handling, Inflight Entertainment |
| Flight delays | Departure Delay in Minutes, Arrival Delay in Minutes |

**Target variable:** `satisfaction`

The target contains two classes:

- `satisfied`
- `neutral or dissatisfied`

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical data visualization
- **Scikit-learn** — Data preprocessing and machine learning
- **Joblib** — Model serialization and loading
- **Jupyter Notebook** — Interactive development and analysis

## ⚙️ Project Workflow

### 1. Data Loading and Cleaning

The dataset is loaded into a Pandas DataFrame. The data is inspected to understand its structure, data types, statistical summaries, and missing values. Unnecessary identifier columns are removed where appropriate.

### 2. Exploratory Data Analysis (EDA)

Exploratory data analysis is performed to understand the distribution of passenger satisfaction and investigate numerical and categorical features.

Visualizations help explore passenger characteristics, service ratings, and flight delay patterns.

### 3. Data Preprocessing

The data is prepared for machine learning through the following steps:

- Separating input features from the target variable.
- Splitting data into training and testing sets.
- Handling missing numerical values using median imputation.
- Handling missing categorical values using most-frequent imputation.
- Encoding categorical features using One-Hot Encoding.
- Scaling numerical features using StandardScaler.

A Scikit-learn preprocessing pipeline helps apply the appropriate transformations consistently.


### 4. Model Training

Logistic Regression is used as the classification algorithm to learn the relationship between passenger information and satisfaction labels.

The trained model estimates the probability of each satisfaction class and predicts the most likely class according to its classification threshold.

### 5. Model Evaluation

The trained model is evaluated on held-out test data to measure its predictive performance.

The evaluation can include:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

These metrics help assess the model's overall performance and its ability to distinguish between satisfied and neutral/dissatisfied passengers.

### 6. Model Saving and Prediction

The trained model is saved using Joblib so that it can be loaded and reused without retraining every time.

The separate prediction notebook, `new_pred.ipynb`, is included for the prediction workflow.

## 📁 Repository Structure

```text
airline_passenger_satisfaction_prediction/
│
├── data/                       # Dataset files
├── Log_Pred.ipynb               # Data analysis and model training
├── new_pred.ipynb               # Prediction workflow
├── logistic-reg_trained         # Saved trained model
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

## 🚀 Getting Started

### Prerequisites

Install Python and Git. Python 3.10 or another version compatible with your installed dependencies is recommended.

### 1. Clone the repository

```bash
git clone https://github.com/Apuroop-sae/airline_passenger_satisfaction_prediction.git
```

### 2. Navigate to the project directory

```bash
cd airline_passenger_satisfaction_prediction
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

Activate the environment.

**Windows**

```bash
.venv\Scripts\activate
```
```

### 4. Install the dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the training notebook

```bash
jupyter notebook Log_Pred.ipynb
```

Run the notebook cells in order to explore the data, perform preprocessing, train the model, and evaluate its performance.

### 6. Run the prediction notebook

```bash
jupyter notebook new_pred.ipynb
```

Follow the notebook cells to load the saved model and perform predictions using the expected input features.

## 📈 Overall Model Performance

Model Training — Log_Pred.ipynb

| Metric | Result |
|---|---|
| Accuracy | 87% |
| Precision | 88% |
| Recall | 87.5% |
| F1-score | 87% |

Prediction and Evaluation — new_pred.ipynb

| Metric | Result |
|---|---|
| Accuracy | 87% |
| Precision | 87% |
| Recall | 86.5% |
| F1-score | 87% |

*Replace the placeholders with your actual test-set results. Do not report unverified performance values.*

## 💡 Key Learnings

- Understanding the end-to-end machine learning workflow.
- Performing exploratory data analysis on real-world data.
- Handling missing values and categorical features.
- Building preprocessing pipelines with Scikit-learn.
- Applying Logistic Regression to a binary classification problem.
- Evaluating classification performance using multiple metrics.
- Saving and reusing trained machine learning models.

## 🔮 Future Improvements

- Compare Logistic Regression with other classification algorithms.
- Perform hyperparameter tuning to improve model performance.
- Analyze model coefficients to understand feature relationships.
- Build an interactive prediction interface using Streamlit.
- Explore model interpretability and additional evaluation techniques.

## 👨‍💻 Author

**Apuroop**

GitHub: [@Apuroop-sae](https://github.com/Apuroop-sae)



#### This project is intended for educational purpose only.
