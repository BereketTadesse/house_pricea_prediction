# 🏡 House Price Prediction using Linear Regression

## 📌 Overview
This project predicts **house prices** using a **Linear Regression** model trained on key housing features. To improve model performance, a **log transformation** is applied to the target variable `SalePrice` to handle skewness. The pipeline also includes preprocessing steps to handle missing values.

---

## 📊 Features Used

The following features are used for predicting house prices:

- **GrLivArea**: Above-ground living area (square feet)
- **BsmtFullBath**: Basement full bathrooms
- **BsmtHalfBath**: Basement half bathrooms
- **FullBath**: Full bathrooms above grade
- **HalfBath**: Half baths above grade
- **BedroomAbvGr**: Bedrooms above grade (excludes basement)

---

## 🔧 Data Preprocessing

### ✅ Missing Values
- No missing values in the **training dataset**
- Rows with missing values in the **test dataset** were removed

### ✅ Target Variable Transformation
- Applied `np.log1p()` to `SalePrice` to normalize skewed distribution
- Used `np.expm1()` to convert model predictions back to actual price scale

### ✅ Train-Test Split
- 80% Training data, 20% Testing data
- Random state fixed for reproducibility

---

## 🤖 Model Details

- **Algorithm**: Linear Regression (via `scikit-learn`)
- **Evaluation Metrics**:
  - Mean Squared Error (MSE)
    
---

## 🚀 How to Use

### 🛠️ Clone the Repository
```bash
git clone https://github.com/BereketTadesse/house_pricea_prediction.git
cd house_pricea_prediction
```

### 📚 Dependencies
- Python 3.6+
- pandas
- numpy
- scikit-learn
- scipy
- matplotlib

### ▶️ Run the Jupyter Notebook
```bash
jupyter notebook house_price_prediction.ipynb
```
---

**Happy Predicting! 🎉**
