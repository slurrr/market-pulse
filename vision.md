# market-pulse — Vision

## Purpose

**market-pulse** v0 exists to answer one question, continuously and coherently:

> *What is the market doing right now, why is it doing it, and what condition is it in?*

The system is not a signal generator, not a strategy, and not a prediction engine in isolation.  
It is a **market state and health aggregation engine** designed to compress massive, multi-source market information into a **cohesive, interpretable view of conditions**.

Silence is acceptable. False confidence is not.

---

## Core Philosophy

- **Outcome-driven, not mechanism-driven**  
  We care *what* the market state is and *why*, not *how* it is computed.

- **Regime > Indicators**  
  Signals are contextual. Regimes define meaning.

- **HTF first, LTF second**  
  Lower timeframes are timing and texture, not sources of truth.

- **Failure is information**  
  What *didn’t* happen is often more important than what did.

- **Clarity over actionability**  
  The system should describe the market even when no action is taken.

---

## What market-pulse must always try to answer

### 1. Structure & Regime (HTF → LTF alignment)

**What kind of market is this?**

- Is the market accepting value or rejecting it at current prices?
- Is HTF structure trending, ranging, or transitioning?
- Is volatility expanding or contracting?
- Is this continuation, distribution, or accumulation?
- Are we above or below HTF VWAPs, value areas, or anchors?
- Are HTF highs/lows being defended or cleanly violated?

**Representative signals (non-exhaustive):**
- HTF VWAP slope and distance
- Range expansion vs compression
- Clean breaks vs failed breaks of HTF levels

---

### 2. Liquidity & Inventory (who holds risk)

**Where is risk currently sitting?**

- Is positioning crowded or light?
- Is inventory long-heavy or short-heavy?
- Is price moving to rebalance inventory or build imbalance?
- Is behavior liquidity-seeking or liquidity-avoiding?
- Where are forced participants likely trapped?

**Representative signals:**
- Liquidation clusters
- Open interest change vs price change
- Persistent funding skew
- Stop density relative to structure

---

### 3. Spot vs Perps (real demand vs leverage)

**Is the move structurally real?**

- Is spot leading or lagging perps?
- Is perp aggression unsupported by spot flow?
- Are large spot participants absorbing leveraged flow?
- Is delta translating into price, or being absorbed?

**Representative signals:**
- Spot CVD vs Perp CVD divergence
- Basis expansion / contraction
- Price up with flat spot activity (suspect)

---

### 4. Order Flow Quality (efficiency of movement)

**How expensive is price movement?**

- How much volume is required to move price?
- Is price moving on thin books or heavy participation?
- Are market orders stacking without progress?
- Are key levels showing absorption or icebergs?

**Representative signals:**
- Volume per tick / per % move
- Delta → price response ratio
- Repeated failures at the same level

---

### 5. Volatility State & Optionality

**Is the market primed to move?**

- Is volatility expanding or compressing?
- Are we exiting a volatility squeeze?
- Are moves being bought or sold?
- Is volatility regime shifting before price?

**Representative signals:**
- ATR regime shifts
- Implied vs realized volatility divergence
- Duration of range compression

---

### 6. Momentum & Exhaustion (LTF texture, not direction)

**Is the move healthy or decaying?**

- Are higher highs forming with weaker participation?
- Is momentum accelerating or decelerating?
- Are pullbacks shallow (trend health) or deep (distribution)?
- Are counter-trend moves rejected quickly?

**Representative signals:**
- Momentum slope vs price slope
- Failed continuation attempts
- Time spent moving vs consolidating

---

### 7. Relative Strength & Rotation

**Where is attention naturally flowing?**

- Which assets are leading vs lagging?
- Is capital rotating BTC → ETH → alts, or reversing?
- Are risk-on or defensive assets outperforming?
- Is rotation orderly or violent?

**Representative signals:**
- Relative strength vs BTC / ETH
- Sector-level flow (L1s, memes, infra, AI, etc.)
- Correlation expansion or breakdown

---

### 8. Event & Reflexivity Layer

**Is price responding to something external—or anticipating it?**

- Is positioning building ahead of known events?
- Is funding/OI reacting to news or to price?
- Is price moving before the narrative appears?
- Is post-event follow-through present or absent?

**Representative signals:**
- Pre-event positioning behavior
- Post-event continuation vs fade
- Sentiment extremes without price confirmation

---

### 9. Failure Modes (first-order predictive signals)

**Where is the market wrong?**

- Where did price fail to do what it *should* have done?
- Are breakouts failing quickly?
- Are breakdowns being reclaimed?
- Are strong signals producing weak outcomes?

**Representative signals:**
- Failed break + fast reclaim
- High delta with no continuation
- Liquidations without follow-through

---

## Non-Goals

- No fixed indicators
- No fixed models
- No fixed architecture
- No requirement to always have an opinion
- No obligation to generate trades or actions

---

## Success Criteria

market-pulse is successful if:

- It presents a **coherent, unified view of current market conditions** across structure, liquidity, volatility, flow, and behavior
- Disparate data sources resolve into a **small number of intelligible market states**, not a pile of signals
- The dashboard answers *“what is happening”* before *“what should I do”*
- Market health, balance, stress, and instability are **visually and conceptually obvious**
- Regime transitions, pressure build-ups, and structural shifts are observable **without interpretation gymnastics**
- Relative strength and rotation emerge naturally from the system, without being forced as a goal
- The system remains useful even when **no trades are taken**

Optional but desirable:

- It helps allocate *attention* by showing where conditions are most dynamic or unstable
- It highlights contradictions, tensions, and unresolved market states instead of collapsing them

Explicitly **not** required:

- Actionability
- Trade recommendations
- Timing precision
- Suppression of “untradable” conditions

---

## Guiding Principle for Agents

> **Preserve meaning.  
> Sacrifice structure freely.  
> Never fake confidence.**

This document is the only invariant. Everything else is negotiable.
