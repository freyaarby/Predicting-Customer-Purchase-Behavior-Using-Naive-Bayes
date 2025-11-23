# 📊 Predicting Costumer Purchase Behavior Using Naive Bayes

A complete classification project to predict whether a customer will purchase a product after seeing an advertisement.  
This project covers data preprocessing, EDA, feature scaling, modeling using **Gaussian Naive Bayes**, and performance comparison between balanced and imbalanced training data.

---

## ✨ Project Overview  
This project aims to classify **consumer purchase behavior** using demographic and financial variables.  
By understanding purchasing patterns, companies can improve **ad targeting**, reduce marketing costs, and increase conversion rates.

Source code:  
`prediksi_daya_beli_konsumen_berdasarkan_iklan_melalui_klasifikasi_naive_bayes.py`



## 📁 Dataset Description  
Dataset: **Social Network Ads**  
Shape: **400 rows × 5 columns**

### Columns:
- **User ID** — Unique identifier  
- **Gender** — Male/Female  
- **Age** — Age of the user  
- **EstimatedSalary** — Approximate annual income  
- **Purchased** — Target label (0 = No, 1 = Yes)

This dataset is widely used in ML classification tasks.



## 🧹 Data Preprocessing  
Steps performed:

1. Dropped irrelevant column: `User ID`  
2. Checked & removed duplicates  
3. Encoded categorical column (`Gender`)  
4. Applied **StandardScaler** on numerical features  
5. Split data into training/test with:
   - **Balanced scenario (40/40/20)**  
   - **Imbalanced scenario (70/10/20)**  

These steps ensure clean, fair model training.



## 🔍 Exploratory Data Analysis (EDA)  

Performed EDA includes:  
- Scatter plot: Age vs. Salary grouped by Purchased  
- Boxplots for feature distribution  
- Checking class imbalance  
- Observing purchasing patterns  

### 🔑 Insight:
Customers who purchased tend to be:
- older (**>40 years old**)  
- with higher estimated salary  

This aligns with common marketing behavior.



## 🤖 Modeling — Gaussian Naive Bayes  

Naive Bayes is selected because:  
- efficient for small/medium datasets  
- works well with numerical features  
- fast & interpretable classifier  

Two models were trained:
### 📘 **Model 1 — Balanced Split (40/40/20)**  
### 📙 **Model 2 — Imbalanced Split (70/10/20)**  


