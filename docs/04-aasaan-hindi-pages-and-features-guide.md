# Microsoft Defender & CrowdStrike Falcon — Aasaan Hindi Guide

**Project:** Security — Deep Research & Study Notes  
**Owner / Content Creator:** Sandeep Barupal  
**Copyright:** © 2026 Sandeep Barupal. All rights reserved, except as stated below.

> Yeh document learning aur research ke liye hai. Ismein product ke page areas ko aasan Hindi (Hinglish) mein samjhaya gaya hai. Kuch headings actual console navigation hain aur kuch related screens ko samajhne ke liye banaye gaye research groups hain. Har customer ke account mein saare pages available hon, yeh zaroori nahi.

---

## 1. Sabse pehle: Ye platforms kya karte hain?

Microsoft Defender aur CrowdStrike Falcon company ke computers, servers, user accounts, cloud services aur data ko cyber attacks se bachane ke liye security tools provide karte hain.

Simple example: Agar kisi employee ke computer mein harmful file aa jaye, security platform us activity ko detect kar sakta hai, alert bana sakta hai, security team ko investigation mein help kar sakta hai aur permission hone par device ko isolate ya doosra response action le sakta hai.

**Important words:**
- **Threat:** Koi possible cyber danger, jaise malware ya hacker activity.
- **Alert:** Security system ki warning.
- **Incident:** Ek hi attack se jude alerts aur evidence ka group.
- **Endpoint:** Computer, laptop, server ya supported mobile device.
- **EDR:** Device par hone wali activity ko dekhkar attack pakadna aur response mein help karna.
- **XDR:** Email, identity, endpoint aur cloud jaise multiple sources ke security signals ko jodkar attack samajhna.
- **SIEM:** Alag-alag systems ke logs aur events ko ek jagah collect aur search karna.
- **SOAR:** Security ke repeat hone wale tasks ko rules aur workflows se automate karna.
- **Vulnerability:** Software ya system ki security weakness.
- **Threat hunting:** Security data mein chhupe ya abhi alert na bane suspicious behavior ko dhoondhna.

---

# Part A — Microsoft Defender

## 2. Microsoft Defender ke main pages

Microsoft Defender ek family of security products hai. Defender portal mein wahi modules dikhte hain jo organization ke license, setup aur permissions mein enabled hote hain.

### 2.1 Home / Security Overview
**Is page ka kaam:** Company ki overall security ka short summary dikhana.

Yahan aam taur par:
- Active incidents aur alerts ka summary.
- High-risk devices ya users ki information.
- Vulnerability / exposure ka overview.
- Recent security activity.
- Investigation ke shortcuts.

**Example:** Security manager login karke jaldi dekh sakta hai ki kitne serious incidents open hain.

### 2.2 Incidents
**Is page ka kaam:** Ek attack se jude kai alerts ko ek case ki tarah manage karna.

Features:
- Incidents ki list.
- Severity aur status filters.
- Incident assign karna.
- Incident ko active ya resolved mark karna.
- Related alerts, devices aur users dekhna.
- Attack ki timeline aur investigation notes dekhna.

**Example:** Ek phishing email se user account aur laptop dono affect hue. Related alerts ek incident ke andar dikh sakte hain.

### 2.3 Alerts
**Is page ka kaam:** Security system ne jo warning detect ki hai, uski detail dekhna.

Features:
- Alert list aur severity.
- Alert ka source aur time.
- Kis device ya user se alert related hai.
- Alert evidence aur description.
- Related incident.
- Available response actions.

**Alerts aur Incidents ka difference:** Alert ek warning/detection hota hai. Incident ek ya zyada related alerts ko jodkar banaya gaya investigation case ho sakta hai.

### 2.4 Devices / Device Inventory
**Is page ka kaam:** Company ke computers aur servers ki list rakhna.

Features:
- Device name aur operating system.
- Device risk aur exposure level.
- Last activity / last seen.
- Sensor health.
- Related alerts aur incidents.
- Installed software aur vulnerabilities.
- Device details aur activity timeline.
- Supported cases mein device isolate karna ya investigation package collect karna.

### 2.5 Vulnerability Management / Exposure
**Is page ka kaam:** Software aur devices ki security weaknesses dhoondhna.

Features:
- Weakness / CVE list.
- Affected software aur devices.
- Severity aur risk.
- Security recommendations.
- Fix karne ke steps.
- Remediation progress.
- Software inventory aur security baseline.

**Example:** Kisi company ke computers mein purana browser version hai. Platform affected devices aur update recommendation dikhane mein help kar sakta hai.

