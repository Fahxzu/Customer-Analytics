# Customer Analytics

## 🎯 Problem Statement
Improve customer **campaign response** using data analysis.  
Target: Analyze customer behavior based on the `Campaign Response` label.

- **Campaign Response values:**
  - `0`: Reject Offer  
  - `1`: Accept Offer (PA Insurance Product)  
  - `2`: Accept Offer (Life Insurance Product)

---

## ✅ Objective
Understand customer **personality traits** and behaviors that correlate with each type of campaign response to tailor marketing strategies.

---

## 🧠 Solution Plan

### 1. Analysis
#### 1.1 Personality Analysis by Campaign Response
- **Goal**: Identify key differences in customer personality for each response type (Reject, Accpet_PA, Accpet_Life).
- **Steps**:
  - Segment customers by `Campaign Response`.
  - Analyze key attributes:  
    - Demographics (Age, Gender, Occupation, etc.)  
    - Campaign behavior
  - Use statistical summaries and visualizations to compare distributions.

### 2. Model Building
#### 2.1 Model Building to retension customer
- **Goal**: Select customer Reject and probability > 10 to personality for tele sell.
- **Steps**:
  - Build a classification model to **predict campaign response** using customer features.
  - Algorithms: Logistic Regression, Random Forest, XGBoost. 
  - Evaluate using metrics like accuracy, precision, recall, and F1-score.
  - Select max F1-score and select model to predict prob.
  - Select prob > 10 to analysis personality and group segment to tele sell.

#### 2.2 Customer Segmentation using Clustering
- **Goal**: Search new customer segments.
- **Steps**:
  - Feature selection , encoding categorical variables and convert target label.
  - Standardize and Find optimal number of Clusters (Elbow Method).
  - Apply KMeans clustering and Visualize. 

---

### Ref : feature important
- **Goal** : selelct feature for building model.
- **Result** : F1-score of before and after select feature are not different, so I attached it for reference.

---

