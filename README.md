# California House Price Prediction

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

## Project Overview

This project predicts California house prices using Machine Learning regression models. The California Housing dataset was cleaned, preprocessed, analyzed, and used to train multiple regression algorithms. The models were evaluated using standard regression metrics, and the Random Forest Regressor achieved the best performance.

---

## Dataset

- **Dataset:** California Housing Dataset
- **Rows:** 20,640
- **Features:** 9
- **Target Column:** `median_house_value`

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- Joblib
- Google Colab

---

## Project Workflow

- Data Loading
- Data Cleaning
- Missing Value Handling
- Duplicate Check
- Exploratory Data Analysis (EDA)
- Label Encoding
- Train-Test Split
- Model Training
- Model Evaluation
- Model Comparison
- House Price Prediction

---

## Machine Learning Models

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

---

## Model Performance

| Model | R² Score |
|--------|---------:|
| Linear Regression | 0.6137 |
| Decision Tree Regressor | 0.6418 |
| Random Forest Regressor | **0.8075** |

### Best Model

**Random Forest Regressor** achieved the highest R² Score (**0.8075**) and was selected as the final prediction model.

---

## Evaluation Metrics (Linear Regression)

| Metric | Value |
|--------|------:|
| MAE | 51820.75 |
| MSE | 5062019613.46 |
| RMSE | 71147.87 |
| R² Score | 0.6137 |

---

## Sample Prediction

```python
sample = pd.DataFrame({
    "longitude": [-122.23],
    "latitude": [37.88],
    "housing_median_age": [41],
    "total_rooms": [880],
    "total_bedrooms": [129],
    "population": [322],
    "households": [126],
    "median_income": [8.3252],
    "ocean_proximity": [3]
})

prediction = rf.predict(sample)

print("Predicted House Price:", prediction[0])
```

### Output

```text
Predicted House Price: 425952.33
```

> **Note:** Using a Pandas DataFrame with feature names avoids the Scikit-Learn warning about missing feature names during prediction.

---

## Project Files

```
California-House-Price-Prediction/
│
├── California_House_Price_Prediction.ipynb
├── housing.csv
├── requirements.txt
└── README.md
```

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Requirements

```
numpy
pandas
matplotlib
scikit-learn
joblib
```

---

## Conclusion

Three regression models were trained and evaluated for predicting California house prices.

- Linear Regression achieved an R² Score of **0.6137**.
- Decision Tree Regressor achieved an R² Score of **0.6418**.
- Random Forest Regressor achieved the highest R² Score of **0.8075**.

Therefore, the **Random Forest Regressor** was selected as the final model because it provided the most accurate predictions.

---

## Author

**Rajendra Prasad Pedamallu**
