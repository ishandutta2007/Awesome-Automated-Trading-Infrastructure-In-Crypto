# Awesome-Automated-Trading-Infrastructure-In-Crypto

# Top Automated Trading Infrastructure in Crypto Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Market Making, Execution Engines & Algorithmic Trading Frameworks*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Automated Trading Infrastructure in Crypto**. These tools enable trading firms, market makers, and quantitative traders to build, backtest, and deploy automated strategies across centralized and decentralized exchanges—with institutional-grade execution, risk controls, and multi-exchange connectivity.

**Examples** include Hyperliquid, dYdX, Uniswap, GMX, Wintermute, Flowdesk, GSR, Aevo, Vertex Protocol, and Orderly Network (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom strategy development, and open execution infrastructure—ideal for quantitative traders, market makers, and developers seeking transparent, vendor-independent trading systems.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Hyperliquid](https://hyperliquid.xyz/)**  
  Decentralized perpetual exchange with fully on-chain order book. Features sub-second finality, zero gas fees, and native API for market makers. Supports up to 100x leverage on perpetual futures with deep liquidity.

- **[dYdX](https://dydx.exchange/)**  
  Leading decentralized derivatives exchange. v4 runs on Cosmos SDK with off-chain order book and on-chain settlement. Features cross-margining and institutional-grade APIs.

- **[Uniswap](https://uniswap.org/)**  
  Largest decentralized exchange by volume. v4 introduces hooks for custom AMM logic. Provides SDK for programmatic trading and liquidity provision.

- **[GMX](https://gmx.io/)**  
  Decentralized perpetual and spot exchange on Arbitrum and Avalanche. Features zero price impact trades, oracle-based pricing, and multi-asset pools.

- **[Wintermute](https://www.wintermute.com/)**  
  Leading algorithmic market maker providing liquidity across CEX and DEX venues. Offers OTC trading, derivatives, and treasury management services.

- **[Flowdesk](https://flowdesk.co/)**  
  Full-service digital asset trading and market making firm. Provides liquidity provision, execution algorithms, and treasury solutions for token issuers.

- **[GSR](https://www.gsr.io/)**  
  Crypto market maker and liquidity provider with proprietary trading technology. Offers programmatic trading, OTC options, and structured products.

- **[Aevo](https://aevo.xyz/)**  
  Decentralized options and perpetuals exchange built on OP Stack. Features portfolio margining, RFQ system, and institutional-grade infrastructure.

- **[Vertex Protocol](https://vertexprotocol.com/)**  
  Cross-margin DEX with unified order book for spot, perpetuals, and money markets. Features on-chain risk engine and sub-second finality.

- **[Orderly Network](https://orderly.network/)**  
  Omnichain liquidity infrastructure providing unified order book across multiple chains. Offers SDK for building DEX frontends with shared liquidity.

## Open-Source GitHub Projects

- **[Hummingbot](https://github.com/hummingbot/hummingbot)**  
  The leading open-source, institutional-grade crypto trading framework (Apache-2.0). Running in production since 2019 with 50+ exchange connectors actively maintained. Features **standardized interfaces** across all exchanges, **multi-instance deployment** (hundreds of bots on one server via Docker isolation), **shared market data connections** for efficiency, and **automatic reconnection** with fill reconciliation . Supports CEX spot/perpetual (Binance, Coinbase, Kraken, Hyperliquid, dYdX) and DEX via Gateway (Uniswap, Jupiter, Raydium) . **Self-hosted with no custody**—your keys never leave your infrastructure . 10,000+ Discord members and monthly releases . The **Condor AI harness** enables agentic strategies where LLMs analyze markets while deterministic infrastructure handles execution and risk limits .

- **[Freqtrade](https://github.com/freqtrade/freqtrade)**  
  Free, open-source crypto trading bot (GPL-3.0) with **53,000+ GitHub stars** as of August 2026 . The most feature-rich open-source bot framework: **web UI**, **Telegram integration**, **Hyperopt** for strategy optimization, and **100+ exchange support** via CCXT . **FreqAI** ships inside Freqtrade for machine learning trade signals with **background retraining**—supports LightGBM, XGBoost, CatBoost, and any Python ML library, plus reinforcement learning via stable-baselines3 . Battle-tested by thousands of traders on Binance, OKX, Gate.io, and KuCoin . **Note**: Default RL reward function is a showcase, not production-ready—badly trained agents find "cheats" without winning trades .

- **[Jesse](https://github.com/jesse-ai/jesse)**  
  Advanced crypto trading framework (MIT) emphasizing **clean strategy syntax** and **realistic backtesting** . Strategy code is readable Python classes—no pandas DataFrame mental model required . **Backtesting engine accounts for position sizing, realistic fees, partial fills, price slippage, and multi-timeframe data** without lookahead bias requiring configuration . Multi-timeframe analysis is native and elegant . **Exchange support is more limited** than Freqtrade (growing), and no web UI or Telegram integration out of the box . Best for developers prioritizing code clarity and trustworthy backtest results.

- **[NautilusTrader](https://github.com/nautechsystems/nautilus_trader)**  
  Open-source algorithmic trading platform (LGPL-3.0) with **Rust core and Python API** . **Same strategy code runs for backtesting and live trading**—eliminating backtest-to-live divergence . **25,000+ GitHub stars** . Listed as a developer framework by Kraken for building custom bots .

- **[OctoBot Market Making](https://github.com/Drakkar-Software/OctoBot-Market-Making)**  
  Open-source market-making strategy automation software (GPL-3.0) based on OctoBot . Supports **15+ exchanges** including Binance, MEXC, Bitmart, Hyperliquid, CoinEx, and KuCoin . Designed to **improve crypto market liquidity** by reducing bid-ask spread, enabling large trades, and ensuring fair market price . Features **configurable order book design** (number of bids/asks, price range), **automatic order replacement** on fill, and **arbitrage protection** using reference price from more liquid exchange . **Paper trading** mode for strategy testing before live deployment . Self-custody with no third-party trust .

- **[CCXT](https://github.com/ccxt/ccxt)**  
  Unified trading API library (MIT) supporting **100+ crypto exchanges** in JavaScript, TypeScript, Python, C#, PHP, Go, Java, and Rust . **44,000+ GitHub stars** . Provides **56 unified capabilities, 18 watch* methods, and standardized interfaces** across exchanges . **Rate limiter on by default** (unlike some exchange SDKs) and automatic reconnection handling . The **foundation for most open-source trading bots** including Freqtrade and Hummingbot .

- **[OpenSQT Market Maker](https://github.com/dennisyang1986/opensqt_market_maker)**  
  High-performance, low-latency crypto market maker in Go (license varies) . **Millisecond-level response** with full WebSocket-driven market data and order flow—no polling delays . Features **smart grid strategy** with Super Slot system for managing concurrent orders, **proactive risk control** monitoring K-line volume anomalies, **automatic reconciliation** syncing local and exchange state, and **high-concurrency architecture** (Goroutine + Channel + Sync.Map) . Supports Binance, Bitget, Gate.io, Bybit, and backpack . Claims $100M+ traded with $3M daily volume on ETHUSDC .

- **[ADAMANT Tradebot](https://github.com/adamant-im/adamant-tradebot)**  
  Free, self-hosted market-making software for token issuers (license varies) . **No third-party access to exchange API keys** and **no token or fund transfer** to external market maker . Features initial order book filling, dynamic order book building, spread maintenance, price range settings, and reference price/arbitrage logic across pairs . Management via **ADAMANT Messenger** (secure command-based control without public admin panel) . Free version supports Azbit, P2PB2B, StakeCube, Coinstore, FameEX, and NonKYC .

- **[PQTS (Protheus Quant Trading System)](https://pypi.org/project/pqts/)**  
  Open-source quant trading system (license varies) with **PnL truth ledger + strategy auto-disable list** . Features multi-market, multi-strategy simulation suites with optimization telemetry, **shadow parity + operational SLO flow** (market/order/fill parity telemetry, reconciliation daemon with auto-halt on mismatch), **execution drift reports**, and **incident automation** with Telegram/Discord notifications . Runs in engine, API, or stream modes .

### Additional Strong Open-Source Options

- **[NautilusTrader](https://github.com/nautechsystems/nautilus_trader)** — Rust-core execution engine with Python API (LGPL-3.0) .
- **[Lean (QuantConnect)](https://github.com/QuantConnect/Lean)** — Algorithmic trading engine (Apache-2.0) supporting Python and C# .
- **[Backtrader](https://github.com/mementum/backtrader)** — Python backtesting library (GPL-3.0) .
- **[cryptofeed](https://github.com/bmoscon/cryptofeed)** — WebSocket data feed handler for crypto exchanges (MIT) .
- **[barter-rs](https://github.com/barter-rs/barter-rs)** — Rust framework for event-driven live-trading and backtesting .
- Community **n8n** workflows for trading signal routing and portfolio alerting.

**Frameworks for building custom systems**: Combine **Hummingbot** for multi-exchange execution and market making with **Freqtrade + FreqAI** for ML-driven strategies, **Jesse** for realistic backtesting, **CCXT** for unified exchange connectivity, and **OpenSQT** for high-frequency grid strategies—creating a fully self-hosted, institutional-grade automated trading platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Automated trading systems handling capital and API keys must follow security best practices (key isolation, least privilege, audit logging) and comply with applicable financial regulations.
- **Star count measures interest, not capability.** The most-starred AI trading repos (TradingAgents with 96K+ stars, ai-hedge-fund with 62K+) **do not place live orders**—they simulate and backtest . Only FreqAI (inside Freqtrade) and NautilusTrader execute live crypto trades among the top ML-focused repos .
- **Backtesting realism varies significantly.** Jesse's engine is trustworthy out of the box; Freqtrade's requires careful configuration to avoid lookahead bias . Always validate strategies against live paper trading before deploying capital.
- **Self-hosted means you own the risk.** Hummingbot, Freqtrade, and OctoBot keep keys on your infrastructure—no custody risk, but installation, updates, and key security are your responsibility . Self-hosted open-source solutions require proper security hardening, server maintenance, and ongoing strategy development.

---

**Made for quantitative traders, market makers, crypto funds, and developers building transparent trading infrastructure.**  
Let's make Automated Trading Infrastructure in Crypto more open, data-driven, and reliable.
