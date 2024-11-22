# **Diamond Price Prediction Using EDA and Regression Models**

## **Overview**
This project aims to analyze and predict diamond prices based on their intrinsic features such as carat, cut, color, clarity, and other attributes. Using exploratory data analysis (EDA) and regression modeling, we uncover insights about the factors influencing diamond prices and build predictive models.

---

## **Dataset**
The dataset contains information about diamonds, including their physical and quality characteristics. Key features include:

- **carat:** Weight of the diamond.
- **cut:** Quality of the diamond's cut (e.g., Fair, Good, Very Good, Premium, Ideal).
- **color:** Diamond color grade, from D (best) to J (worst).
- **clarity:** Clarity of the diamond (e.g., IF, VVS1, VVS2, SI1).
- **depth:** Total depth percentage (z / mean(x, y)).
- **table:** Width of the top of the diamond relative to the widest point.
- **price:** Price of the diamond in USD (target variable).

The dataset is available in `data/raw_data.csv`.

---

## **Steps Taken**
### 1. **Exploratory Data Analysis (EDA)**
- Visualized data distribution and outliers.
- Analyzed correlations between features using a heatmap.
- Explored relationships between features (e.g., carat vs. price) using scatter plots.

### 2. **Data Preprocessing**
- Converted categorical features to numerical values using Label Encoding.
- Handled outliers using interquartile range (IQR) filtering.
- Standardized and normalized the dataset using `StandardScaler` and `MinMaxScaler`.

### 3. **Dimensionality Reduction**
- Applied Principal Component Analysis (PCA) to reduce feature redundancy while retaining variance.

### 4. **Regression Modeling**
- Built regression models to predict diamond prices.
- Evaluated models using metrics like R² and Mean Squared Error (MSE).

---

## **Key Findings**
- **Carat weight** is the most influential feature for predicting diamond prices, with a strong positive correlation.
- Premium-quality diamonds (Ideal cuts) command higher prices, but their influence is secondary to carat weight.
- PCA reduced the dataset to fewer dimensions, retaining over 95% of the original variance.

---
## **How to Run the Project**
### **1. Clone the Repository**
```bash
git clone https://github.com/username/diamond-price-prediction-eda.git
cd diamond-price-prediction-eda
```

### **2. Install Dependencies**
Ensure you have Python installed, then install the required libraries:
```bash
pip install -r requirements.txt
```

---

## **Requirements**
The project uses the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `joblib`
- `jupyter`

Install all dependencies with:
```bash
pip install -r requirements.txt
```

---


---

## **Contributing**
Contributions are welcome! If you have suggestions or improvements, feel free to open an issue or submit a pull request.

---

## **License**
This project is licensed under the [MIT License](LICENSE).

---
