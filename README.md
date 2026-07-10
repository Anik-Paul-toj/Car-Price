# 🚗 Car Selling Price Prediction using Machine Learning

A Machine Learning project that predicts the **selling price of used cars** using various regression algorithms. The project covers the complete ML workflow including **data preprocessing, exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, and model evaluation**.

---

## 📌 Project Overview

Estimating the resale value of a used car is a common regression problem. The selling price depends on multiple factors such as:

- Manufacturing Year
- Present Market Price
- Kilometers Driven
- Fuel Type
- Seller Type
- Transmission Type
- Number of Previous Owners

This project compares multiple machine learning algorithms to identify the model that predicts car prices with the highest accuracy.

---

## 📂 Dataset

**Source:** Vehicle Dataset from CarDekho

### Dataset Statistics

| Property | Value |
|----------|------:|
| Original Samples | 301 |
| Samples after Outlier Removal | 276 |
| Features | 9 |
| Missing Values | 0 |

### Features

| Feature | Description |
|----------|-------------|
| Car_Name | Name of the car |
| Year | Manufacturing year |
| Present_Price | Current showroom price (Lakhs) |
| Kms_Driven | Total kilometers driven |
| Fuel_Type | Petrol / Diesel / CNG |
| Seller_Type | Dealer / Individual |
| Transmission | Manual / Automatic |
| Owner | Number of previous owners |
| Selling_Price | Target variable |

---

## 🛠 Data Preprocessing

The following preprocessing steps were performed:

- Missing value analysis
- Data type verification
- Exploratory data analysis
- Outlier removal using the IQR Method
- Label Encoding of categorical variables
- Feature Scaling using StandardScaler
- Train-Test Split (80% Training, 20% Testing)

---

## 📊 Exploratory Data Analysis

The project includes multiple visualizations to understand the dataset.

### Numerical Analysis

- Distribution of numerical features
- Correlation Heatmap
- Outlier Detection

### Categorical Analysis

- Fuel Type Distribution
- Seller Type Distribution
- Transmission Distribution

### Relationship Analysis

- Year vs Selling Price
- Present Price vs Selling Price
- Kilometers Driven vs Selling Price
- Fuel Type vs Selling Price
- Transmission vs Selling Price

---

## 🤖 Machine Learning Models

The following regression models were trained and evaluated.

| Model |
|--------|
| Linear Regression |
| Polynomial Regression |
| Decision Tree Regressor |
| Random Forest Regressor |
| Gradient Boosting Regressor |
| Support Vector Regressor (SVR) |
| XGBoost Regressor |

Hyperparameter tuning was performed using **GridSearchCV** for applicable models.

---

## 📈 Model Performance

| Model | R² Score | MAE | RMSE |
|------|---------:|---------:|---------:|
| 🥇 XGBoost Regressor | **0.9605** | **0.3832** | **0.5844** |
| 🥈 Gradient Boosting Regressor | 0.9590 | 0.3904 | 0.5957 |
| 🥉 Random Forest Regressor | 0.9412 | 0.4381 | 0.7132 |
| Polynomial Regression (Degree 2) | 0.9335 | 0.5052 | 0.7581 |
| Support Vector Regressor | 0.9214 | 0.5386 | 0.8244 |
| Decision Tree Regressor | 0.8738 | 0.6164 | 1.0447 |
| Linear Regression | 0.8398 | 0.8934 | 1.1771 |

---

## 🏆 Best Performing Model

### XGBoost Regressor

| Metric | Score |
|--------|-------:|
| R² Score | **0.9605** |
| Mean Absolute Error | **0.3832** |
| Root Mean Squared Error | **0.5844** |

The XGBoost Regressor achieved the highest prediction accuracy and was selected as the final model.

---

## 🔮 Sample Prediction

### Input

| Feature | Value |
|----------|------:|
| Year | 2014 |
| Present Price | 5.59 |
| Kilometers Driven | 27000 |
| Fuel Type | Petrol |
| Seller Type | Dealer |
| Transmission | Manual |
| Owner | 0 |

### Predicted Selling Price

**₹3.66 Lakhs**

---

## 📸 Generated Visualizations

The project generates several visualizations including:

- Distribution Histograms
- Count Plots
- Scatter Plots
- Box Plots
- Correlation Heatmap
- Actual vs Predicted Price Comparison

Example outputs are stored inside the **graphs/** directory.

---

## 📁 Project Structure

```text
Car-Price-Prediction/
│
├── graphs/
│   ├── heatmap.png
│   ├── actual_vs_predicted.png
│   └── ...
│
├── label_encoder_Fuel_Type.pkl
├── label_encoder_Seller_Type.pkl
├── label_encoder_Transmission.pkl
├── standard_scaler.joblib
│
├── Car_Price_Prediction.ipynb
├── requirements.txt
└── README.md
```

---

## ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Joblib
- Google Colab

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/car-price-prediction.git
```

Move into the project directory

```bash
cd car-price-prediction
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the notebook

```bash
jupyter notebook
```

Or open the notebook directly in **Google Colab**.

---

## 📦 Required Libraries

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
joblib
kagglehub
```

---

## 🚀 Future Improvements

- Deploy using Streamlit
- Build a Flask/FastAPI REST API
- Add CatBoost and LightGBM models
- Implement SHAP Explainability
- Perform Feature Selection
- Use Optuna for Hyperparameter Optimization
- Deploy on Render or Hugging Face Spaces

---

## 🎯 Learning Outcomes

This project demonstrates:

- Data Cleaning
- Data Visualization
- Exploratory Data Analysis
- Outlier Detection
- Feature Engineering
- Label Encoding
- Feature Scaling
- Regression Algorithms
- Hyperparameter Tuning
- Model Comparison
- Model Evaluation
- Machine Learning Deployment Preparation

---

## 👨‍💻 Author

**Anik Paul**

B.Tech Computer Science Engineering Student

Interested in **Machine Learning, Artificial Intelligence, Data Science, and Full-Stack Development**.

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
