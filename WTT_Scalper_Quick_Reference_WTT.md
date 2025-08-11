# WTT Scalper Trading System - Quick Reference Guide

**WaveRider Trading Technologies**  
**Advanced Scalp Channel-Based Scalping Strategy**  
**Rev1.6**

---

## System Overview

The WTT Scalper is a sophisticated trading system designed for short-term scalping opportunities using scalp channels. It focuses exclusively on squeeze release signals, combining volatility expansion detection, trend filtering, and volume confirmation to identify high-probability entry and exit points with conservative risk management.

---

## Key Features

### 🎯 Single-Timeframe Analysis
Simplified and reliable scalp channel analysis focused on the current timeframe for consistent performance.

### 📈 Squeeze Release Detection
Identifies high-probability volatility expansion opportunities with volume confirmation and trend filtering.

### 🔍 Squeeze Detection
Detects low volatility periods (squeezes) and alerts when volatility expansion begins.

### 📊 Trend Filtering
Uses 50-period EMA to ensure trades align with the overall market direction.

### 🛡️ Dynamic Risk Management
ATR-based stop losses and profit targets that adapt to current market volatility.

### 📋 Performance Tracking
Comprehensive tracking of trades, win rate, drawdown, and overall performance metrics.

### 🎨 Color-Coded Risk Management
Stop losses match signal colors for intuitive visual association and easier risk identification.

---

## Input Settings

| Group | Setting | Default | Description |
|-------|---------|---------|-------------|
| **Scalp Channels** | Channel Length | 20 | Period for scalp channel calculation |
| | Channel Multiplier | 2.0 | ATR multiplier for channel width |
| | MA Type | EMA | Moving average type (SMA, EMA, WMA, HMA) |
| | Source | Close | Price source for calculations |
| **Trading** | Volume Filter | True | Require above-average volume for signals |
| | Volume MA Length | 20 | Period for volume average calculation |
| **Risk Management** | ATR Length | 14 | Period for ATR calculation |
| | Stop Loss ATR Multiplier | 1.5 | ATR multiplier for stop loss distance |
| | Profit Target ATR Multiplier | 2.5 | ATR multiplier for profit target distance |
| | Risk Per Trade (%) | 2.0 | Percentage risk per trade |
| **Squeeze** | Enable Squeeze Detection | True | Enable squeeze detection feature |
| | Bollinger Bands Length | 20 | Period for Bollinger Bands calculation |
| | BB Multiplier | 2.0 | Standard deviation multiplier for BB |
| **Visual** | Show KC Bands | True | Display scalp channel bands |
| | Show Trend MA | False | Display 50-period EMA trend line |
| | Show Trade Signals | True | Display entry and exit signals |
| | Show Performance Table | False | Display performance metrics table |

---

## Signal Types

| Signal Type | Condition | Visual Indicator | Description |
|-------------|-----------|------------------|-------------|
| **Long Squeeze** | Squeeze release + price above KC middle + uptrend + volume | Orange triangle (small) | Squeeze release signal |
| **Short Squeeze** | Squeeze release + price below KC middle + downtrend + volume | Purple triangle (small) | Squeeze release signal |

---

## Alert System

### Available Alerts

- **LONG Signal:** "WTT Scalper: LONG signal at [price] | Check levels on chart"
- **SHORT Signal:** "WTT Scalper: SHORT signal at [price] | Check levels on chart"
- **Squeeze Detected:** "WTT Scalper: SQUEEZE detected - Low volatility period, prepare for breakout"
- **Squeeze Release:** "WTT Scalper: SQUEEZE RELEASE - Volatility expansion beginning"

> **Note:** All alerts use `alert.freq_once_per_bar` to prevent spam and include dynamic price information.

---

## Visual Elements

### Chart Components

- **Scalp Channels:** Orange bands with purple middle line
- **Trend MA:** 50-period EMA (optional display)
- **Squeeze Signals:** Small triangles (orange for long, purple for short)
- **Squeeze Indicator:** Tiny orange squares at top/bottom when squeeze active
- **Stop Loss:** Color-coded dots (orange for long, purple for short) showing exit levels
- **Profit Targets:** Green dots showing take-profit levels
- **Performance Table:** Dark theme with bright text showing metrics

---

## Performance Metrics

The system tracks comprehensive performance data including:

- **Total Trades:** Number of completed trades
- **Win Rate:** Percentage of profitable trades
- **Total P&L:** Overall percentage gain/loss
- **Max Drawdown:** Largest peak-to-trough decline
- **Current Position:** Active trade status (LONG/SHORT/FLAT)
- **Bars in Trade:** Duration of current position
- **Squeeze Status:** Current squeeze condition (ACTIVE/NONE)

---

## Strategy Version

### 🚀 Automated Trading Features

The WTT Scalper is also available as a **Pine Script Strategy** with additional features for automated trading and backtesting.

### Strategy-Specific Features

- **Automated Trading:** Real entry/exit orders with stop losses and profit targets
- **Position Management:** Proper risk management with ATR-based sizing
- **Backtesting Capability:** Full strategy testing in TradingView
- **Pyramiding Options:** Add to winning positions (optional)
- **Fixed Position Sizing:** Option to use fixed dollar amounts
- **Enhanced Performance Tracking:** Real P&L and drawdown calculations

---

## Revision History

### Recent Updates

- **R1.6:** Enhanced alert precision and visual improvements - increased alert price precision to 5 decimal places for all signal types, optimized code structure with functions, added squeeze cloud visualization with purple fill and orange boundary lines, improved signal visibility with small triangles and dotted vertical lines, enhanced color scheme consistency with WTT branding
- **R1.5:** Simplified performance table - streamlined to show only essential metrics (win rate and squeeze status), changed squeeze indicator squares to orange for better WTT branding consistency
- **R1.4:** Trailing stop enhancement - added trailing stop functionality that activates when price reaches 50% of profit target, implemented ATR-based trailing stops with visual indicators
- **R1.3:** Squeeze-only strategy - converted to squeeze release signals only, changed visual signals to directional triangles, updated stop loss colors to match signals, improved signal quality and reduced noise
- **R1.2:** Simplified interface - removed unnecessary input controls, hardcoded trend filter to 50-period EMA, removed unused inputs, streamlined alerts
- **R1.1:** Fixed plot issues - resolved "Undeclared identifier 'plot'" errors, improved Pine Script v5 compatibility
- **R1.0:** Initial release - comprehensive scalp channel-based trading system

---

**© 2024 WaveRider Trading Technologies - WTT Scalper Trading System**  
*Designed for conservative scalping with advanced risk management*
