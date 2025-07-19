# -Task-5-Personal-Loan-Acceptance-Prediction-using-the-Bank-Marketing-Dataset-
# Personal Loan Acceptance Prediction

## 📌 Objective

The goal of this project is to predict which customers are likely to accept a personal loan offer using the **Bank Marketing Dataset** from the UCI Machine Learning Repository.

---

## 🗂️ Dataset Information

**Source**: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)  
**File Used**: `bank-full.csv`  
**Records**: 45,211  
**Features**: 17 input attributes + 1 target (`y`)

### Key Features:
- **age**: Customer’s age
- **job**: Type of job
- **marital**: Marital status
- **education**: Education level
- **default**: Has credit in default?
- **balance**: Average yearly balance in euros
- **housing**: Has a housing loan?
- **loan**: Has a personal loan?
- **contact**: Contact communication type
- **day/month**: Last contact date
- **campaign**: Number of contacts during the campaign
- **pdays**: Days since the client was last contacted (999 = not contacted)
- **previous**: Number of contacts before the campaign
- **poutcome**: Outcome of previous marketing campaign
- **y**: **Target variable** – Did the client subscribe to a term deposit? (`yes` = 1, `no` = 0)

---

## 🧪 Exploratory Data Analysis (EDA)

Performed basic exploration:
- Checked distributions of `job`, `marital`, `education`, etc.
- Visualized acceptance rates by job and marital status
- Handled categorical features using one-hot encoding

---

## ⚙️ Model Building

Two models were trained and evaluated:
- ✅ **Logistic Regression**
- ✅ **Decision Tree Classifier**

### Preprocessing Steps:
- Converted categorical variables using `pd.get_dummies()`
- Converted target `y` to binary (1 for "yes", 0 for "no")
- Used 70/30 train-test split

---

## 📈 Evaluation Metrics

- **Accuracy**
- **Precision / Recall / F1 Score**
- **Confusion Matrix**
- **Feature Importance (coefficients & tree splits)**

---

## 💡 Key Insights

- Customers with **higher balance**, **cellular contact**, and **previous successful campaign** were more likely to accept the offer.
- **Management** and **entrepreneur** job roles showed higher acceptance.
- **Married** clients were slightly less likely to accept compared to **single** clients.

---

## 📂 Folder Structure

