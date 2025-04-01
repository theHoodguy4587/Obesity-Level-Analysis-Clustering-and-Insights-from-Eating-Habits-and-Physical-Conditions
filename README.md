# Obesity Level Analysis: Clustering and Insights from Eating Habits and Physical Conditions

## 📌 Overview
This project analyzes **obesity levels** in individuals from **Mexico, Peru, and Colombia**, focusing on their **eating habits** and **physical conditions**. The dataset consists of **2111 records** with **17 attributes**, and the target variable `NObesity` categorizes obesity levels into:
- **Insufficient Weight**
- **Normal Weight**
- **Overweight Level I**
- **Overweight Level II**
- **Obesity Type I**
- **Obesity Type II**
- **Obesity Type III**

**Methods used:**
- Exploratory Data Analysis (**EDA**)
- Data Preprocessing (Feature Encoding, Scaling, Handling Categorical Data)
- **KMeans Clustering** for pattern identification

## 📂 Dataset Information
- **Instances:** 2111
- **Features:** 16 (excluding target variable `NObesity`)
- **Data Source:**
  - **77% synthetic data** (generated using Weka & SMOTE)
  - **23% real data** (collected from users via a web platform)

## 🔍 Exploratory Data Analysis (EDA)
Performed **EDA** to uncover patterns, correlations, and data distributions:
- **Visualization:**
  - Histograms & box plots for numerical features
  - Count plots for categorical variables
- **Correlation Analysis:**
  - Pearson correlation matrix for numeric features
  - Heatmaps to identify relationships

## 🛠 Data Preprocessing
### **Steps Taken:**
1. **Handling Categorical Variables:**
   - Encoded categorical columns (e.g., Gender, CALC) into numeric form
2. **Feature Scaling:**
   - Standardized numerical data using `StandardScaler`
3. **Checking Data Imbalance:**
   - Verified the distribution of `NObesity` categories
4. **Feature Selection:**
   - Dropped redundant or low-variance features

## 🤖 KMeans Clustering
### **Goal:** Identify natural groupings in the data without using labels.

### **Steps:**
1. **Finding Optimal `k` (Elbow Method):**
   - Tested `k` values from 1 to 10 using WCSS (Within-Cluster Sum of Squares)
   - Identified the **elbow point** for optimal clustering
2. **Clustering Implementation:**
   - Applied `KMeans` with the chosen `k`
   - Analyzed cluster characteristics
3. **Visualization:**
   - **PCA (Principal Component Analysis)** for 2D cluster representation
   - **Scatter plots** to understand group separation

## 📊 Key Insights
- Found distinct patterns in eating habits and physical activity influencing obesity levels.
- Clusters showed correlations between BMI, daily caloric intake, and physical activity.
- Suggested possible **dietary & lifestyle recommendations** based on cluster behaviors.

## 🚀 Next Steps
- Try **Hierarchical Clustering** for better cluster interpretation.
- Apply **Supervised Learning (Classification Models)** to predict obesity levels.
- Improve feature engineering for better separability.

## 📜 References
- Dataset from **'Data in Brief' (2019)** by Fabio Mendoza Palechor & Alexis De la Hoz Manotas.
- Weka & SMOTE for synthetic data generation.

---
📧 **For inquiries & collaborations:** Feel free to connect!
