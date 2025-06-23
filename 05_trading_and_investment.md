## Trading & Investment

### **OMS / EMS (Order & Execution Management Systems)**

Platforms used by traders and asset managers to manage orders across markets:

* **OMS (Order Management System)**: Tracks lifecycle of orders — entry, modification, allocation, and compliance checks.
* **EMS (Execution Management System)**: Focused on routing, splitting, and executing orders across venues.

**Features**: FIX protocol support, real-time pricing, rule-based routing, and best execution tracking.

| Product                    | Description                                              | Licence                                         | GitHub Link                                                                                    |
| -------------------------- | -------------------------------------------------------- | ----------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **QuickFIX/J**             | JVM FIX messaging engine                                 | BSD 2-Clause (QuickFIX)        | [https://github.com/quickfix-j/quickfixj](https://github.com/quickfix-j/quickfixj)             |
| **Marketcetera CE**        | Open-source OMS / EMS & algo-trading platform            | GPL v2 ([en.wikipedia.org][2], [github.com][3]) | [https://github.com/Marketcetera/marketcetera](https://github.com/Marketcetera/marketcetera)   |
| **AlgoTrader (community)** | Algo-trading & routing stack                             | GPL v2                         | [https://github.com/curtiszimmerman/AlgoTrader](https://github.com/curtiszimmerman/AlgoTrader) |
| **FIX8**   |           C++ / Python FIX engine                           | LGPL v3                        | [https://github.com/fix8/fix8](https://github.com/fix8/fix8)                                   |
| **Lean**       |     LEAN is an event-driven, professional-caliber algorithmic trading platform built with a passion for elegant engineering and deep quant concept modeling. Out-of-the-box alternative data and live-trading support.                 | Apache 2.0                                                                            | [https://github.com/QuantConnect/Lean](https://github.com/QuantConnect/Lean)                   |


### **Market-Data Feeds**

Provides access to real-time and historical financial market data:

* Includes prices, volumes, quotes, corporate actions, and news
* Feeds from exchanges, aggregators, or vendors (e.g. Bloomberg, Refinitiv)
* Often normalized and streamed into trading algorithms, dashboards, or risk systems

**Used by**: Front-office traders, quant teams, and back-testing tools.
| Product                   | Description                                             | Licence                                                    | GitHub Link                                                                                |
| ------------------------- | ------------------------------------------------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| **TimeBase CE**           | High-speed tick-data store                              | Apache 2.0                                                 | [https://github.com/finos/TimeBase-CE](https://github.com/finos/TimeBase-CE)               |
| **OpenMAMA**              | Open, middleware-agnostic market-data API               | LGPL 2.1                                                   | [https://github.com/finos/OpenMAMA](https://github.com/finos/OpenMAMA)                     |
| **Chronicle Queue + FIX** | Micro-second IPC queue; optional low-latency FIX codecs | Apache 2.0 (Queue); FIX engine is commercial/closed-source | [https://github.com/OpenHFT/Chronicle-Queue](https://github.com/OpenHFT/Chronicle-Queue)   |
| **finance-go**            | Go library for real-time & historical market data       | MIT                                                        | [https://github.com/piquette/finance-go](https://github.com/piquette/finance-go)           |

### **Order-Routing**

Manages the distribution of orders to exchanges, ECNs, or brokers:

* Implements smart order routing (SOR) to optimize fill rates and costs
* Handles venue-specific constraints (latency, fees, regulation)
* Often integrated into EMS or custom algorithmic trading engines

**Includes**: Pre-trade risk checks, regulatory controls (e.g. MiFID II), and analytics on route efficiency.

| Product                  | Description                                                                                  | Licence    | GitHub Link                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **Lean Broker Adapters** | Broker-connector toolkit (example: Interactive Brokers plugin) for the LEAN trading platform | Apache 2.0 | [https://github.com/QuantConnect/Lean.Brokerages.InteractiveBrokers](https://github.com/QuantConnect/Lean.Brokerages.InteractiveBrokers) |

---

### **Clearing & Settlement**

Post-trade processing to finalize securities transactions:

* **Clearing**: Matching and netting trades, calculating margin, and risk exposure
* **Settlement**: Final transfer of cash and securities (e.g. T+2, DvP)

**Systems involved**: CCPs, custodians, and CSDs (e.g. Euroclear, DTCC)

**Includes**: Trade confirmations, reconciliations, and corporate actions.

| Product                              | Description                                                                                         | Licence    | GitHub Link                                                                        |
| ------------------------------------ | --------------------------------------------------------------------------------------------------- | ---------- | ---------------------------------------------------------------------------------- |
| **Hyperledger Fabric**               | Permissioned DLT framework for clearing & settlement (modular consensus, pluggable smart-contracts) | Apache 2.0 | [https://github.com/hyperledger/fabric](https://github.com/hyperledger/fabric)     |
| **Corda OS**                         | Notary-based settlement ledger for bilateral & multilateral workflows                               | Apache 2.0 | [https://github.com/corda/corda](https://github.com/corda/corda)                   |
| **DAML Ledger (digital-asset/daml)** | Smart-contract runtime & SDK for multi-party settlement on permissioned ledgers                     | Apache 2.0 | [https://github.com/digital-asset/daml](https://github.com/digital-asset/daml)     |
| **Stellar Core**                     | Distributed cross-border token-settlement node (anchors & on-ledger exchange)                       | Apache 2.0 | [https://github.com/stellar/stellar-core](https://github.com/stellar/stellar-core) |

---

### **Collateral Management**

Manages assets pledged to reduce credit risk in derivative and repo markets:

* Margin calculation (initial, variation), eligibility rules, and optimization
* Supports OTC and centrally cleared trades
* Integration with trading, risk, and treasury systems

**Critical for**: Regulatory compliance (e.g. EMIR, Dodd-Frank), liquidity planning, and risk mitigation.

| Product                       | Description                                                                  | Licence                                                | GitHub Link                                                                                                  |
| ----------------------------- | ---------------------------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| **OpenGamma Strata**          | SIMM-ready risk & margin utilities (trade models, market data, analytics)    | Apache 2.0 ([github.com][1], [strata.opengamma.io][2]) | [https://github.com/OpenGamma/Strata](https://github.com/OpenGamma/Strata)                                   |
| **ORE Collateral**            | QuantLib-based margin engine inside the Open Source Risk Engine (ORE)        | BSD 3-Clause (modified)                                | [https://github.com/OpenSourceRisk/Engine](https://github.com/OpenSourceRisk/Engine)                         |
| **QuantLib**                  | Pricing library with collateral & CSA models                                 | BSD 3-Clause                                           | [https://github.com/lballabio/QuantLib](https://github.com/lballabio/QuantLib)                               |
| **PyPortfolioOpt Collateral** | Python                                                                       | MIT                                                    | [https://github.com/robertmartin8/PyPortfolioOpt](https://github.com/robertmartin8/PyPortfolioOpt)           |
