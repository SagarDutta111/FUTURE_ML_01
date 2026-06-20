#  Walmart Sales Forecasting using Machine Learning

##  Project Overview

This project predicts Walmart's weekly sales using Machine Learning. The model is built using the Random Forest Regressor algorithm and utilizes historical sales, store information, holiday data, and date-based features to forecast future sales.

##  Features

* Data preprocessing and cleaning
* Merging multiple datasets (`train.csv`, `stores.csv`, `features.csv`)
* Date feature extraction (Year, Month, Week, Day)
* Machine Learning model training using Random Forest Regressor
* Model evaluation using MAE and R² Score
* Visualization of Actual vs Predicted Sales
* Future sales prediction for custom inputs

##  Dataset Files

The project uses the following datasets:

* `train.csv` – Historical weekly sales data
* `stores.csv` – Store information
* `features.csv` – Additional store and holiday-related features

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

##  Data Processing

The following preprocessing steps were performed:

1. Merge datasets using Store and Date columns.
2. Convert Date column to datetime format.
3. Extract:

   * Year
   * Month
   * Week
   * Day
4. Handle missing values.
5. Select relevant features for training.

##  Machine Learning Model

Algorithm Used:

**Random Forest Regressor**

### Input Features

* Store
* Dept
* IsHoliday
* Year
* Month
* Week
* Day

### Target Variable

* Weekly_Sales

##  Model Evaluation

Evaluation metrics used:

* Mean Absolute Error (MAE)
* R² Score

##  Visualization

The project includes a comparison plot between:

* Actual Weekly Sales
* Predicted Weekly Sales

This helps evaluate the model's forecasting performance visually.

##  Future Prediction

Users can provide future store information and date-related values to predict upcoming weekly sales.

Example Input:

```python
Store = 1
Dept = 1
IsHoliday = 0
Year = 2026
Month = 6
Week = 25
Day = 20
```

The trained model returns the predicted weekly sales for the given input.

##  How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/walmart-sales-forecasting.git
```

2. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

3. Open the notebook:

```bash
jupyter notebook FUTURE_ML_01.ipynb
```

4. Run all cells sequentially.

##  Project Structure

```text
├── FUTURE_ML_01.ipynb
├── train.csv
├── stores.csv
├── features.csv
└── README.md
```

##  Future Improvements

* Hyperparameter tuning
* Feature engineering
* Cross-validation
* XGBoost implementation
* Deployment using Streamlit or Flask

##  Author

Anannya Mandal

If you found this project useful, consider giving it a  on GitHub.
