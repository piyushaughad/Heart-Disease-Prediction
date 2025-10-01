# 🫀 Heart Disease Prediction using Machine Learning  

This project applies machine learning techniques to predict the likelihood of a heart attack based on patient health data. It explores various classification models, performs data preprocessing, visualization, and evaluation to determine the most effective model for heart disease prediction.  

---

## 📌 Project Overview  
Cardiovascular diseases are the leading cause of mortality worldwide. Early prediction can help doctors intervene and save lives.  
This project leverages **machine learning models** such as:  
- **Support Vector Machine (SVM)**  
- **Decision Tree (with pruning)**  
- **Random Forest**  
- **Logistic Regression**  

After comparing performance metrics, the **Decision Tree with post-pruning** and **Random Forest** provided the best balance of accuracy and recall.  

---

## 📊 Dataset  
- **Rows**: 303 (after cleaning: 302)  
- **Columns**: 14 (physiological and medical features)  
- **Target**:  
  - `0` → Less chance of heart attack  
  - `1` → More chance of heart attack  

### Features  
| Feature  | Description |
|----------|-------------|
| Age      | Age in years (29–77) |
| Sex      | 1 = Male, 0 = Female |
| Cp       | Chest pain type (1–4) |
| Trestbps | Resting blood pressure (mm Hg) |
| Chol     | Serum cholesterol (mg/dl) |
| Fbs      | Fasting blood sugar >120 mg/dl (1 = true; 0 = false) |
| Restecg  | Resting ECG results (0–2) |
| Thalach  | Maximum heart rate achieved |
| Exang    | Exercise-induced angina (1 = yes; 0 = no) |
| Oldpeak  | ST depression induced by exercise |
| Slope    | Slope of peak exercise ST segment (1–3) |
| Ca       | Number of major vessels (0–3) |
| Thal     | 0 = Normal, 2 = Fixed defect, 3 = Reversible defect |
| Target   | 0 = Less chance, 1 = More chance |

---

## 🛠️ Workflow  
1. **Data Preprocessing**  
   - Handling duplicates  
   - Outlier detection & capping  
   - Standardization  
   - PCA for feature analysis  

2. **Exploratory Data Analysis (EDA)**  
   - Target distribution  
   - Age, gender, and health factors vs. target  
   - Correlation matrix  

3. **Model Training & Evaluation**  
   - Hyperparameter tuning applied for each model  
   - Metrics: Accuracy, Precision, Recall, F1 Score  

---

## 📈 Model Performance  

| Model                | Accuracy | Recall | Precision | F1 Score |
|----------------------|----------|--------|-----------|----------|
| SVM (linear kernel) | 81%      | 84%    | 82%       | 83%      |
| Decision Tree (pruned) | 82% | 88% | 81%       | 84% |
| Random Forest       | 82% | 84%    | 84%   | 84% |
| Logistic Regression | 82%      | 82%    | 85%       | 83%      |

✅ **Best Models**: Decision Tree (post-pruning) & Random Forest  

---

## 📂 Repository Structure  
├── Fianl_code_Piyush_Aughad.ipynb # Jupyter notebook with full implementation

├── README.md # Project documentation


---

## 🚀 How to Run  
1. **Clone the repository:**  
Run in yaml

   ```bash
   git clone https://github.com/your-username/heart-disease-prediction.git
   cd heart-disease-prediction

2. **Install dependencies:**
Run in bash

pip install -r requirements.txt

3. **Run the Jupyter Notebook:**
Run in bash

jupyter notebook Fianl_code_Piyush_Aughad.ipynb

