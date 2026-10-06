# MNQ Scalp Stacks — Command Center

A clean static rebuild from the supplied dashboard screenshots. Open index.html, or upload it to the root of a GitHub repository and enable GitHub Pages for the main branch / root folder. No installation, build process, API keys, or database required.

## Included
- Official TradingView Advanced Chart embeds for CME_MINI:MNQ1!, initially 5m and 1m, with timeframe switching and a full TradingView link.
- Responsive command center, manual practice risk ticket, BUY/SELL/HOLD, close/flatten, kill switch, local checklist, journal and JSON export.
- Risk uses $0.50 per MNQ tick per contract and blocks practice entries above the manual risk limit.
- No unsupported confidence scores, zero-lag claims, fake win rates, or referral rewards.

## Important behavior
All trade buttons are LOCAL PRACTICE. Manual fill/exit prices are independent of the chart. Stop/target prices are planning values, not automatic executions. P&L excludes fees and slippage. Screenshot price tiles are historical references, not live data. Journal and account state persist in localStorage on this browser/origin; export to retain a backup.

TradingView requires an internet connection. Its symbol/interval availability and market-data delays depend on the exchange and widget support. An unavailable widget is not replaced with fabricated market data; use the full-chart link. Configure your EMA/VWAP/RSI in TradingView. Embedded charts do not import your private Pine scripts or saved account layouts. Chart iframe prices cannot populate the local risk ticket.

## Connections still needed for a production service
An authorized market data feed; a server-side authenticated webhook receiver supporting BUY/SELL/HOLD; server-side Discord/AI keys; a broker integration with verified risk controls; authentication and durable per-user storage. Never add secrets to index.html. GitHub Pages serves static files only.

## Validation
JavaScript syntax and local practice behavior were checked. The TradingView iframe itself was not visually verified in this environment; test its symbol and intraday availability on the deployed page. No live orders were placed.

Suggested repository: mnq-scalp-stacks
Description: Free MNQ practice dashboard with TradingView charts, risk planning, and a local trading journal.
