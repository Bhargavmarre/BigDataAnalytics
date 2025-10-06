# Breast Cancer Data Analysis Using PySpark

**Author:** Bhargav Marre  
**Roll No:** 2211CS010363  
**Academic Year:** 2025 – 2026  

---

## 📖 Project Overview
This project performs **Exploratory Data Analysis (EDA)** on a **Breast Cancer dataset** using **PySpark 4.0.1**.  
It mirrors the workflow of large-scale government data analytics, applying the same data engineering and analysis pipeline to a medical dataset for early tumor diagnosis insights.

The primary goal is to identify **patterns and correlations among tumor features** and understand how they distinguish between **malignant and benign** cases.

---

## 🧠 Objectives
- Apply **PySpark DataFrame API** for scalable data handling  
- Clean, preprocess, and normalize large medical datasets  
- Perform **statistical and correlation analysis**  
- Visualize feature relationships and separability between classes  
- Derive meaningful **diagnostic insights** for further ML-based research  

---

## 📊 Dataset Description
- **Source:** Breast Cancer Diagnostic Dataset (UCI / Kaggle)  
- **Records:** ~500 samples  
- **Target Variable:** Diagnosis (M = Malignant, B = Benign)  
- **Key Features:**  
  - Mean Radius  
  - Texture  
  - Perimeter  
  - Area  
  - Smoothness  
  - Compactness  
  - Concavity  
  - Symmetry  
- **Data Cleaning:**  
  - Removed duplicates  
  - Handled missing values  
  - Renamed columns for PySpark compatibility  

---

## ⚙️ Technologies Used
| Component | Version / Tool |
|------------|----------------|
| Language | Python 3.x |
| Framework | PySpark 4.0.1 |
| JDK | 25 |
| Libraries | Pandas, Seaborn, Matplotlib |
| Environment | Jupyter Notebook |

---

## 🧩 Operations Performed
1. **Data Loading** using PySpark `read.csv()`  
2. **Column Normalization** (rename and clean headers)  
3. **Null & Duplicate Handling**  
4. **Automatic Numeric Type Detection & Casting**  
5. **Summary Statistics & Medians Calculation**  
6. **Correlation Matrix Generation**  
7. **Visualization** using Matplotlib & Seaborn  
   - Feature Distributions  
   - Boxplots (Diagnosis-wise)  
   - Correlation Heatmap  

---

## 💡 Key Insights
- Malignant tumors show significantly higher **radius, area, and perimeter** values.  
- Strong positive correlation exists between **radius**, **area**, and **perimeter**.  
- **Compactness** and **concavity** are critical indicators of malignancy.  
- Visual EDA confirms clear separability between tumor classes.  

---

## 📈 Sample Visualizations
- **Feature Distribution Histograms**  
- **Boxplots by Diagnosis (M vs B)**  
- **Correlation Heatmap**

> These visualizations help identify relationships and separability between classes for further ML modeling.

---

## 🧭 Recommendations
- Use **PCA** or **feature selection** to reduce redundancy.  
- Train a **classification model** using PySpark MLlib.  
- Develop **real-time dashboards** for clinical decision support.  
- Incorporate **privacy-preserving analytics** for healthcare compliance.  

---

## 🚀 How to Run
1. Install required tools:
   ```bash
   pip install pyspark pandas matplotlib seaborn
