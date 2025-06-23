## Risk, Finance & Compliance

### **Credit / Market / Operational Risk**

Manages the institution’s exposure to various forms of financial and non-financial risk:

* **Credit Risk**: Assesses counterparty default risk using scorecards, PD/LGD models, exposure limits, and collateral.
* **Market Risk**: Tracks sensitivities to interest rates, FX, equities, and commodities using VaR, stress testing, and scenario analysis.
* **Operational Risk**: Evaluates risks from internal processes, systems, people, or external events (e.g. fraud, cyberattacks, process failures).

**Outputs**: Risk-weighted assets (RWA), capital requirements, loss scenarios, and risk dashboards.

| Product                           | Description                                      | Licence               | GitHub Link                                                                                        |
| --------------------------------- | ------------------------------------------------ | --------------------- | -------------------------------------------------------------------------------------------------- |
| **OpenGamma Strata**              | SIMM & VaR analytics library (Java)              | Apache 2.0            | [https://github.com/OpenGamma/Strata](https://github.com/OpenGamma/Strata)                         |
| **Open Source Risk Engine (ORE)** | QuantLib-based pricing & risk platform           | Modified BSD 3-Clause | [https://github.com/OpenSourceRisk/Engine](https://github.com/OpenSourceRisk/Engine)               |
| **QuantLib**                      | Core quantitative-finance/risk analytics library | BSD 3-Clause          | [https://github.com/lballabio/QuantLib](https://github.com/lballabio/QuantLib)                     |
| **OpenRisk-Quant**                | Python risk-quantification toolkit               | Apache 2.0            | [https://github.com/Netflix-Skunkworks/riskquant](https://github.com/Netflix-Skunkworks/riskquant) |

---

### **Actuarial Models**

Used primarily by insurance and pensions to price products and predict long-term liabilities:

* Life expectancy, morbidity, lapse rate, and claims frequency models
* Supports pricing, reserving (e.g. IBNR), solvency assessments, and reinsurance planning
* Often implemented via statistical programming (e.g. R, SAS) or domain-specific tools

**Feeds into**: IFRS 17/US GAAP actuarial valuations, capital modeling, and product design.

| Product                   | Description                                                           | Licence                                      | GitHub Link                                                                                            |
| ------------------------- | --------------------------------------------------------------------- | -------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| **ChainLadder (R)**       | Claims-triangle reserving and stochastic loss-development models      | GPL v3                     | [https://github.com/mages/ChainLadder](https://github.com/mages/ChainLadder)                           |
| **Prophet**               | Additive-model time-series/actuarial projection system (Python/R)     | MIT                        | [https://github.com/facebook/prophet](https://github.com/facebook/prophet)                             |
| **MortalityTables (R)**   | Global mortality-table datasets and utilities for actuarial work      | GPL (≥ 2)           | [https://github.com/cran/MortalityTables](https://github.com/cran/MortalityTables)                     |

---

### **Regulatory Reporting**

Systems that generate mandatory reports for regulators and supervisory bodies:

* Covers liquidity (LCR, NSFR), capital adequacy (COREP, FINREP), and financial statements
* Supports jurisdiction-specific formats (e.g. XBRL, XML) and submission cycles
* Ensures data lineage, traceability, and auditability

**Can include**: Report generators, validation engines, and data quality checks.

| Product                                                         | Description                                                                                                                                               | Licence                                               | GitHub Link                                                                                                                      |
| --------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **FINOS Open RegTech – Open-Source Regulatory Reporting (ORR)** | Rulebook/validation engine and reference implementation for converting ISDA DRR & other regulatory logic into executable Spark jobs and ISO 20022 output. | Apache 2.0                           | [https://github.com/finos-labs/opensource-reg-reporting](https://github.com/finos-labs/opensource-reg-reporting)                 |
| **Google Reg-Reporting Blueprint**                              | BigQuery-centric solution architecture, Terraform modules and dbt templates that automate ingestion, transformation and generation of regulatory reports. | Apache 2.0                         | [https://github.com/GoogleCloudPlatform/reg-reporting-blueprint](https://github.com/GoogleCloudPlatform/reg-reporting-blueprint) |
| **Suade RegCore (FIRE Data Standard)**                          | Open taxonomy and rules engine for granular regulatory data exchange; provides JSON schemas, validators and code samples.                                 | Apache 2.0          | [https://github.com/SuadeLabs/fire](https://github.com/SuadeLabs/fire)                                                           |
| **Open CDM (ISDA Common Domain Model)**                         | Machine-readable model of financial products, events and lifecycle processes used across DLT, risk and reporting stacks.                                  | Community Specification License 1.0  | [https://github.com/finos/common-domain-model](https://github.com/finos/common-domain-model)                                     |
| **fincen**                                                      | Go library and REST server for creating, validating and batching FinCEN BSA XML filings (SAR, CTR, FBAR, etc.).                                           | Apache 2.0                           | [https://github.com/moov-io/fincen](https://github.com/moov-io/fincen)                                                           |

## Risk, Finance & Compliance – AML / Fraud & Transaction Monitoring (extract)

This capability area monitors customer and counter‑party behaviour to uncover sanctions breaches, money‑laundering typologies, fraud patterns and cyber‑crime in real time, then drives investigation workflows and statutory reporting.

### Key capability slices

* **AML**: Screening (sanctions, PEPs), transaction monitoring, SAR/STR filing
* **Fraud**: Real-time detection using rules, heuristics, and ML (e.g. synthetic identity, account takeover)
* **Screening** – sanctions / PEP / adverse‑media matching using deterministic or fuzzy algorithms.
* **Transaction Monitoring** – behaviour, velocity and anomaly detection across payments, cards, wallets and crypto rails.
* **Screening & Reference Data** – deterministic / fuzzy matching against sanctions, PEP, adverse‑media & intel feeds.
* **Case Management & SAR/STR filing** – investigation workflow, alert triage, narrative capture and e‑filing to FIUs.
* **Regulatory Reporting APIs** – generate XML or ISO 20022 reports for BSA / FATF regimes.

| Product                 | Core focus                                                                                      | Licence                          | GitHub / Site                                                                            |
| ----------------------- | ----------------------------------------------------------------------------------------------- | -------------------------------- | ---------------------------------------------------------------------------------------- |
| **Tazama**              | Real‑time transaction‑monitoring engine (ISO 20022 ingest, rule processors; proven ≈ 2–3 k TPS) | Apache 2.0                       | [tazama.org](https://tazama.org)                                                         |
| **Jube**                | C# / Blazor real‑time AML transaction‑monitoring with UI‑driven rule sets & graph visualiser    | AGPL v3.0                        | [github.com/jube‑home/jube](https://github.com/jube‑home)                                |
| **Marble**              | No‑code rule‑builder & decision engine for fraud/AML with case manager; batch or real‑time      | Elastic License v2               | [github.com/checkmarble/marble](https://github.com/checkmarble/marble)                   |
| **Ezrules**             | Python rule‑engine + UI for authoring/back‑testing AML rules; deployable via Docker/K8s         | Apache 2.0                       | [github.com/sofeikov/ezrules](https://github.com/sofeikov/ezrules)                       |
| **Trench**              | Event‑driven fraud & abuse prevention pipeline with Typescript SDK & web dashboard              | AGPL v3.0                        | [github.com/trytrench/trench](https://github.com/trytrench/trench)                       |
| **Watchman**            | High‑throughput sanctions & PEP screening micro‑service (OFAC, EU, UN, etc.)                    | Apache 2.0                       | [github.com/moov‑io/watchman](https://github.com/moov-io/watchman)                       |
| **OpenSanctions**       | Aggregated open sanctions & PEP data with Graph API & on‑prem search                            | MIT (code) / CC BY‑SA 4.0 (data) | [github.com/opensanctions/opensanctions](https://github.com/opensanctions/opensanctions) |
| **MISP Threat Sharing** | IOC / fraud‑indicator sharing & enrichment platform; integrates with watchlists                 | AGPL v3.0                        | [github.com/MISP/MISP](https://github.com/MISP/MISP)                                     |
| **goAML**               | UNODC FIU platform for STR collection, analysis & dissemination; free to member states          | Freeware (UNODC)                 | [unodc.org/goaml](https://www.unodc.org/unodc/en/global-it-products/goaml.html)          |
| **Moov‑FinCEN**         | Go library & REST API to generate/validate FinCEN SAR/CTR XML for BSA e‑filing                  | Apache 2.0                       | [github.com/moov‑io/fincen](https://github.com/moov-io/fincen)                           |
| **Drools**              | General‑purpose rules/CEP engine used as the policy layer in many AML stacks                    | Apache 2.0                       | [drools.org](https://drools.org) / github.com/apache/incubator‑kie‑drools                |

> **Integration note** – These engines and data feeds draw heavily on the datasets in the *Reference Data Appendix* (sanctions, PEPs, LEI, adverse media). Transaction‑monitoring alerts then feed the *Regulatory Reporting* services for automated SAR/STR generation.

### **Finance / GL (https://General Ledger)**

Handles the financial accounting backbone of the institution:

* Chart of accounts, journal entries, trial balances, and financial statements
* Supports IFRS/GAAP, cost allocations, and multi-currency consolidation
* Integrates with subledgers (e.g. lending, cards) and ERP platforms

**Used by**: CFO office, auditors, and financial controllers.

| Product                 | Description                                                               | Licence         | GitHub Link                                                                              |
| ----------------------- | ------------------------------------------------------------------------- | --------------- | ---------------------------------------------------------------------------------------- |
| **ERPNext**             | Double-entry general-ledger, financial reports & dashboards               | GPL v3          | [https://github.com/frappe/erpnext](https://github.com/frappe/erpnext)                   |
| **Odoo Accounting**     | Multi-ledger bookkeeping with OCR invoice capture                         | LGPL v3         | [https://github.com/odoo/odoo](https://github.com/odoo/odoo)                             |
| **Dolibarr Accounting** | SMB-focused bookkeeping inside Dolibarr ERP/CRM                           | GPL v3          | [https://github.com/Dolibarr/dolibarr](https://github.com/Dolibarr/dolibarr)             |
| **GnuCash**             | Desktop double-entry accounting application                               | GPL v2 or later | [https://github.com/Gnucash/gnucash](https://github.com/Gnucash/gnucash)                 |
| **Ledger-CLI**          | Plain-text command-line accounting tool                                   | BSD 3-Clause    | [https://github.com/ledger/ledger](https://github.com/ledger/ledger)                     |
| **Tigerbeetle**         | Distributed financial accounting database for high performance and safety | Apache-2.0      | [https://github.com/tigerbeetle/tigerbeetle](https://github.com/tigerbeetle/tigerbeetle) |