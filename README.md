# 🔋 Energy Consumption Prediction

This project predicts household energy usage using the UCI Individual Household Electric Power Consumption Dataset. After cleaning and preprocessing the data, advanced feature engineering techniques were applied (hour, weekday, rolling averages, and lag features). Models used include Random Forest and XGBoost, both achieving highly accurate results.

# 📊 Model Performance
Model	MAPE	MAE	R² Score
Random Forest	2.11%	0.0138	0.99855
XGBoost	2.31%	0.0136	0.99893

➡️ XGBoost performed the best, achieving over 99% accuracy.

# 🛠️ Technologies Used

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

XGBoost

ucimlrepo (for dataset import)

# 🔧 Features

Full data cleaning (missing values, outliers, type conversion)

Datetime index creation

Feature engineering:

Hour, weekday, weekend

Rolling averages (3, 6, 12 intervals)

Lag features (1 hour, 24 hours)

Machine learning models

Model comparison and evaluation

# 🚀 How to Run
pip install -r requirements.txt
python notebook.ipynb

# 📁 Dataset

UCI Machine Learning Repository – Individual household electric power consumption
Loaded using:

from ucimlrepo import fetch_ucirepo
dataset = fetch_ucirepo(id=235)

📌 Conclusion

The project successfully demonstrates high-accuracy energy consumption forecasting. With R² scores above 0.998, both models are suitable for real-world applications like smart energy systems and demand prediction.
