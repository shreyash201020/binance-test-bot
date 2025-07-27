# 🔁 Binance Testnet Trading Bot

A simplified Python-based trading bot that can place **market** and **limit** orders on the **Binance USDT-M Futures Testnet** using the official Binance API.

## 📌 Features

* ✅ Place **market** and **limit** orders
* ✅ Supports both **buy** and **sell** sides
* ✅ Command-Line Interface (CLI) for user interaction
* ✅ Logs all API calls and errors
* ✅ Configurable with `.env` file
* ✅ Modular & clean structure
* 🏆 Bonus-ready: Easy to extend for Stop-Limit, TWAP, OCO, or a simple GUI

---

## 🧩 Requirements

* Python 3.7+
* Binance Futures Testnet account
* API Key & Secret (from testnet)

---

## 🛠 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/shreyash201020/binance-test-bot.git
cd binance-test-bot
```

### 2. Set up a Virtual Environment (optional but recommended)

```bash
python -m venv venv
venv\Scripts\activate   # On Windows
# OR
source venv/bin/activate  # On macOS/Linux
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔐 Environment Configuration

1. Create a `.env` file in the root directory.

```bash
touch .env
```

2. Add your API credentials and base URL:

```env
API_KEY=your_testnet_api_key
API_SECRET=your_testnet_api_secret
BASE_URL=https://testnet.binancefuture.com
```

> ⚠️ You must register at [Binance Futures Testnet](https://testnet.binancefuture.com/) and generate your keys under the **USDT-M Futures** section.

---

## 🚀 How to Run

```bash
python main.py
```

You'll see a prompt:

```text
Welcome to Binance Testnet Trading Bot
Enter order type (market/limit): 
```

Follow the prompts to place your order:

* Choose order type: `market` or `limit`
* Choose side: `buy` or `sell`
* Enter symbol: `BTCUSDT`, `ETHUSDT`, etc.
* Enter quantity: e.g., `0.001`
* If limit order, enter price too

Example interaction:

```
Enter order type (market/limit): market
Enter symbol (e.g., BTCUSDT): BTCUSDT
Enter side (buy/sell): buy
Enter quantity: 0.001
```

---

## 📁 Project Structure

```
binance-test-bot/
│
├── main.py                 # Entry point
├── trading_bot.py          # Core trading logic
├── config.py               # Environment and API setup
├── utils.py                # Logging and helpers
├── .env                    # API credentials (not pushed to GitHub)
├── requirements.txt        # Required libraries
└── README.md               # Project documentation
```

---

## 📄 Log Files

* All API requests, responses, and errors are logged in `bot.log`.

Example entry:

```
2025-07-27 10:30:41 - INFO - Market buy order placed: {'orderId': ..., 'status': 'FILLED'}
```

---

## 🧪 Testnet Trading Dashboard

Use this to verify your trades visually:

🔗 [https://testnet.binancefuture.com/en/futures/BTCUSDT](https://testnet.binancefuture.com/en/futures/BTCUSDT)

---

## 🧠 Bonus Ideas (Optional)

Add one or more of the following to stand out:

* Stop-limit or OCO orders (`client.create_oco_order`)
* TWAP/Grid algorithmic order
* Frontend using Flask or Tkinter
* Auto-cancel stale orders
* Risk management (e.g., stop loss)

---

## 📬 Submit Your Work

Send your:

* ✅ GitHub repo link
* ✅ Log file (`bot.log`)
* ✅ Resume (optional)

To:

```
📧 saami@bajarangs.com  
📧 nagasai@bajarangs.com  
📧 chetan@bajarangs.com  
CC ➤ sonika@primetrade.ai  
```

Subject: **"Junior Python Developer – Crypto Trading Bot"**

---

## 👨‍💻 Author

**Shreyash Chaudhari**
GitHub: [shreyash201020](https://github.com/shreyash201020)
