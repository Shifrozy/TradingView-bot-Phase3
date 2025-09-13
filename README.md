# 📊 Multi-Factor TradingView Indicator

A custom **Pine Script v6** indicator that combines multiple technical signals into a unified scoring system with a polished **6-factor dashboard** and **Support/Resistance visualization**.

---

## ✨ Features
- ✅ **Multi-factor scoring system** with:
  - MACD (trend/momentum)
  - RSI (relative strength)
  - Volume analysis
  - Trend filter
  - ATR ratio (volatility filter)
  - Support & Resistance scoring
- ✅ **Visual dashboard** with color-coded scores (green = bullish, red = bearish).
- ✅ **Support/Resistance visualization** for quick decision making.
- ✅ **Configurable inputs** for flexible trading styles.
- ✅ **Optimized** with safe array handling and consistent indicator calls to avoid Pine Script runtime errors.
- ✅ Works on **any timeframe and market**.

---

## 🖥️ Dashboard Preview
The indicator displays a **6-factor dashboard** in the corner of your chart showing:
- Factor name
- Current value
- Bullish/Bearish color cue

---

## ⚡ Signals
- Buy/Sell signals are generated **only when multiple factors align** (not on every candle).
- Designed to avoid false signals by combining momentum, trend, volatility, and SR zones.

---

## 🔧 Inputs
- Toggle each factor **on/off** independently.
- Adjust lookback lengths (e.g., RSI length, ATR length).
- Dashboard positioning controls.

---

## 🚀 How to Use
1. Copy the script code from this repository.
2. Open **TradingView → Pine Editor**.
3. Paste the script, save, and click **Add to chart**.
4. Adjust inputs in the settings menu.

---

## 📌 Notes
- Built with **Pine Script v6**.
- Always test on **paper trading** before applying to live markets.
- The indicator is for **educational purposes only** and not financial advice.

---

## 🛠️ Developer Notes
- All `ta.*` functions are called **on each bar calculation** (per Pine best practices).
- Array operations (`array.get`, `array.set`) are wrapped with **bounds checks** to prevent runtime errors.
- History strings/maps are capped to prevent exceeding TradingView’s string length limit.
- Fully modular code: each factor has its own calculation function for easy modification.

---

## 📄 License
This project is licensed under the **MIT License** – free to use, modify, and distribute with attribution.
