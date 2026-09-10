# 🚗 Car Price Prediction with Machine Learning

## 📌 CodeAlpha Data Science Internship – Task 3

This project is developed as part of the **CodeAlpha Data Science Internship**.

The objective of this project is to build a Machine Learning model that predicts the **selling price of a car** based on different features such as car age, present price, kilometers driven, fuel type, transmission type, selling type, and number of previous owners.

---

## 🎯 Project Objective

The main objectives of this project are:

* Load and explore the car dataset.
* Check for missing and duplicate values.
* Perform data preprocessing.
* Create useful features using feature engineering.
* Convert categorical data into numerical form.
* Split the dataset into training and testing data.
* Train a Machine Learning regression model.
* Predict car selling prices.
* Evaluate model performance.
* Visualize the prediction results.
* Save the trained model for future use.

---

## 📊 Dataset Features

The dataset contains the following features:

| Feature       | Description                                |
| ------------- | ------------------------------------------ |
| Car_Name      | Name of the car                            |
| Year          | Manufacturing year of the car              |
| Selling_Price | Selling price of the car (Target Variable) |
| Present_Price | Current market price of the car            |
| Driven_kms    | Total kilometers driven                    |
| Fuel_Type     | Type of fuel used                          |
| Selling_type  | Dealer or Individual                       |
| Transmission  | Manual or Automatic                        |
| Owner         | Number of previous owners                  |

---

## ⚙️ Feature Engineering

A new feature called **Car_Age** was created using the manufacturing year of the car.

This feature helps the model understand how old the car is.

After feature engineering, unnecessary columns such as `Car_Name` and `Year` were removed from the training data.

---

## 🤖 Machine Learning Model

The project uses:

### 🌲 Random Forest Regressor

Random Forest is an ensemble machine learning algorithm that uses multiple decision trees to make predictions.

The model is trained using:

```python
RandomForestRegressor(
    n_estimators=100,
    random_state=42
)
```

---

## 🔄 Project Workflow

```text
Car Dataset
     ↓
Data Exploration
     ↓
Data Cleaning
     ↓
Feature Engineering
     ↓
Categorical Data Encoding
     ↓
Feature Selection
     ↓
Train-Test Split
     ↓
Random Forest Regressor
     ↓
Model Training
     ↓
Car Price Prediction
     ↓
Model Evaluation
     ↓
Data Visualization
     ↓
Save Model
```

---

## 📈 Model Evaluation

The model was evaluated using the following regression metrics:

* **MAE (Mean Absolute Error)**
* **MSE (Mean Squared Error)**
* **RMSE (Root Mean Squared Error)**
* **R² Score**

For regression problems, R² Score is used to measure how well the model explains the variation in car selling prices.

---

## 📊 Data Visualization

The project includes visualizations such as:

* Actual vs Predicted Car Prices
* Random Forest Feature Importance

These visualizations help understand the model's predictions and identify which features have the greatest impact on car prices.

---

## 💾 Saved Model

The trained Random Forest model is saved using Joblib as:

```text
car_price_model.pkl
```

The saved model can be loaded later and used to predict car prices without training the model again.

---

## 🛠️ Technologies and Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Joblib

---

## 📁 Project Structure

```text
Task3_Car_Price_Prediction
│
├── Car_Price_Prediction.ipynb
├── car data.csv
├── car_price_model.pkl
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone <repository-url>
```

### 2. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 3. Open the Jupyter Notebook

```bash
jupyter notebook Car_Price_Prediction.ipynb
```

### 4. Run All Cells

Run the notebook cells to:

* Load the dataset.
* Preprocess the data.
* Train the Random Forest model.
* Make predictions.
* Evaluate the model.
* Generate visualizations.

---

## 🌍 Real-World Applications

Car price prediction models can be useful for:

* Used car marketplaces.
* Car dealerships.
* Online car selling platforms.
* Car buyers and sellers.
* Vehicle price estimation systems.

---

## 👨‍💻 Author

**Dharmendra Kumar Singh**

**CodeAlpha Data Science Internship**
