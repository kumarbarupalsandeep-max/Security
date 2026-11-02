# Security Platforms — Detailed Page & Feature Catalog

**Project:** Security — Deep Research & Study Notes  
**Owner / Content Creator:** Sandeep Barupal  
**Copyright:** © 2026 Sandeep Barupal. All rights reserved, except as stated below.

## Research ka scope

Yeh document do enterprise cybersecurity platforms ke publicly documented console areas, pages, sub-pages aur important features ko samajhne ke liye hai:

1. Microsoft Defender portal / Microsoft Defender XDR.
2. CrowdStrike Falcon console.

**Important:** Neeche kuch headings exact published navigation labels hain, aur kuch ek page ke tabs, detail views ya research ke liye grouped capabilities hain. In sab ko ek jaisa na samjhein. Dono products mein navigation, license, permissions, purchased modules, tenant settings aur product updates ke kaaran differences aa sakte hain.

---

# Part A — Microsoft Defender

Microsoft Defender portal ek central portal hai jahan provisioned Microsoft security products ke incidents, alerts, hunting, actions aur threat intelligence ko ek saath dekha ja sakta hai. Portal mein wahi modules show hote hain jo organization ke subscription aur configuration mein available hon.

## A1. Portal-wide pages and controls

### 1. Home / Overview
Purpose: Organization ki overall security activity aur urgent work ka summary.

Documented / commonly surfaced information:
- Active incidents aur alerts ka summary.
- Pending response actions.
- Threat analytics se relevant threats.
- Security product ke dashboard cards.
- Investigation ke liye shortcuts.

Note: Homepage cards aur available summary data organization ke enabled products ke mutabik differ kar sakte hain.

### 2. Global Search
Purpose: Portal mein security entities aur relevant pages dhoondhna.

Searchable entity types documented by Microsoft:
- Devices.
- Users.
- Files.
- IP addresses.
- URLs.
- Vulnerability management information (vulnerabilities, software, recommendations).

### 3. Notifications
Purpose: Relevant security events aur portal notifications ko dekhna.

Feature examples:
- Product notifications.
- Incident / response notifications where configured.
- Notification preferences settings.

## A2. Unified security operations

### 4. Incidents
Purpose: Ek hi attack ya threat se jude multiple alerts ko ek investigation record mein review karna.

Features:
- Incidents ki list.
- Severity, status, date aur assignment ke basis par filtering.
- Incident summary aur description.
- Related alerts.
- Affected devices, users aur other entities.
- Incident timeline / attack story.
- Evidence aur related activity.
- Owner / assignment and status management.
- Investigation notes and history.

### 5. Incident Details
Purpose: Selected incident ki full investigation.

Common detail sections:
- Incident overview.
- Alert list.
- Affected assets and identities.
- Evidence / entities.
- Timeline.
- Investigation / response status.
- Available response actions.
- Activity history.

### 6. Alerts
Purpose: Individual security detections ko review karna.

Features:
- Alert list.
- Severity, service source, date aur status filters.
- Alert-to-incident relationship.
- Affected device / user / entity.
- Alert description and evidence.
- Available alert-level response actions.

### 7. Alert Details
Purpose: Ek detection ka evidence aur context samajhna.

Common detail areas:
- Detection name and description.
- Severity / category.
- Related incident.
- Impacted device or user.
- Evidence and related events.
- Actions taken and action status.

### 8. Hunting — Advanced Hunting
Purpose: Query ke through environment ke security events mein suspicious behavior dhoondhna.

Microsoft documentation mein do modes:
- Guided mode: visual query builder; KQL likhna zaroori nahi.
- Advanced mode: Kusto Query Language (KQL) based query editor.

Features:
- Query builder / query editor.
- Time range.
- Tables and fields.
- Query execution.
- Result table and visualizations.
- Result filtering / sorting.
- Investigation pivots.
- Result export or follow-up actions where supported.
- Query ko incident se link karna where supported.

### 9. Hunting — Custom Detection Rules
Purpose: Saved hunting logic ko scheduled detection rule banana.

