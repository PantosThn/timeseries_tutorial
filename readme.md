## 📈 timeseries_103: Advanced Forecasting Techniques

In this section, we explore multiple advanced modeling approaches for time series forecasting, from traditional statistical models to modern machine learning techniques.

### Feature Engineering

A crucial step before applying ML models is transforming the raw time series into a format that these algorithms can learn from. We perform:
- Extraction of time-based features (e.g., day of week, month, holiday indicators)
- Lag features and rolling statistics (moving averages, standard deviations)
- Encoding cyclical patterns using sine and cosine transformations
- Train/test splits based on time rather than random sampling

These engineered features turn the time series into a supervised learning problem, allowing us to use algorithms that are not inherently designed for sequential data.

---

### Forecasting Models Covered

#### 1. **SARIMAX (Seasonal ARIMA with eXogenous variables)**
A classical statistical approach that handles:
- Seasonality
- Trend
- Exogenous variables

SARIMAX is interpretable and works well for linear time series, but struggles with complex nonlinear patterns.

#### 2. **Facebook Prophet**
Prophet provides an intuitive way to model:
- Trend shifts
- Seasonality (daily, weekly, yearly)
- Holidays/special events

It’s great for business forecasting with minimal tuning, and supports uncertainty intervals.

#### 3. **Gradient Boosting Algorithms**

We transform the time series into a tabular format and apply powerful ensemble algorithms:

- **LightGBM**
- **XGBoost**
- **CatBoost**

These models can capture nonlinear relationships and interaction effects between features. When paired with proper feature engineering, they often outperform traditional methods in real-world settings.

#### 4. **Scikit-learn Models**
We also experiment with standard machine learning models from `sklearn`, such as:
- Linear Regression
- Ridge and Lasso Regression
- Random Forest Regressor

These serve as baselines and demonstrate how classical ML models compare to more complex boosting techniques.

---

### 🎯 Takeaway

This part of the tutorial bridges the gap between traditional forecasting and modern ML techniques. It shows that with the right feature engineering, even non-sequential models can yield highly accurate time series forecasts.
