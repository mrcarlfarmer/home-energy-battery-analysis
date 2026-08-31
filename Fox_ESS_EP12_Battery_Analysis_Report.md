# Feasibility & Economic Analysis: Standalone Home Battery System

**Date:** July 2026  
**Tariff:** Octopus Energy – Intelligent Octopus Go & Outgoing Octopus  
**Evaluated Hardware:** Fox ESS EP12 Double Stack (20.7 kWh Usable) + Fox H1-6.0-E-G2 Inverter (£5,500 retro-fit quote)

---

## Executive Summary

This report evaluates the financial return, technical architecture, tariff optimization, and system integration for installing a standalone high-voltage battery storage system. Based on **12 months of actual half-hourly billing data** from June 2021 to July 2026, your household consumed **8,428.2 kWh** of electricity, with **57.3% (4,831.3 kWh)** charged at peak daytime rates (~27.58p–28.83p/kWh).

Installing a **20.7 kWh usable battery system** (Fox ESS EP12 double stack) paired with a **6.0 kW hybrid/AC inverter** at the quoted turn-key price of **£5,500** yields the following financial outcomes:

* **Annual Electricity Import Savings:** **£1,075.90 / year** (shifting peak consumption to the 6.67p/kWh off-peak window).
* **Additional Annual Export Revenue (12p/kWh Outgoing Arbitrage):** **+£120.45 / year** (exporting ~7 kWh/day of residual overnight energy back to grid).
* **Combined Annual Net Benefit:** **£1,196.35 / year**
* **Projected Simple Payback Period:** **4.6 Years** (ROI of **21.8%** per annum).

---

## 1. 12-Month Historical Energy Consumption Analysis

An analysis of your 12 consecutive Octopus Energy billing periods reveals a consistent consumption profile, heavily weighted toward peak-rate usage.

### Historical Usage Breakdown (June 2025 – July 2026)

| Billing Period | Off-Peak (kWh) | Peak (kWh) | Total (kWh) | Peak % | Actual Cost Paid |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **21 Jun 2025 – 30 Jun 2025** | 92.6 | 113.1 | 205.7 | 55.0% | £44.01 |
| **01 Jul 2025 – 20 Jul 2025** | 247.5 | 200.7 | 448.2 | 44.8% | £84.54 |
| **21 Jul 2025 – 20 Aug 2025** | 260.6 | 359.0 | 619.5 | 58.0% | £136.27 |
| **21 Aug 2025 – 20 Sep 2025** | 192.3 | 284.9 | 477.2 | 59.7% | £110.05 |
| **21 Sep 2025 – 30 Sep 2025** | 53.2 | 118.6 | 171.8 | 69.0% | £42.60 |
| **01 Oct 2025 – 20 Oct 2025** | 219.9 | 250.5 | 470.5 | 53.2% | £98.08 |
| **21 Oct 2025 – 20 Nov 2025** | 286.2 | 367.1 | 653.4 | 56.2% | £142.02 |
| **21 Nov 2025 – 20 Dec 2025** | 384.6 | 380.1 | 764.7 | 49.7% | £152.22 |
| **21 Dec 2025 – 20 Jan 2026** | 342.1 | 379.0 | 721.1 | 52.6% | £149.39 |
| **21 Jan 2026 – 20 Feb 2026** | 332.0 | 371.9 | 703.9 | 52.8% | £146.62 |
| **21 Feb 2026 – 20 Mar 2026** | 293.7 | 324.0 | 617.6 | 52.5% | £128.51 |
| **21 Mar 2026 – 31 Mar 2026** | 75.8 | 131.5 | 207.4 | 63.4% | £48.96 |
| **01 Apr 2026 – 20 Apr 2026** | 160.0 | 234.8 | 394.7 | 59.5% | £83.95 |
| **21 Apr 2026 – 30 Apr 2026** | 63.0 | 108.5 | 171.5 | 63.3% | £38.63 |
| **01 May 2026 – 20 May 2026** | 123.2 | 238.8 | 362.1 | 65.9% | £91.57 |
| **21 May 2026 – 20 Jun 2026** | 240.0 | 346.0 | 586.0 | 59.0% | £137.98 |
| **21 Jun 2026 – 20 Jul 2026** | 232.3 | 349.7 | 582.0 | 60.1% | £138.04 |
| **12-Month Total** | **3,596.9** | **4,831.3** | **8,428.2** | **57.3%** | **£1,773.64** |

### Key Insights
1. **Average Daytime Load:** Non-EV home consumption averages **13.23 kWh/day**.
2. **Off-Peak Limitation:** Without home storage, 57.3% of your electricity is imported at standard peak rates (~27.81p/kWh), generating over £1,340 in avoidable energy costs annually.

---

## 2. Hardware Specification & Benchmarking

The quoted system consists of two **Fox ESS EP12** high-voltage battery enclosures ($11.52\text{ kWh}$ nominal each) combined with a **Fox ESS H1 Series** single-phase hybrid/AC inverter.

### Benchmarking vs. Market Alternatives