Features:
- Existing rule list.
- New rule wizard.
- Query configuration.
- Alert title, description and severity.
- Alert enrichment details.
- Scope configuration.
- Automated response action selection where supported.
- Rule on/off status.
- Last run, next run and run status.
- Triggered alerts and triggered actions.
- Edit, run, disable or delete controls according to permissions.

### 10. Actions & Submissions — Action Center
Purpose: Pending aur completed remediation actions ko central place se review karna.

Main views:
- Pending actions.
- History / completed actions.

Features:
- Pending approval queue.
- Approve or reject supported actions.
- Bulk review where action type permits.
- Action status.
- Target entity / asset.
- Completed action history.
- Audit trail of actions.
- Cross-product remediation view for supported devices, email/collaboration content and identities.

### 11. Actions & Submissions — Submissions
Purpose: Suspicious objects ko further security analysis ke liye submit karna.

Documented submission categories can include:
- Files.
- Email / email attachments.
- URLs.
- Teams messages.

Available categories and workflow depend on relevant product and permissions.

### 12. Threat Analytics
Purpose: Emerging threats aur campaigns ko samajhna aur apni organization par unka effect assess karna.

Dashboard / report features:
- Latest threats.
- High-impact threats.
- Highest-exposure threats.
- Threat categories and search.
- Threat report overview.
- Analyst report.
- Related incidents.
- Impacted assets.
- Endpoint exposure.
- Recommended actions.
- Indicators where available.

Threat reports may cover:
- Threat actors and campaigns.
- Attack techniques.
- Critical vulnerabilities.
- Common attack surfaces.
- Prevalent malware.

## A3. Endpoint and asset pages

### 13. Assets — Devices / Device Inventory
Purpose: Organization ke visible devices ko list aur manage karna.

Documented inventory views can include:
- All devices.
- Computers & mobile.
- Network devices.
- IoT / OT.
- Uncategorized.

Common fields:
- Device name.
- Domain.
- Risk level.
- Exposure level.
- Operating system / platform.
- Criticality.
- Onboarding status.
- Sensor health state.
- Mitigation status.

Features:
- Search, filter and sort.
- High-risk device identification.
- Onboarding progress.
- Unhealthy sensor identification.
- Device detail page open karna.

### 14. Device Details
Purpose: Ek device ki security condition aur related activity dekhna.

Common areas (available data depends on license / device telemetry):
- Device profile and identifiers.
- Risk and exposure.
- Related alerts and incidents.
- Security recommendations.
- Installed software.
- Device event timeline.
- Sensor / onboarding health.
- Available response actions.

### 15. Device Response Actions
Purpose: Supported endpoint response workflows manage karna.

Documented examples include:
- Device isolation.
- Release from isolation.
- Investigation package collection.
- Other supported investigation / response actions.

High-impact actions ke liye correct permission, connected service aur policy required hote hain.

## A4. Vulnerability and exposure pages

Microsoft Defender Vulnerability Management ki navigation existing tenants aur preview / integrated experiences mein alag ho sakti hai. Official documentation existing navigation mein Endpoints > Vulnerability management aur integrated preview experience mein Exposure management areas show karti hai.

### 16. Vulnerability Management — Overview / Dashboard
Features:
- Organization exposure summary.
- Device security score / exposure score where applicable.
- Important recommendations.
- Exposed assets overview.
- Trend and risk summary.

### 17. Recommendations
Features:
- Security recommendation list.
- Weakness count.
- Related software / components.
- Threat context.
- Exposed device count.
- Remediation type and activity.
- Tags and recommendation details.
- Request remediation.
- Create exception where permitted.
- Report inaccurate data.

### 18. Remediation
Features:
- Remediation activity list.
- Request status.
- Priority and due date where configured.
- Related recommendation.
- Assigned IT / service management context.
- Progress tracking.
- Export.
- Mark complete.

### 19. Inventories
Features:
- Organization asset inventory.
- Software inventory.
- Software vendor and product.
- Software versions.
- Weaknesses and threats associated with software.
- Exposed devices.
- Software detail and related devices.

