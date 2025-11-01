# Obesity Level Classification — Machine Learning Project

###  Overview
This project predicts **obesity categories** based on lifestyle + physical attributes using supervised machine learning.  
We perform preprocessing, EDA, model training, hyperparameter tuning and compare multiple ML algorithms.

###  Dataset
- **Total Samples:** 17,644  
- **Attributes:** 17 (Lifestyle, physical, behavioural)  
- **Target Classes:** Insufficient Weight, Normal Weight, Overweight I, Overweight II, Obesity I, Obesity II, Obesity III

###  Preprocessing Steps
- Manual categorical encoding  
- StandardScaler applied on continuous features  
- Combined two datasets + performed KS Test to validate distribution similarity  
- PCA for visualization of dataset overlap

###  EDA Highlights
Explored factors like:
- Height vs Weight relation
- Transportation mode vs obesity level
- Gender-based class distribution
- Alcohol / High calorie food / Vegetable consumption impact
- Physical activity correlations
- Pearson correlation heatmap

###  Models Trained
| Model | Best Test Accuracy |
|-------|--------------------|
| KNN | 82.03% |
| Random Forest | 90.33% |
| XGBoost  | **91.04%** |

XGBoost performed best (highest F1-macro & micro).

###  Techniques Used
- Feature Scaling  
- KS Test  
- PCA  
- RandomizedSearchCV (Hyperparameter tuning)  
- Classification Metrics: Accuracy, Precision, Recall, F1-score, Micro/Macro


### 🏁 Conclusion
XGBoost with regularization gives the most stable and accurate results for obesity classification compared to Random Forest and KNN.

---

**Preprocessing and EDA**
https://colab.research.google.com/drive/1xLuFnZ2HvDC2_U1rL526x6PhNgrGpxkl?usp=sharing

**Model Training**
https://colab.research.google.com/drive/1YeEyDQeXwx6WmhqYwhNWvUaoCCI_UPWa?usp=sharing
