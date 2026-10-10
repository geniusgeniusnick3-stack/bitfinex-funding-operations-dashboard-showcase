# Bitfinex Funding Operations Dashboard

A read-only showcase of a funding-operations dashboard for portfolio and lifecycle visibility.

> **This repository is a sanitized demonstration bundle.** It contains synthetic demo data and does not represent a live account or live performance.

## What this demonstrates

- Funding positions and open offers
- Funding lifecycle visibility
- Earnings and balance presentation
- Event and system-health views
- Read-only, multilingual dashboard UI
- Clear separation between current funding state and persisted lifecycle records

## Data and safety boundaries

The public showcase intentionally does **not** include:

- Exchange API credentials or authenticated API clients
- Order, cancel, or execution actions
- Private account identifiers or raw account history
- Production bot code, schedulers, or deployment configuration
- Private funding rules, rate-selection logic, allocation rules, or risk controls
- Live performance claims

All history records use synthetic identifiers such as `DEMO-000001` and `DEMO-EARN-000001`. The dashboard is display-only and has no live exchange connection.

## Run locally

From this directory:

```bash
/opt/homebrew/bin/python3 -m http.server 8766 --bind 127.0.0.1
```

Open:

```text
http://127.0.0.1:8766/index.html
```

## Repository structure

```text
index.html                    Dashboard UI
PRODUCT.md                    Product scope and safety constraints
data/dashboard_demo.json      Sanitized overview data
data/dashboard_history.json   Synthetic history records
data/dashboard_history.js     Browser-embedded history artifact
```

## Scope

This repository is for interface and operations-visibility demonstration only. It is not a trading system, lending engine, execution tool, or performance report.