### 20. Weaknesses / Vulnerabilities
Features:
- CVE inventory.
- Severity and vulnerability context.
- Affected software / devices.
- Related recommendations.
- Exploit / threat context when available.

### 21. Event Timeline
Features:
- Vulnerability and software-related events.
- Event time and affected component.
- Related software / device.
- Investigation links.

### 22. Baselines Assessment
Features:
- Security baseline assessment.
- Configuration compliance status.
- Configuration changes and deviations.

## A5. Email and collaboration security

### 23. Email & Collaboration — Explorer / Real-time Detections
Purpose: Email-based malware, phishing and other threats investigate karna.

Important licensing difference:
- Real-time detections: Defender for Office 365 Plan 1.
- Threat Explorer: Defender for Office 365 Plan 2.
- Threat Explorer includes additional views, filtering, saved queries, threat hunting and remediation capabilities compared with Real-time detections.

Features / views can include:
- All email (Explorer).
- Malware.
- Phish.
- Campaigns (Explorer).
- Email direction / delivery context.
- Sender and recipient details.
- Subject and time filters.
- URL and click-verdict information.
- Attachment / malware information.
- Threat tags and investigation details.
- Automated investigation / remediation capabilities where supported.

## A6. Cloud apps and adjacent security products

### 24. Cloud Apps — Cloud Discovery
Purpose: Organization mein use ho rahi cloud applications aur Shadow IT ko identify karna.

Features:
- Discovered cloud app inventory.
- App category / function.
- App risk assessment.
- User, IP, device and transaction context where collected.
- Snapshot and continuous discovery reports.
- App discovery filters.

### 25. Cloud Apps — App Catalog
Features:
- Cloud app search.
- App details and risk attributes.
- App tags.
- Business-ready / unsanctioned app classification where configured.

### 26. Cloud Apps — Policies
Features:
- App discovery policies.
- Risk / compliance-based policy conditions.
- Usage-based policy conditions.
- Alert generation.
- Policy-triggered actions where supported.

### 27. Identity Protection
Purpose: Identity-related attacks aur suspicious user behavior investigate karna.

Relevant identity security capabilities may include:
- Identity-related alerts and incidents.
- User / identity context.
- Suspicious activity and sign-in context (when the relevant signals are integrated).
- Identity sensor / service health.
- Related device and alert context.
- Investigation and response options permitted by the tenant.

Exact navigation and available views must be rechecked against the organization's Defender for Identity license and portal configuration.

### 28. Cloud Security / Defender for Cloud Integration
Purpose: Cloud resources and cloud security signals ko Defender portal ke broader investigation experience se connect karna.

Research areas:
- Cloud resources and asset context.
- Cloud security recommendations.
- Cloud findings / alerts.
- Related incidents.
- Configuration and risk posture.

Exact cloud pages are also available in the relevant Defender for Cloud experience; do not assume every cloud feature is a native page in the Defender XDR console.

### 29. Microsoft Sentinel
Purpose: Security information and event management (SIEM) and security orchestration workflows.

Research pages / capabilities:
- Analytics rules.
- Incidents.
- Logs / event search.
- Workbooks and dashboards.
- Data connectors.
- Hunting.
- Automation rules and playbooks.

Microsoft has documented the Sentinel experience in the Defender portal. The exact portal path and feature availability can change with the migration / unified experience.

### 30. Settings — Microsoft Defender XDR
Documented configuration areas include:
- Email notifications for incidents, response actions and threat analytics.
- Permissions and roles.
- Streaming API.
- Asset rule management.
- Alert tuning.
- Critical asset management.

---

# Part B — CrowdStrike Falcon

CrowdStrike Falcon console is modular. The navigation and pages visible in one tenant depend on subscribed modules, enabled services, assigned roles and console updates.

## B1. Global console and navigation

