
Below is a more **exhaustive catalogue of openly-licensed projects** limited to well-maintained projects that still see commits/releases and have production references.

## Customer & Channels

### CRM

Manages customer interactions and lifecycle. These systems help financial institutions:

* Track leads and customer profiles
* Manage sales pipelines and marketing campaigns
* Log support tickets and service requests
* Integrate with contact centers and digital channels

| Product            | Description                                        | Licence              | GitHub Link                                                                                          |
| ------------------ | -------------------------------------------------- | -------------------- | ---------------------------------------------------------------------------------------------------- |
| SuiteCRM           | SugarCRM fork; sales, service & marketing modules  | AGPLv3               | [https://github.com/salesagility/SuiteCRM](https://github.com/salesagility/SuiteCRM)                 |
| Odoo (Community)   | Modular ERP/CRM with Studio low-code builder       | LGPLv3               | [https://github.com/odoo/odoo](https://github.com/odoo/odoo)                                         |
| EspoCRM            | Lean LAMP stack, entity modeller and BPM workflows | GPLv3                | [https://github.com/espocrm/espocrm](https://github.com/espocrm/espocrm)                             |
| ERPNext            | Full ERP; CRM module plus customer portal          | GPLv3                | [https://github.com/frappe/erpnext](https://github.com/frappe/erpnext)                               |
| Dolibarr           | SMB-focused ERP/CRM with plug-in market            | GPLv3                | [https://github.com/Dolibarr/dolibarr](https://github.com/Dolibarr/dolibarr)                         |
| Vtiger (Community) | Mature PHP CRM; basis for many forks               | VPL or GPL           | [https://github.com/vtiger-crm/vtigercrm](https://github.com/vtiger-crm/vtigercrm)                   |
| OroCRM CE          | Symfony-based B2B/B2C CRM with flexible data model | OSL 3.0              | [https://github.com/oroinc/crm](https://github.com/oroinc/crm)                                       |
| CiviCRM            | Constituent/donor management for non-profits       | AGPLv3               | [https://github.com/civicrm/civicrm-core](https://github.com/civicrm/civicrm-core)                   |
| YetiForce CRM      | Vtiger derivative with 80+ built-in modules        | YPL (similar to GPL) | [Old repo] [https://github.com/YetiForceCompany/YetiForceCRM](https://github.com/YetiForceCompany/YetiForceCRM) |


### Identification & Verification (KYC / Digital Identity)

Provides customer identity proofing, authentication and ongoing verification across channels:

* Document verification, biometric checks, liveness detection
* KYC / CIP onboarding flows with regulatory record-keeping
* Step-up authentication and risk-based re‑verification
* APIs / SDKs for web, mobile and branch systems

| Product               | Description                                                                                                                  | Licence    | GitHub Link                                                                                            |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ---------- | ------------------------------------------------------------------------------------------------------ |
| **Keycloak**          | Java identity and access management server supporting OAuth2/OIDC, SAML and identity brokering; extensible SPI for KYC flows | Apache 2.0 | [https://github.com/keycloak/keycloak](https://github.com/keycloak/keycloak)                           |
| **Ballerine**         | Headless TypeScript stack for KYC/KYB orchestration, document checks and sanctions screening                                 | Apache 2.0 | [https://github.com/ballerine-io/ballerine](https://github.com/ballerine-io/ballerine)                 |
| **Authentik**         | Python/Go workforce and consumer IAM with flexible policy engine and multi-factor auth                                       | GPL 3      | [https://github.com/goauthentik/authentik](https://github.com/goauthentik/authentik)                   |
| **MOSIP**             | Modular open‑source national ID platform with biometrics, deduplication and eKYC APIs                                        | MPL 2.0    | [https://github.com/mosip/mosip](https://github.com/mosip/mosip)                                       |
| **Hyperledger Indy**  | Ledger and protocols for decentralised identifiers (DIDs) and verifiable credentials                                         | Apache 2.0 | [https://github.com/hyperledger/indy-node](https://github.com/hyperledger/indy-node)                   |
| **Hyperledger Aries** | Interoperable agent framework for SSI credential issuance and verification                                                   | Apache 2.0 | [https://github.com/hyperledger/aries-framework-go](https://github.com/hyperledger/aries-framework-go) |
| **walt.id SSI Kit**   | Java/Kotlin toolkit for issuing, holding and verifying W3C VC credentials                                                    | Apache 2.0 | [https://github.com/walt-id/waltid-ssikit](https://github.com/walt-id/waltid-ssikit)                   |
| **OpenKYC (IDKit)**   | Golang self‑hosted API for KYC and face‑match using machine‑learning models                                                  | GPL 3      | [https://github.com/openkyc/openkyc](https://github.com/openkyc/openkyc)                               |

### Branch / Contact-Centre

Infrastructure for in-person and telephonic engagement. This includes:

* IP telephony (VoIP), IVR, and PBX systems
* Call recording, call routing, and agent dashboards
* Blended inbound/outbound dialers and contact management
* Unified communications for branches or distributed agents

| Product       | Description                                                  | Licence                               | GitHub Link                                                                                      |
| ------------- | ------------------------------------------------------------ | ------------------------------------- | ------------------------------------------------------------------------------------------------ |
| Asterisk      | Canonical OSS telephony engine (IVR, queues, recording)      | GPL v2                                | [https://github.com/asterisk/asterisk](https://github.com/asterisk/asterisk)                     |
| FreePBX       | GUI for Asterisk (good for quick branch roll-outs)           | GPL v3                                | [https://github.com/FreePBX](https://github.com/FreePBX)                                         |
| FreeSWITCH    | High-scale media server (WebRTC, conferencing)               | MPL 2.0                               | [https://github.com/signalwire/freeswitch](https://github.com/signalwire/freeswitch)             |
| ViciDial      | Blended inbound/outbound dialler & agent desktop             | AGPL v2                               | [https://github.com/inktel/Vicidial](https://github.com/inktel/Vicidial)                         |
| Wazo Platform | Programmable UCaaS stack with multi-tenant APIs              | GPL v3 \*                             | [https://github.com/wazo-platform/wazo-platform](https://github.com/wazo-platform/wazo-platform) |
| GOautodial    | Web UI around ViciDial/Asterisk plus omni-channel add-ons    | GPL v2 / AGPL v2 (web apps)           | [https://github.com/goautodial](https://github.com/goautodial)                                   |
| FusionPBX     | FreeSWITCH-based PBX with multi-tenant GUI                   | MPL 1.1     [Not sure about this one] | [https://github.com/fusionpbx/fusionpbx](https://github.com/fusionpbx/fusionpbx)                 |
| Issabel PBX   | Elastix successor bundling Asterisk, call-centre & reporting | GPL v3                                | [https://github.com/IssabelFoundation/pbx](https://github.com/IssabelFoundation/pbx)             |
| sipXcom       | SIP/XMPP UC server for 5–50 k seats                          | AGPL v3                               | [https://github.com/sipXcom/sipxecs](https://github.com/sipXcom/sipxecs)                         |

### Mobile (frameworks & reference apps)

Frameworks and toolkits for building banking apps. They support:

* Cross-platform app development (Android/iOS/Web)
* Native and hybrid user interfaces
* Integration with backend services and APIs
* OTA updates and security controls

| Product                     | Description                                              | Licence                        | GitHub Link                                                                                    |
| --------------------------- | -------------------------------------------------------- | ------------------------------ | ---------------------------------------------------------------------------------------------- |
| React Native                | Meta-backed JS/TS framework (iOS, Android, web)          | MIT         | [https://github.com/facebook/react-native](https://github.com/facebook/react-native)           |
| Flutter                     | Google Dart UI toolkit; pixel-perfect, 120 fps           | BSD 3-Clause  | [https://github.com/flutter/flutter](https://github.com/flutter/flutter)                       |
| Apache Cordova              | Wrappers for HTML/JS hybrid apps                         | Apache 2.0    | [https://github.com/apache/cordova](https://github.com/apache/cordova)                         |
| Ionic Framework             | Mobile-optimised Web Components atop Cordova/Capacitor   | MIT           | [https://github.com/ionic-team/ionic-framework](https://github.com/ionic-team/ionic-framework) |
| NativeScript                | Direct JS/TS access to native APIs (no WebView)          | MIT           | [https://github.com/NativeScript/NativeScript](https://github.com/NativeScript/NativeScript)   |
| Kotlin Multiplatform Mobile | Share business logic across Android/iOS                  | Apache 2.0    | [https://github.com/JetBrains/kotlin](https://github.com/JetBrains/kotlin)                     |
| .NET MAUI                   | C#/XAML multi-platform UI (Android, iOS, macOS, Windows) | MIT           | [https://github.com/dotnet/maui](https://github.com/dotnet/maui)                               |
| Expo                        | Managed tool-chain & OTA updates for React Native apps   | MIT          | [https://github.com/expo/expo](https://github.com/expo/expo)                                   |

### Agency / Broker Portals

Self-service or intermediary-facing platforms. These provide:

* Role-based access for agents, brokers, or third-party partners
* Document and product management interfaces
* Secure portals for submitting applications or managing clients
* Integration with CRM or underwriting systems

| Product                     | Description                                               | Licence                                             | GitHub Link                                                                                              |
| --------------------------- | --------------------------------------------------------- | --------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **Liferay Portal CE**       | Enterprise portal with fragment builder, roles & staging  | LGPL v2.1 or later                | [https://github.com/liferay/liferay-portal](https://github.com/liferay/liferay-portal) |
| **Frappe Framework**        | Python/JS low-code platform (powers ERPNext)              | MIT                               | [https://github.com/frappe/frappe](https://github.com/frappe/frappe)                   |
| **Drupal**                  | Highly-extensible CMS (API-first via JSON API & GraphQL)  | GPL v2 or later              | [https://github.com/drupal/drupal](https://github.com/drupal/drupal)                    |
| **Joomla!**                 | GPL CMS with 10 k+ extensions and ACL                     | GPL v2 or later                    | [https://github.com/joomla/joomla-cms](https://github.com/joomla/joomla-cms)            |
| **Plone**                   | Secure Python CMS with fine-grained workflows             | GPL v2                             | [https://github.com/plone/Plone](https://github.com/plone/Plone)                        |
| **OpenCMS**                 | Java-based portal with WYSIWYG editor & multisite support | LGPL v2.1                          | [https://github.com/alkacon/opencms-core](https://github.com/alkacon/opencms-core)      |
| **dotCMS (Community)**      | Hybrid headless CMS/portal written in Java                | BSL 1.1 (Business Source License)  | [https://github.com/dotCMS/core](https://github.com/dotCMS/core)                        |
| **ERPNext Customer Portal** | Ready-made agent/customer workspace atop ERPNext          | GPL v3                             | [https://github.com/frappe/erpnext](https://github.com/frappe/erpnext)                  |


