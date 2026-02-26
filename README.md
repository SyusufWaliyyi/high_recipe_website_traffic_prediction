# high_recipe_website_traffic
developing the machine learning model to predict which recipes will lead to **high website traffic**

# 🍽️ Recipe Traffic Prediction Project

## 👤 Author
**Shamsuddeen Yusuf**  
Data Analyst | Machine Learning Enthusiast | Production Engineer  

---

## 📌 Project Overview
This project applies **data science and machine learning** to predict which recipes are likely to generate **high user traffic (≥80%)**, helping businesses minimize the risk of featuring low-performing content.

The solution combines **data cleaning**, **exploratory data analysis**, and **predictive modeling** to deliver **actionable insights** for editorial and operational decision-making.

---

## 🎯 Objectives
- Predict high-traffic recipes with high reliability
- Reduce the probability of featuring low-engagement recipes
- Support data-driven content placement decisions

---

## 🧠 Key Skills Demonstrated
- Data Cleaning & Validation
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Binary Classification Modeling
- Model Evaluation & Comparison
- Business Impact Translation

---

## 🗂️ Project Structure

---

## 🧹 Data Validation & Cleaning

- **Dataset size:** 947 recipes
- **Missing values:**  
  - 52 missing entries in calories, protein, sugar, and carbohydrates  
  - Imputed using **median values**
- **Category refinement:**  
  - `"Chicken Breast"` consolidated into `"Chicken"`
- **Servings:**  
  - Text noise removed (e.g., *"as a snack"*)
  - Converted to numeric format
- **Target variable:**  
  - `high_traffic` converted to binary:
    - `1` → High Traffic
    - `0` → Low or Missing Traffic

---

## 📊 Key Insights from Exploratory Data Analysis

### 🔑 Category Dominance
- Recipe category is the **strongest predictor** of traffic.
- Highest-performing categories:
  - **Vegetable**
  - **Potato**

### 🥗 Nutrition vs Preference
- High calorie content does **not** guarantee popularity.
- Users favor **meal type and category** over nutrient density.

### ☕ Underperforming Segment
- **Beverages** consistently generate low traffic regardless of nutrition.

---

## 🤖 Model Training

### Problem Type
- **Binary Classification**

### Features Used
- Category
- Servings
- Calories
- Carbohydrates
- Sugar
- Protein

### Models Implemented
| Model | Purpose |
|-----|--------|
| Logistic Regression | Baseline, interpretable, fast |
| Random Forest Classifier | Captures non-linear relationships |

---

## 🧪 Model Evaluation

### Evaluation Metrics
- **Accuracy**
- **Precision** (critical to avoid false positives)

### Key Findings
- Random Forest handled categorical variation more robustly.
- Confusion matrices were used to visualize prediction errors.
- Both models achieved **reliable performance**, with Random Forest slightly outperforming in robustness.

---

## 📦 Installation & Usage

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/SyusufWaliyyi/high_recipe_website_traffic.git
cd high_recipe_website_traffic
