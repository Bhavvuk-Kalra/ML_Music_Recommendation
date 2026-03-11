## **🎵 Music Recommendation System – ML Model Comparison 🎵**
**⭐ Best Model:** LightGBM  
**📊 Task:** Binary Classification  
**🎯 Goal:** Predict whether a song should be recommended to a user

### **📌 Project Overview:**

This project builds a machine learning system to predict whether a user will listen to a song again.  
The goal is to model user listening behavior and improve music recommendation systems using historical interaction data.
The project explores multiple machine learning algorithms, performs extensive feature engineering, and compares model performance to identify the best predictive model.

### **📊 Dataset:**

The dataset contains user-song interaction records along with metadata about songs and users.

Main datasets used
- train.csv - user-song interaction data with target variable
- songs.csv - song metadata
- members.csv - user metadata
- test.csv - unseen user-song pairs

🎯 Target Variable:

The target column represents whether a song should be recommended to a user again.

1 - Can Recommend again.

0 - Cannot Recommend again.

(The task is to predict this binary outcome using features derived from the datasets)


### **⚙️ Project Workflow:**

1️⃣ Exploratory Data Analysis

(Visualizations and statistical exploration were performed to understand)

- user behavior
- song metadata
- interaction patterns

2️⃣ Data Preprocessing

- Data cleaning
- Handling missing values
- Merging datasets
- Outlier handling
- Sampling for training efficiency

3️⃣ Feature Engineering

Several behavioral and metadata features were created to improve predictive performance.

Examples

User behavior features
- user_song_count
- user_unique_songs
- user_unique_artists

Song popularity features
- song_play_count
- song_user_count

Artist features
- artist_song_count
- artist_popularity

Metadata features
- genre_count
- song_name_length
- membership_days
- account_age_days

4️⃣ Model Training

Multiple machine learning models were trained and compared.

Models used include:
- AdaBoost
- CatBoost
- Decision Tree
- Gaussian Naive Bayes
- KMeans Clustering
- KNN
- LightGBM
- Logistic Regression
- Random Forest
- XGBoost

5️⃣ Hyperparameter Tuning

Several models were tuned using RandomizedSearchCV to improve performance.

6️⃣ Model Evaluation

Models were evaluated using the following metrics
- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

### **📈 Model Performance Comparison:**

The trained models were evaluated and compared to identify the best-performing algorithms.
The final results show that gradient boosting models such as LightGBM, XGBoost and CatBoost achieved the strongest performance for this task.

<img width="560" height="659" alt="Performance Comparison" src="https://github.com/user-attachments/assets/1467b354-9b0f-4dc6-9448-ae6afba07510" />

### **📂 Repository Structure:**

```
ML_Music_Recommendation/
│
├── datasets/              # Original datasets
│   └── processed/         # Cleaned and processed datasets
│
├── models/                # Saved trained models (.pkl)
├── notebooks/             # Jupyter notebooks for analysis
│   ├── 01_EDA.ipynb
│   ├── 02_Feature_Engineering.ipynb
│   ├── 03_Model_Training.ipynb
│   └── 04_Model_Evaluation.ipynb
│
├── results/               # Model comparison results and visualizations
│
├── README.md
└── requirements.txt
```

### **🛠 Technologies Used:**

- Python
- pandas
- NumPy
- scikit-learn
- LightGBM
- XGBoost
- CatBoost
- Matplotlib
- Seaborn


### **🚀 Future Improvements:**

Possible future enhancements include:
- advanced user preference modeling
- sequential recommendation models
- deep learning based recommendation systems
- hybrid collaborative filtering approaches


### **👤 Author:**

Bhavvuk D Kalra

Data Analyst | Machine Learning Enthusiast

LinkedIN: (https://linkedin.com/in/bhavvuk-kalra)
