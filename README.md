# 🧠 FX Strategy: From Macro Signals to ML-Driven Positioning

This repository showcases a project combining macroeconomic intuition with machine learning techniques to build adaptive, risk-aware FX trading strategies — designed at daily frequency and structured to be interpretable, scalable, and testable.

---

## 🚀 Project Highlights

- **Macro-Informed Features**: Incorporates interest rate differentials and technical indicators (RSI, EMA, momentum).
- **Machine Learning Signals**: Binary classifiers (Random Forests) generate directional forecasts.
- **Volatility-Aware Position Sizing**: Dynamically sizes positions based on rolling volatility.
- **Confidence-Based Filtering**: Trades only when model confidence exceeds a threshold (e.g. 0.60).
- **Risk Management**: Includes ATR-based stop-loss logic and daily max drawdown caps.
- **Modular Design**: Easily extendable to other assets, features, or ML models.

---

## 📈 Strategy Variants

### 1. **Baseline Approach**
- Feature set includes macro + technical indicators
- Random Forest classifier used across currency pairs
- Daily returns computed via signal * volatility-adjusted weights

### 2. **Confidence Threshold Experiment**
- Runs the same pipeline with different thresholds: 0.55 vs 0.60
- Demonstrates the effect of **small tuning changes** on cumulative performance
- Animation and plots included for visualization

---

## 📊 Key Insights

- Even modest adjustments to confidence filtering (0.55 → 0.60) significantly alter the strategy’s cumulative returns and Sharpe Ratio.
- Model outputs are only useful when filtered through volatility and confidence — otherwise, the signals resemble noise.
- Not a high-frequency strategy: operates on daily close data, more suitable for macro overlays or asset allocation frameworks.

---

## 🛠️ Tools & Stack

- **Python**: Data manipulation and modeling
- **Pandas / NumPy**: Time series operations
- **Matplotlib**: Visualization & animation
- **scikit-learn**: ML modeling (Random Forests)
- **yfinance**: FX data retrieval
- **Colab / Jupyter**: Development environment

---

## 📂 Files

- `fx_strategy_baseline.ipynb` – first version with macro-informed ML
- `fx_strategy_conf_threshold.ipynb` – includes confidence sweep and comparison
- `fx_strategy_comparison.gif / .mp4` – optional animation showing live performance divergence
- `README.md` – this file

---

## 🔍 Future Work

- Incorporate macro regime-switching models (e.g., hidden Markov, economic surprise indices)
- Walk-forward or cross-validation frameworks for more robust testing
- Integrate alternative ML models (e.g., LightGBM, ensemble stacks)
- Use risk budgeting techniques (e.g., CVaR, Kelly optimization)

---

## 💬 Let’s Connect

If you're working in **quant research, systematic macro, or data-driven trading** — or you're hiring — feel free to connect!

> "In research, even a 1% improvement isn’t small — it’s a new edge."

---

**Keywords:** `quant research`, `FX trading`, `machine learning`, `systematic macro`, `volatility targeting`, `confidence thresholds`, `portfolio construction`, `financial ML`, `alpha engineering`
