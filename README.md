# 🚗 MSCS 634 - Project Deliverable 1: Exploratory Data Analysis on CarDekho Dataset

👨‍🎓 **Student Name:** Chandra Kiran Billingi  
📚 **Course:** MSCS 634 - Advanced Big Data and Data Mining  
📅 **Deliverable:** Project Phase 1 – Dataset Preparation and EDA  

---

## 📊 Dataset Summary

The dataset used in this project is sourced from **CarDekho**, a leading car marketplace. It contains detailed information on used cars such as name, year, selling price, kilometers driven, fuel type, transmission, engine, mileage, and power.

- **Rows:** 8,000+  
- **Columns:** 13  
- **Target variable:** `price` (selling price of used cars)

---

## 🧼 Data Cleaning Steps

The following cleaning steps were performed:

1. **Handling Missing Values:**
   - `mileage`, `engine`, `max_power`: Cleaned strings (e.g., `"19.7 kmpl"`) and converted to numeric.
   - Filled missing numeric values with column means.

2. **Removing Duplicates:**
   - Removed duplicate records using `df.drop_duplicates()`.

---

## 📈 Exploratory Data Analysis (EDA)

Visualizations and statistical summaries helped identify patterns and distributions:
- **Histogram & KDE plots** for mileage, engine, power, and price.
- **Boxplots** to detect outliers in price and power.
- **Correlation heatmap** to explore relationships among features.
- **Pairplots** for multivariate relationships.

---

---

## ⚠️ Challenges Faced

| Challenge | Resolution |
|----------|-------------|
| Missing values in important columns | Imputed using mean values |
| Deprecation warning with `distplot` | Replaced with `sns.histplot()` for Seaborn compatibility |
| Chained assignment warning in pandas | Replaced with explicit assignments (`df[col] = ...`) |

