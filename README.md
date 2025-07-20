# **🚘 Used Car Price Prediction with Machine Learning**

This project uses real-world used car data to predict selling prices based on multiple features like brand, engine size, mileage, and more. Through robust data cleaning, feature engineering, and model building, we achieved a strong R² score of 0.92+ using Random Forest Regression 🌲

-----------------------------------------------
## **🧰 Tech Stack**
Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost (optional)

Modeling: Random Forest Regressor

EDA & Visualization: Pairplots, Heatmaps, Scatterplots

Tools: Jupyter Notebooks, pickle for saving models

------------------------------------------------
## **🧠 Objective**
Predict the selling price of used cars based on:

🚙 Car brand and model

⛽ Fuel type

⚙️ Transmission type

🛞 Engine capacity & mileage

🧍 Owner count and seller type

📅 Year of manufacture
------------------------------------------------
## **🔍 Dataset Overview**

📁 Source: Kaggle

📊 Rows: 8,128

🧾 Features: 13

🛠️ Format: .csv
------------------------------------------------
## **⚙️ Workflow Summary**

✅ 1. Data Preprocessing
Cleaned string fields (e.g. mileage, engine, max_power) by removing units and converting to numeric types.

Removed the torque column due to messy and inconsistent formatting.

Filled or dropped missing values where appropriate.

Encoded categorical columns:

Car brand (name)

Fuel type

Transmission type

Seller type

Ownership history
------------------------------------------------
🧹 2. Feature Engineering
Extracted brand from the car name using .str.split().

Converted fuel efficiency (mileage) to numeric.

Mapped brands to integer codes for model compatibility.
------------------------------------------------
📈 3. Exploratory Data Analysis
Used sns.pairplot() to explore feature relationships.

Correlation heatmap to identify the strongest predictors of price.

Identified top contributing features: year, mileage, max_power, engine.
------------------------------------------------
🧪 4. Modeling
Split into training (80%) and test (20%) sets.

Scaled features using StandardScaler.

Built a Random Forest Regressor (sklearn.ensemble).

Trained and evaluated model performance.
------------------------------------------------
## **📊 Results**
Metric	Value
R² Score	0.93 🚀
Mean Squared Error (MSE)	0.0568 📉

A strong fit indicating the model can reliably estimate car prices based on feature inputs.

📉 Visual Evaluation
📌 Actual vs Predicted Plot
(If saved)
Visually confirmed predictions align closely with actual values using a scatterplot.
