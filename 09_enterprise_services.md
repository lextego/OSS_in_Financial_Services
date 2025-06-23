## Enterprise Services

### **Identity & Access**

Manages authentication, authorization, and user identity lifecycle:

* Supports SSO, MFA, OAuth2/OIDC, LDAP/AD federation
* Role-Based Access Control (RBAC) and Attribute-Based Access Control (ABAC)
* Critical for customer onboarding, staff access, and API security

**Common tools**: Keycloak, WSO2 Identity Server, Authelia

| Product                  | Description                                               | Licence                      | GitHub Link                                                                                                                              |
| ------------------------ | --------------------------------------------------------- | ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **Keycloak**             | SSO & IdM platform                                        | Apache 2.0  | [https://github.com/keycloak/keycloak](https://github.com/keycloak/keycloak)                                            |
| **Gluu Server CE**       | Multi-protocol identity provider (SAML, OIDC, LDAP, FIDO) | MIT         | [https://github.com/GluuFederation/gluu4/tree/4.5/community-edition-setup](https://github.com/GluuFederation/gluu4/tree/4.5/community-edition-setup) |
| **authentik**            | Go-/Python-based IdP with flexible policy flows           | MIT         | [https://github.com/goauthentik/authentik](https://github.com/goauthentik/authentik)                                    |
| **WSO2 Identity Server** | Enterprise customer-/workforce IAM (CIAM)                 | Apache 2.0  | [https://github.com/wso2/product-is](https://github.com/wso2/product-is)                                                |
| **Authelia**             | Self-hosted SSO reverse-proxy (2FA, LDAP/OIDC/SAML)       | Apache 2.0  | [https://github.com/authelia/authelia](https://github.com/authelia/authelia)                                            |


### Customer Identity Management

Covers digital identity verification, customer registration, and regulatory compliance workflows. Tools in this space support:

* Self-registration and onboarding flows
* eKYC and digital ID integrations
* Identity proofing and multi-factor authentication (MFA)
* Consent management and access control

| Product                  | Description                                                                                             | Licence                                            | GitHub Link                                                                                                                      |
| ------------------------ | ------------------------------------------------------------------------------------------------------- | -------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **Keycloak**             | Enterprise-grade IAM with configurable self-registration, MFA and social-login flows                    | Apache 2.0                       | [https://github.com/keycloak/keycloak](https://github.com/keycloak/keycloak)                                                     |
| **MOSIP**                | Modular digital-ID stack (eKYC API, dedupe, credential issuance) used by several national ID programmes | MPL 2.0 (core) / MIT (reference)  | [https://github.com/mosip/mosip](https://github.com/mosip/mosip)                                                                 |
| **Gluu Server CE**       | OpenID Connect / SAML SSO plus FIDO2, SCIM and adaptive auth                                            | MIT                              | [https://github.com/GluuFederation/community-edition-containers](https://github.com/GluuFederation/community-edition-containers) |
| **authentik**            | Go-based IdP with policy engine & tenant isolation                                                      | MIT                              | [https://github.com/goauthentik/authentik](https://github.com/goauthentik/authentik)                                             |
| **privacyIDEA**          | Pluggable MFA / token-management server (OTP, WebAuthn, YubiKey)                                        | AGPL v3                           | [https://github.com/privacyidea/privacyidea](https://github.com/privacyidea/privacyidea)                                         |
| **WSO2 Identity Server** | API-centric CIAM & consent management under Apache licence                                              | Apache 2.0                        | [https://github.com/wso2/product-is](https://github.com/wso2/product-is)                                                         |


### **Workflow / BPM (Business Process Management)**

Orchestrates multi‑step business processes and human/system interactions:

* Supports modeling with BPMN/DMN (and CMMN), task routing, SLAs, and approvals
* Used in case management, KYC flows, loan underwriting, etc.
* Enables low‑code automation and integration across systems

| Product                | Description                                                                                                                                   | Licence    | GitHub Link                                                                                        |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | -------------------------------------------------------------------------------------------------- |
| **Activiti**           | Lightweight BPMN 2.0 process engine for Java apps                                                                                             | Apache 2.0 | [https://github.com/Activiti/Activiti](https://github.com/Activiti/Activiti)                       |
| **Flowable**           | Fork of Activiti providing BPMN, DMN & CMMN engines with Spring Boot & REST APIs                                                              | Apache 2.0 | [https://github.com/flowable/flowable-engine](https://github.com/flowable/flowable-engine)         |
| **jBPM**               | Java toolkit combining workflow (BPMN) & business‑rules (Drools)                                                                              | Apache 2.0 | [https://github.com/kiegroup/jbpm](https://github.com/kiegroup/jbpm)                               |
| **Kogito**             | Cloud‑native business‑automation runtime (BPMN/DMN) built on Quarkus/Spring Boot                                                              | Apache 2.0 | [https://github.com/kiegroup/kogito-runtimes](https://github.com/kiegroup/kogito-runtimes)         |
| **Node‑RED**           | Low‑code, event‑driven workflow builder & runtime                                                                                             | Apache 2.0 | [https://github.com/node-red/node-red](https://github.com/node-red/node-red)                       |


### **Document Management**

Handles creation, storage, and retrieval of electronic documents:

* Features include versioning, metadata tagging, full-text search, and access control
* Supports document scanning, e-signatures, and audit trails
* Integrated into customer onboarding, compliance, and HR workflows

**Open-source options**: Alfresco CE, Nextcloud, Mayan EDMS

| Product                             | Description                                                                                                   | Licence                                   | GitHub Link                                                                                                  |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------- | ----------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Alfresco Community Edition (CE)** | Enterprise-grade document-management system (DMS) with content‐services API, workflows and records management | LGPL v3                  | [https://github.com/Alfresco/alfresco-community-repo](https://github.com/Alfresco/alfresco-community-repo)   |
| **Nextcloud Server**                | Self-hosted file-sync & share platform with Collabora / OnlyOffice integration and rich app ecosystem         | AGPL v3                  | [https://github.com/nextcloud/server](https://github.com/nextcloud/server)                                   |
| **Mayan EDMS**                      | Document-scanning, OCR and workflow-enabled electronic DMS                                                    | Apache 2.0               | [https://github.com/mayan-edms/mayan-edms](https://github.com/mayan-edms/mayan-edms)                         |
| **OpenKM (Community)**              | Java-based DMS with hierarchical folders, metadata, versioning and workflow                                   | GPL v2  | [https://github.com/openkm/document-management-system](https://github.com/openkm/document-management-system) |
| **Paperless-ngx**                   | Minimalist Django-based DMS for scanning, indexing and archiving documents                                    | GPL v3  | [https://github.com/paperless-ngx/paperless-ngx](https://github.com/paperless-ngx/paperless-ngx)             |

### **DevSecOps**

Practices and tooling for secure, continuous software delivery:

* Combines CI/CD pipelines with security testing (SAST, DAST, container scanning)
* Automates deployment to cloud, on-prem, or hybrid environments
* Ensures code, infrastructure, and secrets are governed


| Product          | Description                                                  | Licence                        | GitHub / Repo Link                                                                                     |
| ---------------- | ------------------------------------------------------------ | ------------------------------ | ------------------------------------------------------------------------------------------------------ |
| **Jenkins**      | Extensible CI/CD automation server                           | MIT           | [https://github.com/jenkinsci/jenkins](https://github.com/jenkinsci/jenkins)          |
| **GitLab CE**    | All-in-one SCM & CI/CD platform with built-in security scans | MIT      | [https://gitlab.com/gitlab-org/gitlab](https://gitlab.com/gitlab-org/gitlab)          |
| **SonarQube CE** | Code-quality, SAST & “Clean Code” gates                      | LGPL v3  | [https://github.com/SonarSource/sonarqube](https://github.com/SonarSource/sonarqube)  |
| **Trivy**        | Container, code, IaC & SBOM scanner                          | Apache 2.0    | [https://github.com/aquasecurity/trivy](https://github.com/aquasecurity/trivy)        |
| **OWASP ZAP**    | Web-app DAST proxy & scanner                                 | Apache 2.0    | [https://github.com/zaproxy/zaproxy](https://github.com/zaproxy/zaproxy)             |

### **Cloud / Infrastructure**

Core IT stack for compute, storage, and networking:

* Kubernetes, Terraform, and infrastructure-as-code practices
* Multi-cloud or hybrid strategies for high availability and resilience
* Observability, autoscaling, secrets management, and provisioning automation

| Product                     | Description                                                                                         | Licence                              | GitHub Link                                                                          |
| --------------------------- | --------------------------------------------------------------------------------------------------- | ------------------------------------ | ------------------------------------------------------------------------------------ |
| **Kubernetes**              | CNCF container-orchestration platform for automating deployment, scaling & operations of containers | Apache 2.0                           | [https://github.com/kubernetes/kubernetes](https://github.com/kubernetes/kubernetes) |
| **OKD**                     | Upstream, community distribution of Red Hat OpenShift (Kubernetes + Operators + DevOps tooling)     | Apache 2.0                           | [https://github.com/openshift/origin](https://github.com/openshift/origin)           |
| **Terraform (Open Source)** | Declarative Infrastructure-as-Code CLI for building, changing & versioning cloud resources          | BUSL 1.1 (≥ v1.6) / MPL 2.0 (≤ v1.5) | [https://github.com/hashicorp/terraform](https://github.com/hashicorp/terraform)     |
| **Ansible**                 | Agent-less configuration-management & automation engine using YAML playbooks                        | GPL v3                               | [https://github.com/ansible/ansible](https://github.com/ansible/ansible)             |
| **K3s**                     | Lightweight, single-binary Kubernetes distribution optimised for edge & IoT                         | Apache 2.0                           | [https://github.com/k3s-io/k3s](https://github.com/k3s-io/k3s)                       |

### **Observability**

Enables monitoring, alerting, and tracing of distributed systems:

* Metrics (e.g. CPU, memory, transactions), logs, and traces
* Supports anomaly detection, alert thresholds, and SLO dashboards
* Integral for performance tuning, incident response, and capacity planning

**Popular stacks**: Prometheus + Grafana, ELK/EFK stack, OpenTelemetry

| Product                     | Description                                                 | Licence                      | GitHub Link                                                                                                            |
| --------------------------- | ----------------------------------------------------------- | ---------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Prometheus**              | Metrics collection, time-series storage & alerting rules    | Apache 2.0  | [https://github.com/prometheus/prometheus](https://github.com/prometheus/prometheus)                                   |
| **Grafana**                 | Visual dashboards, alerting & data-source plugins           | AGPL v3     | [https://github.com/grafana/grafana](https://github.com/grafana/grafana)                                               |
| **Loki**                    | Log aggregation system designed for Prometheus-style labels | Apache 2.0  | [https://github.com/grafana/loki](https://github.com/grafana/loki)                                                     |
| **Jaeger**                  | CNCF distributed-tracing platform (spans, sampling, UI)     | Apache 2.0  | [https://github.com/jaegertracing/jaeger](https://github.com/jaegertracing/jaeger)                                     |
| **OpenTelemetry Collector** | Vendor-neutral collector/agent for metrics, logs & traces   | Apache 2.0  | [https://github.com/open-telemetry/opentelemetry-collector](https://github.com/open-telemetry/opentelemetry-collector) |
