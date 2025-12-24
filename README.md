# AutoTrade-MT4/5 🚀

---

## ⚙️ Features
- 💰 **Auto-Compound Lot Sizing** — dynamically adjusts position size based on account balance.
- 🎯 **Configurable Risk & Reward** — default: Risk 10%, R:R 1:2 (+20% target).
- 🧭 **Multiple Entry Signals**
  - MA Cross
  - FVG (Fair Value Gap)
  - OB (Order Block)
- 🧩 **Optional ATR-based Stop Loss**
- 📈 **Compatible with Prop Firm rules** (risk management oriented)
- **Many settings for trading strategies**

---

## 🧮 Pengaturan kunci (dibagian `"current"`):
| Kunci | Nilai Standart | Description |
|------------|----------|-------------|
| `rapid_fire_mode` | `true` | mengaktifkan pemeriksaan cepat _multi-symbol/multi-timeframe_. |
| `dynamic_lot_sizing` | `true` | Menghitung lot berdasarkan risiko per _trade_. |
| `risk_percent_per_trade` | `1.0` | Persentase saldo yang dipertaruhkan per _trade_ (digunakan dalam lot dinamis). |
| `max_total_positions` | `10` | Jumlah maximum _trade_ yang dibuka secara bersamaan. |
| `max_daily_trades` | `100` | Jumlah maximum _trade_ yang diizinkan dalam 1 hari. |
| `auto_close_target` | `0.4` | Profit dalam USD yang memicu _Auto_Close_. |

---

## 💻 How to use:

### Step 1: Update your terminal
```bash
sudo apt update && sudo apt upgrade -y
````
---

### Step 2: Clone the Bot Repository

```bash
git clone https://github.com/Gizmocryp/bot_tradeMT5.git
cd bot_tradeMT5
```

---

### Step 3: Install requirement

```bash
pip install requirements.txt
```

---

### Step 4: Create Your `.env` File

Inside `bot_tradeMT5` folder, run:

```bash
nano .env
```

Paste your wallet details:
```
# MT5 Account Configuration
MT5_LOGIN=
MT5_PASSWORD=
MT5_SERVER=
MT5_PATH=

# Trading Settings
RISK_PER_TRADE=0.01
MAX_DAILY_TRADES=10

# API Keys (if needed)
EXNESS_API_KEY=your_api_key
EXNESS_SECRET_KEY=your_secret_key
```
**Save & Exit**: `CTRL + X`, then `Y`, then `ENTER`

---

## 🚀 Running the Bot

Run Script:

```bash
pyhton main.py
```
