# Job Prediction Data Science Project

## 📌 Project Overview
This project is based on the **`aug_train.csv` dataset**, which contains job seeker profiles and related features.  
The main goal of this project is to **predict whether a candidate will be looking for a new job or not** using **Machine Learning models**.

We performed **Data Cleaning, Exploratory Data Analysis (EDA), Feature Engineering, and Model Building** to solve this classification problem.

---

## 📂 Dataset Information
- **Dataset Name:** aug_train.csv  
- **Rows:** ~19,000  
- **Columns:** 14  
- **Target Variable:** `target` (1 = looking for a job change, 0 = not looking)  

### 🔑 Key Features:
- `gender`, `city`, `relevent_experience`, `enrolled_university`, `education_level`, `major_discipline`  
- `experience`, `company_size`, `company_type`, `last_new_job`  
- `training_hours`  

---

## 🧹 Data Preprocessing
1. **Handling Missing Values**  
   - Filled categorical missing values with `mode`.  
   - Filled numerical missing values with `median`.  

2. **Encoding Categorical Variables**  
   - Used **Label Encoding** and **OneHot Encoding** for categorical columns.  

3. **Feature Scaling**  
   - Standardized numerical features (e.g., `training_hours`) using `StandardScaler`.  

4. **Train-Test Split**  
   - 80% Training  
   - 20% Testing  

---

## 📊 Exploratory Data Analysis (EDA)
- Distribution of job seekers across education levels and company size.  
- Correlation analysis of numerical features.  
- Visualization of target balance (job change vs no change).  

---

## 🤖 Machine Learning Models
We applied multiple ML models and compared their performance:

1. **Logistic Regression**  
2. **Random Forest Classifier**  
3. **Support Vector Machine (SVM)**  

---

## 📈 Model Evaluation
We compared the models based on **Accuracy, Precision, Recall, F1-Score**.

| Model                | Accuracy | Precision | Recall | F1-Score |
|-----------------------|----------|-----------|--------|----------|
| Logistic Regression   | 0.78     | 0.76      | 0.74   | 0.75     |
| Random Forest         | 0.84     | 0.83      | 0.81   | 0.82     |
| SVM                   | 0.80     | 0.78      | 0.76   | 0.77     |

✅ **Best Model:** Random Forest (highest overall performance).  

---

## 📉 ROC-AUC Curve
We also plotted the ROC-AUC curve to evaluate model performance.  
Random Forest achieved the best AUC score compared to Logistic Regression and SVM.

---

## 🚀 Conclusion
- Data preprocessing (handling missing values, encoding, scaling) was crucial.  
- Random Forest outperformed other models in predicting job change tendency.  
- Logistic Regression and SVM also performed decently but had lower recall.  

---

## 🛠️ Tech Stack
- **Python**  
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn  

---

## 📌 How to Run
1. Clone this repo  
   ```bash
   git clone https://github.com/your-username/job-prediction-dataset.git
   cd job-prediction-dataset
