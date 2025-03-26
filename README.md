# **Well-Log Lithology Classification - HCML One**

## **Overview**
This repository contains our project submission for **SCALE-UP 2025 Geo-energy Hackathon**. Our team, **HCML One**, participated in the **Professional** category and secured **7th place** with a final score of **0.6276**. The goal of this competition was to develop a machine learning model to predict lithology types using well log data.

## **Project Description**
Lithology classification is crucial in oil and gas exploration, as it helps geologists and engineers understand subsurface rock formations. This project leverages **machine learning** to classify lithology based on well log data, optimizing the exploration process for energy resources.

### **Dataset & Features**
We used a well log dataset containing various geophysical measurements, including:
- **Gamma Ray (GR)**
- **Bulk Density (RHOB)**
- **Neutron Porosity (NPHI)**
- **Resistivity Logs (RDEP, RMED, RSHA)**
- **Sonic Logs (DTC, DTS)**
- **Caliper Log (CALI)**
- **Self Potential (SP)**
- **Mud Weight (MUDWEIGHT)**
- **X, Y, Z Coordinates**
- **Measured Depth (DEPTH_MD)**

## **Approach & Methodology**
### **1. Data Preprocessing**
- Handled missing values using interpolation and nearest-neighbor estimation.
- Normalized and scaled numerical features.
- Engineered new features for better model representation.

### **2. Feature Selection & Engineering**
- Analyzed feature importance using correlation heatmaps.
- Applied **Principal Component Analysis (PCA)** for dimensionality reduction.

### **3. Model Selection & Training**
- Tested various machine learning models, including:
  - **Random Forest**
  - **XGBoost**
  - **CatBoost**
  - **Neural Networks**
- Fine-tuned hyperparameters using **GridSearchCV** and **Optuna**.

### **4. Evaluation & Submission**
- The models were evaluated using the **Weighted F1 Score**.
- The best-performing model was selected based on cross-validation results.
- The final predictions were formatted and submitted for leaderboard ranking.

## **Results**
🏆 **Final Score:** **0.6276**
📊 **Leaderboard Rank:** **7th Place (Professional Category)**


## **Installation & Usage**
### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/HCML-One-WellLog-Classification.git
cd HCML-One-WellLog-Classification
```

### **2. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3. Run Data Preprocessing**
```bash
python src/preprocessing.py
```

### **4. Train the Model**
```bash
python src/model_training.py
```

### **5. Evaluate the Model**
```bash
python src/evaluation.py
```

### **6. Generate Submission File**
```bash
python src/generate_submission.py
```

## **Lessons Learned**
- Effective **feature engineering** significantly improves model performance.
- **Hyperparameter tuning** optimizes model accuracy but requires computational trade-offs.
- **Ensemble learning** techniques, such as blending multiple models, can enhance predictive performance.

## **Acknowledgments**
We extend our gratitude to **SCALE-UP 2025 Geo-energy Hackathon**, **Husky-CNOOC Madura Limited (HCML)**, and our mentors for their guidance and support throughout the competition.

## **Contributors**
- **Yudha Adi Putra**
- **Sherly**
- **Alvin**

---
📩 **For inquiries, feel free to contact us!**
yudhaadiputra26@gmail.com