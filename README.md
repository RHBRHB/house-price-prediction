# 🏠 House Price Prediction — Data Cleaning

Cleaned the Kaggle House Prices dataset as the first step toward building a price prediction model.

---

## 📊 Dataset

- **Source:** Kaggle — House Prices: Advanced Regression Techniques
- **Rows:** 1,460
- **Original Columns:** 81
- **Target Variable:** SalePrice

---

## 🧹 What I Did

### 1. Handled Missing Values
- Dropped columns with **>50% missing** (Alley, PoolQC, Fence, MiscFeature, MasVnrType)
- Filled numeric columns with **median**
- Filled categorical columns with **mode**

### 2. Capped Outliers
- Used **IQR method** (1.5x rule)
- Capped: LotArea, GrLivArea, TotalBsmtSF, GarageArea

### 3. Engineered 7 New Features

| Feature | Description |
|---------|-------------|
| TotalSF | Total square footage (living + basement + garage) |
| HouseAge | Age of the house (2026 - YearBuilt) |
| YearsSinceRemodel | Years since last remodel |
| PricePerSF | Price per square foot (SalePrice / TotalSF) |
| TotalBath | Total bathrooms (full + half) |
| TotalPorchSF | Total porch area |
| IsRenovated | 1 if remodeled, else 0 |

---

## 📂 Files

- `cleaned_house_prices.csv` — Cleaned dataset ready for modeling
- `house_price_cleaning.ipynb` — Full Jupyter notebook with all steps

---

## 🚀 Next Steps

- Train ML models (Random Forest, XGBoost)
- Deploy a Streamlit app

---

## 🛠️ Tools Used

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- Google Colab

---

## 👨‍💻 Author

[RHB]
