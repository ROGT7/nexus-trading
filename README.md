# Nexus Trading

Autonomous evolutionary trading system using genetic algorithms to discover and optimize trading strategies.

## Features

- Genetic Algorithm Evolution - Strategies evolve through natural selection
- Multi-Coin Support - BTC, ETH, SOL, HYPE, and more
- Real-Time Market Data - Kraken, Binance, Bybit, Hyperliquid feeds
- Continual Learning - Population weights updated every 5 minutes with real-time data
- Regime Detection - Adapts to changing market conditions
- Walk-Forward Validation - Out-of-sample testing prevents overfitting

## Strategy

Hybrid model combining:
- 60% Technical signals (RSI, MACD, Bollinger, Stochastic, Williams %R, ROC, OBV)
- 40% MoP-JEPA predictions (5 future predictions)

## Backtest Results

| Coin | Win Rate |
|------|----------|
| BTC  | 67.6%    |
| HYPE | 58.8%    |
| Multi-coin (BTC+ETH+SOL) | 55.8% |

## Architecture

The continual learning module bridges the training-live gap by:
1. Fetching real-time candles every 5 minutes
2. Comparing real-time vs historical data
3. Detecting regime changes
4. Re-evaluating top genomes on real-time data
5. Adjusting fitness and persisting updated population

## License

MIT
