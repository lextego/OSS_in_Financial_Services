## Origination & Servicing

### **Loan / Policy Origination**

End-to-end process of onboarding new credit or insurance customers. It includes:

* Application capture (online, branch, agent)
* Document submission and identity verification
* Eligibility checks and initial scoring
* Pre-approval, offer presentation, and acceptance

**Typical features**: Workflow orchestration, credit bureau integration, e-signatures, and data validation.

| Product                  | Description                                                | Licence    | GitHub Link                                                                                                  |
| ------------------------ | ---------------------------------------------------------- | ---------- | ------------------------------------------------------------------------------------------------------------ |
| **OpenCBS LOS**          | Workflow-driven loan-origination solution                  | GPL v3     | [https://github.com/OpenCBS/Loan-Origination-Solution](https://github.com/OpenCBS/Loan-Origination-Solution) |
| **Fineract CN Credit**   | Micro-service loan-origination (part of Fineract CN)       | Apache 2.0 | [https://github.com/apache/fineract-cn-portfolio](https://github.com/apache/fineract-cn-portfolio)           |
| **Mifos X Origination**  | Inclusive-finance loan-origination on the Mifos X platform | MPL 2.0    | [https://github.com/openMF/](https://github.com/openMF/)                                       |
| **Odoo Loan Management** | Loan module (with OCR) for Odoo                            | GPl V3     | [https://github.com/odoo/odoo](https://github.com/odoo/odoo)                                                 |
| **ERPNext Loans**        | Loan onboarding, schedules & lifecycle on ERPNext          | GPL v3     | [https://github.com/frappe/lending](https://github.com/frappe/lending)                                       |

### **Underwriting**

Risk assessment and pricing decisioning engine used in both lending and insurance:

* Rule-based or machine learning underwriting decisions
* Incorporates risk factors, scoring models, and exception handling
* Includes automated or assisted decisioning with audit trail

**Used by**: Credit teams, underwriters, or decision engines in microfinance, consumer lending, and insurance.

| Product                    | Description                          | Licence                       | GitHub Link                                                                                      |
| -------------------------- | ------------------------------------ | ----------------------------- | ------------------------------------------------------------------------------------------------ |
| **Drools**                 | Rules/DMN engine                     | Apache 2.0                    | [https://github.com/kiegroup/drools](https://github.com/kiegroup/drools)                         |
| **OpenL Tablets**          | Excel-style business-rules platform  | LGPL 2.1                      | [https://github.com/openl-tablets/openl-tablets](https://github.com/openl-tablets/openl-tablets) |
| **Open Risk Engine (ORE)** | Credit/market-risk analytics library | Modified BSD (BSD 3-Clause) , | [https://github.com/OpenSourceRisk/Engine](https://github.com/OpenSourceRisk/Engine)             |


### **Credit Decisioning**

Focused purely on deciding whether to approve or decline a credit application:

* Scorecard evaluation (e.g. FICO, internal models)
* Policy rules (e.g. debt-to-income, employment)
* Real-time data pulls from bureaus, bank statements, or alternate data

**Often integrated into**: Loan origination platforms or standalone rules engines (e.g. Drools, OpenL Tablets).

Example open source companies: 

| Product           | Description                                               | Licence                        | GitHub Link                                                                                      |
| ----------------- | --------------------------------------------------------- | ------------------------------ | ------------------------------------------------------------------------------------------------ |
| **Drools**        | Integrated with LOS as a rules / DMN engine               | Apache 2.0    | [https://github.com/kiegroup/drools](https://github.com/kiegroup/drools)                         |
| **OpenL Tablets** | Decision-table platform (Excel-style business rules)      | LGPL 2.1      | [https://github.com/openl-tablets/openl-tablets](https://github.com/openl-tablets/openl-tablets) |
| **H2O-3**         | Open-source ML scoring engine (distributed, in-memory)    | Apache 2.0    | [https://github.com/h2oai/h2o-3](https://github.com/h2oai/h2o-3)                                 |
| **Scikit-learn**  | Python ML toolkit; credit-risk packs available            | BSD 3-Clause  | [https://github.com/scikit-learn/scikit-learn](https://github.com/scikit-learn/scikit-learn)     |

---

### **Collections**

Tools and workflows for recovering overdue payments and managing delinquency:

* Automated reminders, dialer queues, and repayment plans
* Integration with core ledger, CRM, and contact centers
* Escalation paths (soft collections, legal, write-off)

**Advanced features**: Risk-based segmentation, promise-to-pay tracking, and compliance reporting.

| Product                     | Description                                    | Licence                         | GitHub Link                                                                                                              |
| --------------------------- | ---------------------------------------------- | ------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| **Odoo Collections**        | AR & dunning module ( `account_followup` )     | LGPL v3  | [https://github.com/odoo/odoo](https://github.com/odoo/odoo)                                            |
| **ERPNext Debt Collection** | Configurable dunning for overdue invoices      | GPL v3         | [https://github.com/frappe/erpnext](https://github.com/frappe/erpnext)                                  |
| **SuiteCRM Collections**    | Collections workflow via Cases & Tasks         | AGPL v3        | [https://github.com/salesagility/SuiteCRM](https://github.com/salesagility/SuiteCRM)                    |
| **Dolibarr Follow-up**      | Overdue-invoice reminder (Follow-up) module    | GPL v3       | [https://github.com/Dolibarr/dolibarr](https://github.com/Dolibarr/dolibarr)                          |

---

### **Claims Handling**

Primarily used in insurance, this refers to processing customer claims:

* Submission intake (online, mobile, agent)
* Validation, triage, and fraud detection
* Adjuster workflows, payout approvals, and settlement

**Can also include**: Integration with external data (accident reports, medical records), rules engines, and customer communications.

| Product                    | Description                                                                | Licence                                             | GitHub Link                                                                                                                       |
| -------------------------- | -------------------------------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **openIMIS Claims**        | Health-insurance FNOL & claims processing module for the openIMIS platform | AGPL v3                            | [https://github.com/openimis/openimis-be-claim_py](https://github.com/openimis/openimis-be-claim_py)                             |
| **ERPNext Claims**         | Policy-linked claims management inside ERPNext                             | GPL v3                             | [https://github.com/frappe/erpnext](https://github.com/frappe/erpnext)                                           |
| **openUnderwriter Claims** | P\&C claims module within the OpenUnderwriter suite                        | GPL v2                        | *Not on GitHub – code on Bitbucket:* [https://bitbucket.org/openunderwriter](https://bitbucket.org/openunderwriter) |
