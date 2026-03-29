

# 🏦 Loan Approval Prediction: ML-Powered Risk Analysis

## 🚀 Project Overview

This project develops a robust, automated **Loan Approval System** designed to assist financial institutions in making data-driven lending decisions. By analyzing historical applicant profiles—including credit scores (CIBIL), income levels, and asset distributions—the model predicts the probability of loan approval while significantly mitigating credit risk.

## ❗ Business Problem

Traditional manual loan appraisals are often slow, inconsistent, and prone to human bias. In the banking sector, incorrect decisions lead to two primary "cost" types:

  * **False Positives (Credit Risk):** Approving high-risk applicants who eventually default, leading to capital loss.
  * **False Negatives (Opportunity Cost):** Rejecting creditworthy applicants, resulting in lost interest revenue and reduced market share.

**The Goal:** Build a classification engine that maximizes approval accuracy while maintaining a high **Recall** for rejected cases to safeguard the institution's assets.

## 🎯 Objectives

  * **EDA:** Uncover hidden correlations between financial assets and approval rates.
  * **Data Pipeline:** Implement a clean preprocessing workflow (Label Encoding & Standard Scaling).
  * **Model Benchmarking:** Compare the interpretability of **Decision Trees** against the robustness of **Random Forests**.
  * **Performance Optimization:** Achieve a balance between Precision and Recall suitable for a risk-sensitive environment.

## 📊 Dataset Description

The dataset encompasses comprehensive financial and demographic applicant data:

  * **Financial Metrics:** Annual Income, Loan Amount, Loan Term, and CIBIL Score.
  * **Asset Portfolio:** Residential, Commercial, Luxury, and Bank asset values.
  * **Demographics:** Education level, Employment status, and Number of dependents.
  * **Target:** `loan_status` (Approved / Rejected).

## 🧠 Methodology

### 1\. Preprocessing & Engineering

  * Stripped leading/trailing whitespace from column headers and categorical entries.
  * Encoded categorical features using `LabelEncoder`.
  * Standardized numerical features via `StandardScaler` to ensure asset values didn't disproportionately bias the model.

### 2\. Modeling Approach

  * **Decision Tree Classifier:** Used as a baseline "White-Box" model to visualize decision logic.
  * **Random Forest Classifier:** Implemented an ensemble strategy to reduce variance and improve generalization.

### 3\. Evaluation Strategy

  * Utilized **Stratified Train-Test Splitting (75/25)** to maintain class proportions.
  * Prioritized the **Confusion Matrix** and **Recall** to ensure "Rejected" cases were accurately identified.

## 📈 Key Results & Insights

✅ **Model Superiority:** The **Random Forest Classifier** achieved a state-of-the-art accuracy of **98.31%**, significantly outperforming the standalone Decision Tree.

🔍 **The CIBIL Factor:** Feature importance analysis revealed that the **CIBIL Score** accounts for approximately **80% of the model's predictive power**.

💡 **Business Impact:** \* **Risk Mitigation:** The model achieved a **Recall of 0.99 for Rejected Loans**, meaning it successfully catches nearly 100% of high-risk applicants.

  * **Operational Scalability:** Automating "clear-cut" approvals allows human underwriters to focus exclusively on complex edge cases.

## 📂 Project Structure

```text
loan-approval-prediction/
│
├── data/                    # Dataset (CSV)
├── notebooks/               # Jupyter Notebooks with EDA & Modeling
├── images/                  # Visualizations (Confusion Matrices, Feature Importance)
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

## ⚙️ Installation & Usage

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/Muradamen/loan-approval-prediction.git
    cd loan-approval-prediction
    ```
2.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the Analysis**
    ```bash
    jupyter notebook
    ```

## 💼 Skills Demonstrated

  * **Machine Learning:** Supervised Classification, Ensemble Methods.
  * **Data Engineering:** Preprocessing, Scaling, Label Encoding.
  * **Business Intelligence:** Risk Analysis, Feature Importance, Model Interpretation.
  * **Communication:** Technical Documentation & Insight Generation.

## 👨‍💻 Author

**Murad Amin** 🔗 [LinkedIn](https://www.linkedin.com/in/muradamin) | 🔗 [GitHub](https://github.com/Muradamen)



⭐ *If you find this project valuable for your credit risk research, please consider giving it a star\!*

#ALXProjectPortfolio 🚀

If you want next step, I can help you:
👉 Turn this into a **deployed ML app (VERY powerful for recruiters)**