### 1. Falcon Console Navigation
Published console guide describes global areas and utilities such as:
- Navigation menu.
- Central search.
- Customer ID (CID) switcher for applicable multi-CID setups.
- Bookmarks.
- Recently visited pages.
- Notifications.
- User profile and settings.
- Search suggestions and search results.
- Filters and reusable table controls.

### 2. Falcon Status Dashboard
Features:
- Platform feature status.
- Service / component status.
- Status details.
- Tech alerts.
- Available operational actions.

### 3. Dashboards and Reports
Features:
- Preset dashboards.
- Private dashboards.
- Shared dashboards.
- Custom dashboard widgets.
- Data visualizations.
- Filters and drill-down.
- Scheduled reports.
- Export formats according to report type.

## B2. Endpoint Security

Published Falcon console navigation documents the following endpoint monitoring areas.

### 4. Endpoint Security — Activity Dashboard
Features:
- Endpoint activity summary.
- Detection / prevention activity.
- Endpoint-related trends.
- Links into more detailed monitoring pages.

### 5. CrowdScore Incidents
Purpose: Endpoint-related incident overview and prioritization.

Features:
- Incident list.
- Incident score / priority context.
- Host details.
- Incident name and description.
- Tags.
- Incident investigation and status context.
- Notifications for new incidents where configured.

### 6. Endpoint Detections
Purpose: Endpoint detections review karna.

Features:
- Endpoint detection list.
- Detection details.
- Host and user context.
- Detection attributes.
- Related process / file / behavior context where available.
- Detection review and follow-up.

### 7. XDR Detections
Purpose: Multiple security signals se unified detection view.

Features:
- Unified detection records.
- Detection source / attributes.
- Contextual relationships.
- Investigation pivots.

### 8. Mobile Detections
Purpose: Mobile security detections review karna where the relevant mobile capability is enabled.

Features:
- Mobile detection records.
- Device context.
- Detection details and status.
- Investigation follow-up.

### 9. Quarantined Files
Purpose: Isolated suspicious files review karna.

Features:
- Quarantined file list.
- File and host context.
- Quarantine status.
- Permitted file review / release operations, subject to role permissions.

## B3. Investigate

Published Falcon console menu description shows investigation tools including Search, Hunt, Timelines, Hosts, Processes, Users, Visibility Reports and Headline Vulnerabilities. The exact list can vary by tenant.

### 10. Search
Features:
- Search for supported entities and records.
- Search suggestions.
- Search results.
- Filtered result sets.

### 11. Hunt
Features:
- Threat hunting queries / investigation.
- Search telemetry for suspicious activity.
- Pivot to related entities.
- Query-based investigation where enabled.

### 12. Timelines
Features:
- Chronological activity view.
- Event sequence.
- Related host / user context.
- Time filters.

### 13. Hosts
Features:
- Host lookup.
- Host summary.
- Related host events.
- Link to host management details.

### 14. Processes
Features:
- Process investigation.
- Process / host relationship.
- Related detection and event context where collected.

### 15. Users
Features:
- User lookup.
- Related identity and activity context.
- Related detection investigation.

### 16. Visibility Reports
Features:
- Security visibility / coverage information.
- Findings and report views available to the subscribed module.

### 17. Headline Vulnerabilities
Features:
- Important vulnerability visibility.
- Vulnerability investigation links.
- Affected asset context when available.

### 18. UI Path / Identity Protection investigation entry
These are contextual investigation entry points shown in the published console menu description; their available details depend on the relevant product and tenant.

## B4. Host Setup and Management

### 19. Host Management
Published console guide describes:
- Host inventory.
- Host search and filtering.
- Host summary panel.
- Host timeline and event list.
- Host status and activity.
- Export host data.
- Quick and configured exports.
- Content update state.
- Inactive / duplicate host management.
- Hide / restore host workflow.
- Network containment status.
- Detection settings on a host.

### 20. Host Groups
Features:
- Host group inventory.
- Search host groups.
- Group details.
- Static and dynamic groups.
- Assign / remove hosts.
- Group tags.
- Assigned policies.
- Assigned exclusions.

