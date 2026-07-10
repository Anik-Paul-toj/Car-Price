````markdown
# 🚗 Car Selling Price Prediction using Machine Learning

A complete Machine Learning project that predicts the **selling price of used cars** using multiple regression algorithms. The project includes **Exploratory Data Analysis (EDA), Data Preprocessing, Feature Engineering, Model Training, Hyperparameter Tuning, Model Evaluation, and Prediction**.

---

# 📌 Project Overview

The price of a used car depends on several factors such as:

- Manufacturing Year
- Present Market Price
- Kilometers Driven
- Fuel Type
- Seller Type
- Transmission
- Number of Previous Owners

This project builds and compares several Machine Learning regression models to accurately estimate the selling price of a used vehicle.

---

# 📂 Dataset

**Dataset Source**

Vehicle Dataset from CarDekho

Dataset contains **301 car records** with **9 features**.

After removing outliers using the **IQR Method**, the dataset contains:

- **276 samples**

---

# 📊 Features

| Feature | Description |
|----------|-------------|
| Car_Name | Name of the Car |
| Year | Manufacturing Year |
| Present_Price | Current Ex-showroom Price (Lakhs) |
| Kms_Driven | Distance Driven (KM) |
| Fuel_Type | Petrol / Diesel / CNG |
| Seller_Type | Dealer / Individual |
| Transmission | Manual / Automatic |
| Owner | Number of Previous Owners |
| Selling_Price | Target Variable |

---

# 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Checked missing values
- Verified data types
- Statistical summary
- Removed outliers using the IQR Method
- Label Encoding for categorical variables
- Feature Scaling using StandardScaler
- Train-Test Split (80:20)

---

# 📈 Exploratory Data Analysis (EDA)

Several visualizations were created to understand the dataset.

### Numerical Feature Distribution

- Year
- Selling Price
- Present Price
- Kilometers Driven
- Owner

### Categorical Feature Distribution

- Fuel Type
- Seller Type
- Transmission

### Scatter Plots

- Year vs Selling Price
- Present Price vs Selling Price
- Kilometers Driven vs Selling Price

### Box Plots

- Selling Price
- Present Price
- Kilometers Driven
- Fuel Type vs Selling Price
- Transmission vs Selling Price

### Correlation Heatmap

Relationship between all numerical features.

---

# ⚙️ Machine Learning Models Used

The following regression algorithms were trained and compared.

1. Linear Regression
2. Polynomial Regression
3. Decision Tree Regressor
4. Random Forest Regressor
5. Gradient Boosting Regressor
6. Support Vector Regressor (SVR)
7. XGBoost Regressor

Hyperparameter tuning was performed using **GridSearchCV** wherever applicable.

---

# 📏 Evaluation Metrics

Models were evaluated using:

- R² Score
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

---

# 🏆 Model Performance

| Model | R² Score | MAE | RMSE |
|--------|---------:|---------:|---------:|
| **XGBoost Regressor** | **0.9605** | **0.3832** | **0.5844** |
| Gradient Boosting Regressor | 0.9590 | 0.3904 | 0.5957 |
| Random Forest Regressor | 0.9412 | 0.4381 | 0.7132 |
| Polynomial Regression (Degree 2) | 0.9335 | 0.5052 | 0.7581 |
| Support Vector Regressor | 0.9214 | 0.5386 | 0.8244 |
| Decision Tree Regressor | 0.8738 | 0.6164 | 1.0447 |
| Linear Regression | 0.8398 | 0.8934 | 1.1771 |

---

# 🥇 Best Model

The **XGBoost Regressor** achieved the highest performance.

### Performance

- **R² Score:** 0.9605
- **MAE:** 0.3832
- **RMSE:** 0.5844

This model was selected as the final prediction model.

---

# 🔍 Sample Prediction

### Input

| Feature | Value |
|---------|------|
| Year | 2014 |
| Present Price | 5.59 |
| Kms Driven | 27000 |
| Fuel Type | Petrol |
| Seller Type | Dealer |
| Transmission | Manual |
| Owner | 0 |

### Predicted Selling Price

**₹3.66 Lakhs**

---

# 📊 Generated Visualizations

The project generates the following plots:

- Distribution Histograms
- Count Plots
- Scatter Plots
- Box Plots
- Correlation Heatmap
- Actual vs Predicted Price Graph

All graphs are exported into the **graphs/** directory.

---

# 📁 Project Structure

```
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
├── README.md
└── graphs.zip
```

---

# 🛠 Technologies Used

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

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/car-price-prediction.git

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

or open in **Google Colab**.

---

# 📦 Requirements

```
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

# 📈 Future Improvements

- Deploy the model using Flask or FastAPI
- Build a Streamlit web application
- Perform Feature Selection
- Use CatBoost and LightGBM
- Apply Cross Validation for more robust evaluation
- Add SHAP Explainability
- Hyperparameter optimization using Optuna
- Model deployment on Render or Hugging Face Spaces

---

# 📚 Learning Outcomes

This project demonstrates:

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Outlier Detection
- Feature Scaling
- Label Encoding
- Multiple Regression Algorithms
- Hyperparameter Tuning
- Model Comparison
- Performance Evaluation
- Real-world Price Prediction

---

# 👨‍💻 Author

**Anik Paul**

B.Tech CSE Student

Machine Learning | AI | Data Science | Full Stack Developer

---

## ⭐ If you found this project helpful, consider giving it a Star!
````
