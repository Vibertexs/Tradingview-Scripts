## 📊 NNFX-Inspired Indicator Development

This repository is inspired by the **No Nonsense Forex (NNFX)** algorithmic trading approach developed by VP. NNFX is a rule-based, mechanical system that removes emotion and guesswork from trading. Instead of relying on discretionary setups or popular retail patterns, it builds a complete strategy from tested components—each with a specific role.

The goal of this repository is to **tune existing public indicators or create new ones** that fit into the NNFX framework. While I'm actively working toward building a successful automated system, the tools and concepts here are made available to help anyone who comes across this project.

---

### 🧠 NNFX Theory – Core Principles

The NNFX method is built on six essential components:

1. ### 🟦 Baseline  
   A trend-detecting indicator (usually a moving average).  
   **Rule**: Only take trades in the direction of the trend.  
   Examples: EMA, ZEMA, HMA, DEMA

2. ### ✅ Confirmation Indicator  
   Confirms entries in the direction of the trend.  
   Should be **non-price-based** — often momentum, volatility, or rate-of-change indicators.  
   Examples: CCI, MACD, WAE, DSS, custom oscillators

3. ### 📏 ATR (Average True Range)  
   Used strictly to calculate **Stop Loss (SL)** and **Take Profit (TP)** levels based on market volatility.  
   Typical settings: SL = 1×ATR, TP = 1.5×ATR (customizable)

4. ### ⛔ Exit Indicator *(optional but recommended)*  
   Allows early exit if the trade shows signs of reversal or weakening.  
   Examples: RSI cross, fast momentum drop, structure break

5. ### 🔊 Volume Filter  
   Not true tick volume, but a proxy to detect **bad market conditions** like low liquidity or false moves.  
   Helps avoid entries in dead or dangerous zones (like the Asian session).  
   Examples: WAE, CMF, market session filters

6. ### ⚠️ News Filter  
   Avoids entering or holding trades near **high-impact news events** (like NFP, CPI, FOMC).  
   Can be manual or integrated with an API/calendar.

---

### 🧪 What This Repo Offers

This repository contains:
- Modified public indicators that are **optimized for algorithmic use**
- Custom-built tools like **ATR-ZEMA bands**, **trend filters**, and **volume-adjusted indicators**
- Experimentation with **risk-adjusted momentum**, **adaptive baselines**, and **entry/exit logic**

I'm working to test and combine these components into a full NNFX-style bot. Even though I may not release the final strategy itself, the tools here are free for others to use, study, and build their own systems.

---

### 💡 Goals

- Help traders **build rules-based algorithms** without emotional or inconsistent decisions  
- Provide tools that integrate seamlessly into the **NNFX structure**  
- Encourage experimentation with **less common indicators** and data-driven testing

---

### 🤝 For You

If you’re trying to build your own algo, this repo can serve as a base or inspiration. I hope the indicators and logic here help you create a strategy that’s clean, logical, and built to last.

