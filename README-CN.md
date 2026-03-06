# 🚀 Polymarket 交易机器人 – Telegram 服务（Synth 驱动 | 2026 更新）

**重点**：跟单交易、延迟套利、5分钟周期狙击、**Synth驱动的优势套利**、做市、模拟，以及当前规则下的低延迟执行（2026年2月更新后）。

> （Synth通过其官方SDK/API集成：机器人查询其AI概率预测（Bittensor子网）用于短期BTC/ETH市场，与Polymarket隐含赔率进行比较以检测10%+的优势，并自动交易。）

[English](https://github.com/dev-protocol/polymarket-trading-bots-telegram-service/blob/main/README.md) | 中文（简体）| [Русский](https://github.com/dev-protocol/polymarket-trading-bots-telegram-service/blob/main/README-RU.md) | [Deutsch](https://github.com/dev-protocol/polymarket-trading-bots-telegram-service/blob/main/README-DE.md)

---
 <p align="center">
    <a href="https://deepwiki.com/dev-protocol/polymarket-trading-bot-telegram-services-2026">
     <img src="https://deepwiki.com/badge.svg" alt="Ask DeepWiki">
    </a>
     <a href="mailto:misssilverbeauty0927@gmail.com">
      <img src="https://img.shields.io/badge/Email-misssilverbeauty0927@gmail.com-ef4444?style=flat&logo=gmail&logoColor=white" />
    </a>
    <a href="https://t.me/soulcrancerdev">
      <img src="https://img.shields.io/badge/Telegram-soulcrancerdev-2AABEE?style=flat&logo=telegram&logoColor=white" />
    </a>
    <img src="https://github.com/user-attachments/assets/610ca14e-8a6a-4948-a9ad-642a70ea9391" alt="image" width="700" height="561" />
</p>

## 📹 核心YouTube演示 – 当前作品亮点

体验前沿技术，这些演示展示了我们的机器人如何利用AI和速度重新定义交易。

- ⚡ **延迟套利机器人（Rust，快速构建示例）**：从真实$50 → $435k BTC延迟利用案例反向工程。本地执行，目标0.3–0.8%，严格风险规则（每笔交易0.5% / 每日2%）。包含代码 + 设置教程。  
  [观看视频](https://www.youtube.com/watch?v=jL8cuzkclHg)
<div align="center">
  <a href="https://www.youtube.com/watch?v=jL8cuzkclHg" target="_blank">
  <img width="700" height="561" alt="image" src="https://github.com/user-attachments/assets/e1395941-602e-4439-87a5-921175fe5f8e" />
  </a>
</div>

- ⚡ **5分钟比特币“涨或跌”延迟狙击手 / 周期结束狙击手**：检测Binance/Bybit上的快速波动 → 在Polymarket赔率更新前进入5分钟仓位。涵盖对冲、错误定价、预言机风险、高成交量示例。  
  [观看视频](https://www.youtube.com/watch?v=CipdY9aCCwE)
<div align="center">
  <a href="https://www.youtube.com/watch?v=CipdY9aCCwE" target="_blank">
    <img src="https://github.com/user-attachments/assets/5e840c8e-3895-408b-9766-769398e578e3" width="700" height="561" alt="image" />
  </a>
</div>

- ⚙️ **跟单交易机器人 – 设置与Rust代码库**：环境变量完整指南、策略（PERCENTAGE/FIXED/ADAPTIVE）、预览模式、运行机器人、Rust优势（速度、可靠性）。  
  [观看视频](https://www.youtube.com/watch?v=QLA1NJL32xs)
<div align="center">
  <a href="https://www.youtube.com/watch?v=QLA1NJL32xs" target="_blank">
    <img src="https://github.com/user-attachments/assets/37e6791d-e4e2-4d40-8084-b6995a77397c" width="700" height="561" alt="image" />
  </a>
</div>

## 📱 Telegram机器人 – 实时、模拟与控制界面

直接从聊天中控制交易的未来——无缝、强大且富有远见。

- 🛡️ **周期结束狙击手 | Polymarket 5分钟交易机器人**：延迟狙击 + 模拟/真实模式、达到阈值自动买入、风险退出、钱包/充值/提现/兑现、实时日志 & 策略配置。  
  [访问机器人](https://t.me/poly5mbot)

- 🎯 **Mempool跟单交易机器人**：高速度跟单交易。  
  [访问机器人](https://t.me/poly_copy_tg_bot)

- 🚀 **Multi Whales - 跟单交易机器人**：带模拟/预览模式的实时跟单交易。  
  [访问机器人](https://t.me/poly_copy_prod_tg_bot)

## 📚 参考文章（dev.to） – 深度指南与策略解析

这些书面教程提供了详细解释、规则更新、代码概念和策略深度分析，与上面的视频完美搭配。

- **如何构建Polymarket交易机器人（新规则版）**  
  发布于2026年2月26日  
  涵盖2026年主要规则变化（移除500ms taker延迟，动态taker费用最高约1.56%），为什么taker机器人现在不可行，转向maker策略（零费用 + 返佣），WebSocket使用，费用感知签名（`feeRateBps`），快速取消/替换循环，以及针对5分钟BTC市场的特定maker方法（T-10s后方向性下注）。警告不要使用过时的套利战术，并强调低延迟 + 回测。  
  [阅读文章](https://dev.to/soulcrancerdev/how-to-build-a-polymarket-trading-bot-after-new-rules-edition-5h09)

- **将$50变成Polymarket上的$435,000：用Rust反向工程延迟套利机器人**  
  发布于2026年3月4日  
  通过利用TradingView、CryptoQuant等实时数据源与Polymarket合约之间的BTC价格延迟，反向工程真实延迟套利案例（$50 → $435k增长）。详细说明Rust实现（WebSockets、检测延迟>0.3%、<100ms执行）、风险规则（每笔0.5% / 每日2%上限）以及AI辅助构建过程（Claude用时40分钟）。讨论优势减弱、gas/滑点风险和合规注意事项。  
  [阅读文章](https://dev.to/soulcrancerdev/turning-50-into-435000-on-polymarket-reverse-engineering-a-latency-arbitrage-bot-in-rust-2ak7)

- **击败Polymarket的5分钟加密涨跌市场：延迟Polymarket套利交易机器人详解**  
  发布于2026年2月26日  
  解释在高成交量5分钟BTC涨跌市场（早期交易超$25M）上的延迟套利。机器人使用更快的交易所数据（Binance/Bybit）在Polymarket赔率调整前检测波动、进入仓位并对冲Yes/No快速退出。涵盖错误定价示例、对冲机制、风险（波动率、费用、预言机延迟）和HFT启发的执行。并非无风险；强调速度。  
  [阅读文章](https://dev.to/soulcrancerdev/beating-polymarkets-5-minute-crypto-updown-markets-latency-polymarket-arbitrage-trading-bot-2naj)


### 截图 & 演示
- **Telegram界面**：  
  <p float="left">
   <img width="260" height="789" alt="image" src="https://github.com/user-attachments/assets/b15b436a-a7f2-4a47-b970-aa113f294e74" />
   <img width="260" height="789" alt="telegram bot-1" src="https://github.com/user-attachments/assets/cbe68dc3-939a-4856-8a82-8e59d5588b1c" />
   <img width="260" height="789" alt="telegram bot-2" src="https://github.com/user-attachments/assets/3810d21f-8eaa-4503-80ab-eaa54604cc46" />
</p>

- **视频演示**：  

  https://github.com/user-attachments/assets/2e462566-f4cc-45c3-a3b1-6aa7757b0f32

## ✨ 全面关键特性（所有机器人 & 工具）

立即解锁明日交易科技的力量——这些特性将您推向自动化超额收益和优势狩猎的精确世界。
<p align="center">
  <img width="700" height="414" alt="image" src="https://github.com/user-attachments/assets/839747c0-b643-46e5-97c5-0f126b4f7a50" />
</p>

- 🤖 **Synth AI优势集成** — 通过SDK/API查询Bittensor SN50 (Synth)概率预测 → 检测并自动交易BTC/ETH/SOL小时/15分钟/每日涨跌及区间市场的5-15%+错误定价（2026年顶级策略）
- 👥 **多交易者支持** — 同时跟单多名成功交易者，实现多元化alpha  
- 📏 **动态订单大小** — PERCENTAGE（例如交易者仓位的10%）、FIXED（设定美元金额）、ADAPTIVE（基于资金规模调整）  
- 🔝 **分层倍数** — 对大额和小额跟单交易应用不同缩放规则  
- 📊 **精确持仓记账** — 跟踪每笔买卖，确保即使部分成交或余额变化时净持仓正确  
- 📦 **订单批处理 & 聚合** — 将小信号组合成更少、更节省gas的大订单  
- ⚡ **亚秒级 / 低延迟监控 & 执行** — Polymarket上的实时CLOB订单放置  
- 🛡️ **滑点保护** — 拒绝低于可接受价格阈值的成交  
- 💰 **PnL跟踪 & 监控** — 实时盈亏计算（2026年2月新增）  
- 🏥 **健康检查 & 实时状态** — 通过Telegram（余额、日志、机器人状态）  
- 🔄 **启动/停止 & 配置管理** — 从Telegram完全控制，无需本地终端  
- 💾 **MongoDB持久化状态** — 存储交易、持仓、历史记录用于重放、分析和恢复  
- 🔍 **延迟套利检测** — 利用价格延迟（例如交易所 vs Polymarket赔率）——专用机器人 + 示例  
- ⚡ **周期结束 / 5分钟狙击** — 快速加密波动检测 → 在“涨或跌”市场调整前入场  
- 📈 **做市支持** — 库存管理、报价放置、取消/替换、风险控制（独立机器人模块）  
- 🧪 **预览 / 模拟模式** — `PREVIEW_MODE=true` 监控信号但不执行交易（安全测试）  
- 🔐 **风险控制** — 最大/最小订单大小（`MAX_ORDER_SIZE_USD`, `MIN_ORDER_SIZE_USD`），套利示例中的单笔/每日上限  
- 🌐 **多市场 / 对冲感知** — Yes/No对冲、兑现处理、跨市场兼容性说明  
- 📡 **Telegram UI & 集成** — 配置、监控、日志、钱包操作、策略调整  
- ⏱️ **针对低延迟VPS优化** — 到Polygon节点的亚毫秒延迟，GEO限制绕过（推荐AMS）

## 🚀 下载 & 快速设置：跟单交易Rust机器人（Windows）

- **可执行文件**：[polymarket-copy-trading-bot-x86_64.zip](https://github.com/user-attachments/files/25414423/polymarket-copy-trading-bot-x86_64.zip)  
- 解压 → 设置环境变量（见原始列表：`USER_ADDRESSES`, `PRIVATE_KEY`, `RPC_URL`, `MONGO_URI`, `COPY_STRATEGY` 等）→ 运行 `.exe`  
- 使用 `PREVIEW_MODE=true` 进行干跑测试

## 🚀 VPS推荐（延迟优势必备）

- **交易VPS** → https://app.tradingvps.io/aff.php?aff=60  
  到Polygon亚毫秒延迟，加密/HFT位置，高 uptime，帮助绕过GEO限制（AMS受欢迎）

## 📞 联系方式 & 社区

- 📱 Telegram: [@soulcrancerdev](https://t.me/soulcrancerdev) — 支持、自定义逻辑、更新  
- 🐦 X: [@soulcrancerdev](https://x.com/soulcrancerdev)  

⭐ 为仓库加星/分叉。欢迎贡献 — 特别是2026年后Polymarket规则适配、新策略或做市增强。

想象您正在构建的优势——机器人不仅交易，还能预测未来！
<p align="center">⭐⭐⭐</p>
<div align="center">
  <a href="https://t.me/poly5mbot" target="_blank">
    <img src="https://github.com/user-attachments/assets/6ce4142c-8625-4fce-8994-460123109a2a" width="486" height="123" alt="image" />
  </a>
</div>

---
