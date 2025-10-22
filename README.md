# DINC Candle Counter - TradingView Indicator

A powerful Pine Script indicator for TradingView that implements advanced candle counting with time-based sequence analysis including Time Expansion, Time Contraction, and Time Distortion patterns.

## 🚀 Features

- **Multiple Sequence Types**: Time Expansion, Time Contraction, Time Distortion, Gann Cardinal/Ordinal, and Custom sequences
- **Advanced Candle Analysis**: Inside/outside candle detection with customizable comparison methods
- **Flexible Display Options**: Configurable positioning, colors, and label sizes
- **Multi-Instance Support**: Run multiple indicators simultaneously with different settings
- **Alert System**: Automatic notifications when sequence numbers are reached
- **Interactive Starting Point**: Click and drag to adjust the counting start position

## 📁 Project Files

- `dinc_candle_counter.pine` - Main Pine Script indicator code
- `DINC_Candle_Counter_Guide.md` - Complete usage guide and documentation
- `DINC_Example_Configurations.md` - Pre-configured setups for different trading scenarios

## 🔢 Supported Sequences

### Time-Based Analysis
- **Time Expansion (A)**: `(4,7,9,15)`, `(7,11,15,19)`, `(1,6,9,11)`
- **Time Contraction (B)**: `(3,4,7,8)`, `(4,5,8,9)`, `(2,3,6,7)`
- **Time Distortion (C)**: `(7,9,12,14)`, `(8,11,13,15)`, `(3,4,5,7)`

### Traditional Gann Analysis
- **Gann Cardinal**: `1,2,4,8,16,32,64,128`
- **Gann Ordinal**: `3,6,12,24,48,96,192`

### Custom Sequences
- Define your own comma-separated number sequences
- Example: `1,7,13,21,33`

## 🛠️ Quick Start

1. **Copy** the code from `dinc_candle_counter.pine`
2. **Open** TradingView Pine Editor
3. **Paste** the code and save as "DINC Candle Counter"
4. **Add** to your chart
5. **Click** immediately on the chart to set the starting point
6. **Configure** your desired sequence and display settings

## 📚 Documentation

- **[Complete Guide](DINC_Candle_Counter_Guide.md)** - Detailed documentation with all features explained
- **[Example Configurations](DINC_Example_Configurations.md)** - Ready-to-use setups for different markets and strategies

## 🎯 Use Cases

- **Market Timing**: Identify key turning points using time-based sequences
- **Trend Analysis**: Track expansion and contraction phases
- **Volatility Monitoring**: Detect periods of market distortion
- **Gann Analysis**: Apply traditional time cycle analysis
- **Multi-Timeframe Analysis**: Combine sequences across different timeframes

## ⚙️ Key Settings

- **Sequence Selection**: Choose from predefined or create custom sequences
- **Inside Candle Handling**: Configure how inside bars are counted
- **Display Options**: Position numbers above/below with color customization
- **Multiple Instances**: Use different sequences simultaneously
- **Alert System**: Get notified when sequence numbers are reached

## 🔄 Version History

- **Latest**: Enhanced with all time-based sequences (A, B, C)
- **Oct 27, 2023**: Custom sequences and outside bar double counting
- **Jan 10, 2023**: Inside candle options and multiple pivot references
- **Dec 24, 2022**: Gann sequences and display enhancements
- **Dec 16, 2022**: Initial release

## 💡 Tips

- Always click the chart immediately after adding the indicator
- Use "Display Only Sequence Numbers" to reduce clutter
- Adjust vertical shift when using multiple instances
- Combine with price action analysis for best results
- Document which sequences work best for your markets

## 📈 Trading Applications

- **Scalping**: Short-term sequences on 1-5 minute charts
- **Swing Trading**: Medium-term sequences on hourly/4-hour charts
- **Position Trading**: Long-term sequences on daily/weekly charts
- **Market Analysis**: Identify expansion/contraction cycles
- **Risk Management**: Use sequence numbers for stop-loss placement

This indicator provides a comprehensive solution for time-based market analysis, combining modern sequence analysis with traditional Gann methodologies.