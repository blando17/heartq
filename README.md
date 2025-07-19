# Heart Disease Predictor 

This project builds a logistic regression model to predict the presence of heart disease based on medical attributes. It uses clinical data to assess whether a patient is likely to suffer from heart disease.

## 📁 Dataset

The dataset used is `heart_disease_data.csv`, which contains **303 samples** and **14 columns**.

### Features:
- age
- sex
- cp (chest pain type)
- trestbps (resting blood pressure)
- chol (cholesterol)
- fbs (fasting blood sugar)
- restecg (resting ECG results)
- thalach (maximum heart rate achieved)
- exang (exercise-induced angina)
- oldpeak (ST depression)
- slope (slope of the ST segment)
- ca (number of major vessels)
- thal (thalassemia)

### Target:
- `target` → 1 (Presence of heart disease), 0 (No heart disease)

##  Workflow

### 1. **Data Collection & Preprocessing**
- Loaded data using `pandas`
- Verified missing values (none found)
- Split features and target

### 2. **Train-Test Split**
- Used `train_test_split` from scikit-learn
- 80% for training, 20% for testing
- Stratified based on class label

### 3. **Model Training**
- Trained a **Logistic Regression** model
- Used scikit-learn's `LogisticRegression()`

### 4. **Evaluation**
- **Training Accuracy**: 85.12%
- **Testing Accuracy**: 81.96%

### 5. **Prediction System**
- Built a user prediction system to input new patient data
- Predicts presence or absence of heart disease using trained model

##  Key Insights

- Logistic Regression performs well on structured health datasets
- Features like chest pain type (`cp`), cholesterol, and maximum heart rate (`thalach`) are influential

##  Libraries & Tools

- Python
- Pandas, NumPy
- Scikit-learn (LogisticRegression, train_test_split, accuracy_score)

##  How to Use

1. Load the dataset: `heart_disease_data.csv`
2. Run the preprocessing and model training steps
3. Use the predictive system to check new input values
4. Model will output a diagnosis (Heart Disease or Not)

##  Conclusion

This project demonstrates how machine learning can aid in early detection of heart disease, enabling faster and potentially life-saving interventions.
