# WTT Scalper R1.7

## WaveRider Trading Technologies - Keltner Channel Trading System

A sophisticated scalping indicator designed for high-frequency trading using Keltner Channel analysis, squeeze detection, and comprehensive performance tracking.

---

## 🚀 **FEATURES**

### **Core Trading System**
- **Keltner Channel Analysis**: Advanced channel-based entry/exit signals
- **Squeeze Detection**: Volatility contraction and expansion identification
- **Volume Confirmation**: Enhanced signal validation with volume filters
- **Trend Filtering**: 50-period EMA trend confirmation
- **Performance Tracking**: Comprehensive success rate and ratio metrics

### **Risk Management**
- **ATR-based Stop Loss**: Dynamic stop loss calculation (1.5x ATR)
- **Profit Targets**: Optimized profit target levels (2.5x ATR)
- **Trailing Stops**: Dynamic trailing stop with 50% profit target activation
- **Position Sizing**: Risk-based position sizing (2% risk per trade)

### **Visual Elements**
- **Trade Signals**: Directional triangles for squeeze releases
- **Squeeze Indicators**: Subtle orange squares for squeeze detection
- **Performance Table**: Real-time success metrics display
- **Squeeze Cloud**: Purple fill with orange boundary visualization

---

## 📊 **SIGNAL GENERATION**

### **Entry Conditions**
- **Squeeze Release**: Volatility expansion from contraction
- **Volume Confirmation**: Above-average volume requirement
- **Trend Alignment**: Price above/below 50-period EMA
- **Channel Breakout**: Price breaks Keltner Channel boundaries

### **Exit Strategy**
- **Stop Loss**: ATR-based dynamic stop loss
- **Profit Target**: ATR-based profit target levels
- **Trailing Stop**: Activates at 50% of profit target
- **Squeeze Re-entry**: Volatility contraction signals

---

## ⚙️ **PARAMETERS**

### **Scalp Channel Settings**
- **Channel Length**: 20 periods (default)
- **Channel Multiplier**: 2.0 (default)
- **MA Type**: EMA/SMA/WMA/HMA options
- **Source**: Close price (default)

### **Trading Settings**
- **Volume Filter**: Enabled (requires above-average volume)
- **Volume MA Length**: 20 periods

### **Risk Management**
- **ATR Length**: 14 periods
- **Stop Loss Multiplier**: 1.5x ATR
- **Profit Target Multiplier**: 2.5x ATR
- **Trailing Stop Multiplier**: 1.0x ATR
- **Risk Per Trade**: 2.0%

### **Squeeze Detection**
- **Enable Squeeze**: Enabled
- **Bollinger Bands Length**: 20 periods
- **BB Multiplier**: 2.0

### **Visual Settings**
- **Show KC Bands**: Disabled (default)
- **Show Trend MA**: Disabled (default)
- **Show Trade Signals**: Enabled

---

## 📈 **PERFORMANCE METRICS**

### **Success Tracking**
- **Win Rate**: Percentage of profitable trades
- **Success Ratio**: Risk/reward ratio analysis
- **Squeeze Status**: Current market volatility state
- **Trade Count**: Total number of signals generated

### **Real-time Monitoring**
- **Performance Table**: Live success metrics
- **Squeeze Indicators**: Visual squeeze detection
- **Signal Quality**: Entry/exit timing analysis

---

## 🎯 **TRADING STRATEGY**

### **Conservative Approach**
- **Multi-confirmation**: Volume, trend, and squeeze alignment
- **Risk Management**: Strict 2% risk per trade
- **Quality Over Quantity**: Focus on high-probability setups
- **Performance Monitoring**: Continuous system evaluation

### **Entry Rules**
1. Wait for squeeze release signal
2. Confirm volume is above average
3. Verify trend alignment
4. Enter at channel breakout level
5. Set ATR-based stop loss and profit target

### **Exit Management**
- **Stop Loss**: ATR-based dynamic level
- **Profit Target**: 2.5x ATR from entry
- **Trailing Stop**: Activates at 50% of profit target
- **Squeeze Re-entry**: Exit on volatility contraction

---

## 🔔 **ALERT SYSTEM**

### **Signal Alerts**
- **Long Entry**: Channel breakout with volume confirmation
- **Short Entry**: Channel breakdown with volume confirmation
- **Squeeze Release**: Volatility expansion signals
- **Performance Updates**: Success rate notifications

### **Alert Information**
- **Price**: 5-decimal precision
- **Volume**: Above/below average status
- **ATR**: Current volatility level
- **Squeeze Status**: Contraction/expansion state

---

## 📝 **VERSION HISTORY**

### **R1.7** (Current)
- Performance tracking implementation and system optimization
- Signal-based success rate and ratio metrics
- Enhanced performance display table
- Optimized trailing stop functionality
- Improved squeeze cloud visibility

### **R1.6**
- Enhanced alert precision (5 decimal places)
- Optimized code structure with functions
- Added squeeze cloud visualization
- Improved signal visibility and color scheme

### **R1.5**
- Simplified performance table
- Streamlined metrics display
- Enhanced WTT branding consistency

### **R1.4**
- Trailing stop enhancement
- ATR-based trailing stop functionality
- Visual trailing stop indicators

### **R1.3**
- Squeeze-only strategy implementation
- Removed traditional breakout signals
- Enhanced signal quality and reduced noise

### **R1.2**
- Simplified interface
- Removed unnecessary input controls
- Streamlined user experience

### **R1.1**
- Fixed plot issues
- Pine Script v5 compatibility
- Improved code structure

### **R1.0**
- Initial release
- Comprehensive Keltner Channel system
- Multi-timeframe support and risk management

---

## 🛠️ **INSTALLATION**

1. **Download**: Clone or download the repository
2. **Pine Script**: Open TradingView Pine Script editor
3. **Copy Code**: Copy the contents of `src/WTT_Scalper_Rev1.7.pine`
4. **Paste**: Paste into TradingView Pine Script editor
5. **Apply**: Add to chart and configure parameters

---

## 📞 **SUPPORT**

For questions, issues, or feature requests, please refer to the WaveRider Trading Technologies documentation or contact the development team.

---

## 📄 **LICENSE**

This project is part of the WaveRider Trading Technologies suite of professional trading indicators.

---

*WaveRider Trading Technologies - Professional Trading Solutions*
