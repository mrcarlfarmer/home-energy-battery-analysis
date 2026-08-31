# Home Energy Battery Analysis

Analysis of the feasibility, technical configuration, and economic return of a standalone home battery system on Octopus Energy tariffs.

## Background

This analysis was prompted by participation in the [Switch Together](https://switchtogether.co.uk/) group-buying programme for sustainable home upgrades, including battery storage.

## Tariff

Analysis uses the **Octopus Intelligent Go** import tariff:

| Rate | Price | Hours |
| :--- | :--- | :--- |
| Peak | 30.27p/kWh | 05:00–23:00 |
| Off-peak | 6.9p/kWh | 23:00–05:00 |

Rates are subject to change; update this table and re-run the analysis if the tariff changes.

## Running the analysis

The notebook runs on Windows with Python 3.13 and a local virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\python -m pip install pandas matplotlib ipykernel
```

Open `notebooks/battery_savings_analysis.ipynb` in VS Code, select the `.venv` kernel, and run all cells.

## Contents

- [Fox ESS EP12 Battery Analysis Report](Fox_ESS_EP12_Battery_Analysis_Report.md): feasibility and economic analysis of a 20.7 kWh usable Fox ESS EP12 double-stack battery with a Fox H1-6.0-E-G2 inverter.
- [Battery savings analysis notebook](notebooks/battery_savings_analysis.ipynb): reproducible analysis of the half-hourly data — consumption costs, idealised vs capacity-constrained battery simulation (20.7 kWh / 6 kW / 90% round-trip), a day-by-time battery-exceedance view, and a heuristic that estimates and removes EV charging to isolate home-only load.
- [Half-hourly consumption data](files/010725%20-%20010726%20electricity%20consumption.csv): one year of half-hourly electricity consumption (1 Jul 2025 – 1 Jul 2026).
- Generated charts and the EV-decomposition dataset (`consumption_ev_decomposed.csv`) are written to `notebooks/outputs/` when the notebook runs.

## Report Highlights

- Analyses 12 months of half-hourly household electricity billing data.
- Evaluates import savings, export arbitrage, and projected payback.
- Covers hardware comparisons, Home Assistant automation, and pre-installation checks.

## Scope

The figures and recommendations in the report are based on the tariff, hardware quote, and energy-use data available in July 2026. Reassess them when any of those inputs change.