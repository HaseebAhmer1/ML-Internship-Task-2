# ML-Internship-Task-2
# 📝 Data Preprocessing Report

## 🎯 Objective
The goal was to build a **systematic preprocessing workflow** for the Airbnb NYC dataset.  
This involved handling missing values, detecting and treating outliers, encoding categorical variables, scaling numerical features, validating data integrity, and exploring feature relationships.  
Each step was supported by **visualizations** to better understand the dataset’s structure and quality.

---

## 📈 Tasks & Outcomes

- **Missing Values Visualization**  
  *Outcome:* Heatmap revealed where data was incomplete. Guided imputation strategies (median for numeric, mode for categorical).  
  *Learning:* Missingness patterns can indicate whether data is MCAR, MAR, or MNAR.

- **Outlier Detection**  
  *Outcome:* Boxplots and histograms highlighted extreme values in `price` and `minimum_nights`.  
  *Learning:* Outliers distort scaling and model performance; domain rules (e.g., nights > 365) help filter unrealistic entries.

- **Categorical Encoding Visualization**  
  *Outcome:* Countplots showed distribution of `room_type` and `neighbourhood_group`.  
  *Learning:* Balanced categories are suitable for One-Hot Encoding, while imbalanced ones may need alternative strategies.

- **Scaling Visualization**  
  *Outcome:* Histograms before and after scaling confirmed normalization of `price`.  
  *Learning:* Scaling ensures features with large ranges don’t dominate models, especially in distance-based algorithms.

- **Data Validation Visualization**  
  *Outcome:* Histograms of `availability_365` confirmed values were within logical bounds (0–365).  
  *Learning:* Validation checks prevent logical inconsistencies and improve dataset reliability.

- **Correlation Heatmap**  
  *Outcome:* Heatmap revealed relationships among numerical features.  
  *Learning:* Strong correlations can cause multicollinearity, requiring feature selection or dimensionality reduction.

---

## 📚 Key Learnings
- Visualizations are **diagnostic tools** that make preprocessing decisions more transparent.  
- Handling missing values requires understanding the mechanism (MCAR/MAR/MNAR).  
- Outlier detection is both statistical (Z-score, IQR) and domain-driven.  
- Encoding and scaling are essential for preparing features for machine learning.  
- Validation ensures logical consistency and prevents flawed inputs.  
- Correlation analysis helps identify redundant features and guides feature engineering.
