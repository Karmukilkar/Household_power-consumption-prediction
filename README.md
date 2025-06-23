# Power Household Consumption Regression Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-orange.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.0%2B-yellow.svg)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.0%2B-green.svg)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11%2B-cyan.svg)](https://seaborn.pydata.org/)

## 📊 Project Overview

This project analyzes and predicts household power consumption using various regression models. The workflow covers data preprocessing, feature engineering, exploratory data analysis, model building (Linear Regression, Random Forest, Gradient Boosting, Neural Networks), evaluation, and visualization.

---

## 🛠️ Technical Tags

- Data Preprocessing
- Regression Modeling
- Feature Engineering
- Hyperparameter Tuning
- Visualization
- Python
- Scikit-learn
- Pandas
- Matplotlib/Seaborn

---

## 🚀 Approach

1. **Data Preprocessing:**  
   - Load and clean raw data
   - Handle missing values and convert data types
2. **Feature Engineering:**  
   - Extract date/time features, create rolling averages, aggregate sub-metering, and define target variable
3. **Exploratory Data Analysis:**  
   - Visualize distributions, trends, and correlations
4. **Modeling:**  
   - Train and evaluate Linear Regression, Random Forest, Gradient Boosting, and Neural Network models
5. **Evaluation:**  
   - Use MSE, RMSE, and MAPE for model comparison
6. **Model Saving:**  
   - Serialize trained models for future use

---

## 📁 Project Structure

```
power_household/
│
├── process.ipynb                # Data preprocessing and feature engineering notebook
├── ml.ipynb                     # Model building, evaluation, and saving notebook
├── power_consum.csv             # Raw data file
├── power_consumption_cleaned.csv# Cleaned and processed data
├── linera_model.pkl             # Saved Linear Regression model
├── RF_model.pkl                 # Saved Random Forest model
├── GB_model.pkl                 # Saved Gradient Boosting model
├── Neural_model.pkl             # Saved Neural Network model
└── README.md                    # Project documentation
```

---

## 📈 Key Insights

- **Seasonal Trends:** Power consumption peaks in winter, especially January, and drops in summer/vacation months.
- **Feature Importance:** Global active power, voltage, and sub-metering are strong predictors.
- **Model Performance:** Ensemble models (Random Forest, Gradient Boosting) outperform linear regression.
- **Standardization:** Improves model convergence and accuracy.

---

## 📝 How to Run

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/power_household.git
    cd power_household
    ```

2. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Create `requirements.txt` with pandas, numpy, scikit-learn, matplotlib, seaborn, scipy, etc.)*

3. **Run Notebooks:**
    - Open `process.ipynb` for data preprocessing.
    - Open `ml.ipynb` for model training and evaluation.

---

## 📊 Visualization Examples

- Distribution plots for all features
- Yearly and monthly power consumption barplots
- Correlation heatmap
- Boxplots for outlier detection

---

## 🤖 Model Evaluation

| Model                | MSE      | RMSE     | MAPE     |
|----------------------|----------|----------|----------|
| Linear Regression    | 7.129252 | 0.000844	| 0.000147 |
| Random Forest        | 0.000043 | 0.006527 | 0.001451 |
| Gradient Boosting    | 0.007653 | 0.087481 | 0.230922 |
| Neural Network       | 0.007582 | 0.087074 | 0.231992 |

*(Fill in with your actual results)*

---

## 💡 Recommendations

- Add weather/holiday data for improved predictions
- Use hyperparameter tuning for optimal model performance
- Consider robust scaling or outlier removal for stability
- Deploy the best model for real-time prediction

---

## 📚 References

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
- [Seaborn Documentation](https://seaborn.pydata.org/)

---

## © License

This project is licensed under the MIT License.
