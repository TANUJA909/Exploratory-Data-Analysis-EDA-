# Task 2: Exploratory Data Analysis (EDA) – Titanic Dataset

## Objective
To explore the Titanic dataset, understand its structure, identify patterns, visualize distributions, and derive insights that will guide machine learning model building.

---

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn


---

## Dataset
Dataset: [Titanic Dataset – Kaggle](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

---

## Steps Performed

### 1. Data Import & Inspection
- Loaded dataset using `pandas.read_csv()`.
- Viewed first few rows with `df.head()`.
- Checked dataset shape, data types, and non-null counts with `df.shape` and `df.info()`.
- Generated descriptive statistics using `df.describe()`.

### 2. Missing Values Analysis
- Identified missing values using `df.isnull().sum()`.
- Found `Age` and `Embarked` had a few missing values, while `Cabin` had many.

### 3. Numerical Feature Analysis
- Plotted histograms for `Age` and `Fare` to check distribution.
- Detected right skew in `Fare` distribution.
- Plotted boxplots for `Age` and `Fare` to identify outliers.

### 4. Categorical Feature Analysis
- Countplots for `Pclass`, `Sex`, `Embarked`, and `Survived`.
- Observed survival rate differences between male and female passengers, and across ticket classes.

### 5. Correlation Analysis
- Created a heatmap for numerical correlations.
- Observed moderate correlation between `Fare` and `Pclass`.

### 6. Relationship Analysis
- Grouped survival rates by `Sex`, `Pclass`, and `Embarked` to detect patterns.
- Females and passengers in first class had significantly higher survival rates.

### 7. Missingness Visualization
- Visualized null values using a heatmap.

---

## Key Insights
1. Dataset contains 891 rows and 12 columns.
2. `Cabin` column has excessive missing values and is likely to be dropped in preprocessing.
3. Females had a survival rate of over 70%, much higher than males.
4. First-class passengers had the highest survival rates, third-class the lowest.
5. Fare is heavily right-skewed with several extreme outliers.
6. Age distribution is roughly normal, with most passengers between 20 and 40 years old.

---




## Prepared By
Tanuja Deshmukh  
AI & ML Internship – Task 2
