# WTT Scalper Trading System - Quick Reference Guide

<div align="center">

# 🚀 WTT Scalper Trading System
### Advanced Keltner Channel-Based Scalping Strategy
**Version: Rev1.5** | **WaveRider Trading Technologies**

---

</div>

## 📋 System Overview

The **WTT Scalper** is a sophisticated trading system designed for short-term scalping opportunities using Keltner Channels. It focuses exclusively on **squeeze release signals**, combining volatility expansion detection, trend filtering, and volume confirmation to identify high-probability entry and exit points with conservative risk management.

---

## ⭐ Key Features

| Feature | Description |
|---------|-------------|
| 🔄 **Single-Timeframe Analysis** | Simplified and reliable Keltner Channel analysis focused on the current timeframe for consistent performance |
| 🎯 **Squeeze Release Detection** | Identifies high-probability volatility expansion opportunities with volume confirmation and trend filtering |
| 📊 **Squeeze Detection** | Detects low volatility periods (squeezes) and alerts when volatility expansion begins |
| 📈 **Trend Filtering** | Uses 50-period EMA to ensure trades align with the overall market direction |
| 🛡️ **Dynamic Risk Management** | ATR-based stop losses and profit targets that adapt to current market volatility |
| 📈 **Performance Tracking** | Comprehensive tracking of trades, win rate, drawdown, and overall performance metrics |
| 🎨 **Color-Coded Risk Management** | Stop losses match signal colors for intuitive visual association and easier risk identification |

---

## ⚙️ Input Settings

### **Keltner Channel Settings**
| Setting | Default | Description |
|---------|---------|-------------|
| **KC Length** | `20` | Period for Keltner Channel calculation |
| **KC Multiplier** | `2.0` | ATR multiplier for channel width |
| **MA Type** | `EMA` | Moving average type (SMA, EMA, WMA, HMA) |
| **Source** | `Close` | Price source for calculations |

### **Trading Settings**
| Setting | Default | Description |
|---------|---------|-------------|
| **Volume Filter** | `True` | Require above-average volume for signals |
| **Volume MA Length** | `20` | Period for volume average calculation |

### **Risk Management Settings**
| Setting | Default | Description |
|---------|---------|-------------|
| **ATR Length** | `14` | Period for ATR calculation |
| **Stop Loss ATR Multiplier** | `1.5` | ATR multiplier for stop loss distance |
| **Profit Target ATR Multiplier** | `2.5` | ATR multiplier for profit target distance |
| **Risk Per Trade (%)** | `2.0` | Percentage risk per trade |

### **Squeeze Settings**
| Setting | Default | Description |
|---------|---------|-------------|
| **Enable Squeeze Detection** | `True` | Enable squeeze detection feature |
| **Bollinger Bands Length** | `20` | Period for Bollinger Bands calculation |
| **BB Multiplier** | `2.0` | Standard deviation multiplier for BB |

### **Visual Settings**
| Setting | Default | Description |
|---------|---------|-------------|
| **Show KC Bands** | `True` | Display Keltner Channel bands |
| **Show Trend MA** | `False` | Display 50-period EMA trend line |
| **Show Trade Signals** | `True` | Display entry and exit signals |
| **Show Performance Table** | `False` | Display performance metrics table |

---

## 📊 Signal Types

| Signal Type | Condition | Visual Indicator | Description |
|-------------|-----------|------------------|-------------|
| **Long Squeeze** | Squeeze release + price above KC middle + uptrend + volume | 🟠 Orange triangle (small) | Squeeze release signal |
| **Short Squeeze** | Squeeze release + price below KC middle + downtrend + volume | 🟣 Purple triangle (small) | Squeeze release signal |

---

## 🔔 Alert System

### **Available Alerts**
- **🟠 LONG Signal:** `"WTT Scalper: LONG signal at [price] | Check levels on chart"`
- **🟣 SHORT Signal:** `"WTT Scalper: SHORT signal at [price] | Check levels on chart"`
- **🟡 Squeeze Detected:** `"WTT Scalper: SQUEEZE detected - Low volatility period, prepare for breakout"`
- **🟢 Squeeze Release:** `"WTT Scalper: SQUEEZE RELEASE - Volatility expansion beginning"`

