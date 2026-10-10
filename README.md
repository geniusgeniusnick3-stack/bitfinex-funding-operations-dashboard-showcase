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

## Why Bitfinex

Bitfinex provides a peer-to-peer Funding market. This dashboard focuses on making the separate funding states easy to read: wallet balance, open offers, and active funding credits.

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
README.md                     Bilingual project documentation
data/dashboard_demo.json      Sanitized overview data
data/dashboard_history.json   Synthetic history records
data/dashboard_history.js     Browser-embedded history artifact
```

## Scope

This repository is for interface and operations-visibility demonstration only. It is not a trading system, lending engine, execution tool, or performance report.

---

# Bitfinex 放貸作業儀表板

這是一個**唯讀的放貸作業儀表板展示版**，用來展示資產狀態、放貸生命週期、收益紀錄與系統事件的可視化方式。

> **本 repository 是脫敏展示套件。** 裡面的資料全部是合成示範資料，不代表任何真實帳戶，也不代表真實績效。

## 展示內容

- 有效放貸與未成交掛單
- 放貸生命週期與狀態追蹤
- 收益與餘額呈現
- 事件紀錄與系統健康狀態
- 唯讀、多語言儀表板介面
- 區分交易所目前 funding segment 與保存下來的放貸生命週期紀錄

## 為什麼是 Bitfinex

Bitfinex 有提供 P2P Funding 放貸市場。這個儀表板把錢包餘額、未成交掛單與有效放貸分開呈現，讓目前資金狀態比較容易閱讀。

## 資料與安全邊界

這個公開展示版刻意**不包含**：

- 交易所 API 憑證或已驗證 API client
- 下單、撤單或執行功能
- 私人帳戶識別資料或完整 raw history
- 實盤 bot、排程器或部署設定
- 私人放貸規則、利率選擇邏輯、資金配置規則或風控參數
- 真實績效宣稱

所有歷史資料都使用合成 ID，例如：

```text
DEMO-000001
DEMO-EARN-000001
```

這個儀表板只有展示功能，不會連接交易所，也不能進行任何交易或放貸操作。

## 本機啟動

在此 repository 目錄執行：

```bash
/opt/homebrew/bin/python3 -m http.server 8766 --bind 127.0.0.1
```

然後開啟：

```text
http://127.0.0.1:8766/index.html
```

## Repository 結構

```text
index.html                    儀表板介面
PRODUCT.md                    產品範圍與安全限制
README.md                     中英雙語專案說明
data/dashboard_demo.json      脫敏展示摘要資料
data/dashboard_history.json   合成歷史紀錄
data/dashboard_history.js     瀏覽器使用的嵌入資料
```

## 專案範圍

本 repository 只用於展示介面與放貸作業可視化能力，不是交易系統、放貸引擎、下單工具，也不是績效報告。
