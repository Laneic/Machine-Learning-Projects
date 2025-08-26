# Classification Models Summary

## 🔑 Key Learnings

### Types of Learning
- **Supervised Learning** → Uses labeled data (classification, regression).  
- **Unsupervised Learning** → Uses unlabeled data (clustering, dimensionality reduction).  
- **Classification** is supervised.  
- **Clustering** (like K-Means) is unsupervised → usually no train/test split.

### General Concepts
- `fit()` → trains the model.  
- `predict()` → makes predictions for new/unseen data.  
- Accuracy can be improved with hyperparameter tuning, ensembles, and feature engineering.  

### Data Preprocessing
- Scaling is crucial for distance-based models (**KNN, SVM, Logistic Regression**).  
- Not needed for tree-based models (**Decision Tree, Random Forest, Naive Bayes**).  

### Models Overview
- **KNN** → distance-based, needs scaling, sensitive to noise/outliers.  
- **SVM** → finds separating hyperplane, works best with scaling, kernel trick for non-linear data.  
- **Logistic Regression** → probabilistic, simple yet powerful, works well with scaling.  
- **Naive Bayes** → assumes independence, fast, no scaling required, robust to irrelevant features.  
- **Decision Tree** → uses information gain/entropy, interpretable, no scaling required.  
- **Random Forest** → ensemble of trees, reduces overfitting, very strong baseline.  

---

## 📊 Results on Dataset

### Logistic Regression
- **Accuracy**: 0.966  
- **Class 0** → Precision: 0.99, Recall: 0.97, F1: 0.98  
- **Class 1** → Precision: 0.92, Recall: 0.97, F1: 0.94  

### SVM (RBF Kernel)
- **Accuracy**: 0.930  
- **Class 0** → Precision: 0.91, Recall: 0.99, F1: 0.95  
- **Class 1** → Precision: 0.98, Recall: 0.77, F1: 0.87  

### Decision Tree
- **Accuracy**: 0.919  
- **Class 0** → Precision: 0.94, Recall: 0.95, F1: 0.94  
- **Class 1** → Precision: 0.88, Recall: 0.84, F1: 0.86  

### Random Forest
- **Accuracy**: 0.975  
- **Class 0** → Precision: 0.98, Recall: 0.98, F1: 0.98  
- **Class 1** → Precision: 0.96, Recall: 0.95, F1: 0.96  

### Naive Bayes
- **Accuracy**: 0.948  
- **Class 0** → Precision: 0.98, Recall: 0.95, F1: 0.96  
- **Class 1** → Precision: 0.88, Recall: 0.95, F1: 0.92  

---

## 📋 Comparison Table

| Model              | Accuracy | Precision (0/1) | Recall (0/1) | F1-Score (0/1) |
|--------------------|----------|-----------------|--------------|----------------|
| Logistic Regression| 0.966    | 0.99 / 0.92     | 0.97 / 0.97  | 0.98 / 0.94    |
| SVM (RBF)          | 0.930    | 0.91 / 0.98     | 0.99 / 0.77  | 0.95 / 0.87    |
| Decision Tree      | 0.919    | 0.94 / 0.88     | 0.95 / 0.84  | 0.94 / 0.86    |
| Random Forest      | 0.975    | 0.98 / 0.96     | 0.98 / 0.95  | 0.98 / 0.96    |
| Naive Bayes        | 0.948    | 0.98 / 0.88     | 0.95 / 0.95  | 0.96 / 0.92    |

---

✅ **Best performer so far:** Random Forest (Accuracy ~97.5%)
