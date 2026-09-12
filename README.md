# Nexus Trading

Quantitative trading and financial operations.

## Strategy

- **Hybrid Model**: 60% technical signals (RSI, MACD, Bollinger, Stochastic, Williams %R, ROC, OBV) + 40% MoP-JEPA predictions
- **Learning Rate**: 0.05
- **Backtest**: Multi-coin BTC+ETH+SOL = 55.8% WR global (BTC 67.6%, HYPE 58.8%)
- **Objective**: Win rate > 80% before live trading with leverage

## Components

- Evolutionary Trader — Genetic algorithm with 30 genomes per coin
- OmniFusionCore — MoP-JEPA 5 futures + Liquid Core + KAN + Active Inference
- Paper Trading Engine — Risk-free strategy validation
- Live Trading — Hyperliquid integration (gated by validation)
- Win Rate Tracker — Auto-adjustment based on performance
- Trading Optimizer — Pattern detection and parameter tuning
- Hedging Sovereign — Capital preservation
- Colony — 1000 algorithms in 45 groups with evolution and mutations

## Exchanges

- Hyperliquid (perpetual futures)
- Kraken (spot, withdrawals)

## Safety

- Live execution gated by validation and authorization
- Clear distinction between paper/backtest/live results
- Risk controls on position sizing
- Withdrawal mechanism verification

## License

MIT