### 2.6 Advanced Hunting
**Is page ka kaam:** Security data mein search/query chala kar unusual activity dhoondhna.

Features:
- Query editor ya guided query builder.
- Time range select karna.
- Search results ko table mein dekhna.
- Results filter aur sort karna.
- Query save/history, where supported.
- Device, user aur event details par drill-down.

**Example:** Analyst check kar sakta hai ki pichhle 24 ghanton mein kisi device par unusual process chala tha ya nahi.

### 2.7 Threat Analytics
**Is page ka kaam:** Naye cyber attacks, campaigns aur threats ke baare mein information dena.

Features:
- New / important threats.
- Threat reports.
- Attack techniques.
- Organization par possible impact.
- Affected assets aur recommended actions.

### 2.8 Action Center
**Is page ka kaam:** Security issue solve karne ke liye chal rahe actions ka status dekhna.

Features:
- Pending actions.
- Completed actions.
- Failed actions.
- Action kisne start kiya.
- Kis device/file par action hua.
- Approval aur action history, where supported.

### 2.9 Email & Collaboration Security
**Is page ka kaam:** Fake emails, phishing links aur harmful attachments ki jaanch karna.

Features:
- Email search / Explorer.
- Sender aur receiver details.
- Email subject aur delivery status.
- Phishing / malware detections.
- Suspicious URLs aur attachments.
- Related messages / campaigns.
- Supported email remediation.

**Note:** Threat Explorer aur real-time detection jaise views ki availability Microsoft 365 / Defender for Office 365 license par depend karti hai.

### 2.10 Identity Protection
**Is page ka kaam:** User accounts aur identity se jude risks dekhna.

Features:
- Users / identities.
- Risky users aur identity alerts.
- Suspicious sign-in ya account activity, where integrated.
- Related devices aur applications.
- Investigation aur permitted response.

### 2.11 Cloud Apps
**Is page ka kaam:** Company ke cloud applications ke use aur risk ko samajhna.

Features:
- Discovered cloud apps ki list.
- App risk details.
- App usage / activity reports, when connected.
- Policies aur policy alerts.
- Unsanctioned apps ki identification, where configured.

### 2.12 Cloud Security
**Is page ka kaam:** Cloud servers, services aur resources ki security condition dekhna.

Features:
- Cloud assets.
- Security recommendations.
- Misconfiguration findings.
- Cloud workload risks.
- Compliance posture, where supported.

**Note:** Defender for Cloud ki kuch screens alag experience mein hoti hain; unhe automatically Defender XDR ke same page ka hissa na samjhein.

### 2.13 Reports
**Is page ka kaam:** Security activity ka summary aur report dekhna.

Possible reports:
- Threat / incident reports.
- Device reports.
- Vulnerability reports.
- Email security reports.
- Security trends.

Available report types connected products par depend karte hain.

### 2.14 Settings & Permissions
**Is page ka kaam:** Portal aur users ko safely configure karna.

Features:
- User roles aur permissions.
- Security settings.
- Notifications.
- Integrations / data connectors.
- API configuration.
- Audit history.

### 2.15 Microsoft Sentinel (related security product)
**Iska kaam:** Multiple systems se logs collect karna, unhe search karna aur security incidents investigate karna.

Common areas:
- Logs.
- Analytics rules.
- Incidents.
- Workbooks / dashboards.
- Data connectors.
- Hunting.
- Automation rules / playbooks.

**Note:** Sentinel ek separate Microsoft security product hai jo Defender portal experience ke saath integrate ho sakta hai. License aur portal setup ke hisaab se availability badal sakti hai.

---

# Part B — CrowdStrike Falcon

## 3. CrowdStrike Falcon ke main pages

Falcon ek modular security platform hai. Customer ke purchased modules, account settings aur user permissions ke hisaab se console ke pages alag ho sakte hain.

### 3.1 Dashboard / Overview
**Is page ka kaam:** Security team ko poore environment ka short status dikhana.

Features:
- Threat aur detection summary.
- Protected hosts ka overview.
- Recent activity.
- Security trends.
- Dashboard widgets aur filters.

### 3.2 Hosts / Host Management
**Is page ka kaam:** Company ke computers aur servers ko manage aur monitor karna.

Features:
- Host / device list.
- Hostname, operating system aur IP details.
- Falcon sensor status.
- Last seen information.
- Host groups aur tags.
- Host details aur related detections.
- Policy assignment, where permitted.

### 3.3 Endpoint Detections
**Is page ka kaam:** Computer par suspicious activity aur possible attack ki details dekhna.

