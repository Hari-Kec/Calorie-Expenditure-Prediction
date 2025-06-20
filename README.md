# 🏃‍♂️ Calorie Expenditure Prediction

This project leverages machine learning to predict **calorie expenditure** based on physical and biometric input data. It aims to provide accurate insights into the number of calories burned during physical activity using regression techniques and model evaluation.

---

## 📌 Project Objectives

* Load and preprocess biometric and activity datasets
* Train machine learning regression models to predict calories burned
* Evaluate model performance using metrics such as MAE, MSE, and R²
* Visualize predictions vs actual values
* Save and load trained models for deployment

---

## 📁 Dataset Overview

The dataset includes:

* **Age**
* **Height**
* **Weight**
* **Duration of Exercise**
* **Heart Rate**
* **Body Temperature**
* **Calories Burned (Target)**

Data is assumed to be in CSV format and loaded using `pandas`.

---

## ⚙️ Technologies Used

* Python 3.x
* Jupyter Notebook
* `pandas`, `numpy`, `seaborn`, `matplotlib`
* `scikit-learn` (Linear Regression, RandomForest, etc.)
* `joblib` for model serialization

---

## 📊 Model Training

Models used:

* **Linear Regression**
* **Random Forest Regressor**
* Performance metrics:

  * Mean Absolute Error (MAE)
  * Mean Squared Error (MSE)
  * R² Score

```python
from sklearn.linear_model import LinearRegression
from sklearn.ensemble import RandomForestRegressor
```

---

## 🧪 Evaluation

* Comparison of predicted vs actual calories
* R² score visualization
* Error analysis using seaborn & matplotlib
* Feature importance for Random Forest

---

## 💾 Model Persistence

Save model:

```python
import joblib
joblib.dump(model, 'calorie_predictor.pkl')
```

Load model:

```python
model = joblib.load('calorie_predictor.pkl')
```

---

## 📈 Example Output

```
Input: [Age, Height, Weight, Duration, Heart Rate, Body Temp]
Prediction: 230.57 Calories
```

Visuals include:

* Pairplot of features
* Heatmaps for correlation
* Line plots of actual vs predicted calories

---

## 🚀 Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/Hari-Kec/calorie-expenditure-prediction.git
   cd calorie-expenditure-prediction
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:

   ```bash
   jupyter notebook Calorie_Expenditure_prediction.ipynb
   ```

---

## 📌 To-Do

* Integrate with a web frontend (Streamlit or Flask)
* Add support for real-time input
* Deploy model to cloud (Heroku, AWS)

---

## 📜 License

This project is licensed under the **MIT License**.

---

