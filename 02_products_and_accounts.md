
## Products & Accounts

### Digital Banking

Front-end platforms for retail or business banking. They typically include:

* Web/mobile access to accounts, payments, and statements
* APIs for customer authentication and transaction workflows
* Integration with core banking and payment processors
* Support for PSD2/Open Banking interfaces

| Product               | Description                                                                      | Licence                | GitHub Link                                                                          |
| --------------------- | -------------------------------------------------------------------------------- | ---------------------- | ------------------------------------------------------------------------------------ |
| **Apache Fineract**   | Headless core-banking & GL engine with OpenAPI spec                              | Apache-2.0             | [https://github.com/apache/fineract](https://github.com/apache/fineract)             |
| **Mifos X**           | Digital-finance platform built on Fineract (loans/savings, mobile & wallet apps) | Apache-2.0 Apache-2.0  | [https://github.com/openMF](https://github.com/openMF)                               |
| **Cyclos**            | Retail internet/mobile banking plus card & remittance modules                    | MIT                    | [https://github.com/cyclosproject](https://github.com/cyclosproject)                 |
| **Open Bank Project** | PSD2 / Open-Banking–ready API gateway with 400 + reference endpoints             | AGPL-v3 (dual-licence) | [https://github.com/OpenBankProject](https://github.com/OpenBankProject)             |
| **Mojaloop**          | Instant-payment switch/hub (DFSP model)                                          | Apache-2.0             | [https://github.com/mojaloop](https://github.com/mojaloop)                           |
| **Stellar**      | Distributed ledger for wallet balances & tokenised deposits                      | Apache-2.0             | [https://github.com/stellar](https://github.com/stellar)   |

### **Core Banking / Ledger**

Systems that handle the foundational records of financial institutions, including:

* General ledger and sub-ledger accounting
* Real-time balances and transaction posting
* Product factory for loans, deposits, and accounts
* APIs for integration with channels and services

**Typical functions**: Customer accounts, product lifecycle management, transaction journals, regulatory reporting hooks.

| Product             | Description                                                               | Licence    | GitHub Link                                                                              |
| ------------------- | ------------------------------------------------------------------------- | ---------- | ---------------------------------------------------------------------------------------- |
| **Apache Fineract** | Modular CBS & OpenAPI spec                                                | Apache-2.0 | [https://github.com/apache/fineract](https://github.com/apache/fineract)                 |
| **Stellar Core**    | High-throughput distributed ledger                                        | Apache-2.0 | [https://github.com/stellar/stellar-core](https://github.com/stellar/stellar-core)       |
| **Moov Accounts**   | Go-based general-ledger micro-service                                     | Apache-2.0 | [https://github.com/moov-io/accounts](https://github.com/moov-io/accounts)               |
| **Cyclos**          | Account & wallet balances with web/mobile UI                              | MIT        | [https://github.com/cyclosproject](https://github.com/cyclosproject)                     |
| **OpenCBS**         | Lightweight CBS for MFIs/SACCOs                                           | GPL-3.0    | [https://github.com/OpenCBS/OpenCBS-Cloud](https://github.com/OpenCBS/OpenCBS-Cloud)     |
| **Tigerbeetle**     | Distributed financial accounting database for high performance and safety | Apache-2.0 | [https://github.com/tigerbeetle/tigerbeetle](https://github.com/tigerbeetle/tigerbeetle) |

### **Policy Administration (Insurance)**

Back-office systems for managing insurance contracts and coverage. They support:

* Policy creation, renewal, endorsement, and termination
* Coverage terms, riders, and premium calculations
* Integration with underwriting, claims, and billing systems

**Common in**: Life, health, and property insurance environments.

| Product                        | Description                                                | Licence | GitHub Link                                                                                                                   |
| ------------------------------ | ---------------------------------------------------------- | ------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **openIMIS**                   | Open-source health-insurance administration platform       | AGPL v3 | [https://github.com/openimis](https://github.com/openimis/)                                     |
| **openUnderwriter**            | Policy & product configurator for life / P\&C insurers     | GPL v2  | [https://bitbucket.org/openunderwriter](https://bitbucket.org/openunderwriter) |

### **Portfolio Management**

Used by wealth managers, investment firms, and insurers to manage:

* Client portfolios and holdings across asset classes
* Rebalancing, performance tracking, and reporting
* Risk-return analysis and regulatory compliance (e.g. MiFID II)

**Tools may include**: Portfolio modeling, customer profiling, asset allocation, and benchmark comparison.

| Product                   | Description                                          | Licence                        | GitHub Link                                                                                              |
| ------------------------- | ---------------------------------------------------- | ------------------------------ | -------------------------------------------------------------------------------------------------------- |
| **QuantLib**              | Quantitative-finance library for pricing & risk      | BSD 3-Clause  | [https://github.com/lballabio/QuantLib](https://github.com/lballabio/QuantLib)                           |
| **OpenGamma Strata**      | Risk & analytics toolkit for OTC and listed products | Apache 2.0    | [https://github.com/OpenGamma/Strata](https://github.com/OpenGamma/Strata)                               |
| **Lean**                  | Algorithmic-trading/portfolio back-testing engine    | Apache 2.0    | [https://github.com/QuantConnect/Lean](https://github.com/QuantConnect/Lean)                             |
| **Portfolio Performance** | Desktop portfolio tracker and performance analytics  | EPL 1.0       | [https://github.com/portfolio-performance/portfolio](https://github.com/portfolio-performance/portfolio) |
| **Ghostfolio**            | Web-based DIY wealth tracker                         | AGPL v3       | [https://github.com/ghostfolio/ghostfolio](https://github.com/ghostfolio/ghostfolio)                     |

### **Deposit & Savings**

Functional area focused on managing customer deposit products, such as:

* Demand deposits (checking accounts), time deposits (CDs), and savings accounts
* Interest calculation, maturity schedules, and early withdrawal logic
* KYC linkage, transactional limits, and account-level analytics

Often part of broader core banking systems but may be modular in microservice architectures.


| Product              | Description                                             | Licence        | GitHub Link                                                                              |
| -------------------- | ------------------------------------------------------- | -------------- | ---------------------------------------------------------------------------------------- |
| **Fineract Savings** | Modular deposit-product engine built on Apache Fineract | Apache 2.0     | [https://github.com/apache/fineract](https://github.com/apache/fineract)                 |
| **Cyclos Deposits**  | Savings / wallet-balance modules with web & mobile UI   | MIT (frontend) | [https://github.com/cyclosproject](https://github.com/cyclosproject)                     |
| **Mifos X Savings**  | Inclusive-finance deposit accounts in Mifos X           | MPL 2.0        | [https://github.com/openMF/mifos-x](https://github.com/openMF/mifos-x)                   |
| **TigerBeetle**      | Ultra-fast distributed double-ledger database           | Apache 2.0     | [https://github.com/tigerbeetle/tigerbeetle](https://github.com/tigerbeetle/tigerbeetle) |
| **OpenCBS Deposits** | Deposit products for MFIs / SACCOs on OpenCBS           | GPL 3.0        | [https://github.com/OpenCBS/OpenCBS-Cloud](https://github.com/OpenCBS/OpenCBS-Cloud)     |

### **Card Products**

| Product                   | Description                                        | Licence                    | GitHub Link                                                                                    |
| ------------------------- | -------------------------------------------------- | -------------------------- | ---------------------------------------------------------------------------------------------- |
| **OpenEMV**               | Open-source EMV smart-card stack                   | LGPL 2.1                   | [https://github.com/openemv/emv-utils](https://github.com/openemv/emv-utils)                   |
| **Cardpeek**              | Chip-card inspection / decoding tool               | GPL v3                     | [https://github.com/L1L1/cardpeek](https://github.com/L1L1/cardpeek)                           |
| **OpenSC**                | Smart-card middleware & tools                      | LGPL 2.1                   | [https://github.com/OpenSC/OpenSC](https://github.com/OpenSC/OpenSC)                           |
| **hyperswitch**           | Rust-based multi-PSP payments router               | Apache-2.0                 | [https://github.com/juspay/hyperswitch](https://github.com/juspay/hyperswitch)                 |
| **JReactive-8583**        | Netty-based ISO 8583 client/server (Java/Kotlin)   | Apache-2.0                 | [https://github.com/kpavlov/jreactive-8583](https://github.com/kpavlov/jreactive-8583)         |
| **moov-io/iso8583**       | Go implementation for packing/unpacking ISO 8583   | Apache-2.0                 | [https://github.com/moov-io/iso8583](https://github.com/moov-io/iso8583)                       |
| **iso8583-connection**    | Go ISO 8583 connection handler with pooling        | Apache-2.0                 | [https://github.com/moov-io/iso8583-connection](https://github.com/moov-io/iso8583-connection) |
| **Omnipay**               | Framework-agnostic PHP payment-gateway abstraction | MIT                        | [https://github.com/thephpleague/omnipay](https://github.com/thephpleague/omnipay)             |

