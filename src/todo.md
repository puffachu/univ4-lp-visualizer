# TODO: Uniswap V4 LP Lifecycle & Event-Driven Visualizer

This module will visualize the full lifecycle of LP positions and decode relevant Uniswap V4 events — including custom hook events — into understandable flows and timelines.

---

## ✅ Goal

Help developers and LPs track how their positions evolve over time, how fees accumulate, and how hooks affect LP performance — with clean, interactive visualizations.

---

## 🧱 Planned Modules

- [ ] **LP Position Tracker**
  - [ ] Parse `Mint`, `Burn`, `Swap`, `Collect`
  - [ ] Track tickLower, tickUpper, liquidity
  - [ ] Visualize changes in range, liquidity, and value

- [ ] **Fee Accumulation View**
  - [ ] Display protocol and LP fee growth
  - [ ] Track `feeGrowthInside0LastX128`, `feeGrowthInside1LastX128`
  - [ ] Visual PnL estimate based on events

- [ ] **Custom Hook Impact**
  - [ ] Detect hook-enabled swaps or liquidity mods
  - [ ] Show dynamic fees, auto-compounding, etc.

- [ ] **ERC-6909 Tracker**
  - [ ] Visualize LP token mint/burn flows
  - [ ] Link 6909 balances to position state
  - [ ] Map LP tokens to address + liquidity data

- [ ] **Event Decoder & Timeline**
  - [ ] Display chronological events per pool or LP
  - [ ] Parse both native and custom events
  - [ ] Build dependency/event graphs (who triggered what)

---

## 🔜 Short-Term Tasks

- [ ] Scaffold parser for LP lifecycle events
- [ ] Set up basic ERC-6909 decoder
- [ ] Design timeline view (Figma or placeholder)
- [ ] Prepare mock events for testing
- [ ] Integrate CLI modules from `univ4-hook-debugger` (Grant #1)

---

## 🗂 Suggested Folder Structure
```
/src
/events
/lp-tracker
/erc6909
/components
/graphs
/shared
```
---

## 📅 Milestone Targets

**Milestone 1 – LP Position Visualizer Core**
- Mint/Burn/Swap/Collect tracker
- Tick range, liquidity, and fee breakdown

**Milestone 2 – Event Timeline + Custom Hook Parser**
- Chronological view + custom hook event integration
- Simple dependency graph

**Milestone 3 – ERC-6909 Support + UI**
- Token tracker + position-linked LP tokens
- MVP frontend with full LP lifecycle display

---

This file will be updated as development progresses.
