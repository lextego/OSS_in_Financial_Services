## Treasury & Liquidity

### **Cash-flow Forecasting**

Tools that predict short-, medium-, and long-term cash positions across the institution:

* Aggregates expected inflows/outflows from various business units
* Incorporates payment schedules, loan maturities, investment returns, etc.
* Enables proactive liquidity planning and funding decisions

**Outputs include**: Daily liquidity forecasts, stress scenarios, and coverage ratios (e.g. LCR, NSFR).

| Product                    | Description                                                                                                               | Licence                 | GitHub Link                                                                          |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ----------------------- | ------------------------------------------------------------------------------------ |
| **Open Risk Engine (ORE)** | Quant Lib-based library for multi-curve cash-flow projection, valuation and risk                                          | BSD 3-Clause (modified) | [https://github.com/OpenSourceRisk/Engine](https://github.com/OpenSourceRisk/Engine) |
| **QuantLib Cashflows**     | Helper classes/functions for fixed/floating legs, amortising schedules and other cash-flow models (part of QuantLib core) | BSD 3-Clause            | [https://github.com/lballabio/QuantLib](https://github.com/lballabio/QuantLib)       |
| **cashflowpy**†            | Python toolkit for forecasting and analysing investment cash-flows                                                        | MIT                     | [https://github.com/jdvelasq/cashflows](https://github.com/jdvelasq/cashflows)       |


### **ALM (Asset-Liability Management)**

Manages balance sheet risk and profitability by aligning asset and liability structures:

* Tracks interest rate risk, duration gaps, and repricing schedules
* Models economic value and earnings at risk under different scenarios
* Optimizes yield while ensuring regulatory and liquidity compliance

**Used by**: Treasury desks, balance sheet managers, and risk teams.

| Product          | Description                                                                                   | Licence               | GitHub Link                                                                                        |
| ---------------- | --------------------------------------------------------------------------------------------- | --------------------- | -------------------------------------------------------------------------------------------------- |
| **ORE ALM**      | QuantLib-backed ALM stack inside the Open Source Risk Engine                                  | Modified BSD 3-Clause | [https://github.com/OpenSourceRisk/Engine](https://github.com/OpenSourceRisk/Engine)               |
| **QuantLib ALM** | Duration, convexity and other ALM helpers that ship with QuantLib                             | BSD 3-Clause          | [https://github.com/lballabio/QuantLib](https://github.com/lballabio/QuantLib)                     |                                                                                                
| **RiskQuant**    | Python library from Netflix-Skunkworks for scenario-based ALM modelling & risk quantification | Apache 2.0            | [https://github.com/Netflix-Skunkworks/riskquant](https://github.com/Netflix-Skunkworks/riskquant) |


---

### **Funding & Capital**

Planning and execution of funding strategies and capital adequacy:

* Oversees internal and external funding sources (e.g. interbank, bonds, central bank)
* Tracks cost of capital, capital ratios (CET1, Tier 2), and buffer usage
* Supports Basel III/IV and ICAAP regulatory frameworks

**Functions**: Debt issuance, dividend planning, retained earnings management.

| Product                        | Description                                                                       | Licence               | GitHub Link                                                                              |
| ------------------------------ | --------------------------------------------------------------------------------- | --------------------- | ---------------------------------------------------------------------------------------- |
| **OpenGamma Strata (Capital)** | SIMM-ready capital-calculation utilities inside the Strata risk-analytics library | Apache 2.0            | [https://github.com/OpenGamma/Strata](https://github.com/OpenGamma/Strata)               |
| **QuantLib Capital Tools**     | Basel regulatory-capital formula helpers built on QuantLib                        | BSD 3-Clause          | [https://github.com/lballabio/QuantLib](https://github.com/lballabio/QuantLib)           |
| **ORE Capital Manager**        | VaR / RWA aggregation to capital as part of Open Source Risk Engine               | Modified BSD 3-Clause | [https://github.com/OpenSourceRisk/Engine](https://github.com/OpenSourceRisk/Engine)     |

### **FX & Money-Markets**

Manages foreign exchange transactions and short-term liquidity instruments:

* **FX**: Spot, forward, swap, and option transactions across currencies
* **Money Markets**: Instruments like repos, CPs, CDs, interbank lending
* Provides price discovery, position management, and counterparty risk tracking

**Essential for**: International banks, market-making desks, and institutions managing cross-currency exposures.

| Product             | Description                                                                                      | Licence                         | GitHub Link                                                                        |
| ------------------- | ------------------------------------------------------------------------------------------------ | ------------------------------- | ---------------------------------------------------------------------------------- |
| **QuantLib FX**     | FX-curve construction & pricing helpers that ship with the QuantLib quantitative-finance library | BSD 3-Clause                    | [https://github.com/lballabio/QuantLib](https://github.com/lballabio/QuantLib)     |
| **QuickFIX/J FX**   | Java FIX-messaging engine widely used for low-latency FX order-routing & connectivity            | BSD 2-Clause (QuickFIX licence) | [https://github.com/quickfix-j/quickfixj](https://github.com/quickfix-j/quickfixj) |
| **XChange**         | MIT-licensed Java API covering 60 + crypto/FX exchanges (market-data & trading)                  | MIT                             | [https://github.com/knowm/XChange](https://github.com/knowm/XChange)               |                                                                                  
| **ForexConnect-JS** | FXCM’s ForexConnect API (used via JS/TS wrappers) for trading & market data                      | FXCM EULA / proprietary         | [https://github.com/fxcm/ForexConnectAPI](https://github.com/fxcm/ForexConnectAPI) |