### 21. Installation Tokens
Features:
- Create installation token.
- Edit token settings.
- Revoke / restore revoked tokens.
- Require-token configuration.
- Installation status review.
- Troubleshooting token-based sensor deployment.

### 22. Policy Management
Features:
- Policy list and details.
- Policy precedence.
- Default policies.
- Host group assignment.
- Policy assignment details.
- Relevant endpoint prevention / configuration policies.

### 23. Sensor Management
Features:
- Sensor download.
- Sensor version / usage visibility.
- Sensor update policies.
- Sensor health and deployment context.
- Installation / update troubleshooting.

## B5. Threat Intelligence

Published console guide documents Threat Intelligence research and analysis areas including adversaries, reports and feeds, indicators and sandbox. API reference also exposes intelligence, indicator, sandbox, MalQuery and ThreatGraph domains.

### 24. Adversaries
Features:
- Adversary / threat actor profile.
- Actor background and activity.
- Known tactics and techniques where documented.
- Related intelligence reports and indicators.

### 25. Reports and Feeds
Features:
- Threat intelligence reports.
- Intelligence feed browsing.
- Threat research updates.
- Related adversary and indicator references.

### 26. Indicators
Features:
- IP address.
- Domain.
- File hash.
- Other supported indicators.
- Indicator details and context.
- Related intelligence and detections.

### 27. Sandbox
Features:
- Suspicious file submission (with required permission).
- Analysis status.
- Sandbox analysis report.
- Observed behavior and indicators.
- Related file / threat intelligence context.

### 28. MalQuery / Monitoring Rules
Features:
- Malware sample search (subscription dependent).
- YARA-based hunting / saved rules where enabled.
- Scheduled monitoring.
- New match results.
- Notifications for monitored results.

## B6. Identity Protection

### 29. Identity Insights
Features:
- Identity risk insights.
- Graphs and entity context.
- Custom insights where permitted.

### 30. Identity Incidents
Features:
- Identity incident review.
- Incident context and involved identities.
- Investigation and response workflow.

### 31. Identity-Based Detections
Published console guide navigation: Identity Protection > Monitor > Identity-based detections.

Features:
- Identity detection list.
- Detection details.
- User / account context.
- Source endpoint and application context where available.
- Detection attributes and investigation pivots.

### 32. Users and Endpoints
Features:
- Identity user inventory.
- Endpoint / identity relationships.
- User and device context.
- Search and details.

### 33. Threat Hunter
Features:
- Identity threat hunting.
- Investigative query / search activity.
- Related identities and events.

### 34. Identity Reports
Features:
- Identity security reporting.
- Insights and incident-related reports.
- Export / review capabilities where permitted.

### 35. Identity Policies and Administration
Features:
- Identity policy management.
- Domain / sensor administration.
- Notifications.
- Role-based access and administrative controls.

## B7. Exposure Management

### 36. Asset Management / Asset Inventory
Features:
- Asset discovery.
- Internal and external asset visibility.
- Asset details and classification.
- Asset criticality and context.
- Accounts and installed applications where supported.

### 37. External Attack Surface
Features:
- Internet-facing asset discovery.
- Publicly exposed services.
- External asset context.
- Exposure issue filters.
- Risk / remediation context.

### 38. Vulnerability Management — Vulnerabilities
Features:
- Vulnerability inventory.
- Affected assets.
- Severity and vulnerability details.
- Risk prioritization.
- Vulnerability reports.

### 39. Installed Patches
Features:
- Installed patch inventory.
- Host / asset context.
- Remediation tracking and report views.

### 40. Configuration Assessment
Features:
- Configuration findings.
- Security baseline / benchmark deviations.
- Affected assets.
- Assessment results and prioritization.

### 41. Attack Path Analysis
Features:
- Relationships between assets and exposures.
- Possible attack paths.
- Risk prioritization.
- Remediation guidance.

## B8. Cloud Security

### 42. Cloud Posture
Documented report areas include:
- Indicators of misconfiguration.
- Cloud indicators of attack.
- Cloud posture findings.

