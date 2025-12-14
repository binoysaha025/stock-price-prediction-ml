# stock-price-prediction-ml
Stock price forecasting using Monte Carlo simulation and Linear Regression ML model with 95% R² accuracy on AAPL data

# Stock Price Prediction: Monte Carlo Simulation & Machine Learning

A comprehensive stock price forecasting project implementing both statistical simulation and supervised machine learning approaches with train/test validation.

## Project Overview

This project explores two different methodologies for stock price prediction:
1. **Monte Carlo Simulation** - Statistical approach using random sampling based on historical volatility
2. **Linear Regression Model** - Supervised machine learning with sliding window feature engineering

Both models are validated using train/test split methodology and evaluated on Apple Inc. (AAPL) historical stock data.

## Features

### Monte Carlo Simulation
- Simulates 10,000 possible future price paths
- Generates confidence intervals (5th, 50th, 95th percentiles)
- Visualizes uncertainty in predictions
- Based on historical mean returns and volatility

### Linear Regression Model
- Sliding window feature engineering (5-day lookback)
- Train/test split validation (80/20)
- Achieved **R² score of 0.95** on test data
- Comprehensive performance metrics (RMSE, MAE, R²)

## 📊 Results

### Monte Carlo Simulation
- Provides probabilistic forecasts with confidence intervals
- Captures market uncertainty through 10,000 simulated scenarios
- Useful for risk assessment and scenario analysis

### Linear Regression Model
- **Test R² Score:** 0.9509
- **Test RMSE:** $3.30 
- **Test MAE:** $2.49 
- Successfully predicts next-day prices with 95% variance explained

## 🛠️ Technologies Used

- **Python 3.9+**
- **Libraries:**
  - `yfinance` - Financial data acquisition
  - `numpy` - Numerical computing
  - `pandas` - Data manipulation
  - `matplotlib` - Data visualization
  - `scikit-learn` - Machine learning algorithms

## 📁 Project Structure
```
├── monte_carlo_simulation.py    # Monte Carlo implementation
├── linear_regression_model.py   # ML model implementation
├── requirements.txt             # Dependencies
└── README.md                    # Project documentation
```

## 🔧 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/stock-price-prediction.git
cd stock-price-prediction
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## 💻 Usage

### Monte Carlo Simulation
```python
python monte_carlo_simulation.py
```
Generates 10,000 price simulations and visualizes confidence intervals.

### Linear Regression Model
```python
python linear_regression_model.py
```
Trains ML model and displays prediction accuracy metrics.

## Methodology

### Monte Carlo Approach
1. Calculate historical daily returns and volatility
2. Use normal distribution to generate random future returns
3. Simulate 10,000 possible price paths
4. Aggregate results to show confidence intervals

### Machine Learning Approach
1. Feature engineering with 5-day sliding window
2. Train/test split (80/20) for validation
3. Linear regression model training
4. Performance evaluation on unseen test data

## Key Learnings

- Time series forecasting techniques
- Statistical modeling vs machine learning approaches
- Train/test validation methodology
- Feature engineering for financial data
- Model evaluation metrics (RMSE, MAE, R²)

## Visualizations

The project generates multiple visualizations:
- Monte Carlo simulation paths with confidence bands
- Train/test split timeline
- Scatter plots for prediction accuracy

## Future Improvements

- [ ] Add more technical indicators as features
- [ ] Implement LSTM neural network for comparison
- [ ] Expand to multiple stocks
- [ ] Real-time prediction dashboard
- [ ] Incorporate sentiment analysis from news data

## 📝 License

MIT License - feel free to use this project for learning purposes.

## 👤 Author

**Binoy Saha**
- GitHub: https://github.com/binoysaha025
- LinkedIn: https://www.linkedin.com/in/binoysaha025/

## Acknowledgments

- Data sourced from Yahoo Finance via yfinance API
- Inspired by quantitative finance methodologies
