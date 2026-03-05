# 🚗 Car Price Prediction with Machine Learning

## 📌 Overview
This project builds a **Machine Learning model to predict the selling price of used cars** based on various features such as present price, kilometers driven, fuel type, transmission type, and ownership history.

Used car pricing depends on many factors. By analyzing historical car data, this project trains a **Random Forest Regression model** to learn patterns and estimate the selling price of a car.

# 🎯 Objective
The objective of this project is to:
* Analyze a used car dataset
* Perform **data preprocessing and feature engineering**
* Train a **Machine Learning regression model**
* Predict the **selling price of cars**
* Evaluate model performance

# 📂 Dataset Information
The dataset contains information about used cars and their selling prices.

### Features in the Dataset
| Feature       | Description                                       |
| ------------- | ------------------------------------------------- |
| Car_Name      | Name of the car                                   |
| Year          | Manufacturing year of the car                     |
| Selling_Price | Price at which the car was sold (Target Variable) |
| Present_Price | Current ex-showroom price of the car              |
| Driven_kms    | Total kilometers driven                           |
| Fuel_Type     | Type of fuel used (Petrol/Diesel/CNG)             |
| Selling_type  | Dealer or Individual                              |
| Transmission  | Manual or Automatic                               |
| Owner         | Number of previous owners                         |

# ⚙️ Technologies Used
* **Python**
* **Pandas** – Data analysis
* **NumPy** – Numerical computing
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Machine learning algorithms

# 🧹 Data Preprocessing
Several preprocessing steps were performed to prepare the dataset for machine learning.

### 1️⃣ Removing unnecessary columns
The `Car_Name` column was removed since it does not contribute significantly to predicting the price.

### 2️⃣ Feature Engineering
A new feature called **Car_Age** was created:
Car_Age = Current Year - Manufacturing Year
This helps the model understand how old the car is.

### 3️⃣ Encoding Categorical Variables
Categorical variables such as:
* Fuel_Type
* Selling_type
* Transmission
were converted into numerical values using **One-Hot Encoding**.

# 🤖 Machine Learning Model
The project uses **Random Forest Regression**, an ensemble learning algorithm that combines multiple decision trees to produce more accurate predictions.

# 🔀 Train-Test Split
The dataset was divided into:
80% Training Data
20% Testing Data
Training data is used to train the model, while testing data evaluates its performance.

# 📊 Model Training
The Random Forest model was trained using:
model.fit(X_train, y_train)
Where:
* `X_train` → training features
* `y_train` → training target values (selling price)

# 🔮 Making Predictions
The trained model predicts car prices using:
predictions = model.predict(X_test)
Each prediction represents the estimated selling price of a car.

# 📈 Model Evaluation
Model performance is evaluated using **R² Score**:
R2 Score = r2_score(y_test, predictions)

### What R² Score Means
| Score     | Interpretation       |
| --------- | -------------------- |
| 1.0       | Perfect predictions  |
| 0.8 – 0.9 | Very good model      |
| 0.6 – 0.7 | Moderate performance |
A higher score indicates that the model predicts prices more accurately.

# 📉 Visualization
A scatter plot is used to compare **Actual Prices vs Predicted Prices**.
This helps visualize how close the predictions are to the real values.

# 🗂 Project Structure
OIBSIP2
│
├── Car_price_Prediction
│   ├── data
│   │   └── car data.csv
│   ├── car_price_prediction.ipynb
│   ├── car_price_model.pkl
│   └── README.md

# ▶️ How to Run the Project
### 1️⃣ Clone the repository
git clone https://github.com/your-username/OIBSIP2.git
### 2️⃣ Navigate to project folder
cd OIBSIP2/Car_price_Prediction
### 3️⃣ Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn
### 4️⃣ Run the notebook
Open:
car_price_prediction.ipynb
Run all cells to train the model and generate predictions.

# 📚 Learning Outcomes
Through this project, the following skills were developed:
* Data preprocessing
* Feature engineering
* Regression modeling
* Model evaluation
* Machine learning workflow implementation

