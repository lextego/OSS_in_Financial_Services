## Data & Analytics

### **Reference / Data Hubs**

Centralized systems for storing and distributing authoritative data across the enterprise:

* **Reference Data**: Legal entity IDs, product codes, currency definitions, calendars, etc.
* **Master Data Management (MDM)**: Customer, account, or counterparty data across systems
* Provides version control, data enrichment, and golden-source governance

**Critical for**: Ensuring consistency across trading, risk, compliance, and reporting systems.

| Product                          | Description                                            | Licence                        | GitHub Link                                                                                    |
| -------------------------------- | ------------------------------------------------------ | ------------------------------ | ---------------------------------------------------------------------------------------------- |
| **Apache Kafka**                 | Streaming backbone for real-time data pipelines        | Apache 2.0                     | [https://github.com/apache/kafka](https://github.com/apache/kafka)                             |
| **DataHub (LinkedIn)**           | Metadata catalog & master-data management platform     | Apache 2.0                     | [https://github.com/datahub-project/datahub](https://github.com/datahub-project/datahub)       |
| **OpenMetadata**                 | Unified data catalog, governance & observability stack | Apache 2.0                     | [https://github.com/open-metadata/OpenMetadata](https://github.com/open-metadata/OpenMetadata) |
| **Trino**                        | Distributed SQL query engine for lake-house analytics  | Apache 2.0                     | [https://github.com/trinodb/trino](https://github.com/trinodb/trino)                           |
| **Postgres Logical (pglogical)** | Logical-replication extension for PostgreSQL hubs      | PostgreSQL License (BSD-style) | [https://github.com/2ndQuadrant/pglogical](https://github.com/2ndQuadrant/pglogical)           |

### **Data Lineage**

Tracks the flow and transformation of data from source to report:

* Maps where data originated, how it was transformed, and where it’s used
* Helps in impact analysis, audit trails, regulatory compliance (e.g. BCBS 239)
* Visual tools often used to explore dependencies and breakpoints in pipelines

**Used by**: Data governance, audit, and engineering teams.

| Product             | Description                                                                                      | Licence    | GitHub Link                                                                              |
| ------------------- | ------------------------------------------------------------------------------------------------ | ---------- | ---------------------------------------------------------------------------------------- |
| **Apache Atlas**    | Enterprise-grade metadata catalog and data-lineage framework for data lakes                      | Apache 2.0 | [https://github.com/apache/atlas](https://github.com/apache/atlas)                       |
| **OpenLineage**     | Open lineage specification with reference APIs and libraries for capturing job / dataset lineage | Apache 2.0 | [https://github.com/OpenLineage/OpenLineage](https://github.com/OpenLineage/OpenLineage) |
| **Marquez**         | Lineage service and UI that stores, processes, and visualises OpenLineage events                 | Apache 2.0 | [https://github.com/MarquezProject/marquez](https://github.com/MarquezProject/marquez)   |
| **DataHub Lineage** | OpenLineage-based lineage plugin and docs within LinkedIn’s DataHub catalog                      | Apache 2.0 | [https://github.com/datahub-project/datahub](https://github.com/datahub-project/datahub) |
| **Pachyderm**       | Data-pipeline platform with built-in data versioning and end-to-end lineage tracking             | Apache 2.0 | [https://github.com/pachyderm/pachyderm](https://github.com/pachyderm/pachyderm)         |

### **AI / ML Workbenches**

*Integrated environments that let data‑science teams prototype, train, track and deploy models—covering notebooks, pipelines, experiment tracking and model registry.*

| Product      | Description                                                                                                    | Licence    | GitHub Link                                                                  |
| ------------ | -------------------------------------------------------------------------------------------------------------- | ---------- | ---------------------------------------------------------------------------- |
| **Kubeflow** | End‑to‑end ML platform on Kubernetes (JupyterHub, Pipelines, KFServing, Katib hyper‑parameter tuning)          | Apache 2.0 | [https://github.com/kubeflow/kubeflow](https://github.com/kubeflow/kubeflow) |
| **Flyte**    | Kubernetes‑native, type‑safe workflow engine for scalable ML & data pipelines with versioned executions        | Apache 2.0 | [https://github.com/flyteorg/flyte](https://github.com/flyteorg/flyte)       |
| **Metaflow** | Human‑centric ML development framework that scales notebook workflows to production on Kubernetes or AWS Batch | Apache 2.0 | [https://github.com/Netflix/metaflow](https://github.com/Netflix/metaflow)   |
| **MLflow**   | Platform for experiment tracking, model registry & reproducible ML runs; supports model serving / packaging    | Apache 2.0 | [https://github.com/mlflow/mlflow](https://github.com/mlflow/mlflow)         |
| **Kedro**    | Python framework for reproducible, version‑controlled data & ML pipelines with rich plug‑in ecosystem          | Apache 2.0 | [https://github.com/kedro-org/kedro](https://github.com/kedro-org/kedro)     |

### **BI Dashboards**

Business Intelligence platforms for visual reporting and performance monitoring:

* Drag-and-drop dashboards, drill-downs, and alerts for KPIs
* Connects to databases, warehouses, and APIs
* Enables self-service insights and executive reporting

| Product                    | Description                                                                  | Licence                            | GitHub Link                                                                                                            |
| -------------------------- | ---------------------------------------------------------------------------- | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Apache Superset**        | Modern BI platform for interactive dashboards and slice-and-dice exploration | Apache 2.0                         | [https://github.com/apache/superset](https://github.com/apache/superset)                                               |
| **Metabase**               | Easy self-service analytics and visual SQL builder                           | AGPL v3 (Community Edition)        | [https://github.com/metabase/metabase](https://github.com/metabase/metabase)                                           |
| **Redash**                 | Query editor and visualisation layer for multiple data sources               | BSD 2-Clause                       | [https://github.com/getredash/redash](https://github.com/getredash/redash)                                             |
| **Lightdash**              | dbt-native BI & metrics layer                                                | MIT                                | [https://github.com/lightdash/lightdash](https://github.com/lightdash/lightdash)                                       |
| **Grafana**                | Observability dashboards, alerting and plug-in framework                     | AGPL v3                            | [https://github.com/grafana/grafana](https://github.com/grafana/grafana)                                               |
| **amCharts 5**             | Embeddable JavaScript/TypeScript charting library                            | Free (non-commercial) / Commercial | [https://github.com/amcharts/amcharts5](https://github.com/amcharts/amcharts5)                                         |
| **Perspective**            | High-performance streaming analytics & pivot component                       | Apache 2.0                         | [https://github.com/finos/perspective](https://github.com/finos/perspective)                                           |
| **react-financial-charts** | React/D3 components specialised for financial charts                         | MIT                                | [https://github.com/react-financial/react-financial-charts](https://github.com/react-financial/react-financial-charts) |
| **Lightweight Charts**     | Ultra-small interactive price-chart library from TradingView                 | Apache 2.0                         | [https://github.com/tradingview/lightweight-charts](https://github.com/tradingview/lightweight-charts)                 |
| **Vizzu Lib**              | Animated data-story/visualisation JavaScript library                         | Apache 2.0                         | [https://github.com/vizzuhq/vizzu-lib](https://github.com/vizzuhq/vizzu-lib)                                           |
