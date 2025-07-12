#  MSCS 634 - Project Deliverable 3: Classification, Clustering, and Pattern Mining

👨‍🎓 **Student Name:** Chandra Kiran Billingi  
📚 **Course:** MSCS 634 - Advanced Big Data and Data Mining  
📅 **Deliverable:** Project Phase 3 – Modeling and Pattern Discovery  

---

## 🧠 Objective

In this phase, the focus was on applying **machine learning and pattern mining** techniques to extract actionable insights from the CarDekho dataset. This included:

- Building **classification models** for prediction
- Performing **clustering** for customer or vehicle segmentation
- Applying **association rule mining** to find frequent patterns
- Tuning hyperparameters and evaluating model performance

---

## 🧪 Models and Techniques Applied

### ✅ Classification

- **Models Used**: Decision Tree, k-NN, Naïve Bayes, SVM
- **Hyperparameter Tuning**: Applied GridSearchCV on K-NN
- **Evaluation Metrics**: Accuracy, F1 Score, Confusion Matrix, ROC Curve

**Insight**:  
K-NN with hyperparameter tuning performed best, achieving the highest F1 score and balanced accuracy.

---

### 🔄 Clustering

- **Model Used**: K-Means (Elbow Method to determine optimal `k`)
- **Features Clustered**: Engine, Mileage, Max Power
- **Visualization**: 2D Scatter Plots by Cluster

**Insight**:  
Formed distinct groups of cars based on power and efficiency, useful for price tiering or targeted promotions.

---

### 🔍 Association Rule Mining

- **Algorithm**: Apriori and FP-Growth
- **Metrics**: Support, Confidence, Lift
- **Tools**: `mlxtend` library

**Key Rules Discovered**:
- Diesel cars often have manual transmission and higher power.
- Cars with 4 seats frequently correlate with higher mileage variants.

---

## 💼 Real-World Applications

| Use Case | Application |
|----------|-------------|
| Price Prediction | Classification models help suggest competitive resale prices |
| Customer Segmentation | Clustering identifies buyer groups for personalized offers |
| Recommendations | Rules help suggest car variants based on user preferences |
| Inventory Optimization | Insights guide stock management and demand prediction |

---

## ⚠️ Challenges Faced

| Challenge | Resolution |
|----------|-------------|
| Class imbalance | Focused on metrics like F1-score and ROC AUC |
| Feature scaling for SVM & KNN | Applied `StandardScaler` for improved model performance |
| Choosing number of clusters | Used the **Elbow Method** and inertia plots |
| Sparse rule sets at higher thresholds | Adjusted support/confidence to balance relevance vs. quantity |


