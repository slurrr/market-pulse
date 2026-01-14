# Dashboard Notes

## v0.9 Observations (Structural & Cohesion Expansion)
- **New Lens**: **Session VWAP**.
    - *Why*: Provides a "fair value" anchor. Price > VWAP = Bullish Regime. Distance from VWAP = Extension.
- **New Lens**: **Microstructure (Icebergs)**.
    - *Why*: High volume with zero price change is the definition of absorption. Detecting this explicitly (>$5M walls) reveals institutional hands.
- **New Lens**: **Market Cohesion (Correlation)**.
    - *Why*: Distinguishing between "Everything is dumping" (Macro) vs "Rotation" (BTC flat, ETH dumping) is critical for context.

## v0.8 Observations (Orthogonal Expansion)
- **Hypothesis**: "Core Reality" (Price) is not enough. We need to know the *condition* of the market.
- **New Lens**: **Structural Acceptance**.
    - *Why*: Differentiating between "Exploration" (Transient price) and "Acceptance" (Building value) prevents chasing fake breakouts.
- **New Lens**: **Inventory Imbalance**.
    - *Why*: Divergence between Effort (CVD) and Result (Price) is the clearest signal of absorption or exhaustion.
- **New Lens**: **Failure Modes**.
    - *Why*: Markets often reverse after "failed" moves. Detecting a "Rejection" explicitly is high-value.
- **New Lens**: **Participation Breadth**.
    - *Why*: Knowing if a move is Retail-driven (fragile) vs Whale-driven (durable) changes how we treat momentum.
- **New Lens**: **Leverage Health (Basis)**.
    - *Why*: Spot - Perp price difference reveals euphoria (Perp premium) vs fear (Spot premium).
- **New Lens**: **Market Pain (Liquidations)**.
    - *Why*: Large liquidations often mark local tops/bottoms. Knowing *who* is getting rekt (Longs vs Shorts) hints at the next move (Squeeze vs Cascade).

## v0.6 Observations (Situational Awareness)
- **Usefulness**: The **Spot vs Perp Divergence** is the killer feature.
  - *Observation*: Seeing Spot Delta flat while Perp Delta spikes (with price moving up) correctly identified a "Leverage Fakeout" in testing.
- **Usefulness**: The **Liquidity Proxy** ("Cost of Movement") is surprisingly effective without L2 data.
  - *Observation*: "THICK / ABSORBING" status appeared right before a localized bottom, indicating a hidden buy wall.
- **Visuals**: The **Pulsing Header** works well for peripheral awareness. You don't have to stare at the screen to know when volatility kicks in.
- **Noise**: The "Whale Tape" is still a bit fast during high activity. Might need a dynamic threshold (e.g., auto-adjust >$100k during frenzy).
- **Missing**: True "Rotation" visualization is still basic (just % change). Heatmaps or a "Flow Graph" would be better for identifying Sector Rotation (e.g. AI Coins -> Memes).
- **Owner Notes**: v0.6 does a great job of situational awareness. Missing cohesive liquidity context, volatility state, failure modes. The dashboard should be cohesive and contextually rich. Think broader market state lenses.

## Initial Observations (v0.2)
- **Usefulness**: The "Aggression Balance" bar (Buy vs Sell Vol) interacting with "Velocity" is the most potent signal.
  - *Hypothesis*: If Aggression is 80% Buy but Velocity is 0 or negative, someone is absorbing the bid (hidden wall). This is high value information.
- **Noise**: The raw tape is too fast to read. The "Whale Tracker" filter (> $50k) is much more useful.
- **Missing**: No visuals on *Depth* (Limit orders). We only see market orders. We might be blind to walls until we hit them.
- **Owner Notes**: v0.2 shows strong microstructure intuition (aggression / absorption). Lacking cohesive liquidity context, spot vs perps divergence, volatility state, rotation, failure modes. The dashboard should be cohesive and contextually rich.