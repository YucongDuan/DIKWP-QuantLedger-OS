# DIKWP QuantLedger OS

**DIKWP QuantLedger OS** is an offline-first, open-source semantic risk ledger for quantitative trading research, program-trading governance, backtest integrity review, and strategy compliance readiness.

It is **not** a trading bot, broker adapter, investment adviser, signal seller, market manipulation tool, or promise of return. It does not fetch live data, place orders, connect to exchanges, or provide personalized financial advice. It converts quant strategy manifests, data lineage, model features, backtest records, order profiles, and risk controls into DIKWP semantic ledgers and review artifacts.

## Core purpose

AI and quantitative trading systems can create strategy opacity, data leakage, overfit backtests, excessive automation, order-rate risk, regulatory reporting gaps, and hidden purpose drift. QuantLedger OS makes these risks visible before live deployment.

## Outputs

The demo produces:

- `quantledger_report.json`
- `strategy_decision_matrix.csv`
- `dikwp_strategy_ledger.json`
- `backtest_integrity_matrix.csv`
- `program_trading_reporting_checklist.md`
- `risk_limit_policy.md`
- `kill_recovery_matrix.md`
- `model_agent_cards.json`
- `data_lineage_ledger.json`
- `static_boundary_audit_report.json`

## Install

```bash
pip install -e .
```

## Run demo

```bash
quantledger analyze examples/sample_quant_strategy_portfolio.json --out outputs/demo
quantledger static-audit src --out outputs/demo/static_boundary_audit_report.json
```

## Strategic positioning for DIKWP / Yucong Duan

This project should be published as an open governance and audit layer, not as a live alpha engine. Live broker adapters, certified regulatory report packs, exchange-specific reporting templates, enterprise model-risk management modules, and partner-certified deployment support should remain official commercial or certification layers.

## Boundaries

Do not use this tool to:

- execute real trades;
- evade program-trading reporting obligations;
- bypass exchange or broker controls;
- generate market-manipulative order patterns;
- conceal beneficial ownership, funding source, or strategy identity;
- give personalized investment advice;
- claim a backtest guarantees future profit.
