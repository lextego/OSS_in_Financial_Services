## Payments & Transfers

---

### **RTGS / ACH**

Core interbank clearing systems used for settlement:

* **RTNS / RTGS (Real-Time Net Settlement / Real-Time Gross Settlement)**: High-value, real-time, irrevocable payments between banks and Non Banks (e.g. Fedwire, TARGET2).
* **ACH (Automated Clearing House)**: Batch-processed, lower-cost, delayed settlement for payroll, utility bills, etc.

**Features**: Clearing integration, ISO 20022 messaging, reconciliation, and settlement position tracking.

| Product       | Description                                                                    | Licence    | GitHub Link                                                                    |
| ------------- | ------------------------------------------------------------------------------ | ---------- | ------------------------------------------------------------------------------ |
| **Mojaloop**  | Instant-payment / RTNS / RTGS hub (central ledger, settlement & API set)       | Apache 2.0 | [https://github.com/mojaloop](https://github.com/mojaloop)                     |
| **Moov ACH**  | Go-based ACH *micro-service* gateway for origination/download, webhooks & SFTP | Apache 2.0 | [https://github.com/moov-io/achgateway](https://github.com/moov-io/achgateway) |
| **rtp-20022** | Go structs & helpers for Real-Time Payments ISO 20022 messages                 | Apache 2.0 | [https://github.com/moov-io/rtp20022](https://github.com/moov-io/rtp20022)     |

### **Instant Payments**

Real-time, low-latency payment systems supporting 24/7 transactions:

* Consumer or business payments cleared in seconds (e.g. UPI in India, PIX in Brazil, SEPA Instant in EU).
* Uses push-payment mechanisms with request-to-pay options.

**Requires**: High-availability infrastructure, fraud detection, and payment scheme compliance.

| Product                            | Description                                                                  | Licence    | GitHub Link                                                                        |
| ---------------------------------- | ---------------------------------------------------------------------------- | ---------- | ---------------------------------------------------------------------------------- |
| **Mojaloop**                       | DFSP-model instant-payments hub (ISO 20022 APIs, settlement, central ledger) | Apache 2.0 | [https://github.com/mojaloop](https://github.com/mojaloop)                         |
| **Rippled**                        | XRP Ledger server for real-time settlement & on-ledger exchange              | ISC        | [https://github.com/XRPLF/rippled](https://github.com/XRPLF/rippled)               |
| **Lightning-Network Daemon (LND)** | Go implementation of the Bitcoin Lightning Network (Layer 2)                 | MIT        | [https://github.com/lightningnetwork/lnd](https://github.com/lightningnetwork/lnd) |
| **Moov PayGate**                   | ACH / Same-Day ACH gateway with REST API & SFTP integration                  | Apache 2.0 | [https://github.com/moov-io/paygate](https://github.com/moov-io/paygate)           |

### **Card Payments**

Covers the full lifecycle of debit, credit, and prepaid card transactions:

* Transaction authorization, switching, settlement, and dispute handling
* Integration with card networks (Visa, Mastercard, etc.)
* Support for 3D Secure, EMV, and tokenized payments (e.g. Apple Pay, Google Pay)

**Includes**: Merchant acquiring, interchange calculation, and PCI-DSS compliance.

| Product           | Description                                             | Licence                      | GitHub Link                                                                          |
| ----------------- | ------------------------------------------------------- | ---------------------------- | ------------------------------------------------------------------------------------ |
| **Hyperswitch**   | Community card-payments switch / multi-PSP router       | Apache 2.0  | [https://github.com/juspay/hyperswitch](https://github.com/juspay/hyperswitch)       |

### **Cross-border Payments**

International payment flows with currency conversion and compliance:

* SWIFT-based wire transfers or alternative rails (e.g. Ripple, Interledger)
* FX handling, correspondent banking, and compliance screening (e.g. sanctions, AML)

**Focus areas**: Speed, cost transparency (e.g. GPI), and error resolution across jurisdictions.

| Product                                   | Description                                                      | Licence                      | GitHub Link                                                                                    |
| ----------------------------------------- | ---------------------------------------------------------------- | ---------------------------- | ---------------------------------------------------------------------------------------------- |
| **Interledger Protocol (interledger-rs)** | Value-packet routing protocol implementation in Rust             | Apache 2.0  | [https://github.com/interledger/interledger-rs](https://github.com/interledger/interledger-rs) |
| **Stellar Core**                          | Distributed cross-border ledger (XLM network node)               | Apache 2.0  | [https://github.com/stellar/stellar-core](https://github.com/stellar/stellar-core)             |
| **Rippled**                               | XRP Ledger server powering RippleNet rails                       | ISC         | [https://github.com/XRPLF/rippled](https://github.com/XRPLF/rippled)                           |
| **Lightning-Network Daemon (lnd)**        | Bitcoin Layer-2 implementation enabling real-time micro-payments | MIT         | [https://github.com/lightningnetwork/lnd](https://github.com/lightningnetwork/lnd)             |

### **Open Banking / API Gateways**

APIs enabling third-party payment initiation or data access under regulated frameworks:

* PSD2 (EU), Open Banking UK, or similar mandates elsewhere
* Provides secure, standardized APIs for payments and account access
* Consent management and secure customer authentication (SCA)

**Also used by**: Fintech aggregators, neobanks, and embedded finance providers.

| Product                              | Description                                                                                                      | Licence                                       | GitHub Link                                                                                                      |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Open Bank Project (OBP-API)**      | > 400 reference REST/PSD2 endpoints for accounts, payments, entitlements, metadata, etc.                         | AGPL v3 (dual-licence)       | [https://github.com/OpenBankProject/OBP-API](https://github.com/OpenBankProject/OBP-API)                         |
| **WSO2 Open Banking Accelerator**    | PSD2/Open-Banking toolkit (AIS/PIS consent, TPP onboarding, strong-customer-auth flows)                          | Apache 2.0  | [https://github.com/wso2/financial-services-accelerator](https://github.com/wso2/financial-services-accelerator) |
| **ForgeRock AM – Community Edition** | Access-management (IAM, SSO, OAuth/OIDC) with open-banking accelerators; newer enterprise builds are proprietary | CDDL 1.0 (community)         | [https://github.com/ForgeRock/openam-community-edition](https://github.com/ForgeRock/openam-community-edition)   |
| **Gringotts**                        | Unified API/SDK that normalises dozens of payment-gateway APIs under one interface                               | MIT                          | [https://github.com/aviabird/gringotts](https://github.com/aviabird/gringotts)                                   |

---

### **Wallets**

Digital or mobile wallets used for storing balances and initiating payments:

* Closed-loop or open-loop solutions
* Integration with POS, QR codes, P2P transfers, and bill payments
* May include KYC, top-up, and cash-out features

**Examples**: Paytm, M-Pesa, Alipay, Google Pay.
 
| Product                   | Description                                   | Licence                                  | GitHub Link                                                                                                |
| ------------------------- | --------------------------------------------- | ---------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **AlphaWallet**           | Ethereum ERC-20/721 mobile wallet             | MIT                     | [https://github.com/AlphaWallet/alpha-wallet-android](https://github.com/AlphaWallet/alpha-wallet-android) |
| **Electrum**              | Lightweight Bitcoin wallet (desktop & mobile) | MIT                     | [https://github.com/spesmilo/electrum](https://github.com/spesmilo/electrum)                               |
| **Copay (Bitpay Wallet)** | Multi-sig BTC/BCH wallet                      | MIT                     | [https://github.com/bitpay/wallet](https://github.com/bitpay/wallet)                                       |
| **BlueWallet**            | Bitcoin & Lightning mobile wallet             | MIT                     | [https://github.com/BlueWallet/BlueWallet](https://github.com/BlueWallet/BlueWallet)                       |
| **Mycelium**              | Android Bitcoin wallet                        | MS-RSL (mixed licence)  | [https://github.com/mycelium-com/wallet-android](https://github.com/mycelium-com/wallet-android)           |
