# 🚢 Titanic Survival Prediction

## 📌 Project Overview
This project aims to predict the survival of passengers on the Titanic using machine learning. By analyzing various features such as age, gender, ticket class, and fare, we train a **Logistic Regression** model to classify whether a passenger survived or not.

This analysis serves as a classic introduction to data science and machine learning techniques, covering data cleaning, exploratory data analysis (EDA), and model evaluation.

## 📂 Dataset
The dataset contains the following features:
- **Survived**: Target variable (0 = No, 1 = Yes)
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Sex**: Gender of the passenger
- **Age**: Age in years
- **SibSp**: Number of siblings/spouses aboard
- **Parch**: Number of parents/children aboard
- **Fare**: Passenger fare
- **Embarked**: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

> **Note**: Columns like `PassengerId`, `Name`, `Ticket`, and `Cabin` were excluded or dropped during preprocessing as they were deemed less relevant for this specific model or contained too many missing values.

## 🛠️ Technologies Used
- **Python 3.x**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-Learn**: Machine learning model building and evaluation

## ⚙️ Workflow

### 1. Data Collection & Preprocessing
- Loaded the dataset using Pandas.
- **Handling Missing Values**:
  - Dropped the `Cabin` column due to a high volume of missing data.
  - Imputed missing `Age` values with the mean age.
  - Imputed missing `Embarked` values with the mode (most frequent value).
- **Encoding**:
  - Converted categorical columns (`Sex` and `Embarked`) into numerical values for model compatibility.

### 2. Exploratory Data Analysis (EDA)
- Analyzed statistical measures of the data.
- Visualized survival counts based on gender and other demographics to identify key trends.

### 3. Model Training
- **Features (X)**: `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`
- **Target (Y)**: `Survived`
- Split the data into **Training (80%)** and **Testing (20%)** sets.
- Trained a **Logistic Regression** model on the training data.

### 4. Evaluation
The model's performance was evaluated using the accuracy metric:

| Metric | Score |
| :--- | :--- |
| **Training Data Accuracy** | **80.76%** |
| **Test Data Accuracy** | **78.21%** |

## 🚀 How to Run
1. **Clone the repository**:
   ```bash
   https://github.com/PranavbalajiGit/Titanic-Survival-Prediction.git
   ```
2. **Navigate to the project directory**:
   ```bash
   cd Titanic-Survival-Prediction
   ```
3. **Install the required dependencies**:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```
4. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook Titanic_Survival_Prediction.ipynb
   ```

## 📜 Future Improvements
- Experiment with other algorithms like Decision Trees, Random Forests, or SVM.
- Perform more in-depth feature engineering.
- Tune hyperparameters to improve accuracy.

---
*Results and analysis based on the `Titanic_Survival_Prediction.ipynb` notebook.*