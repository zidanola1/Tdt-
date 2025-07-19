# DINC Candle Counter - Example Configurations

## Configuration Examples for Different Market Scenarios

### 1. **Trending Market Analysis (Time Expansion)**
```
Sequence Type: time_expansion_1
Sequence: 4,7,9,15
Display Position: above_candle
Sequence Color: Green (#00FF00)
Display Only Sequence: Yes
Skip Inside Candles: No
Count Outside Double: No
```
**Use Case**: Identify key expansion points during strong trends
**Application**: Look for sequence numbers at potential trend continuation or reversal points

### 2. **Range/Consolidation Analysis (Time Contraction)**
```
Sequence Type: time_contraction_2  
Sequence: 4,5,8,9
Display Position: below_candle
Sequence Color: Orange (#FFA500)
Display Only Sequence: Yes
Skip Inside Candles: Yes
Count Outside Double: No
```
**Use Case**: Analyze consolidation periods and potential breakout timing
**Application**: Monitor for sequence numbers near support/resistance levels

### 3. **Volatility Analysis (Time Distortion)**
```
Sequence Type: time_distortion_1
Sequence: 7,9,12,14
Display Position: above_candle
Sequence Color: Red (#FF0000)
Display Only Sequence: Yes
Skip Inside Candles: No
Count Outside Double: Yes
```
**Use Case**: Track market distortion and unusual volatility periods
**Application**: Identify potential reversal or continuation patterns

### 4. **Traditional Gann Analysis**
```
Sequence Type: gann_cardinal
Sequence: 1,2,4,8,16,32,64,128
Display Position: above_candle
Sequence Color: Blue (#0080FF)
Display Only Sequence: No
Skip Inside Candles: No
Count Outside Double: No
```
**Use Case**: Classical Gann time analysis
**Application**: Combine with price squares and geometric analysis

### 5. **Multi-Timeframe Setup (3 Indicators)**

#### Primary Trend (Expansion)
```
Instance 1:
Sequence Type: time_expansion_2
Sequence: 7,11,15,19
Display Position: above_candle
Vertical Shift: +15
Sequence Color: Green (#00AA00)
Label Size: normal
```

#### Secondary Pattern (Contraction)  
```
Instance 2:
Sequence Type: time_contraction_3
Sequence: 2,3,6,7
Display Position: above_candle
Vertical Shift: +5
Sequence Color: Yellow (#FFAA00)
Label Size: small
```

#### Volatility Monitor (Distortion)
```
Instance 3:
Sequence Type: time_distortion_3
Sequence: 3,4,5,7
Display Position: below_candle
Vertical Shift: -10
Sequence Color: Red (#FF4444)
Label Size: small
```

### 6. **Scalping Setup (Short-term)**
```
Sequence Type: custom
Custom Sequence: 1,3,5,8,13,21
Display Position: above_candle
Sequence Color: Cyan (#00FFFF)
Display Only Sequence: Yes
Max Candles: 50
Skip Inside Candles: Yes
Label Size: small
```
**Use Case**: Quick intraday scalping signals
**Application**: Use on 1-5 minute charts for rapid entry/exit timing

### 7. **Swing Trading Setup (Medium-term)**
```
Sequence Type: time_expansion_3
Sequence: 1,6,9,11
Display Position: above_candle
Sequence Color: Purple (#8A2BE2)
Display Only Sequence: Yes
Max Candles: 100
Skip Inside Candles: No
Count Outside Double: No
Label Size: normal
```
**Use Case**: Multi-day swing trading positions
**Application**: Use on hourly/4-hour charts for swing entry points

### 8. **Position Trading Setup (Long-term)**
```
Sequence Type: gann_ordinal
Sequence: 3,6,12,24,48,96,192
Display Position: above_candle
Sequence Color: Dark Blue (#000080)
Display Only Sequence: Yes
Max Candles: 200
Skip Inside Candles: No
Count Outside Double: No
Label Size: large
```
**Use Case**: Long-term position entries and exits
**Application**: Use on daily/weekly charts for major trend changes

## Market-Specific Configurations

### Forex Markets
```
Recommended: Time Contraction sequences
Rationale: Forex often moves in cycles of contraction/expansion
Best Timeframes: 15min, 1H, 4H
Suggested Sequence: 3,4,7,8 or 2,3,6,7
```

### Stock Markets
```
Recommended: Time Expansion sequences
Rationale: Stocks often follow expansion patterns in trends
Best Timeframes: 1H, Daily
Suggested Sequence: 4,7,9,15 or 7,11,15,19
```

### Cryptocurrency
```
Recommended: Time Distortion sequences
Rationale: Crypto markets exhibit high volatility and distortion
Best Timeframes: 5min, 15min, 1H
Suggested Sequence: 7,9,12,14 or 8,11,13,15
```

### Commodities
```
Recommended: Gann sequences
Rationale: Traditional Gann analysis works well with commodities
Best Timeframes: 4H, Daily, Weekly
Suggested Sequence: 1,2,4,8,16,32,64,128
```

## Advanced Multi-Setup Strategies

### Strategy 1: Triple Confluence
Use three indicators with different sequence types:
1. **Expansion** (green, above, +20 vertical shift)
2. **Contraction** (orange, above, +10 vertical shift) 
3. **Distortion** (red, below, -10 vertical shift)

**Signal**: Enter trades when 2+ sequences align within 1-2 candles

### Strategy 2: Timeframe Cascade
Use same sequence on multiple timeframes:
- **5min chart**: Custom sequence 1,3,5,8
- **15min chart**: Same sequence for confirmation
- **1H chart**: Same sequence for trend direction

**Signal**: Enter when all timeframes show sequence number within session

### Strategy 3: Inside/Outside Bar Strategy
```
Configuration:
Skip Inside Candles: No
Count Outside Double: Yes
Sequence: 3,4,7,8
Monitor: Inside vs outside bar patterns at sequence numbers
```

**Signal**: Look for inside bar compression at sequence numbers, then trade the breakout

## Troubleshooting Common Setups

### Issue: Too Many Numbers
**Solution**: 
- Enable "Display Only Sequence Numbers"
- Reduce "Max Candles" setting
- Use larger gaps between sequence numbers

### Issue: Numbers Not Visible
**Solution**:
- Check sequence numbers are within max candle range
- Adjust vertical shift if overlapping with price
- Verify sequence format (no spaces, comma-separated)

### Issue: Starting Point Issues
**Solution**:
- Always click chart immediately after adding indicator
- Drag the blue line to reposition start point
- Ensure start date/time matches desired candle

### Issue: Multiple Indicators Overlapping
**Solution**:
- Use different vertical shifts (+10, 0, -10)
- Alternate above/below positioning
- Use different label sizes (large, normal, small)

Remember: The key to successful DINC usage is experimentation with different sequences on your preferred markets and timeframes. Document what works best for your trading style and market conditions.