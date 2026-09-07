# Startup Profit Prediction and Analysis 🚀

## 📌 Project Overview
Startups allocate budgets across **R&D**, **Marketing**, and **Administration**. This project performs exploratory data analysis and uses machine learning to predict startup profitability based on expenditure patterns, helping business stakeholders optimize their budget allocation.

---

## 🎯 Objectives
* **Analyze** expenditure patterns and their relationship with startup profits.
* **Identify** primary financial drivers of profitability.
* **Build & Evaluate** a Linear Regression model for profit prediction.
* **Visualize** business metrics and correlations through an interactive Power BI dashboard.

---

## 📊 Dataset Description
The dataset consists of 50 startup records containing operational spending details and profit margins:

| Feature | Description |
| :--- | :--- |
| **R&D Spend** | Research & Development investment |
| **Administration** | Administrative operational expenses |
| **Marketing Spend** | Marketing and promotional investments |
| **State** | Location of the startup (New York, California, Florida) |
| **Profit** | Target variable representing net profit |

---

## 🛠️ Tech Stack & Tools
* **Database & Querying:** MySQL
* **Programming Language:** Python[cite: 1]
* **Libraries:** Pandas, NumPy, Scikit-Learn[cite: 1]
* **Data Visualization:** Power BI[cite: 1]

---

## 📈 Model Performance & Evaluation
A **Multiple Linear Regression** model was trained using an 80/20 train-test split (`test_size=0.2`, `random_state=42`)[cite: 1].

```python
# Feature & Label Selection
features = df[["RD_Spend", "Administration", "Marketing_Spend"]]
label = df["Profit"]

# Train/Test Split
Xtrain, Xtest, Ytrain, Ytest = train_test_split(features, label, test_size=0.2, random_state=42)

# Model Training
model = LinearRegression()
model.fit(Xtrain, Ytrain)

----


----
## Author

Manoj Prabhakar


<img width="1920" height="1080" alt="Screenshot (728)" src="https://github.com/user-attachments/assets/b1b70d1c-fbb8-4bf4-a619-ceac019ea2ff" />
