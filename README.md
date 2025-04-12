# 🏠 Bengaluru House Price Prediction

A Machine Learning project that uses real housing data from Bengaluru to predict property prices. This project walks through a full end-to-end ML pipeline — from data cleaning and feature engineering to model selection and evaluation — and is ideal for anyone interested in real-world data science applications.

---

## 📌 Project Overview

This project tackles the classic regression problem: **predicting housing prices** based on various features such as square footage, number of BHKs, location, and more. The dataset was preprocessed, cleaned, and optimized before training a Linear Regression model.

### ✅ Key Objectives
- Perform exploratory data analysis (EDA)
- Handle missing data and outliers
- Engineer relevant features like `BHK`, `price_per_sqft`, and `location_group`
- Build and evaluate a regression model
- Deploy a clean and ready-to-use prediction pipeline

---

## 🧠 Technologies Used

- **Python**
- **Pandas**, **NumPy** – for data manipulation
- **Matplotlib**, **Seaborn** – for visualization
- **Scikit-learn** – for model building and evaluation

---

## 📊 Dataset

- `bengaluru_house_prices.csv`
- Contains features like:
  - `location`
  - `size` (e.g., 2 BHK)
  - `total_sqft`
  - `bath`
  - `price`

---

## 🧹 Data Cleaning & Feature Engineering Highlights

- Removed irrelevant columns (`area_type`, `society`, etc.)
- Converted non-numeric `total_sqft` values to numeric using custom parsing
- Created new features like:
  - `bhk` (number of bedrooms)
  - `price_per_sqft`
  - Grouped rare locations as `other`
- Removed outliers (e.g., extremely high `price_per_sqft`, inconsistent BHK/sqft ratios)

---

## 📈 Model Building

- **Linear Regression** was used as the final model due to its high interpretability and strong baseline performance.
- Model evaluated using:
  - Cross-validation
  - R² Score
  - Error analysis on test data

---

## 🧪 Sample Predictions

> Predicting the price for a 3 BHK house in JP Nagar with 2000 sqft:
```python
model.predict([[2000, 3, 3, 'JP Nagar']])
```

---

## 💡 Future Improvements

- Implement advanced ML models such as **Random Forest**, **XGBoost**, or **Gradient Boosting** for improved accuracy.
- Deploy the model using **Flask**, **FastAPI**, or **Streamlit** to allow users to interact with it via a web interface.
- Integrate **geospatial visualization** (e.g., using Folium or Plotly) to show pricing heatmaps across Bengaluru.
- Add **automated EDA reports** using tools like Ydata Profiling or Pandas Profiling.
- Incorporate **real-time data updates** or API integrations for current listings.
- Develop a **mobile-friendly frontend** for easy accessibility.

---

## 👨‍💻 Author

**Dhairy Tilva**  
📧 dhairyown@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/dhairy-tilva-ab35a71aa/) • [GitHub](https://github.com/DhairyTilva)

---

## 🏁 License

This project is open-source and available under the MIT License.

---

> If you found this project helpful or insightful, feel free to ⭐ star this repo and connect with me on GitHub!

