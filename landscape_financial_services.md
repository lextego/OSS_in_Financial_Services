The following is a “map of the maps” for identifying the various financial service business maps. It's goal is to create a **canonical list of functional areas inside financial-services firms**.  This map is intended to align the already taxonomies already trusted, whilst creating a scaffolding on which we can start hanging specific open-source projects. 

## Reference taxonomies the industry already trusts

| Who publishes it                | Scope                                             | Why you might use it                                                                                                                                                         | Pointer                                                                                                                              |
| ------------------------------- | ------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **BIAN Service Landscape v32**  | Universal banking (retail, commercial & treasury) | 322 “Service Domains” organised into business-capability layers; used by major banks as a common language for target architectures & API design                              | “All 322 service domains completed … 250 semantic APIs” ([BIAN][1])                                                                  |
| **ISO 20022 Business Areas**    | All payments & securities messages worldwide      | 23 top-level business areas (CARD, PAIN, PACS, CAMT, SEEV, FXTI …); gives you a clean, cross-segment vocabulary that regulators and market-infrastructures already recognise | Example extract shows CARD PAYMENTS, PAYMENTS & CASH, SECURITIES, FX, DERIVATIVES, … ([ISO20022][2])                                 |
| **ACORD Capability Model**      | Insurance (Life, P\&C, Re/Insurance)              | Standard set of insurer capabilities – e.g. Business Management, Channel Management, Contract Administration, Claims, Finance, Sales – widely used by carriers & vendors     | “Top-level capabilities • Business Management • Channel Management … • Claims • Finance • Product • Sales” ([www.slideshare.net][3]) |
| **FINOS Open-Source Landscape** | Capital-markets & FS infrastructure               | Groups open-source projects into categories such as *Data / Business Logic*, *Cloud & DevOps*, *Common Domain Model*, etc.; handy when you start mapping actual OSS assets   | Card-mode view listing projects under *Data / Business Logic* ([landscape.finos.org][4])                                             |

## A consolidated “starter” capability catalogue

Below is a pragmatic roll-up that blends the four sources above.  It’s meant to be *sector-agnostic* at the top level but still granular enough to pin real projects onto it.

| Level-1 Area                   | Example sub-areas you’ll see in the reference models                                                          |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------- |
| **Customer & Channels**        | Onboarding/KYC, CRM, Branch/Contact-Centre, Digital Banking, Mobile, Agency/Broker Portals                    |
| **Products & Accounts**        | Core Banking/Ledger, Policy Administration (insurance), Portfolio Management, Deposit & Savings, Card Issuing |
| **Origination & Servicing**    | Loan/Policy Origination, Underwriting, Credit Decisioning, Collections, Claims Handling                       |
| **Payments & Transfers**       | RTGS / ACH, Instant Payments, Card Payments, Cross-border, Open Banking / API Gateways, Wallets                                 |
| **Trading & Investment**       | OMS/EMS, Market-Data Feeds, Order-Routing, Clearing & Settlement, Collateral Mgmt                             |
| **Treasury & Liquidity**       | Cash-flow Forecasting, ALM, Funding & Capital, FX & Money-Markets                                             |
| **Risk, Finance & Compliance** | Credit/Market/Operational Risk, Actuarial Models, Regulatory Reporting, AML/Fraud, Finance/GL                 |
| **Data & Analytics**           | Reference/Data Hubs, Data Lineage, AI/ML Workbenches, BI Dashboards                                           |
| **Enterprise Services**        | Identity & Access, Workflow/BPM, Document Management, DevSecOps, Cloud/Infrastructure, Observability          |


*(If needed it is possible to slice this table one column deeper using the service-domain lists from BIAN or the message areas from ISO 20022 whenever extra precision is needed.)*

## How to turn the taxonomy into an OSS catalog

1. **Select your backbone**
   *Retail & corporate banking* → BIAN | *Capital-markets* → ISO 20022 + FINOS | *Insurance* → ACORD
2. **Create a matrix** of “Capability × Open-Source project”.  Start with high-impact buckets such as Core-Banking (e.g. Apache Fineract), Digital Channels (e.g. Backbase-OSS components), Market-Data (e.g. TimeBase CE) and work outward.
3. **Capture meta-data** (licence, language, governance maturity, last commit) so stakeholders can judge enterprise readiness.
4. **Iterate with SMEs.**  Ask domain architects or ops leads to sanity-check mappings—this uncovers hidden gaps early.
5. **Publish & keep fresh.**  FINOS releases an updated landscape every few months; scheduling a quarterly sweep keeps your catalog current.

Using these recognised models as your foundation will save you weeks of debate about naming and scope—and will make it far easier for engineers, vendors and regulators to understand where each open-source component fits.

[1]: https://bian.org/deliverables/service-landscape/ "Service Landscape - BIAN"
[2]: https://www.iso20022.org/sites/default/files/documents/D7/ISO20022_BusinessAreas.pdf "Business areas"
[3]: https://www.slideshare.net/havoc2003/the-acord-framework-an-insurance-enterprise-architecture-2011pdf "The Acord Framework - An Insurance Enterprise Architecture (2011).pdf"
[4]: https://landscape.finos.org/?view-mode=card&classify=category&sort-by=name&sort-direction=asc#applications--symphony-ecosystem "FINOS Landscape"

