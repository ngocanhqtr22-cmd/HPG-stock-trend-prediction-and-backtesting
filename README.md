# HPG Stock Trend Prediction and Backtesting

LSTM-based binary classification model predicting HPG stock trend 
(up/not-up) on Vietnam's stock market. Built during internship at 
DSC Securities – Da Nang Branch.

## Results
| Metric | LSTM Strategy | Buy & Hold |
|--------|--------------|------------|
| ROI | 42.36% | 25.42% |
| Sharpe Ratio | 2.15 | 0.40 |
| Max Drawdown | -7.19% | -28.04% |

## Model Overview
- Binary classification: predict if HPG closes higher next session
- 16 technical features across 4 groups: return & momentum, 
  technical oscillators, price-to-trend ratios, volatility & money flow
- Validation: Walk-Forward Validation (5 folds)
- Backtesting: includes real transaction costs (0.25%)

## Data
- HPG historical price: 2,801 sessions (2015–2026)
- Source: Investing.com

## Tech Stack
- Python, TensorFlow/Keras, Pandas, NumPy
- Jupyter Notebook

## Author
Le Thi Ngoc Anh – Fintech, University of Economics Da Nang  
