# ZeusView — Pro Crypto Terminal

<div align="center">

![ZeusView Logo](favicon.svg)

**The most advanced AI-powered crypto trading terminal on the web.**
ترمینال حرفهای هوش مصنوعی ترید کریپتو — قدرتمندترین ابزار تحلیل و معامله در بازارهای مالی.

[🚀 Live Demo / نسخه زنده](https://zeusview-9jxw.arcada.app/)
|
[📖 Requirements / مشخصات فنی](ZeusView-Requirements.md)

</div>

---

## 🌟 Key Highlights

| Feature | Description |
|---|---|
| 📊 **TradingView-grade Charts** | Candle, Heikin-Ashi, Line, Area, OHLC + custom timeframes |
| 🤖 **Zeus AI Copilot** | 38 trader personas, multilingual analysis, long-term memory |
| 💰 **Paper Trading** | Live simulated trading with Bybit data — no real risk |
| ⚡ **Bybit WebSocket** | Real-time quotes, order book depth, live trades |
| 📜 **ZeusScript Editor** | Pine Script–style strategy coding with IntelliSense |
| 🔔 **Smart Alerts** | Price, indicator, conditional alerts → Telegram notifications |
| 🌍 **Multi-market** | Crypto, Forex, Commodities, Iranian market (Rial, Gold, Stocks) |

---

## 📊 Charts & Technical Analysis / چارت و تحلیل تکنیکال

**Chart Types:** Candlestick, Heikin-Ashi, Line, Area, Bar, Baseline

**Timeframes:** 1m – 1M + custom intervals + historical replay

**Indicators:**
- Trend: EMA, SMA, Supertrend, ADX
- Momentum: RSI, Stochastic, MACD, CCI
- Volatility: Bollinger Bands, ATR
- Volume: OBV, VWAP, Volume Profile
- Drawing: Fibonacci (Retracement, Spiral, Circle, Fan), Gann, Elliott Waves, XABCD, Pitchfork, Support/Resistance

**Smart Assistant:** Automatic chart analysis in Farsi with your preferred trading style.

---

## 🌍 Markets / بازارها

| Market | Symbols |
|---|---|
| Bybit Futures & Spot | BTCUSDT, ETHUSDT + hundreds |
| Binance Futures & Spot | All USDT pairs |
| Forex & Commodities | XAUUSD (Gold), EURUSD, USDJPY, DXY, USOIL |
| Indices | SPX500, NAS100 |
| Iran Market | USDIRR, Gold 18K, Coin Bahar Azadi, TEDPIX, Tehran Stock Exchange |

---

## 🤖 Zeus AI — هوش مصنوعی زئوس

| Feature | Description |
|---|---|
| Comprehensive Analysis | Technical + News + Sentiment in one report |
| 38 Trader Personas | Soros, Gann, ICT, Wyckoff, Livermore and more |
| Long-term Memory | Predictions scored against real prices, improves over time |
| Chat Panel | Direct conversation with Zeus beside the chart |
| Multi-language | فارسی، English، العربية، Türkçe، Español، Deutsch، Français，中文，日本語，हिन्दी，Русский |
| AI Paint on Chart | Draw Fibonacci Spiral and any shape directly on chart |
| Telegram Alerts | "When X happens, alert me on Telegram" |

---

## 📜 Strategy Editor / ادیتور استراتژی

Write strategies in **ZeusScript** (Pine Script–style) or **Python** with full IntelliSense:

```javascript
// Golden Cross Strategy
strategy("Golden Cross", overlay=true)
fast = ema(close, 9)
slow = ema(close, 21)
if (crossover(fast, slow))
    strategy.entry("Long", strategy.long)
```

**Backtest output:** Net Profit, Win Rate, Max Drawdown, Sharpe Ratio

---

## 💰 Paper Trading / معامله شبیهسازیشده

Market & Limit orders · Leverage up to 125x · Virtual $10,000 account · Real-time P&L

---

## 🔔 Alerts & Telegram / هشدارها و تلگرام

Price alerts · Indicator crossovers · Conditional alerts via ZeusScript · Push notifications to Telegram

---

## 📰 Market Info / اطلاعات بازار

Live news from CoinDesk, Reuters, The Block · Market screener (top gainers/losers, funding rates) · Built-in web search via Zeus AI

---

## 👥 Community / کامیونیتی

Telegram-style channels · TradeGram social feed · Public user profiles · One-click chart sharing

---

## ⚙️ Customization

Watchlist · Layout presets (save & restore) · Toggleable side panels (Order Book, Alerts, Screener, News, Trading)

---

<div align="center">

**ZeusView** · Built with ❤️ by [morindok](https://github.com/morindok)  
🌐 [Live Demo](https://zeusview-9jxw.arcada.app/)

</div>
