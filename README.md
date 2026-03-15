# AI Business Dashboard & KPI Forecasting

> **Business Use Case:** Startup Analytics, E-commerce Intelligence & Revenue Forecasting

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white) ![Prophet](https://img.shields.io/badge/Prophet-0066CC?style=flat) ![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat&logo=plotly&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white)

## Overview

An end-to-end AI-powered business intelligence dashboard that ingests raw business metrics and forecasts future KPIs using time-series models. Built for founders, analysts, and data teams who need actionable predictions — not just charts.

**Business Impact:** Replaces expensive BI tools (Tableau, Power BI) with an open-source, AI-native forecasting engine tailored for fast-moving businesses.

## Features

- **Multi-KPI Forecasting** — Revenue, churn rate, DAU/MAU, conversion rate, AOV
- **Time-Series Models** — Facebook Prophet, LSTM, ARIMA with auto model selection
- **Interactive Dashboard** — Drag-and-drop date ranges, drill-down by segment
- **Anomaly Detection** — Flags unusual spikes/drops with root cause hints
- **Scenario Planning** — "What-if" simulations (e.g., 20% increase in ad spend)
- **CSV/DB Import** — Upload data via CSV or connect to PostgreSQL/MySQL
- **Automated Alerts** — Email/Slack notifications when KPIs cross thresholds

## Tech Stack

| Layer | Technology |
|-------|------------|
| Forecasting | Facebook Prophet, LSTM (Keras), ARIMA |
| Dashboard | Streamlit + Plotly |
| Data Layer | Pandas, NumPy, SQLAlchemy |
| Database | PostgreSQL / SQLite |
| Alerting | SMTP Email + Slack Webhook |
| Deployment | Docker + Streamlit Cloud |

## Project Structure

```
ai-business-dashboard-kpi-forecasting/
├── app/
│   ├── main.py                 # Streamlit entry point
│   ├── pages/
│   │   ├── overview.py         # KPI overview page
│   │   ├── forecasting.py      # Forecast models page
│   │   ├── anomalies.py        # Anomaly detection page
│   │   └── scenarios.py        # What-if scenario page
│   ├── models/
│   │   ├── prophet_model.py    # Prophet forecasting
│   │   ├── lstm_model.py       # LSTM deep learning model
│   │   └── arima_model.py      # ARIMA baseline
│   ├── data/
│   │   ├── loader.py           # CSV/DB data ingestion
│   │   └── sample_data.csv     # Sample business data
│   └── utils/
│       ├── alerts.py           # Slack/email alerts
│       └── metrics.py          # KPI calculation logic
├── requirements.txt
├── Dockerfile
└── README.md
```

## Setup & Installation

```bash
git clone https://github.com/nkhalfe56-star/ai-business-dashboard-kpi-forecasting
cd ai-business-dashboard-kpi-forecasting
pip install -r requirements.txt
streamlit run app/main.py
```

## Business Case

| Use Case | Value |
|----------|-------|
| Revenue forecasting | Plan hiring, inventory, and cash flow |
| Churn prediction | Proactively retain at-risk customers |
| Anomaly detection | Catch fraud or data issues instantly |
| Scenario planning | Test growth strategies before executing |

## License

MIT License