> **Note:** All alerts use `alert.freq_once_per_bar` to prevent spam and include dynamic price information.

---

## 🎨 Visual Elements

### **Chart Components**
- **🟠 Keltner Channels:** Orange bands with purple middle line
- **📈 Trend MA:** 50-period EMA (optional display)
- **🔺 Squeeze Signals:** Small triangles (orange for long, purple for short)
- **🟠 Squeeze Indicator:** Tiny orange squares at top/bottom when squeeze active
- **🟠🟣 Stop Loss:** Color-coded dots (orange for long, purple for short) showing exit levels
- **🟢 Profit Targets:** Green dots showing take-profit levels
- **📊 Performance Table:** Dark theme with bright text showing metrics

---

## 📈 Performance Metrics

The system tracks comprehensive performance data including:

- **📊 Total Trades:** Number of completed trades
- **📈 Win Rate:** Percentage of profitable trades
- **💰 Total P&L:** Overall percentage gain/loss
- **📉 Max Drawdown:** Largest peak-to-trough decline
- **📍 Current Position:** Active trade status (LONG/SHORT/FLAT)
- **⏱️ Bars in Trade:** Duration of current position
- **🟡 Squeeze Status:** Current squeeze condition (ACTIVE/NONE)

---

## 🤖 Strategy Version

### **Automated Trading Features**
The WTT Scalper is also available as a **Pine Script Strategy** with additional features for automated trading and backtesting.

### **Strategy-Specific Features**
- **🤖 Automated Trading:** Real entry/exit orders with stop losses and profit targets
- **📊 Position Management:** Proper risk management with ATR-based sizing
- **🧪 Backtesting Capability:** Full strategy testing in TradingView
- **📈 Pyramiding Options:** Add to winning positions (optional)
- **💰 Fixed Position Sizing:** Option to use fixed dollar amounts
- **📊 Enhanced Performance Tracking:** Real P&L and drawdown calculations

---

## 📝 Revision History

### **Recent Updates**

#### **R1.5: Simplified Performance Table**
- Streamlined performance table to show only essential metrics (win rate and squeeze status)
- Changed squeeze indicator squares to orange for better WTT branding consistency
- Removed total trades row for cleaner, more focused display
- Maintains all core functionality while providing cleaner performance display

#### **R1.4: Trailing Stop Enhancement**
- Added trailing stop functionality that activates when price reaches 50% of profit target
- Implemented ATR-based trailing stops with visual indicators
- Enhanced risk management for better trade management
- Maintains all core functionality while providing dynamic exit management

#### **R1.3: Squeeze-Only Strategy**
- Converted to squeeze release signals only for higher quality entries
- Removed traditional breakout signals, keeping only squeeze release entries
- Changed visual signals from circles to directional triangles for better clarity
- Updated stop loss colors to match signal colors (orange for long, purple for short)
- Improved signal quality and reduced noise
- Maintains all core functionality while focusing on volatility expansion opportunities

#### **R1.2: Simplified Interface**
- Removed unnecessary input controls for cleaner user experience
- Removed enable_long/enable_short inputs and hardcoded to true
- Removed trend filter inputs and hardcoded to 50-period EMA
- Removed unused show_labels and enable_alerts inputs
- Streamlined interface while maintaining all core functionality

#### **R1.1: Fixed Plot Issues**
- Resolved "Undeclared identifier 'plot'" error
- Simplified plot statements and improved code structure for better Pine Script v5 compatibility
- Maintained all functionality while fixing parsing issues that prevented proper compilation

#### **R1.0: Initial Release**
- Comprehensive Keltner Channel trading system
- Advanced Keltner Channel implementation with multiple timeframe support
- Conservative entry/exit signals, comprehensive risk management, and detailed performance tracking
- Features include breakout detection, squeeze identification, trend filtering, and dynamic stop loss/profit target calculations
- Designed for conservative trading approach with multiple confirmation filters and comprehensive alert system

---

<div align="center">

---

**© 2024 WaveRider Trading Technologies - WTT Scalper Trading System**

*Designed for conservative scalping with advanced risk management*

---

</div>
