# Decisions

## 001. Architecture: Single File HTML/JS
- **Context**: Need to move fast, architecture doesn't matter, "throwaway" code.
- **Decision**: No build step, no framework (React/Vue/etc), just vanilla HTML5 + WebSocket.
- **Reason**: instant feedback loop, zero config, easier to just "open and run".

## 002. Data Source: Binance WebSocket
- **Context**: Need real-time "pulse".
- **Decision**: Connect directly to `wss://stream.binance.com:9443/ws/btcusdt@trade` in the client.
- **Reason**: Public, free, high fidelity, no API key needed for basic market data.

## 003. Initial Metrics
- **Decision**: Focus on Price, Velocity (10s change), Tape Speed (TPS), and Aggression (Buy/Sell Vol Ratio).
- **Reason**: These are the rawest units of "what is happening right now".

## 004. Regime Logic
- **Decision**: Define "Impulse" as high velocity + matched delta direction. Define "Absorption" as velocity opposing delta.
- **Reason**: Simple heuristic to detect if price is moving easily or fighting headwinds.

## 005. Market Pulse v0.6 Expansion (Situational Awareness)
- **Decision**: Shifted to a 3x3 Grid Layout.
  - **Why**: The single-column view was insufficient for monitoring multi-dimensional market state (Liquidity, Structure, Rotation) simultaneously.
- **Decision**: Added Binance Futures WebSocket (`fstream`).
  - **Why**: Spot data alone cannot detect leverage-driven moves or absorption. Comparing Spot CVD vs Perp CVD is a critical signal for "fake" vs "real" moves.
- **Decision**: Implemented "Liquidity Proxy" (Volume / PriceChange).
  - **Why**: We don't have full Orderbook Depth (L2) data via simple websocket streams easily without heaviness. This proxy ("Cost of Movement") effectively highlights hidden walls or thin books without needing L2 parsing.
- **Decision**: Visual "Pulsing" for High Velocity.
  - **Why**: Peripheral vision needs to catch "Panic" or "Euphoria" events even if the user isn't looking directly at the number.
