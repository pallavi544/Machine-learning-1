#  Machine Learning Project – Diabetes Prediction Using Random Forest Classifier

This project demonstrates how to build a diabetes prediction model using the **Random Forest Classifier**. It follows a complete machine learning pipeline including data preprocessing, exploratory data analysis (EDA), model training, evaluation, and result interpretation.

---

##  Project Objective

To predict whether a patient is diabetic based on diagnostic health measurements using a supervised machine learning model.

---

##  Dataset Description

The dataset used is the **Pima Indians Diabetes Dataset**, which contains medical diagnostic data for female patients of Pima Indian heritage.

| Feature                   | Description                                               |
|---------------------------|-----------------------------------------------------------|
| Pregnancies               | Number of times pregnant                                  |
| Glucose                   | Plasma glucose concentration (mg/dL)                      |
| BloodPressure             | Diastolic blood pressure (mm Hg)                          |
| SkinThickness             | Triceps skinfold thickness (mm)                           |
| Insulin                   | 2-Hour serum insulin (mu U/ml)                            |
| BMI                       | Body Mass Index                                           |
| DiabetesPedigreeFunction  | Genetic influence on diabetes                             |
| Age                       | Age of the patient                                        |
| Outcome                   | 1 = Diabetic, 0 = Non-diabetic                            |

---

##  Tools & Technologies Used

- **Python**
- **Jupyter Notebook**
- **Libraries**:
  - pandas, numpy (data manipulation)
  - matplotlib, seaborn (data visualization)
  - scikit-learn (machine learning)

---

##  Workflow

### 1. **Data Loading**
- Data imported from `diabetes2.xlsx`.

### 2. **Data Preprocessing**
- Replaced zero values in `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, and `BMI` with `NaN`.
- Imputed missing values using the **median** of each column.
- Normalized the features using **StandardScaler** to prepare for training.

### 3. **Exploratory Data Analysis**
- Plotted feature distributions and correlations.
- Used a heatmap to visualize relationships among features.
- Identified highly correlated predictors (e.g., Glucose vs Outcome).

### 4. **Model Building – Random Forest Classifier**
- Applied **RandomForestClassifier** from `scikit-learn`.
- Split data into **training and testing sets** (typically 80/20 or 70/30).
- Trained the model using the training set.

### 5. **Model Evaluation**
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

---

##  Results

- **Model Used**: `RandomForestClassifier()`
- **Accuracy**: ~78% (approximate; may vary slightly)
- **Key Insight**:
  - Random Forest was chosen for its robustness, ability to handle missing/imbalanced data, and high accuracy.
  - Glucose, BMI, and Age were among the most important features.

---

## Learning Outcomes
* Gained hands-on experience in applying Random Forest for classification.

* Improved skills in:

* Data cleaning and imputation

* Feature scaling and transformation

* Evaluating classification models

* Understood how health data can be modeled using machine learning.

---

## How to Run Locally
1.Clone the repository:

```bash

git clone https://github.com/pallavi544/Machine-learning-1.git

```

2.Navigate to the folder:

```bash

cd Machine-learning-1

```

3.Install required packages (if not already installed):

```bash

pip install pandas numpy scikit-learn matplotlib seaborn jupyter

```

4.Launch the notebook:

```bash

jupyter notebook "machine learning project 1 (2).ipynb"

```
## View the Notebook Online
**[Click here to view the Jupyter Notebook online](https://github.com/pallavi544/Machine-learning-1/blob/main/machine%20learning%20project%201%20(2).ipynb)**




