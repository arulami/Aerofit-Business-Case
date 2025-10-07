# 🏋️‍♂️ Aerofit Treadmill Customer Profiling – Descriptive Analytics Case Study

## 📘 Project Overview
This project analyzes **Aerofit’s treadmill customer data** to uncover buying patterns, customer segments, and probability-based insights that guide marketing and product positioning.  
The study focuses on three treadmill models — **KP281**, **KP481**, and **KP781** — each targeting different fitness and income groups.

---

## 🎯 Objectives
- Perform **Exploratory Data Analysis (EDA)** and detect outliers  
- Identify how demographics (Age, Gender, Marital Status, Income, Fitness) influence treadmill choice  
- Compute **marginal and conditional probabilities** such as  
  \( P(\text{KP781} \mid \text{Male}) \) to understand customer preferences  
- Create **customer profiles** and derive actionable business recommendations  

---

## 🧩 Dataset Summary
| Feature | Description |
|----------|-------------|
| Product | Treadmill model – KP281, KP481, KP781 |
| Age | Customer age (years) |
| Gender | Male / Female |
| Education | Years of education |
| MaritalStatus | Single / Partnered |
| Usage | Avg. treadmill uses per week |
| Fitness | Self-rated fitness (1–5) |
| Income | Annual income (USD) |
| Miles | Expected miles per week |

---

## 📊 Analysis Workflow
1. **Data Import & Inspection** – structure, datatypes, nulls  
2. **Outlier Detection** – `.describe()` and boxplots (mean vs median)  
3. **Univariate & Bivariate Analysis** – distributions, countplots, boxplots  
4. **Correlation Analysis** – numerical features heatmap  
5. **Probability Computation** – marginal & conditional probabilities  
6. **Customer Profiling & Insights** – mean demographics by product  

---

## 📈 Key Findings
| Product | Key Characteristics |
|----------|---------------------|
| **KP281** | Older, lower-income, beginner users |
| **KP481** | Balanced, mid-income, regular users |
| **KP781** | Younger, higher-income, advanced fitness users |

**Conditional Probabilities**

- \( P(\text{KP781} \mid \text{Male}) = 0.317 \) → **31.7 %**  
- \( P(\text{KP781} \mid \text{Female}) = 0.092 \) → **9.2 %**

---

## 💡 Business Insights
- **KP281** → Target beginners with affordable EMI-based offers  
- **KP481** → Market as an all-rounder treadmill for professionals  
- **KP781** → Focus on premium branding for male customers;  
  reposition for female customers emphasizing health, safety, and ease of use  

---

## ⚙️ Run the Notebook in Google Colab
Click the badge below to open and run the notebook directly in Google Colab:  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/arulamli/Aerofit-Business-Case/blob/main/Aerofit_Business_Case.ipynb)

### Steps
1. Click the badge above to open in Colab  
2. Upload the dataset when prompted:
   ```python
   from google.colab import files
   uploaded = files.upload()  # choose aerofit_treadmill.csv
