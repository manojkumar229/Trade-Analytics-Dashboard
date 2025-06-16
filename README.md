## 📈 Project: Opening Range Breakout (ORB) Strategy Backtest & Power BI Dashboard

### 📌 Objective
Backtest a trading strategy (ORB) on intraday stock data and analyze its performance using Power BI.

### 💡 Strategy Rules
- Use first 5-minute candle of each day to set the breakout range
- **Buy** if price crosses above the high
- **Sell** if price drops below the low
- Target: +0.5% | Stop Loss: -0.25% | Exit time: 15:15 if no outcome
- One long and one short trade per symbol per day

### 📂 Python Script Features
- Read and group intraday 5-min stock data from `.csv`
- Calculate breakout levels and detect trade triggers
- Log trade entries and exits with reasons
- Output a detailed trade log with PnL, timestamps, and performance metrics

### 📊 Power BI Dashboard Features
- Used trade log output from Python
- Added calculated columns:
  - Trade count per day
  - Weekday
  - Cumulative PnL
  - Holding duration
  - Entry hour
- Created KPIs:
  - Total PnL, Win/Loss ratio, Expectancy, Avg Win/Loss
- Built interactive visuals:
  - Cumulative PnL line chart
  - Win vs Loss pie chart
  - PnL heatmap by hour
  - Top winning/losing trades
  - Exit reason distribution

### 🧰 Tools Used
- Python (pandas, NumPy)
- Power BI (DAX, calculated columns, visualizations)
