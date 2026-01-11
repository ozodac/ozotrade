# OZO Trade - Options Auto Trader

## 🚀 Quick Start - Deploy to GitHub Pages

### Step 1: Create GitHub Repository
1. Go to https://github.com
2. Click "New" (green button, top left)
3. Repository name: `ozotrader` or `ozo-trade`
4. Select: **Public**
5. Click "Create repository"

### Step 2: Upload Files
1. On your new repository page, click "uploading an existing file"
2. Drag and drop BOTH files:
   - `index.html` (Original version)
   - `aggressive.html` (More trades version)
3. Click "Commit changes"

### Step 3: Enable GitHub Pages
1. Click "Settings" tab (top right of your repo)
2. Click "Pages" in the left sidebar
3. Under "Source": Select **"main"** branch
4. Click "Save"
5. Wait 1-2 minutes for deployment

### Step 4: Access Your Live Trader!

Your apps will be available at:

**Original Version:**
```
https://YOUR-USERNAME.github.io/ozotrader/
```

**Aggressive Version (More Trades):**
```
https://YOUR-USERNAME.github.io/ozotrader/aggressive.html
```

*Replace YOUR-USERNAME with your actual GitHub username*

---

## 📊 Version Differences

### 🎯 index.html - **Original** (Recommended for Real Trading)
- **Momentum Threshold:** 0.15%
- **Short Momentum:** 0.08%
- **Volatility:** 0.01%
- **Expected Trades:** 15-30 per month
- **Best For:** Conservative, high-quality setups
- **Risk Profile:** Lower (waits for clear signals)

### ⚡ aggressive.html - **Aggressive** (Good for Testing/Slow Markets)
- **Momentum Threshold:** 0.10% (33% easier to trigger)
- **Short Momentum:** 0.05% (38% easier)
- **Volatility:** 0.005% (50% easier)
- **Expected Trades:** 30-50 per month
- **Best For:** Testing, slow market days, learning
- **Risk Profile:** Higher (more trades = more opportunities + more risk)

---

## ⚙️ How to Use

### First Time Setup:
1. Open your deployed GitHub Pages link
2. Click "⚙️ Settings"
3. Choose **SPY** or **SPX**
4. (Optional) Add Tradier Sandbox API key for real broker testing
5. Adjust risk settings if desired (default 2% is safe)
6. Click "Save Settings"

### Start Trading:
1. Click "▶ Start Trading" (green button)
2. Wait 2-3 minutes for data collection
3. First trade should appear within 5-30 minutes (during market hours)

### Market Hours:
- **US Market:** 9:30 AM - 4:00 PM EST (6:30 AM - 1:00 PM PST)
- **Best Time:** First hour (9:30-10:30 AM) and last hour (3:00-4:00 PM)
- Algorithm works best when SPY moves 1%+ per day

---

## 🔧 Tradier Sandbox Setup (Optional)

To test with REAL broker API (fake money):

1. Sign up: https://developer.tradier.com/user/sign_up
2. Verify email
3. Go to "My Applications" → "Create Application"
4. Copy your **Sandbox API Token**
5. Paste into Settings in OZO Trade
6. Now you'll get real options chains and pricing!

---

## 📈 Understanding the Dashboard

**Balance:** Starting $100,000 (simulated)
**Total P&L:** Your profit/loss
**SPY/SPX Price:** Current market price (updates every 5 seconds)
**Win Rate:** % of profitable trades
**Market Trend:** BULLISH (buy calls), BEARISH (buy puts), or NEUTRAL (wait)

**Active Position:**
- Shows when you have an open trade
- Displays real-time P&L
- Exits automatically at profit target (+50%), stop loss (-50%), or time limit (5 min)

---

## 🔬 Backtest Feature

Click "🔬 Backtest" to simulate 30 days of trading:
- Uses historical price patterns
- Shows total trades, win rate, profit factor
- **Profit Factor > 1.5:** Excellent strategy
- **Profit Factor > 1.0:** Profitable
- **Profit Factor < 1.0:** Needs adjustment

---

## ⚠️ Important Notes

### This is PAPER TRADING:
- ✅ Great for learning and testing
- ✅ No real money at risk
- ✅ See how the algorithm performs
- ❌ NOT connected to real brokerage account
- ❌ Profits are simulated (for testing only)

### To Trade with REAL Money:
1. Test thoroughly in simulation (weeks/months)
2. Verify consistent profitability
3. Sign up for Tradier LIVE account (not sandbox)
4. Deposit real money ($5,000+ recommended)
5. Switch to LIVE API key in settings
6. Start with small position sizes
7. **RISK WARNING:** Options can lose 100% of investment

---

## 🎯 Strategy Overview

**What This Algorithm Does:**
1. Analyzes SPY/SPX price movement every 10 seconds
2. Calculates momentum, moving averages, volatility
3. When conditions align → Buys CALL (if bullish) or PUT (if bearish)
4. Exits at +50% profit, -50% loss, or 5-minute time limit
5. Uses 2% of balance per trade (professional risk management)

**It's NOT AI/Machine Learning:**
- Fixed mathematical rules
- No learning or adaptation
- Same logic every time

**Optimization:**
- Originally: Too few trades (6.4/month)
- Optimized: More trades (15-30/month) while maintaining quality
- Aggressive: Even more trades (30-50/month) for testing

---

## 📞 Support

Having issues? Check:
1. ✅ Are you using it during US market hours? (9:30 AM - 4:00 PM EST)
2. ✅ Is the price updating every 5 seconds?
3. ✅ Press F12 → Console tab → Any red errors?
4. ✅ Did market move at least 0.15% today? (SPY needs volatility)

**Slow market day = Few/No trades** (This is GOOD - algorithm waits for quality setups)

---

## 📝 File Descriptions

- `index.html` - Original OZO Trade (0.15% thresholds)
- `aggressive.html` - Aggressive OZO Trade (0.10% thresholds)
- `README.md` - This file

---

## 🚀 Ready to Deploy!

Follow the steps at the top of this README to get OZO Trade live on GitHub Pages in under 5 minutes!

**Your personal trading dashboard will be accessible 24/7 from anywhere!**

---

Built with ❤️ by OZO • Powered by React, Tailwind CSS, Yahoo Finance API, Tradier API