### 43. Cloud Assets
Features:
- Cloud account / asset inventory.
- Cloud resource context.
- Resource relationships and findings.

### 44. Kubernetes and Containers Inventory
Features:
- Kubernetes asset visibility.
- Container inventory.
- Container detail context.
- Image and package relationships.

### 45. Image Assessments
Features:
- Container image vulnerabilities.
- Package findings.
- Malware / secrets / other image detections where supported.
- Image compliance information.

### 46. Container Vulnerabilities and Compliance
Features:
- Running container vulnerability findings.
- Container image compliance.
- CIS benchmark deviations.
- Remediation context.

### 47. Serverless Security
Features:
- Serverless function inventory / context.
- Function vulnerabilities.
- Function detections and related findings.

## B9. Next-Gen SIEM

### 48. Advanced Event Search
Features:
- Search across security events.
- CrowdStrike and supported third-party telemetry.
- Time-based search.
- Field filters.
- Query results and investigation pivots.
- Data access scopes.

### 49. Unified Detections
Published Falcon console guide navigation: Next-Gen SIEM > Monitor and investigate > Detections.

Features:
- Unified detections from supported data sources.
- Detection attributes.
- Severity / source context.
- Investigation and follow-up actions.

### 50. Cases
Features:
- Security case inventory.
- Case details.
- Related detections and events.
- Investigation context and notes.
- Case status and ownership, subject to configured product capabilities.

### 51. Data Connectors / Ingestion
Features documented in Next-Gen SIEM developer resources:
- HTTP Event Collector (HEC) ingestion.
- Third-party data onboarding.
- Custom parser development.
- Data normalization using CrowdStrike Parsing Standard.
- Connector / parser standards and operating limits.

### 52. Correlation Rules
Features:
- Query-based detection logic.
- Rules to generate detections / incidents / cases.
- Rule configuration and management.

### 53. Scheduled Searches
Features:
- Saved or scheduled event searches.
- Query run management.
- Search-based detection workflows.

## B10. Automation and Administration

### 54. Workflows / Fusion SOAR
Features:
- Trigger-based automation.
- Investigation enrichment.
- Response workflow execution.
- Workflow status and history.
- Integration actions.
- Approval / role requirements where configured.

### 55. Notifications
Features:
- Incident notifications.
- Detection notifications.
- Policy / cloud finding notifications where configured.
- Intelligence news and report notifications.

### 56. Dashboards and Reports
Features:
- Preset, private and shared dashboards.
- Custom widgets.
- Charts and tables.
- Drill-down into underlying records.
- Scheduled report configuration.
- Export by supported format.

### 57. User Management
Features:
- User list.
- User details.
- Add / remove users.
- Role assignment.
- Host group and cloud group assignment.
- Access scope assignment.

### 58. Role Management
Features:
- Default roles.
- Custom roles.
- Role permissions.
- Role assignment.
- Subscription-specific permissions.

### 59. Access Scope Management
Features:
- Access scopes for detections and event-search data.
- Data-source / vendor filters.
- User assignment.
- Fine-grained access controls on top of roles.

### 60. Audit Logs and Activity
Features:
- Administrative / activity event visibility.
- User and configuration changes.
- Security operation audit context.
- Search and review based on permission.

---

# Part C — Quick comparison of major page groups

