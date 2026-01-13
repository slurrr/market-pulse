# Data Sources

## Active
- **Binance Spot WebSocket**
  - URL: `wss://stream.binance.com:9443/ws/btcusdt@trade`
  - Purpose: Real-time price, trade volume, aggressive buy/sell classification.
  - Latency: Low (~100-300ms depending on client).
- **Binance Futures WebSocket**
  - URL: `wss://fstream.binance.com/ws/btcusdt@aggTrade`
  - Purpose: Perpetual futures data for Basis and CVD Divergence (Spot vs Perp analysis).

## Candidates (Not implemented)
- **Coingecko API**: For dominance/market cap data (too slow for pulse?).
- **Hyperliquid / DyDx**: For perp funding rates (critical for "Inventory" question in vision.md).
