# DINC Candle Counter - Complete Guide

## Overview
The DINC (Dynamic Inside/Number Candle) Counter is a powerful TradingView indicator that counts candles from a specified starting point and highlights important sequence numbers based on various time analysis methods.

## Key Features

### 1. **Time-Based Sequences**
- **Time Expansion (A)**: Sequences that identify periods of market expansion
  - A1: `4,7,9,15`
  - A2: `7,11,15,19` 
  - A3: `1,6,9,11`

- **Time Contraction (B)**: Sequences that identify periods of market contraction
  - B1: `3,4,7,8`
  - B2: `4,5,8,9`
  - B3: `2,3,6,7`

- **Time Distortion (C)**: Sequences that identify periods of market distortion
  - C1: `7,9,12,14`
  - C2: `8,11,13,15`
  - C3: `3,4,5,7`

### 2. **Traditional Gann Sequences**
- **Gann Cardinal**: `1,2,4,8,16,32,64,128` (horizontal/cardinal numbers)
- **Gann Ordinal**: `3,6,12,24,48,96,192` (cross/ordinal numbers)

### 3. **Custom Sequences**
- Define your own sequences using comma-separated numbers
- Example: `1,7,13,21,33` (default Fibonacci-like sequence)

## How to Use

### Installation
1. Copy the Pine Script code from `dinc_candle_counter.pine`
2. Open TradingView Pine Editor
3. Paste the code and save as "DINC Candle Counter"
4. Add to your chart

### Setup Instructions
1. **Add the indicator to your chart**
2. **Immediately click somewhere on the chart** to fix the starting point
3. Configure your desired settings in the indicator inputs

### Basic Settings

#### Start Date & Time
- Set the exact date and time where counting should begin
- Default: `2025-07-10 10:00`
- **Important**: After adding, click on the chart to establish the starting point

#### Sequence Selection
Choose from predefined sequences or create custom ones:
```
Time Expansion 1: 4,7,9,15
Time Expansion 2: 7,11,15,19
Time Expansion 3: 1,6,9,11
Time Contraction 1: 3,4,7,8
Time Contraction 2: 4,5,8,9
Time Contraction 3: 2,3,6,7
Time Distortion 1: 7,9,12,14
Time Distortion 2: 8,11,13,15
Time Distortion 3: 3,4,5,7
Gann Cardinal: 1,2,4,8,16,32,64,128
Gann Ordinal: 3,6,12,24,48,96,192
Custom: Your own sequence
```

#### Candle Counting Options
- **Number of Candles**: Maximum candles to count (1-500)
- **Skip Time Distortion Candles**: Skip inside candles from counting
- **Count Outside Candles Double**: Count outside bars as 2 instead of 1

### Inside Candle Settings

#### Inside Candle Detection
- **Comparison Type**: `<=` (less than or equal) or `<` (strictly less than)
- **Price Reference**: Choose between High/Low or Open/Close for inside candle calculation
- **Multiple Inside Candles**: Count multiple inside candles back as pivot or just the last one

### Display Settings

#### Number Positioning
- **Above/Below Candles**: Position numbers above or below price bars
- **Vertical Shift**: Fine-tune vertical positioning (positive = higher, negative = lower)

#### Color Customization
- **Normal Number Color**: Color for regular count numbers (default: gray)
- **Sequence Number Color**: Color for sequence numbers (default: red)
- **Display Only Sequence Numbers**: Show only sequence numbers, hide regular counts

#### Label Formatting
- **Label Size**: Choose from tiny, small, normal, large, huge
- **Status Line Display**: Show current settings and count in status line

## Advanced Features

### Multiple Indicators
You can use multiple DINC counters simultaneously:
1. Add the indicator multiple times to your chart
2. Use different sequences for each instance
3. Adjust **Vertical Shift** and **Above/Below** settings so they don't overlap
4. Example setup:
   - Instance 1: Time Expansion sequence, above candles, vertical shift: +10
   - Instance 2: Time Contraction sequence, below candles, vertical shift: -10

### Starting Point Management
- The **blue vertical line** at candle 1 marks your starting point
- **Click and drag** this line to adjust the starting position
- The count will automatically recalculate from the new position

### Alert System
- Automatic alerts when sequence numbers are reached
- Alerts trigger once per bar when a sequence number is hit
- Useful for automated trading systems or notifications

## Practical Applications

### Market Analysis
1. **Time Expansion Sequences**: Identify potential breakout or trending periods
2. **Time Contraction Sequences**: Spot consolidation or ranging markets  
3. **Time Distortion Sequences**: Detect periods of unusual market behavior

### Trading Strategies
- Use sequence numbers as:
  - **Entry points** for new positions
  - **Exit signals** for existing trades
  - **Support/Resistance levels** based on time cycles
  - **Alert triggers** for market events

### Gann Analysis
- Apply traditional Gann time analysis using cardinal and ordinal numbers
- Combine with price analysis for comprehensive market timing
- Use multiple timeframes for broader market perspective

## Tips and Best Practices

### Setup
1. Always **click on the chart immediately** after adding the indicator
2. Start with a well-defined market event (breakout, reversal, etc.)
3. Use clear, liquid markets for best results

### Sequence Selection
1. **Time Expansion**: Use during trending markets
2. **Time Contraction**: Apply in ranging/consolidating markets
3. **Time Distortion**: Helpful during volatile or unusual market conditions
4. **Custom sequences**: Create based on your specific market observations

### Display Optimization
1. Use **"Display Only Sequence Numbers"** to reduce chart clutter
2. Adjust **vertical shift** when using multiple indicators
3. Choose appropriate **label sizes** based on your chart timeframe

### Analysis
1. Combine with price action analysis
2. Look for confluence with other technical indicators
3. Consider multiple timeframe analysis
4. Document which sequences work best for specific markets/conditions

## Troubleshooting

### Common Issues
- **Numbers not appearing**: Check if "Display Only Sequence Numbers" is enabled
- **Wrong starting point**: Click and drag the blue line to reposition
- **Overlapping labels**: Adjust vertical shift settings
- **Too many/few numbers**: Modify the maximum candle count

### Performance Notes
- Maximum 500 labels supported by TradingView
- Indicator updates in real-time as new bars form
- Historical data remains stable once set

## Release History
- **Oct 27, 2023**: Added custom sequences and outside bar double counting
- **Jan 10, 2023**: Enhanced inside candle options and multiple pivot references
- **Dec 24, 2022**: Added Gann sequences, color options, and vertical positioning
- **Dec 16, 2022**: Initial release with basic counting functionality

This comprehensive indicator provides a powerful tool for time-based market analysis, combining traditional Gann methods with modern sequence analysis techniques.