# ZeusView — Pro Crypto Terminal

<div align="center">

![ZeusView Logo](favicon.svg)

**The most advanced AI-powered crypto trading terminal on the web.**
ترمینال حرفهای هوش مصنوعی ترید کریپتو — قدرتمندترین ابزار تحلیل و معامله در بازارهای مالی.

[🚀 Live Demo / نسخه زنده](https://zeusview-9jxw.arcada.app/)
|
[📖 Requirements / مشخصات فنی](ZeusView-Requirements.md)
|
[💬 Community / انجمن](https://t.me/ZeusView)

---

### 🌟 Key Highlights

| Feature | Description |
|---|---|
| 📊 **TradingView-grade Charts** | Candle, Heikin-Ashi, Line, Area, OHLC, Base line + custom timeframes |
| 🤖 **Zeus AI Copilot** | 38 trader personas, multilingual analysis, long-term memory |
| 💰 **Paper Trading** | Live simulated trading with Bybit data — no real risk |
| ⚡ **Bybit WebSocket** | Real-time quotes, order book depth, live trades |
| 📜 **ZeusScript Editor** | Pine Script–style strategy coding with IntelliSense |
| 🔔 **Smart Alerts** | Price, indicator, conditional alerts → Telegram notifications |
| 🌍 **Multi-market** | Crypto, Forex, Commodities, Iranian market (Rial, Gold, Stocks) |

</div>

---

## 🗺️ Table of Contents / فهرست مطالب

| Section / بخش | Link / لینک |
|---|---|
| 📊 Charts & Technical Analysis | #charts-and-technical-analysis |
| 🌍 Markets | #markets |
| 🤖 Zeus AI | #zeus-ai |
| 📜 Strategy & Backtest | #strategy-editor |
| 💰 Paper Trading | #paper-trading |
| 🔔 Alerts & Telegram | #alerts |
| 📰 Market Info | #market-info |
| 👥 Community | #community |
| ⚙️ Customization | #customization |
| 🛠️ Tech Stack | #tech-stack |
| 📐 Architecture | #architecture |
| 🌐 Global SEO | #global-seo |

---

## 📊 Charts and Technical Analysis / چارت و تحلیل تکنیکال

<div align="center">

```
           CANDLE          HEIKIN-ASHI          LINE
          ████                ██                 ────
         ████               ████                █████
        ██████             ██████              ████████
       ████████           ████████            ██████████
```

</div>

**Chart Types / انواع چارت:**
- Candlestick (OHLC) / کندل استیک
- Heikin-Ashi / هایکن آشی
- Line / خطی
- Area / ناحیه‌ای
- Bar / میله‌ای (OHLC)
- Baseline / خط پایه

**Timeframes / تایم‌فریم‌ها:**
- Standard: 1m, 3m, 5m, 15m, 30m, 1H, 4H, 1D, 1W, 1M
- Custom: any interval (e.g., 7min, 45min)
- Replay: step-by-step historical replay at adjustable speed

**Indicators / اندیکاتورها:**

| Category | Indicators |
|---|---|
| Trend | EMA, SMA, Supertrend, ADX |
| Momentum | RSI, Stochastic, MACD, CCI |
| Volatility | Bollinger Bands, Keltner Channels, ATR |
| Volume | OBV, VWAP, Volume Profile, MFI |
| Drawing Tools | Trendline, Support/Resistance, Fibonacci (Retracement, Extension, Spiral, Circle, Fan), Gann Fan/Box, Elliott Waves, XABCD Pattern, Head & Shoulders, Pitchfork, Rectangle, Channel |

**Smart Assistant / دستیار هوشمند زئوس:**
Automatic chart analysis in Farsi with your preferred trading style.

---

## 🌍 Markets / بازارها

| Market / بازار | Symbols / نمادها |
|---|---|
| Bybit Futures & Spot | BTCUSDT, ETHUSDT + hundreds |
| Binance Futures & Spot | All USDT pairs |
| Forex & Commodities | XAUUSD (Gold), EURUSD, GBPUSD, USDJPY, DXY, USOIL |
| Indices / شاخص‌ها | SPX500, NAS100, DJI |
| Iran Market / بازار ایران | USDIRR (Dollar), Gold 18K, Coin Bahar Azadi, TEDPIX, Tehran Stock Exchange |

**Data Feeds / جریانات داده:**
- Crypto: Real-time WebSocket streaming (quotes, order book depth, live trades)
- Forex / Iran: Update every few seconds via REST polling

---

## 🤖 Zeus AI — Zeus Copilot / هوش مصنوعی زئوس

### Capabilities / قابلیت‌ها

| Feature | Detail |
|---|---|
| Comprehensive Analysis | Technical + News + Sentiment in one report |
| 38 Trader Personas | Jerome Levy, Soros, Gann, ICT, Wyckoff, Livermore, etc. |
| Long-term Memory | Suggestions improve with experience — predictions scored against real prices |
| Chat Panel | Direct conversation with Zeus beside the chart |
| Multi-language | Farsi (primary), English, Arabic, Türkçe, Español, Deutsch, Français, Chinese, Japanese, Hindi, Russian |
| AI Paint on Chart | Draw any shape including Fibonacci Spiral directly on chart |
| Telegram Alerts | "When X happens, alert me on Telegram" |

### How Personas Work / عملکرد پرسوناها

```
User selects persona → AI adopts that trader's methodology →
Generates analysis using their specific rules →
Outputs actionable signals with reasoning
```

**Example Personas / مثال پرسوناها:**
- **Soros** — Reflexivity theory, macro themes
- **Gann** — Geometric angles, time cycles, square of 9
- **Wyckoff** — Accumulation/distribution phases
- **ICT** — Order blocks, fair value gaps, liquidity sweeps
- **Livermore** — Price action, pivot points, tape reading

---

## 📜 Strategy Editor / ادیتور استراتژی

### ZeusScript + Python

ZeusScript is a Pine Script–compatible language with extended features:

```javascript
// Example: Golden Cross Strategy / مثال استراتژی تقاطع طلایی
strategy("Golden Cross", overlay=true)

fast = ema(close, 9)
slow = ema(close, 21)

crossup = crossover(fast, slow)
crossdown = crossunder(fast, slow)

if (crossup)
    strategy.entry("Long", strategy.long)

if (crossdown)
    strategy.close("Long")

// Backtest output includes:
// Net Profit, Win Rate, Max Drawdown, Sharpe Ratio, Trade Count
```

**IntelliSense Features / قابلیت‌های هوشمند:**
- Syntax highlighting / رنگ‌آمیزی سینتکس
- Auto-complete (Ctrl+Space) / تکمیل خودکار
- Function signature hints / راهنمای امضای توابع
- Auto-close brackets / بستن خودکار براکت
- Line-by-line error detection / خطایابی خطی

**Strategy Tester Output / خروجی تست استراتژی:**
- Net Profit / سود خالص
- Total Trades / تعداد معاملات
- Win Rate / وینریت
- Max Drawdown / حداکثر افت سرمایه
- Sharpe Ratio / نسبت شارپ
- Profit Factor / ضریب سود

**Bar Replay / بازپخش میله‌ای:**
Step through past candles at any speed to practice strategies.

---

## 💰 Paper Trading / معامله شبیه‌سازی‌شده

| Feature | Description |
|---|---|
| Market Orders | Execute at current price |
| Limit Orders | Set target entry price |
| Leverage | Adjustable leverage (1x–125x) |
| Virtual Account | Simulated balance starting at $10,000 |
| Position Management | Close position, cancel order, view P&L in real-time |

**Why Paper Trade? / چرا معامله مجازی؟**
Practice strategies without risking real capital. Track performance across months and refine your approach before going live.

---

## 🔔 Alerts & Telegram / هشدارها و تلگرام

**Alert Types / انواع آلارم:**
1. **Price Alert** — Above/below a specific price
2. **Indicator Alert** — RSI cross, MACD crossover, volume spike
3. **Conditional Alert** — Any ZeusScript condition (`when RSI > 70 and volume > avg`)

**Telegram Integration / اتصال تلگرام:**
Link your Telegram bot → receive instant push notifications when alerts trigger. Works worldwide.

---

## 📰 Market Info / اطلاعات بازار

| Feature | Description |
|---|---|
| Live News | CoinDesk, Reuters, The Block, CryptoSlate |
| Market Screener | Top gainers/losers, highest volume, funding rates |
| Web Search | Research any topic directly within ZeusView via Zeus AI |

---

## 👥 Community / کامیونیتی

- **Telegram-style channels** — Discuss trades, share ideas
- **"TradeGram" feed** — Instagram-like social feed for charts and analysis screenshots
- **User profiles** — Public profiles showing track record and shared charts
- **Chart sharing** — One-click export with drawings and annotations

---

## ⚙️ Customization / شخصی‌سازی

| Feature | Description |
|---|---|
| Watchlist | Save your favorite symbols |
| Layout Presets | Save & restore chart layouts with one click |
| Side Panels | Toggle Watchlist, Order Book, Alerts, Screener, News, Trading panels |
| Theme | Dark theme by default (configurable light/dark) |

---

## 🛠️ Tech Stack / لایه‌های فنی

```
Frontend          React 19 + TypeScript + Tailwind CSS v4
Charts            Lightweight Charts (TradingView fork) + custom Canvas renderer
Real-time Data    Bybit WebSocket API + Binance WebSocket API
AI Engine         OpenAI API / oxalpha.com internal API
Strategy Engine   ZeusScript JIT compiler (TypeScript) + Python subprocess
Authentication    GitHub OAuth + Google OAuth
Deployment        arcada.app CDN + Vercel edge functions
Database          PostgreSQL (user data) + Redis (caching)
Notifications     Telegram Bot API + Web Push
Community         Real-time WebSocket chat (Telegram-style)
```

---

## 📐 Architecture / معماری

```
┌─────────────────────────────────────────────────────┐
│                    Frontend (React)                  │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌────────┐ │
│  │  Chart   │ │  Zeus AI │ │ Strategy │ │Market │ │
│  │ Renderer │ │ Copilot  │ │  Editor  │ │Widgets│ │
│  └────┬─────┘ └────┬─────┘ └────┬─────┘ └───┬────┘ │
│       │             │             │            │     │
│  ┌────▼─────────────▼────────────▼────────────▼───┐ │
│  │           State Management (Zustand)           │ │
│  │           Real-time WebSocket Layer            │ │
│  └────────────────────┬───────────────────────────┘ │
└───────────────────────┼─────────────────────────────┘
                        │
            ┌───────────▼───────────┐
            │     API Gateway       │
            │  (Vercel Edge)        │
            └───────┬───────┬───────┘
                    │       │
      ┌─────────────▼─┐ ┌──▼─────────────┐
      │  Bybit/Binance │ │  AI Services   │
      │  WebSocket     │ │  (OpenAI/OG)   │
      └────────────────┘ └────────────────┘
```

---

## 🌐 Global SEO — Multilingual Keywords

### English
```
crypto trading terminal, professional trading platform, Bybit API, 
TradingView alternative, free charting tool, paper trading simulator,
crypto backtesting, Pine Script editor, AI trading assistant,
technical analysis software, cryptocurrency trading bot,
live crypto charts, bybit futures trading, ethereum trading,
bitcoin analysis tool, crypto screener, trading alerts telegram,
smart money concepts, ICT trading, Wyckoff method, 
Gann analysis tool, Fibonacci spiral chart, trading strategy backtest
```

### فارسی (Persian)
```
ترمینال ترید کریپتو, ترمینال حرفهای ارز دیجیتال, نمودار معاملاتی,
تحلیل تکنیکال رایگان, ترید شبیه ساز, آموزش ترید, پلتفرم معاملاتی,
ابزار تحلیل بیت کوین, اندیکاتورهای تریدینگ ویو, استراتژی ترید,
بکتست استراتژی, هوش مصنوعی ترید, مشاور معاملاتی, صرافی باینت,
فیوچرز باینت, اسپات ترید, ابزار فیبوناچی, حمایت مقاومت,
RSI MACD, میانگین متحرک, اسکالپ, سوئینگ ترید, پرایس اکشن,
اسمارت مانی SMC, ای سی تی ICT, وایکف, جیم گن, تریدگرام
```

### العربية (Arabic)
```
منصة تداول عملات رقمية,Terminal تداول احترافي,تداول بيتكوين,
تحليل فني,أدوات تداول بالعملات الرقمية,محاكي تداول مجاني,
اختبار استراتيجيات التداول,مؤشرات التداول,ذكاء اصطناعي للتداول,
منصة باینس,由乙方期货交易,التحليل الفني للعملة الرقمية,
تداول الفوركس,منصة ميتاتريد alternativa,Indicadores técnicos,
TradingView alternativa,Fibonacci retracement,مؤشر RSI,
تداول منظم,استراتيجية تداول
```

### Español
```
terminal de trading cripto, plataforma profesional de trading,
gráficos en tiempo real, trading simulado, backtesting estrategias,
asistente IA trading, indicadores técnicos, análisis criptomonedas,
Bitcoin trading, Forex trading, Bybit API, simulador de trading gratis,
herramientas análisis técnico, scrypt pine equivalent, trading alerts
```

### Deutsch
```
Krypto-Trading-Terminal, professionelle Handelsplattform,
technische Analyse, Paper-Trading-Simulator, Backtesting-Strategien,
KI-Trading-Assistent, Bitcoin-Charts, Indikatoren, Bybit Trading,
Algorithmischer Handel, Trading-Strategie testen, Finanzmarkt-Analyse
```

### Français
```
terminal de trading crypto, plateforme de trading professionnelle,
graphiques en temps réel, trading simulé, backtest stratégie,
assistant IA trading, analyse technique, indicadores, Bybit API,
simulateur de trading gratuit, signaux trading, plateforme française
```

### 中文 (Chinese)
```
加密货币交易终端,专业交易平台,实时图表分析,纸交易模拟器,
策略回测,AI交易助手,技术指标,Bybit API,比特币分析工具,
自由交易模拟器,量化交易策略,技术分析软件,加密货币交易所
```

### 日本語 (Japanese)
```
暗号資産取引ターミナル,プロフェッショナル取引プラットフォーム,
リアルタイムチャート,ペーパートレーディング,バックテスト戦略,
AIトレーディングアシスタント,テクニカル指標,Bitcoin分析ツール,
Bybit API,仮想通貨取引,定量分析,トレード戦略
```

### हिन्दी (Hindi)
```
क्रिप्टो ट्रेडिंग टर्मिनल, प्रोफेशनल ट्रेडिंग प्लेटफॉर्म,
रियल-टाइम चार्ट्स, पेपर ट्रेडिंग सिमुलेटर, बैकटेस्ट स्ट्रैटेजी,
एआई ट्रेडिंग असिस्टेंट, तकनीकी संकेतक, बायबिट एपीआई,
क्रिप्टोकरेंसी ट्रेडिंग, शेयर बाजार विश्लेषण
```

### Türkçe (Turkish)
```
kripto trading terminali, profesyonel trading platformu,
gerçek zamanlı grafikler, kağıt trading simülatörü,
strateji backtest, yapay zeka trading asistanı,
teknik göstergeler, Bitcoin analizi, Bybit API,
kripto para trading, alım satım stratejisi
```

### Русский (Russian)
```
криптобиржевой терминал, профессиональная торговая платформа,
технический анализ, симулятор торговли, бэктест стратегий,
ИИ-ассистент для трейдинга, индикаторы, криптовалюты,
бизнес-терминал, торговля биткоином, Bybit API, трейдинг
```

---

## 🏷️ Meta Tags (for HTML head)

```html
<title>ZeusView — Pro Crypto Trading Terminal | AI Charts & Paper Trading</title>
<meta name="description" content="ZeusView is the most advanced open-source crypto trading terminal featuring TradingView-grade charts, AI copilot with 38 trader personas, paper trading, ZeusScript strategy editor, and real-time Bybit data. Free to use.">
<meta name="keywords" content="crypto trading, bybit api, tradingview alternative, paper trading, backtesting, ai trading assistant, zeusscript, pine script, technical analysis, crypto charts, smart money concepts, ict trading, wyckoff, gann, fibonacci, trading alerts telegram">
<meta property="og:title" content="ZeusView — Pro Crypto Trading Terminal">
<meta property="og:description" content="Advanced AI-powered crypto trading terminal with live Bybit data, TradingView-grade charts, 38 trader personas, paper trading, and ZeusScript strategy editor.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://zeusview-9jxw.arcada.app/">
<meta name="twitter:card" content="summary_large_image">
<meta name="robots" content="index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1">
<link rel="canonical" href="https://zeusview-9jxw.arcada.app/">
```

---

## 📄 Open Graph Image (Suggested)

Generate a cover image for social sharing at `1200×630px`:
- Dark background (#0b0e14)
- Gold star logo (from favicon.svg) centered
- Text: **"ZeusView — Pro Crypto Terminal"**
- Subtitle: **"AI Charts · Paper Trading · ZeusScript"**
- Export as `og-image.png` and upload to repo root

---

## 📜 License / مجوز

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

## 🙋 Contributing / مشارکت

Contributions welcome! Please read [ZeusView-Requirements.md](ZeusView-Requirements.md) before submitting PRs.

---

<div align="center">

**ZeusView** · Built with ❤️ by [morindok](https://github.com/morindok)  
🌐 [Live Demo](https://zeusview-9jxw.arcada.app/) · 📖 [Requirements](ZeusView-Requirements.md)

</div>