Features:
- Detection list.
- Detection severity / details.
- Affected host aur user.
- Related process / file activity, where available.
- Detection review aur investigation.

### 3.4 Incidents / CrowdScore
**Is page ka kaam:** Related detections aur activity ko ek incident ke roop mein samajhna aur prioritize karna.

Features:
- Incident list.
- Priority / score context.
- Related hosts aur detections.
- Investigation details.
- Status aur follow-up.

**Note:** Falcon console mein incident aur detection ke exact labels / workflows product updates aur enabled modules ke saath change ho sakte hain.

### 3.5 Real-Time Response (RTR)
**Is page ka kaam:** Authorized security operator ko selected endpoint par remote investigation karne dena.

Features:
- Target host select karna.
- Secure response session start karna.
- Supported commands chalana.
- Command output dekhna.
- Session history aur audit record.
- Session end karna.

**Safety:** Ye powerful tool hai. Iske liye strict permissions, approved commands, logging aur session controls zaroori hain.

### 3.6 Investigate / Search
**Is page ka kaam:** Falcon environment mein available security records aur entities ko search karna.

Features:
- Search box.
- Search suggestions.
- Result list.
- Filters.
- Related records par drill-down.

### 3.7 Hunt / Threat Hunting
**Is page ka kaam:** Security telemetry mein hidden ya unusual activity search karna.

Features:
- Query-based search, where enabled.
- Time range.
- Event / process investigation.
- Related host aur user par pivot.
- Search results aur investigation.

### 3.8 Timelines
**Is page ka kaam:** Device ya security event par kya-kya hua, uska time-wise sequence dekhna.

Features:
- Events ka order.
- Event time.
- Process / activity details.
- Related detections.
- Investigation context.

### 3.9 Threat Intelligence
**Is page ka kaam:** Known hackers, malware aur suspicious internet infrastructure ke baare mein information dekhna.

Features:
- Threat actor profiles.
- IP, domain, URL aur file hash search, where supported.
- Malware / campaign information.
- Indicators of compromise.
- Intelligence reports.
- Related detections.

### 3.10 Exposure Management
**Is page ka kaam:** Company ke assets aur unki weaknesses ka risk samajhna.

Features:
- Asset inventory.
- Vulnerability findings.
- Risk priority.
- External attack surface information, where licensed.
- Remediation tracking.
- Risk trends.

### 3.11 Cloud Security
**Is page ka kaam:** Cloud accounts, servers, containers aur cloud configurations ki security check karna.

Features:
- Cloud account / asset inventory.
- Misconfiguration findings.
- Workload security.
- Container / Kubernetes visibility, where supported.
- Vulnerability findings.
- Compliance posture.
- Remediation recommendations.

### 3.12 Identity Protection
**Is page ka kaam:** User accounts aur identity-based attacks ko identify karna.

Features:
- Identity-related detections.
- User / account context.
- Suspicious account activity.
- Risk details.
- Related endpoint activity.
- Investigation workflow.

### 3.13 Next-Gen SIEM
**Is page ka kaam:** Alag-alag tools aur systems ke security logs ko ek jagah collect aur analyze karna.

Features:
- Log / event search.
- Data sources aur connectors.
- Data ingestion health.
- Saved searches.
- Dashboards.
- Detection rules.
- Cases / investigations.
- Data retention controls, where available.

### 3.14 Automation / Falcon Fusion
**Is page ka kaam:** Repeat hone wale security tasks ko automatic workflow se chalana.

Features:
- Workflow list.
- Workflow builder.
- Triggers aur conditions.
- Action steps.
- Integration actions.
- Approval steps.
- Run history aur error status.

### 3.15 Reports & Dashboards
**Is page ka kaam:** Security team ko performance, detections aur risk ki reports dena.

Features:
- Ready-made dashboards.
- Custom dashboard widgets.
- Filters aur drill-down.
- Scheduled reports, where supported.
- Export options.

### 3.16 Administration / Settings
**Is page ka kaam:** Falcon account aur security configuration manage karna.

Features:
- User management.
- Roles aur permissions.
- Prevention policies.
- Host groups.
- API clients / integrations.
- Audit / activity records.
- Platform configuration.

---

## 4. Dono platforms ka simple comparison

