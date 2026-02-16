# pumpkin-seed varieties project
# Harvesting Brilliance
Pumpkin Seed Classification Project
Harvesting Brilliance: A Taxonomic Tale of Pumpkin Seed Varieties
📌 1. Introduction

Pumpkin seeds are one of the most nutritious and valuable seeds used in food, agriculture, and health industries. Although commonly consumed, their varieties differ significantly in physical features such as area, perimeter, shape, and texture.

This project analyzes pumpkin seed varieties using Machine Learning classification techniques. The trained model is deployed using a Flask web application, where users can enter seed feature values and receive a predicted variety.

🎯 2. Project Objective

Classify pumpkin seeds into different varieties using machine learning.

Build an end-to-end ML pipeline (data → model → deployment).

Develop a Flask web application for user-friendly predictions.

❓ 3. Problem Statement

Pumpkin seed varieties contain multiple morphological features such as:

Area

Perimeter

Major Axis Length

Minor Axis Length

Compactness

Manual identification is difficult and time-consuming. An automated ML-based system is required to predict seed type based on these features.

💡 4. Proposed Solution

Dataset collected from Kaggle

Data cleaning & preprocessing

Exploratory Data Analysis (EDA)

Multiple ML models trained

Best-performing model selected

Model deployed using Flask

UI developed with HTML & CSS

🌍 5. Applications / Use Cases
👨‍🌾 Farmers’ Conference

Identify seed varieties best suited for farming conditions to improve yield and pest resistance.

🥗 Nutrition & Health Industry

Analyze varieties with better protein and mineral content for supplements and healthy foods.

🍪 Food Brands

Develop snacks, oils, and bakery products using specific pumpkin seed varieties.

🔄 6. Project Flow

User enters seed feature values via UI

Input sent to trained ML model

Model predicts the seed variety

Output displayed on the webpage

🏗 7. Technical Architecture
Frontend (HTML/CSS)
        ↓
Flask Backend (app.py)
        ↓
Saved ML Model (model.pkl)
        ↓
Prediction Output (Webpage)
🛠 8. Prerequisites
Software Requirements

VS Code / Anaconda Navigator

Python 3.10+

Flask Web Framework

Python Packages Used

numpy

pandas

scikit-learn

matplotlib

seaborn

scipy

pickle-mixin

Flask

openpyxl

📊 9. Dataset Collection

Dataset source: Kaggle

Format: .csv / .xlsx

Contains morphological features and target class

🧹 10. Data Preparation
10.1 Dataset Information

df.info() – Check column names & datatypes

df.shape – Check dataset size

10.2 Missing Values

df.isnull().sum() – Identify missing values

10.3 Outlier Handling

Seaborn boxplot used for detection

Outliers removed/handled

10.4 Feature Scaling

Min-Max Scaling applied (values between 0–1)

Scaled features: Area, Perimeter, Major Axis Length, etc.

📈 11. Exploratory Data Analysis (EDA)
Descriptive Statistics

df.describe() – Mean, Std, Min, Max

Univariate Analysis

Distplot – Feature distribution

Countplot – Target distribution

Bivariate Analysis

Scatter plot – Area vs Perimeter

Multivariate Analysis

Pairplot – Relationship between multiple features

✂ 12. Splitting Dataset

train_test_split()

80% Training Data

20% Testing Data

🤖 13. Model Building

The following algorithms were used:

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

Naive Bayes (Multinomial NB)

Support Vector Machine (SVM)

Gradient Boosting Classifier

📊 14. Performance Testing & Hyperparameter Tuning

Evaluation Metrics:

Accuracy Score

Classification Report

Models were compared based on accuracy.

🏆 15. Best Model Selection

Decision Tree, Random Forest, and Gradient Boosting achieved the highest accuracy.

The best-performing model was selected for deployment.

🚀 16. Model Deployment

Saved files:

model.pkl

scaler.pkl

label_encoder.pkl

Used inside Flask application for prediction.

🌐 17. Web Application Development

Flask integrates the ML model with web UI.

HTML Pages

index.html → Home page

check.html → Input form

predict.html → Prediction result

All stored inside the templates/ folder.

🧠 18. Flask Backend (app.py)

The Flask app:

Loads model & scaler

Takes user input

Converts input to array

Applies scaling

Predicts seed class

Displays result

📁 19. Project Folder Structure
PumpkinSeedProject/
│
├── app.py
├── model_training.py
├── model.pkl
├── scaler.pkl
├── label_encoder.pkl
│
├── dataset/
│    └── Pumpkin_Seeds_Dataset.xlsx
│
├── templates/
│    ├── index.html
│    ├── check.html
│    └── predict.html
│
└── static/
     ├── css/
     │     └── style.css
     └── images/
           ├── banner.jpg
           └── seeds.jpg
▶ 20. How to Run the Project
Step 1: Install Required Packages
pip install numpy pandas scikit-learn matplotlib seaborn flask openpyxl
Step 2: Train Model
python model_training.py
Step 3: Run Flask App
python app.py
Step 4: Open in Browser
http://127.0.0.1:5000
Step 5: Predict

Click Check

Enter feature values

Click Submit

View prediction

✅ 21. Result

The model successfully predicts pumpkin seed variety.

Output Classes:

Çerçevelik

Ürgüp Sivrisi

The Flask UI provides real-time predictions with a user-friendly interface.

🎓 22. Conclusion

This project demonstrates how Machine Learning can classify pumpkin seed varieties using morphological features.

The trained model achieved high accuracy and was successfully deployed using Flask.

Applications include agriculture, nutrition, and food industries.

🔮 23. Future Scope

Use deep learning models for better accuracy

Add more seed varieties (multi-class classification)

Deploy on cloud (AWS / Heroku)

Add database for storing predictions

Improve UI with visualization dashboard