| Security area | Microsoft Defender | CrowdStrike Falcon |
|---|---|---|
| Central overview | Defender portal home / service dashboards | Falcon Status Dashboard; Dashboards and Reports |
| Incidents | Incidents and Incident details | CrowdScore incidents; SIEM Cases |
| Alerts / detections | Alerts and Alert details | Endpoint, XDR, Identity, Mobile, Data Protection and Unified detections |
| Device / host inventory | Assets > Devices | Host Management; Hosts |
| Investigation | Advanced Hunting; incident investigation | Search; Hunt; Timelines; Hosts; Processes; Users |
| Endpoint response | Device isolation and supported actions | Quarantine; Real-Time Response; Network Containment |
| Threat intelligence | Threat Analytics | Adversaries; Reports and Feeds; Indicators; Sandbox; MalQuery |
| Vulnerabilities | Recommendations; Remediation; Inventories; Weaknesses; Event Timeline | Vulnerabilities; Installed Patches; Configuration Assessment |
| Identity | Defender for Identity signals and investigation | Identity Insights; Incidents; Detections; Users; Threat Hunter |
| Cloud | Defender for Cloud Apps; Defender for Cloud integration | Cloud Posture; Cloud Assets; Containers; Image Assessments |
| SIEM | Microsoft Sentinel in Defender portal | Next-Gen SIEM; Advanced Event Search; Connectors; Parsers; Correlation Rules |
| Automation | Action Center; supported automated response | Workflows / Fusion SOAR; RTR workflows |
| Administration | Settings, Roles, Permissions, API and asset rules | User Management, Roles, Access Scopes, Policies, Audit and Notifications |

---

# Part D — Important limitations and research notes

1. Yeh page catalog publicly documented console areas aur module capabilities ka research map hai. Isse universal, identical menu tree na samjhein.
2. Microsoft Defender portal mein user ko sirf wahi security features dikhte hain jo unke subscriptions / services enable karte hain.
3. CrowdStrike Falcon console mein purchased modules, assigned roles, access scopes aur tenant configuration ke mutabik pages badalte hain.
4. Same feature alag product version ya portal update mein naye menu path par move ho sakta hai.
5. Some entries are actual navigation pages; others are tabs, detail views, APIs, workflows or investigation capabilities.
6. Real-time response, quarantine, isolation, policy changes aur other high-impact actions role / permission dependent hain.
7. Product screenshots, proprietary UI text, icons, logos, source code or design assets are not reproduced in this research note.
8. All feature descriptions in this file are original summaries in simple Hinglish. Official links are provided for verification.

---

# Part E — Official sources

## Microsoft sources

1. Defender portal overview and unified experiences: https://learn.microsoft.com/en-us/defender-xdr/microsoft-365-defender-portal
2. Device inventory: https://learn.microsoft.com/en-us/defender-endpoint/machines-view-overview
3. Advanced hunting modes: https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-modes
4. Custom detection rules: https://learn.microsoft.com/en-us/defender-xdr/custom-detection-rules
5. Action Center: https://learn.microsoft.com/en-us/defender-xdr/m365d-action-center
6. Threat Analytics: https://learn.microsoft.com/en-us/microsoft-365/security/defender/threat-analytics
7. Threat Explorer / Real-time detections: https://learn.microsoft.com/en-us/defender-office-365/threat-explorer-threat-hunting
8. Vulnerability recommendations: https://learn.microsoft.com/en-us/defender-vulnerability-management/tvm-security-recommendation
9. Vulnerability remediation: https://learn.microsoft.com/en-us/defender-vulnerability-management/tvm-remediation
10. Cloud discovery: https://learn.microsoft.com/en-us/defender-cloud-apps/set-up-cloud-discovery
11. Cloud discovery policies: https://learn.microsoft.com/en-us/defender-cloud-apps/policies-cloud-discovery

## CrowdStrike sources

1. Falcon Console Management guide (official PDF): https://downloads.ctfassets.net/k6m8nslhjx0z/3QCndWbQV9L5rt6kYHxBjq/2f571bd8a378367b1aa9e1b445bd1f8b/CrowdStrike_Falcon_Console_Management.pdf
2. Falcon API reference and product domains: https://developer.crowdstrike.com/api-reference/overview/
3. Falcon Next-Gen SIEM developer documentation: https://developer.crowdstrike.com/ngsiem/
4. Falcon UI extension locations (examples of console page context): https://developer.crowdstrike.com/foundry/experience-capabilities/ui-extensions/
5. Falcon Exposure Management: https://www.crowdstrike.com/en-us/platform/exposure-management/

## Research update

Research compiled: 2026-11-02. Since product consoles change, re-check official documentation and release notes before treating any navigation path or capability as current in a specific tenant.