| Research area | Microsoft Defender | CrowdStrike Falcon |
|---|---|---|
| Main dashboard | Security overview | Falcon dashboard |
| Devices | Device inventory | Hosts / host management |
| Warnings | Alerts | Detections |
| Attack cases | Incidents | Incidents / CrowdScore workflows |
| Device protection | Defender for Endpoint | Falcon endpoint security |
| Investigation | Advanced Hunting | Search / Hunt / Timelines |
| Weaknesses | Vulnerability Management | Exposure Management |
| Email safety | Defender for Office 365 | Product / integration dependent |
| User accounts | Identity protection | Identity protection |
| Cloud | Defender for Cloud / Cloud Apps | Falcon Cloud Security |
| Logs | Microsoft Sentinel | Falcon Next-Gen SIEM |
| Automation | Investigation / response automation and Sentinel playbooks | Falcon Fusion workflows |
| Reports | Product-specific reports | Dashboards and reports |
| Settings | Roles, permissions, connectors | Roles, policies, API and integrations |

**Comparison rule:** Table ka matlab yeh nahi ki dono products ke features bilkul same hain. Har product ki capability, license aur setup alag ho sakta hai.

---

## 5. Security team ka kaam kaise chalta hai?

1. **Monitor:** Platform devices, accounts aur connected systems se security data dekhta hai.
2. **Detect:** Suspicious activity identify hoti hai.
3. **Alert:** Security team ko warning milti hai.
4. **Triage:** Analyst check karta hai ki warning kitni serious hai.
5. **Investigate:** Device, user, file aur event ki detail dekhi jaati hai.
6. **Respond:** Permission ke hisaab se threat ko block, isolate ya remediate kiya ja sakta hai.
7. **Recover:** Affected system ko safe condition mein wapas laaya jata hai.
8. **Report:** Incident aur action ka record maintain hota hai.

---

## 6. Common page elements jo research mein dekhe gaye

Har relevant page par ye controls mil sakte hain:
- Search bar.
- Filters.
- Sortable table.
- Date / time range.
- Severity aur status.
- Detail page / side panel.
- Related devices, users aur incidents.
- Activity history.
- Export.
- Bulk actions, where supported.
- Loading, empty aur error states.
- Permission warning.

Ye common research observations hain; har product ke har page par sab controls hona zaroori nahi.

---

## 7. Research aur real product ke beech difference

- Dashboard par sample alert dikhana real threat detection nahi hai.
- Sample device list dikhana real endpoint protection nahi hai.
- Fake “Isolate Device” button real computer ko network se isolate nahi karta.
- Static vulnerability table real vulnerability scanning nahi hai.
- Mock logs real SIEM ingestion nahi hain.
- Static AI answer real security investigation ka proof nahi hai.

Real security action ke liye authorized connectors, endpoint agents, backend services, permissions, logging aur tested response systems chahiye.

---

## 8. Official sources

### Microsoft
- Defender documentation: https://learn.microsoft.com/en-us/defender/
- Defender XDR incidents: https://learn.microsoft.com/en-us/defender-xdr/incidents-overview
- Device inventory: https://learn.microsoft.com/en-us/defender-endpoint/machines-view-overview
- Advanced Hunting: https://learn.microsoft.com/en-us/defender-xdr/advanced-hunting-overview
- Defender for Office 365 Explorer: https://learn.microsoft.com/en-us/defender-office-365/threat-explorer
- Vulnerability Management: https://learn.microsoft.com/en-us/defender-vulnerability-management/next-gen-threat-and-vulnerability-management
- Microsoft Sentinel: https://learn.microsoft.com/en-us/azure/sentinel/

### CrowdStrike
- Falcon platform: https://www.crowdstrike.com/platform/
- Falcon documentation: https://falcon.crowdstrike.com/documentation/
- Developer documentation: https://developer.crowdstrike.com/
- Next-Gen SIEM: https://www.crowdstrike.com/platform/next-gen-siem/
- Cloud Security: https://www.crowdstrike.com/platform/cloud-security/
- Exposure Management: https://www.crowdstrike.com/platform/exposure-management/

---

## 9. Copyright, trademark aur ownership note

Microsoft Defender, Microsoft, CrowdStrike aur Falcon apne respective owners ke product / brand names aur trademarks hain. Is research ka un companies se koi affiliation, endorsement ya sponsorship nahi hai.

Is document ka explanatory text original Hinglish wording mein likha gaya hai. Third-party facts, product names aur official documentation apne respective owners ke hain. Official website ke paragraphs, screenshots, logos, icons ya proprietary design ko copy karke reproduce nahi kiya gaya hai.

**Research checked / updated:** 4 November 2026. Product features aur navigation badal sakte hain; implementation ya final comparison se pehle official documentation dobara verify karein.
