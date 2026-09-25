# 📊 Week 3 — Statistical Modeling & Hypothesis Testing

## Statistical Modeling and Hypothesis Testing using Python

This project focuses on applying statistical concepts to a real-world public dataset. The analysis explores relationships between health-related variables using **Multiple Linear Regression**, hypothesis testing, parameter estimation, and statistical diagnostics.

---

## 🎯 Objective

The main objective of this project is to:

* Formulate a clear research question and statistical hypotheses.
* Clean and prepare a publicly available dataset.
* Build a suitable statistical regression model.
* Estimate model parameters and test their statistical significance.
* Check assumptions such as multicollinearity, normality, and residual behavior.
* Interpret the results and identify limitations of the analysis.

---

## 🔎 Research Question

**Can BMI be statistically explained by selected health and demographic variables?**

The project investigates whether variables such as age, blood pressure, glucose level, insulin, skin thickness, and other measurements are significantly associated with BMI.

---

## 🧪 Hypotheses

### Null Hypothesis — H₀

The selected predictor variables do not have a statistically significant linear relationship with BMI.

### Alternative Hypothesis — H₁

At least one selected predictor variable has a statistically significant linear relationship with BMI.

The significance level used in the analysis is:

**α = 0.05**

---

## 📁 Dataset

The project uses a **publicly available health/diabetes dataset** containing medical and demographic measurements.

Important variables include:

| Variable                 | Description                  |
| ------------------------ | ---------------------------- |
| Pregnancies              | Number of pregnancies        |
| Glucose                  | Plasma glucose concentration |
| BloodPressure            | Diastolic blood pressure     |
| SkinThickness            | Skin fold thickness          |
| Insulin                  | Serum insulin level          |
| BMI                      | Body Mass Index              |
| DiabetesPedigreeFunction | Diabetes pedigree function   |
| Age                      | Age of the individual        |
| Outcome                  | Diabetes outcome             |

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Statsmodels
* Scikit-learn
* Jupyter Notebook

---

## 🔬 Methodology

### 1. Data Loading

The dataset was imported using Pandas and inspected for its structure, data types, and missing values.

### 2. Data Cleaning

The dataset was checked for:

* Missing values
* Invalid values
* Duplicate observations
* Incorrect data types
* Potential outliers

### 3. Exploratory Data Analysis

Descriptive statistics and visualizations were used to understand:

* Variable distributions
* Correlations
* BMI relationships with predictors
* Potential patterns and outliers

### 4. Multicollinearity Analysis

Variance Inflation Factor (**VIF**) was calculated to identify highly correlated predictors.

This step was important because severe multicollinearity can make regression coefficients unstable and make individual p-values difficult to interpret.

### 5. Regression Model

A **Multiple Linear Regression** model was fitted with BMI as the dependent variable.

General form:

```text
BMI = β₀ + β₁X₁ + β₂X₂ + ... + βₖXₖ + ε
```

where:

* β₀ = intercept
* β₁...βₖ = regression coefficients
* X = predictor variables
* ε = error term

### 6. Hypothesis Testing

For each regression coefficient:

```text
H₀: βᵢ = 0
H₁: βᵢ ≠ 0
```

A predictor was considered statistically significant when:

```text
p-value < 0.05
```

### 7. Model Diagnostics

The following diagnostics were performed:

* Residual vs fitted plot
* Q-Q plot
* Multicollinearity/VIF analysis
* R² and adjusted R²
* Coefficient significance tests

---

## 📈 Model Evaluation

The model was evaluated using:

### R²

Measures the proportion of variation in BMI explained by the predictors.

### Adjusted R²

Provides a more conservative measure of model fit by accounting for the number of predictors.

### P-values

Used to determine whether individual predictors provide statistically significant evidence of association with BMI.

### Residual Analysis

Residual plots were used to investigate:

* Non-linearity
* Unequal variance
* Potential outliers
* Approximate normality of errors

---

## 💡 Key Findings

The statistical analysis demonstrates that BMI can be modeled using measurable health and demographic variables.

The full model also showed evidence of **multicollinearity among some predictors**, which can inflate coefficient uncertainty and complicate interpretation.

Therefore, the analysis considered a reduced predictor set for more reliable statistical inference.

The regression results were interpreted using:

* Regression coefficients
* Standard errors
* t-statistics
* p-values
* Confidence intervals
* R² / adjusted R²
* Residual diagnostics

The results provide statistical evidence about which variables are associated with BMI while also showing why model assumptions and diagnostics are important.

---

## 📊 Visualizations

The project includes:

1. BMI distribution and target relationship
2. Residual vs fitted values
3. Q-Q plot of residuals
4. VIF analysis for multicollinearity

These visualizations help validate the assumptions of the statistical model.

---

## 📂 Project Structure

```text
Week-3-Statistical-Modeling/
│
├── data/
│   └── dataset.csv
│
├── figures/
│   ├── 01_bmi_target.png
│   ├── 02_residuals_fitted.png
│   ├── 03_qq.png
│   └── 04_vif_full.png
│
├── Week_3_Statistical_Modeling_Code.py
├── Week_3_Statistical_Modeling_Hypothesis_Testing_Report.docx
└── README.md
```

---

## 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/your-username/week-3-statistical-modeling.git
```

Move into the project:

```bash
cd week-3-statistical-modeling
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
```

Run the Python script:

```bash
python Week_3_Statistical_Modeling_Code.py
```

For a Jupyter Notebook workflow:

```bash
jupyter notebook
```

---

## 📚 What I Learned

Through this project, I strengthened my understanding of:

* Statistical hypothesis formulation
* Null and alternative hypotheses
* Multiple linear regression
* Parameter estimation
* P-values and statistical significance
* Confidence intervals
* R² and adjusted R²
* Multicollinearity and VIF
* Residual analysis
* Q-Q plots
* Model assumptions
* Statistical interpretation

---

## 🔮 Future Improvements

Future versions of this project could include:

* Robust regression techniques
* Feature selection using statistical criteria
* Transformation of skewed variables
* Cross-validation
* Regularization techniques such as Ridge and Lasso
* Non-linear regression models
* Additional statistical tests
* Comparison of multiple model specifications

---

## 👨‍💻 Author

**Kartik Koli**

BCA Student | Aspiring AI/ML Engineer

Interested in:

**Artificial Intelligence • Machine Learning • Data Science • Generative AI**

---

## ⭐ Project Highlights

This project demonstrates an end-to-end statistical workflow:

```text
Dataset
   ↓
Data Cleaning
   ↓
Exploratory Analysis
   ↓
Hypothesis Formulation
   ↓
Regression Modeling
   ↓
Parameter Estimation
   ↓
P-value Testing
   ↓
Multicollinearity Check
   ↓
Residual Diagnostics
   ↓
Interpretation
```

---

⭐ **If you find this project useful, consider starring the repository!**
