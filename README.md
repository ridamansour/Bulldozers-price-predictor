# 🚜 Bulldozer Price Estimator using Machine Learning

This project builds a machine learning model to predict the selling price of used bulldozers based on various features like brand, age, kilometers driven, fuel type, and more. The goal is to assist buyers and sellers in making informed decisions.

---

## 📌 Project Overview

* **Objective**: Predict the price of a bulldozer based on input features.
* **Dataset**: A cleaned and preprocessed dataset of used bulldozers.
* **Outcome**: A regression model capable of estimating bulldozer prices with reasonable accuracy.

---

## 📊 Features Used

Key input features include:

* `name` – bulldozer model name
* `year` – Year of purchase
* `km_driven` – Kilometers driven
* `fuel` – Type of fuel (Petrol/Diesel/etc.)
* `seller_type` – Individual, Dealer, etc.
* `transmission` – Manual or Automatic
* `owner` – Ownership status
* `mileage`, `engine`, `max_power` – Engine performance indicators
* `seats` – Number of seats

Target variable:

* `selling_price` – bulldozer's selling price in lakhs

---

## 🛠 Workflow

1. **Data Cleaning & Preprocessing**

   * Handling missing values
   * Converting categorical features to numerical
   * Feature engineering (e.g., extracting brand names)

2. **Exploratory Data Analysis (EDA)**

   * Distribution of price, fuel type, transmission type
   * Correlation heatmap and feature importance

3. **Modeling**

   * Regression models explored:

     * **Linear Regression**
     * **Lasso Regression**
     * **Ridge Regression**
     * **Random Forest Regressor**
   * Best performance achieved using **Random Forest**

4. **Model Evaluation**

   * R² Score
   * Mean Absolute Error (MAE)
   * Cross-validation

---

## 📁 File Structure

```
├── bulldozer-price-prediction.ipynb   # Main notebook
├── data/
│   └── bulldozers.csv                 # Raw or cleaned bulldozer dataset
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
```

---

## 📦 Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/ridamansour/bulldozer-price-prediction.git
cd bulldozer-price-prediction
pip install -r requirements.txt
```

---

## 🚀 Running the Project

```bash
jupyter notebook bulldozer-price-prediction.ipynb
```

Make sure the dataset file (typically `bulldozers.csv`) is located in the correct folder (`/data`) or as referenced in the notebook.

---

## 📌 Results

* Final model: **Random Forest Regressor**
* Achieved R² score: \~0.86+ (depending on parameters)
* Predicts used bulldozer prices with decent real-world accuracy

---

## 🔮 Future Improvements

* Deploy as a web app using Flask or Streamlit
* Add more recent or diverse data
* Hyperparameter tuning (e.g., GridSearchCV for Random Forest)
* Feature selection or PCA

---

## 📄 License

This project is open-sourced.
