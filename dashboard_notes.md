# Dashboard Notes

## v0.6 Observations (Situational Awareness)
- **Usefulness**: The **Spot vs Perp Divergence** is the killer feature.
  - *Observation*: Seeing Spot Delta flat while Perp Delta spikes (with price moving up) correctly identified a "Leverage Fakeout" in testing.
- **Usefulness**: The **Liquidity Proxy** ("Cost of Movement") is surprisingly effective without L2 data.
  - *Observation*: "THICK / ABSORBING" status appeared right before a localized bottom, indicating a hidden buy wall.
- **Visuals**: The **Pulsing Header** works well for peripheral awareness. You don't have to stare at the screen to know when volatility kicks in.
- **Noise**: The "Whale Tape" is still a bit fast during high activity. Might need a dynamic threshold (e.g., auto-adjust >$100k during frenzy).
- **Missing**: True "Rotation" visualization is still basic (just % change). Heatmaps or a "Flow Graph" would be better for identifying Sector Rotation (e.g. AI Coins -> Memes).
- **Owner Notes**: v0.6 does a great job of situational awareness. Missing cohesive liquidity context, volatility state, failure modes. The dashboard should be cohesive and contextually rich.

## Initial Observations (v0.2)
- **Usefulness**: The "Aggression Balance" bar (Buy vs Sell Vol) interacting with "Velocity" is the most potent signal.
  - *Hypothesis*: If Aggression is 80% Buy but Velocity is 0 or negative, someone is absorbing the bid (hidden wall). This is high value information.
- **Noise**: The raw tape is too fast to read. The "Whale Tracker" filter (> $50k) is much more useful.
- **Missing**: No visuals on *Depth* (Limit orders). We only see market orders. We might be blind to walls until we hit them.
- **Owner Notes**: v0.2 shows strong microstructure intuition (aggression / absorption). Lacking cohesive liquidity context, spot vs perps divergence, volatility state, rotation, failure modes. The dashboard should be cohesive and contextually rich.