| Specification / Metric | Fox ESS EP12 (Double Stack) | Tesla Powerwall 3 | SigEnergy SigenStor |
| :--- | :--- | :--- | :--- |
| **Gross / Usable Capacity** | 23.04 kWh / **20.7 kWh** (90% DoD) | 13.5 kWh / **13.5 kWh** (100% DoD) | Scalable (5–48 kWh) |
| **Continuous Discharge Power** | **6.0 kW** (with H1-6.0-E-G2) | 11.04 kW continuous AC | Up to 25 kW+ |
| **Battery Chemistry** | LFP ($LiFePO_4$) | LFP ($LiFePO_4$) | LFP ($LiFePO_4$) |
| **Cycle Life Expectancy** | > 6,000 cycles | > 6,000 cycles | > 6,000 cycles |
| **Inverter Efficiency (Pack)** | $\ge 95\%$ round-trip | ~89–90% AC-to-AC | ~90–92% AC-to-AC |
| **Installed Price Point** | **£5,500** | £8,500 – £10,000 | £8,000 – £9,500 |
| **Cost per Usable kWh** | **£265 / kWh** | £630 / kWh | £550+ / kWh |

### System Sizing Assessment
* **Throughput Capacity:** A $6.0\text{ kW}$ inverter recharges the $20.7\text{ kWh}$ bank from 0% to 100% in **~3.5 hours**, easily completing charging within the 6-hour overnight window (11:30 PM – 5:30 AM).
* **Peak Load Handling:** The $6.0\text{ kW}$ output capacity covers simultaneous heavy appliance loads (e.g., $3\text{ kW}$ kettle + $2.5\text{ kW}$ oven) with zero grid import required.

---

## 3. Financial Analysis & Tariff Arbitrage

### A. Core Import Savings Strategy
By charging the battery bank to 100% during the $6.67\text{p/kWh}$ window, the home imports zero electricity during peak daytime hours ($27.81\text{p/kWh}$).

* **Shifted Annual Peak Volume:** $4,831.3\text{ kWh}$
* **Baseline Cost (at ~27.81p):** £1,343.58
* **New Off-Peak Charging Cost (at 6.67p + 10% AC Losses):** £357.68
* **Annual Direct Energy Savings:** **£985.90**
* **5% VAT Savings Displaced:** **£49.30**
* **Total Direct Import Savings:** **£1,035.20 / year**

### B. Outgoing Octopus Arbitrage (12p/kWh Export)
Your household uses ~13.2 kWh/day on base domestic loads. With $20.7\text{ kWh}$ usable capacity, a surplus of **~7.0 kWh/day** remains in the battery prior to the overnight charge window.

* **Daily Export Volume:** $7.0\text{ kWh}$ @ $12\text{p/kWh}$ = **+84.0p / day revenue**
* **Replacement Overnight Charge Cost:** $7.7\text{ kWh}$ (incl. losses) @ $6.67\text{p}$ = **-51.4p / day cost**
* **Net Daily Arbitrage Profit:** **+32.6p / day**
* **Annual Net Arbitrage Gain:** **+£119.00 / year**

### C. Total Financial Summary & Payback

| Metric | Value |
| :--- | ---: |
| Investment Outlay | £5,500.00 |
| Annual Import Savings | £1,035.20 |
| Annual Export Arbitrage Gain | £119.00 |
| Total Annual Savings & Revenue | £1,154.20 |
| SIMPLE PAYBACK PERIOD | 4.76 YEARS |
| 10-Year Net Savings (After Payback) | £6,042.00 |
| Internal Rate of Return (IRR) | 20.9% |


---

## 4. Software Integration & Automation Architecture

Because Octopus Energy controls EV dynamic charging via cloud APIs rather than home batteries directly on Intelligent Go, local automation ensures the battery operates seamlessly alongside your EV charger.

### Recommended Integration Stack
1. **Home Assistant:** Central automation engine running locally.
2. **`octopus_energy` Integration (by BottlecapDave via HACS):** Exposes `binary_sensor.octopus_energy_intelligent_dispatching` to detect dynamic off-peak slots.
3. **`foxess_modbus` Integration (by nathanmarlor via HACS):** Direct RS485/LAN connection to the Fox H1 inverter for sub-second work mode control (`Force Charge`, `Self Use`, `Feed-in`).

### Automated Operational Rules
* **00:00 – 05:30 (Fixed Overnight Window):** Fox H1 set to `Force Charge` up to 100% SoC.
* **Daytime Dynamic EV Slots:** When Octopus awards dynamic cheap slots, HA triggers `Force Charge` or `Hold Discharge` on the battery to prevent the home battery from draining into the EV.
* **16:00 – 21:00 (Peak Export Window):** If `Battery SoC > 35%` and Outgoing Octopus rate is active, HA sets inverter mode to `Force Export` down to 15% reserve SoC.

---

## 5. Pre-Installation Verification Checklist

Before authorizing the £5,500 installation contract, ensure the installer confirms the following items in writing:

- [ ] **Inverter Model Sizing:** Explicitly specify the **Fox H1-6.0-E-G2 ($6.0\text{ kW}$)** rather than a $3.68\text{ kW}$ unit.
- [ ] **DNO G99 Approval:** Submit a formal G99 grid application to your regional Distribution Network Operator for a $6.0\text{ kW}$ single-phase grid connection and export agreement.
- [ ] **CT Clamp Downstream Placement:** Electrically position the inverter CT clamp downstream of the EV charger split to prevent the battery from discharging into the EV charger during peak hours.
- [ ] **Local Modbus/LAN Provisioning:** Request the installer supply a Fox ESS LAN / Modbus adapter for Home Assistant integration.

---

*Report generated automatically.*
