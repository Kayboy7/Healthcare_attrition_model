### **📌 Healthcare Employee Attrition Prediction**
**Predicting Employee Attrition Using Machine Learning**
---

## **📖 Project Overview**
Employee attrition is a critical issue in healthcare, impacting productivity, cost, and service quality. 
This project uses **Machine Learning** to analyze attrition factors and predict whether an employee will leave.  

Key Goals:
- Understand factors influencing employee attrition.
- Build a predictive model using **Random Forest** and **XGBoost**.
- Optimize performance using **threshold tuning and hyperparameter tuning**.

---

## **📊 Dataset Information**
This Kaggle dataset contains various employee attributes, such as:
- **Demographics**: Age, Gender, Marital Status, Education.
- **Job Factors**: Job Role, Department, Years at Company, Monthly Income.
- **Work Conditions**: Work-Life Balance, Overtime, Environment Satisfaction.

📂 **Dataset Source**: *Kaggle Healthcare Employee Data (Modified)*  
🔍 **Target Variable**: `Attrition` (Yes/No)

---

## **🛠️ Methodology**
### **1️⃣ Data Preprocessing**
- Handled missing values and inconsistent entries.
- Converted categorical variables using **One-Hot Encoding** and **Ordinal Encoding**.
- Standardized numerical features using **StandardScaler**.

### **2️⃣ Exploratory Data Analysis (EDA)**
- Identified attrition trends using **univariate & bivariate analysis**.
- Visualized correlations using **heatmaps & bar charts**.

### **3️⃣ Model Training & Evaluation**
- **Baseline Models**: Logistic Regression, KNN.
- **Advanced Models**: Random Forest, XGBoost.
- **Class Imbalance Handling**: Used `scale_pos_weight` and **threshold tuning**.
- **Hyperparameter Tuning**: Used `GridSearchCV` for fine-tuning.

### **4️⃣ Model Performance**
📈 **Final Model: XGBoost**  
- **Accuracy**: 89%  
- **Precision (Attrite)**: 53%  
- **Recall (Attrite)**: 73% (Improved with threshold tuning)  
- **F1-Score (Attrite)**: 62%

🚀 **Key Improvement**: After tuning, recall increased from **33% → 73%**!

---

## **📂 Project Structure**
```
├── data/                        # Dataset files
├── notebooks/                    # Jupyter Notebooks for EDA & Modeling
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_eda_visualization.ipynb
│   ├── 03_model_training.ipynb
│   ├── 04_hyperparameter_tuning.ipynb
│   ├── 05_threshold_adjustment.ipynb
├── src/                          # Python scripts for training & evaluation
│   ├── preprocess.py             # Data cleaning & encoding functions
│   ├── model_train.py            # Model training & evaluation
│   ├── utils.py                  # Helper functions
├── images/                       # Visualizations
│   ├── confusion_matrix.png
│   ├── precision_recall_curve.png
├── README.md                     # Project documentation
├── requirements.txt               # Python dependencies
├── main.py                        # Main script to run the pipeline
```

## **📈 Results & Insights**
- Employees with **low job satisfaction & work-life balance** had **higher attrition**.
- **Frequent business travel** was a key factor in attrition.
- **XGBoost outperformed Random Forest**, improving recall from 47% → 73%.
- **Threshold tuning** played a crucial role in optimizing the model.

---

## **📌 Future Improvements**
✅ Implement **SMOTE** for better class balance  
✅ Explore **Deep Learning (Neural Networks)** for performance gains  
✅ Develop a **dashboard for HR analytics** using Streamlit  

---

## **🤝 Contributing**
Contributions are welcome! Feel free to open an **Issue** or **Pull Request**.

---

## **📩 Contact** 
📧 **Email**: olayboya@gmail.com  
📢 **LinkedIn**: https://linkedin.com/in/yonnantcheboya
