# 🫀 Heart Disease Prediction Using Machine Learning
*A Comprehensive ML Analysis on Clinical Features*

## 📌 Overview
This project builds a machine learning–based system to predict **heart disease** using 1918 patient records and 11 clinical features.  
The aim is to develop a reliable, high-recall predictive model that supports early diagnosis.

This project includes:
• Data Preprocessing  
• EDA  
• Outlier Treatment  
• Feature Engineering  
• Model Training  
• Hyperparameter Tuning  
• Model Comparison  
• Final Model Selection  

## 📊 Dataset Information
- Samples: **1918**
- Features: **11**
- Target: `HeartDisease` (1 = Disease, 0 = Normal)
  

### Features:
Age, Sex, ChestPainType, RestingBP, Cholesterol, FastingBS, RestingECG, MaxHR, ExerciseAngina, Oldpeak, ST_Slope  

## 🧹 Data Preprocessing
• Missing values handled (ST_Slope → mode)  
• outlier detection 
• IQR-based statistical outlier replacement  
• Ensured data consistency and quality  

## 📈 Exploratory Data Analysis
Performed using histograms, boxplots, heatmaps, pairplots, and categorical-vs-target plots.  
Key findings:
• Chest pain type strongly correlates with disease  
• ST_Slope & ExerciseAngina are major indicators  
• MaxHR & Age show meaningful patterns  

## ⚙️ Feature Engineering
• Label Encoding (binary features)  
• One-Hot Encoding (multi-class features)  
• Scaling numerical features using StandardScaler  
• PCA tested but not used (no improvement)  

## 🤖 Machine Learning Models
• Logistic Regression  
• KNN  
• Naive Bayes  
• SVM  
• Decision Tree  
• Random Forest  

### Evaluation Metrics:
Recall (priority), F1-Score, AUC-ROC, Accuracy  

## 🔍 Hyperparameter Tuning
Applied GridSearchCV on:
• KNN  
• SVM  
• Random Forest  

Improved recall, AUC, and overall model stability.

## 🏆 Best Model: Random Forest
- Accuracy: **~92%**  
- Recall: **~94%**  
- F1-Score: **~93%**  
- AUC-ROC: **~0.96**

Random Forest provided the best balance across all metrics and demonstrated strong generalization, making it ideal for medical prediction.

## 📁 Project Structure
📦 Heart-Disease-Prediction  
 ├── data/  
 ├── notebooks/       
 ├── README.md  
 └── requirements.txt 

 🔮 Future Scope

• Deploy using Streamlit / Flask
• Add SHAP explainability
• Use deep learning for further improvement
• Add more clinical features
• Validate on external hospital datasets

🙌 Contributions

• Built full ML pipeline
• Extensive preprocessing + outlier handling
• EDA + feature engineering
• Model comparison across 6 algorithms
• Hyperparameter tuning
• Final Random Forest model selection

📚 References

• scikit-learn.org
• datacamp.com
• geeksforgeeks.org
• openml.org
• kaggle.com 

## 🚀 How to Run
```bash
git clone https://github.com/your-username/heart-disease-prediction.git
cd heart-disease-prediction
pip install -r requirements.txt
jupyter notebook
