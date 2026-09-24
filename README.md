# E-Commerce Customer Segmentation & Churn Risk Analysis

![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3%2B-orange.svg)
![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-green.svg)
![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)

## 📌 Project Overview

This project delivers an end-to-end data analytics and predictive machine learning solution for e-commerce customer segmentation and churn risk identification. Analyzing **50,000 unique customer profiles**, this project examines customer spending habits across various segments, channel attributions, product categories, and satisfaction scores. 

Furthermore, a **Random Forest Classifier** was developed using a Scikit-Learn machine learning pipeline to proactively predict customer churn risk, achieving an impressive **96.73% overall accuracy**.

* **Author:** Juttu Abhiram
* **Submission Date:** September 2026
* **Primary Notebook:** [`JuttuAbhiram_Ecommerce_Customer_Segmentation.ipynb`](JuttuAbhiram_Ecommerce_Customer_Segmentation.ipynb)
* **Project Documentation Report:** [`JuttuAbhiram_ProjectReport.docx`](JuttuAbhiram_ProjectReport.docx)

---

## 📊 Dataset Information & Source

* **Dataset Name:** E-Commerce Customer Segmentation Dataset (2026)
* **Total Sample Count:** 50,000 Customer Records
* **Attributes Count:** 53 Total Attributes (29 Core Selected Features)
* **Dataset File:** `E-commerce_Customer_Segmentation_2026.csv`
* **Dataset Link:** [https://www.kaggle.com/datasets/datascikhan/e-commerce-customer-segmentation-2026](E-commerce_Customer_Segmentation_2026.csv) 

### Core Selected Features:
* **Customer Demographic & Profile:** `customer_id`, `customer_segment`, `age`, `gender`, `country`, `income_bracket`, `tenure_months`
* **Transactional & Monetary:** `total_purchases`, `avg_order_value_usd`, `total_spent_usd`, `purchase_frequency`, `days_since_last_purchase`
* **Engagement & Channels:** `preferred_category_1`, `shopping_channel`, `device_used`, `payment_method`, `email_open_rate`, `click_through_rate`, `conversion_rate`
* **Service & Satisfaction:** `return_count`, `complaint_count`, `satisfaction_score`, `loyalty_tier`
* **Value & Risk Analytics:** `customer_lifetime_value_usd`, `customer_acquisition_cost_usd`, `customer_profitability_usd`, `rfm_score`, `churn_risk_score`, `customer_health_score`

---

## 🛠️ Technology Stack & Libraries

* **Core Language:** Python 3.9+
* **Data Processing & Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning & Pipeline:** `scikit-learn`
* **Report & Document Generation:** `python-docx`
* **Environment:** Jupyter Notebook / JupyterLab

---

## 📁 Repository Structure

```text
├── JuttuAbhiram_Ecommerce_Customer_Segmentation.ipynb   # Complete Jupyter Notebook code
├── JuttuAbhiram_ProjectName.ipynb                      # Code File submission alias
├── JuttuAbhiram_ProjectReport.docx                     # Complete Project Documentation (.docx)
├── JuttuAbhiram_Ecommerce_Customer_Segmentation_ProjectReport.docx # Named report copy
├── requirements.txt                                    # Python dependencies & libraries list
├── README.md                                           # Project overview & documentation
├── E-commerce_Customer_Segmentation_2026.csv           # E-commerce customer dataset
└── images/                                             # Exported high-resolution visualization charts
    ├── customer_segments_distribution.png
    ├── avg_revenue_by_segment.png
    ├── revenue_by_shopping_channel.png
    ├── revenue_by_product_category.png
    ├── satisfaction_vs_spending.png
    ├── confusion_matrix_heatmap.png
    └── feature_importance.png
```

---

## ⚙️ Setup & Installation Instructions

1. **Clone or Download the Repository:**
   ```bash
   git clone https://github.com/JuttuAbhiram/e_commerce_customer_segment_analysis.git
   cd e_commerce_customer_segment_analysis
   ```

2. **Create and Activate a Virtual Environment (Recommended):**
   ```bash
   # On Windows
   python -m venv venv
   venv\Scripts\activate

   # On macOS/Linux
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 Execution Instructions

1. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Open & Run the Notebook:**
   * Open [`JuttuAbhiram_Ecommerce_Customer_Segmentation.ipynb`](JuttuAbhiram_Ecommerce_Customer_Segmentation.ipynb).
   * Execute cells sequentially (`Kernel` -> `Restart & Run All`) to run data loading, cleaning, EDA, visualization generation, and machine learning model training.

---

## 📈 Key Insights & Analytical Summary

### 1. Customer Segmentation Distribution & Revenue
* **Customer Segment Volume:** Consumer (22,507 | 45.0%), Premium (12,423 | 24.9%), Small Business (9,979 | 20.0%), and Enterprise (5,091 | 10.2%).
* **Average Spend:** Remarkably consistent across segments at ~$50,000 per customer, indicating high monetary value across all customer tiers.

### 2. Multi-Channel Revenue Attribution
* **Mobile App:** $633.20 Million
* **Online Web:** $633.06 Million
* **In-Store:** $628.59 Million
* **Marketplace:** $618.48 Million

### 3. Product Category Spending
* Top spending categories include **Electronics** ($214.2M) and **Fashion** ($213.4M), followed closely by **Automotive** ($212.0M) and **Grocery** ($211.3M).

---

## 🤖 Machine Learning Model Performance

* **Model Architecture:** Random Forest Classifier (200 Trees, Class Weighting `balanced`, Median Imputation, Standard Scaler).
* **Train-Test Split:** 80% Train (40,000) / 20% Test (10,000) Stratified Split.
* **Overall Accuracy:** **96.73%**

### Evaluation Metrics Breakdown:
| Class | Precision | Recall | F1-Score | Support |
| :--- | :---: | :---: | :---: | :---: |
| **High Risk (Target)** | **0.76** | **0.58** | **0.66** | 540 |
| **Low Risk** | **0.98** | **0.99** | **0.98** | 9,460 |
| **Accuracy** | | | **0.97** | 10,000 |
| **Macro Average** | 0.87 | 0.79 | 0.82 | 10,000 |
| **Weighted Average** | 0.96 | 0.97 | 0.97 | 10,000 |

* **Total Predicted High Risk Customers:** **2,577 customers** identified out of 50,000, enabling targeted proactive retention campaigns.

---

## 💡 Strategic Recommendations

1. **Proactive Retention Campaigns:** Reach out to the 2,577 predicted high-risk customers with exclusive loyalty rewards and re-engagement incentives.
2. **Mobile & Web UX Enhancements:** Mobile App and Web channels account for over $1.26 Billion in revenue; continuous UX optimization is essential.
3. **Complaint Handling Protocols:** Reduce days since last purchase and resolve customer complaints rapidly, as these features heavily influence customer churn.

---

## ✒️ Author & Contact Information

* **Author:** Juttu Abhiram
* **Project Name:** E-Commerce Customer Segmentation & Churn Risk Analysis
* **Status:** Complete & Ready for Submission
