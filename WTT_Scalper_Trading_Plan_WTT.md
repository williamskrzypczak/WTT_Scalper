# WTT Scalper Trading Plan

**WaveRider Trading Technologies**  
**Comprehensive Trading Strategy for Scalp Channel-Based Scalping**  
**Rev1.6**

---

## Executive Summary

The WTT Scalper is a sophisticated scalping system designed for short-term trading opportunities using scalp channels. This trading plan provides a comprehensive framework for implementing the system with proper risk management, entry/exit strategies, and performance monitoring.

> **⚠️ Risk Disclaimer**  
> Trading involves substantial risk of loss and is not suitable for all investors. Past performance does not guarantee future results. Always use proper risk management and never risk more than you can afford to lose.

---

## System Overview

### 🎯 Core Strategy
**Squeeze Release Scalping:** The system focuses exclusively on squeeze release signals, identifying high-probability volatility expansion opportunities with volume confirmation and trend filtering.

### ⏱️ Timeframe
**Short-term Scalping:** Designed for quick in-and-out trades, typically holding positions for minutes to hours, not days or weeks.

### 📊 Market Conditions
**Volatility Expansion:** Best suited for markets transitioning from low volatility (squeeze) to high volatility (expansion) periods.

### 🎨 Visual Signals
**Orange/Purple Theme:** Long signals (orange triangles), short signals (purple triangles), with orange squeeze indicators and color-coded risk management.

---

## Pre-Trade Setup

### 📋 Pre-Trade Checklist

- **Market Analysis:** Confirm overall market trend using 50-period EMA
- **Volatility Check:** Look for squeeze conditions (orange squares at top/bottom)
- **Volume Confirmation:** Ensure above-average volume for signal validation
- **Risk Assessment:** Calculate position size based on 2% risk per trade
- **Stop Loss Setup:** Prepare ATR-based stop loss (1.5x ATR)
- **Profit Target:** Set ATR-based profit target (2.5x ATR)
- **Trailing Stop:** Plan for 50% profit target activation

### Setup Configuration

| Component | Setting | Description |
|-----------|---------|-------------|
| **Scalp Channels** | 20-period EMA, 2.0 ATR | Primary scalp channels for squeeze detection |
| **Trend Filter** | 50-period EMA | Confirm overall market direction |
| **Volume Filter** | 20-period SMA | Require above-average volume for signals |
| **Stop Loss** | 1.5x ATR | Conservative risk management |
| **Profit Target** | 2.5x ATR | 1.67:1 risk-reward ratio |
| **Trailing Stop** | 1.0x ATR at 50% PT | Lock in profits after 50% target |

---

## Entry Strategy

### 🟠 Long Entry Conditions

- Squeeze release signal (orange triangle below bar)
- Price above scalp channel middle line
- Uptrend confirmed (price > 50 EMA)
- Above-average volume
- No existing position

### 🟣 Short Entry Conditions

- Squeeze release signal (purple triangle above bar)
- Price below scalp channel middle line
- Downtrend confirmed (price < 50 EMA)
- Above-average volume
- No existing position

### ✅ Entry Best Practices

- **Wait for Confirmation:** Don't enter on the first squeeze release - wait for clear directional movement
- **Volume Validation:** Ensure volume is significantly above average for stronger signals
- **Trend Alignment:** Only trade in the direction of the overall trend
- **Clean Setup:** Avoid entries during major news events or market gaps

---

## Exit Strategy

### 🚪 Exit Conditions

- **Stop Loss:** Exit when price hits the ATR-based stop loss level
- **Profit Target:** Exit when price reaches the profit target level
- **Trailing Stop:** Exit when price hits the trailing stop (after 50% profit target)
- **Trend Reversal:** Exit if price crosses back through the scalp channel middle line
- **Time Stop:** Consider exiting if position held for more than 4 hours

### 🟠 Long Exit Logic

- Stop Loss: Price falls below entry - (1.5 × ATR)
- Profit Target: Price rises above entry + (2.5 × ATR)
- Trailing Stop: Price falls below trailing stop level
- Trend Exit: Price falls below scalp channel middle line

### 🟣 Short Exit Logic

- Stop Loss: Price rises above entry + (1.5 × ATR)
- Profit Target: Price falls below entry - (2.5 × ATR)
- Trailing Stop: Price rises above trailing stop level
- Trend Exit: Price rises above scalp channel middle line

---

## Risk Management

### 🛡️ Risk Management Rules

- **Position Sizing:** Risk maximum 2% of account per trade
- **Maximum Positions:** One position at a time (no pyramiding)
- **Daily Loss Limit:** Maximum 6% loss per day
- **Weekly Loss Limit:** Maximum 15% loss per week
- **Correlation Risk:** Avoid trading multiple correlated instruments simultaneously
- **News Events:** Avoid trading during major economic releases
- **Market Hours:** Focus on high-liquidity periods

### 📊 Position Size Calculation

**Formula:** Position Size = (Account Risk × Account Size) ÷ Stop Loss Distance

- **Account Risk:** 2% of account balance
- **Stop Loss Distance:** 1.5 × ATR
- **Example:** $10,000 account, $200 risk, 50-point stop = 4 contracts

---

## Performance Monitoring

### 📈 Key Metrics

- **Win Rate:** Target 50%+ for profitability
- **Risk-Reward:** 1.67:1 ratio (conservative)
- **Average Trade:** Monitor for consistency
- **Max Drawdown:** Keep below 20%

### 📊 Performance Table

- **Win Rate:** Displayed in performance table
- **Squeeze Status:** Shows current market condition
- **Real-time Updates:** Monitor during trading sessions
- **Historical Review:** Weekly performance analysis

### 📋 Weekly Review Checklist

- Review all trades for the week
- Calculate win rate and average trade
- Identify patterns in winning/losing trades
- Check adherence to risk management rules
- Update trading journal with lessons learned
- Adjust strategy if necessary

---

## Market Conditions

### ✅ Favorable Conditions

- Clear trend direction
- Regular squeeze cycles
- High volume periods
- Low news volatility
- Normal market hours

### ❌ Avoid Trading

- Major news events
- Low volume periods
- Extreme market volatility
- Holiday trading sessions
- Gap openings

---

## Implementation Timeline

| Phase | Duration | Focus |
|-------|----------|-------|
| **Phase 1: Paper Trading** | 2-4 weeks | Learn system signals, practice entries/exits, build confidence |
| **Phase 2: Small Position Sizing** | 4-8 weeks | Live trading with minimal risk, focus on execution quality |
| **Phase 3: Full Position Sizing** | Ongoing | Normal position sizes, continuous optimization |

---

## Success Metrics

### 🎯 Success Criteria

- **Consistent Win Rate:** 50%+ over 50+ trades
- **Positive Expectancy:** Average winning trade > Average losing trade
- **Risk Management:** Never exceed 2% risk per trade
- **Drawdown Control:** Maximum 20% drawdown
- **Execution Quality:** 90%+ adherence to trading plan

---

**© 2024 WaveRider Trading Technologies - WTT Scalper Trading Plan**  
*Designed for conservative scalping with advanced risk management*
