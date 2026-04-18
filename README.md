# Hi, I'm [Your Name] 👋

> **IT & Cloud Support Engineer** · CompTIA A+ · Network+ · Security+ · ITIL 4 · AZ-900 · AZ-104

I build things, break them, diagnose exactly why they broke, and document the whole process.
This GitHub is the proof — seven production-quality repositories built from a fully operational
Proxmox home lab running Windows Server 2022 Active Directory, pfSense VLAN segmentation,
Azure hybrid identity, Splunk SIEM, Nessus vulnerability scanning, and Microsoft Intune.
Not tutorials followed. Not screenshots of someone else's work. Built from scratch.

---

## 🧰 What I Work With

**Cloud & Identity**
![Azure](https://img.shields.io/badge/Azure-AZ--104-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white)
![Entra ID](https://img.shields.io/badge/Entra_ID-AD_Connect-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![Intune](https://img.shields.io/badge/Intune-MDM-0078D4?style=flat-square&logo=microsoft&logoColor=white)

**Security & Monitoring**
![Splunk](https://img.shields.io/badge/Splunk-SIEM-000000?style=flat-square&logo=splunk&logoColor=white)
![Nessus](https://img.shields.io/badge/Nessus-Vulnerability_Scanning-00AC4F?style=flat-square)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-Mapped-red?style=flat-square)

**Networking & Infrastructure**
![pfSense](https://img.shields.io/badge/pfSense-Firewall-212A5E?style=flat-square)
![Proxmox](https://img.shields.io/badge/Proxmox-VE_8.x-E57000?style=flat-square&logo=proxmox&logoColor=white)
![WireGuard](https://img.shields.io/badge/WireGuard-VPN-88171A?style=flat-square)

**Scripting & Automation**
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-5391FE?style=flat-square&logo=powershell&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-Linux_Admin-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)

**Process**
![ITIL 4](https://img.shields.io/badge/ITIL_4-Foundation-6A1FAB?style=flat-square)
![KQL](https://img.shields.io/badge/KQL-Log_Analytics-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white)

---

## 📁 Portfolio Repositories

### 🖥️ [helpdesk-ad-automation](https://github.com/YOUR-USERNAME/helpdesk-ad-automation)
> PowerShell + Python automation for Active Directory and L1 help desk operations

5 PowerShell scripts covering the full AD user lifecycle — bulk creation (45 min → 4 min),
password reset with identity verification and random temp password generation, intelligent
account unlock handling 4 distinct scenarios, complete offboarding automation, and a quarterly
access review report. Plus a Python ticket intake tool that standardises L1 triage across
7 issue types with ITIL 4 P1–P4 classification, SLA targets, and JSON audit logging.

`PowerShell` `Python` `Active Directory` `ITIL 4` `CompTIA A+`

---

### 🌐 [network-noc-runbook](https://github.com/YOUR-USERNAME/network-noc-runbook)
> Structured L1 NOC troubleshooting runbook with OSI-layered methodology

6 procedures covering the most common network incidents — connectivity triage with a
ping interpretation table that maps results directly to OSI layers, DNS failure diagnosis,
PRTG alert response for 6 sensor types, VPN MTU testing and remediation, pfSense VLAN
and inter-VLAN firewall procedures, and a complete ITIL 4 L2 escalation handoff template.
Includes a lab topology diagram with full VLAN firewall rule tables and design justifications.

`CompTIA Network+` `pfSense` `PRTG` `VLAN` `ITIL 4`

---

### 🔐 [soc-incident-response-playbook](https://github.com/YOUR-USERNAME/soc-incident-response-playbook)
> Tier 1 SOC analyst playbooks with MITRE ATT&CK mapping and live Splunk queries

4 operational playbooks — phishing triage (complete P1/P2 cycle from user call script
to forensic preservation), malware alert response (scope assessment, containment rationale,
PowerShell evidence collection), failed authentication investigation (brute force vs spray vs
stuffing vs Pass-the-Hash pattern detection), and false positive classification. Every scenario
mapped to MITRE ATT&CK tactic + technique + ID. 20+ SPL queries tested in a live Splunk
Free instance. MFA enforcement checklist and IAM access review procedure aligned to ISO 27001,
SOC 2, and GDPR-equivalent data protection frameworks.

`CompTIA Security+` `Splunk` `SPL` `MITRE ATT&CK` `ITIL 4`

---

### ☁️ [azure-hybrid-lab](https://github.com/YOUR-USERNAME/azure-hybrid-lab)
> Fully documented Azure hybrid cloud lab — AZ-104 in practice, not theory

A working Azure environment connecting on-premises AD (contoso.local) to Entra ID via
AD Connect with Password Hash Sync. VNet with two subnets, NSG deny-all with explicit
allows, Azure Bastion eliminating public management port exposure. RBAC assigned at
subscription/resource group/resource scope demonstrating least privilege at each level.
Log Analytics Workspace with 8 KQL queries verified returning real data. CPU metric
alert tested end-to-end (generated load → alert fired → email received). Intune device
compliance, Win32 app silent deployment, and Conditional Access integration.

The design decisions document answers every architecture question before it is asked:
why PHS over PTA, why Bastion over public RDP, why RBAC at RG scope not subscription.
The troubleshooting log documents 5 real issues — including the Stop vs Restart
distinction for AllocationFailed, and a pfSense rule accidentally blocking AD Connect sync.

`AZ-104` `Azure` `Entra ID` `AD Connect` `Intune` `KQL` `Log Analytics`

---

### 📋 [azure-l1-support-runbook](https://github.com/YOUR-USERNAME/azure-l1-support-runbook)
> Azure Portal L1 support runbook — what to do when an alert fires, not just what things are

6 runbooks covering the most common Azure support ticket types: VM troubleshooting
(power states, Activity Log, Resource Health, Boot Diagnostics, Serial Console),
Entra ID user management (the critical cloud-only vs synced account distinction that
prevents the "change reverts in 30 minutes" mistake), NSG and network diagnostics
(IP Flow Verify, Effective Security Rules, Connection Troubleshoot), App Service
recovery (502/503/504 triage, deployment slot rollback, Kudu console), storage
access (RBAC vs firewall vs access key vs SAS token diagnosis), and cost management
(orphaned resource cleanup checklist, budget alerts, quota management). Plus 25+ KQL
queries and a reference for 20 common Azure error codes with root cause and L1 action.

`AZ-104` `Azure` `KQL` `ITIL 4`

---

### ⚙️ [windows-linux-support-scripts](https://github.com/YOUR-USERNAME/windows-linux-support-scripts)
> 14 production-quality scripts solving real recurring ticket types across Windows and Linux

**PowerShell (8 scripts):** DNS flush with post-flush resolution verification · print queue
clear with full spooler lifecycle management · colour-coded disk space report with cleanup
guidance · network stack reset with mandatory typed confirmation · comprehensive system info
collection · multi-host multi-port TCP connectivity tester with service name lookup ·
consolidated multi-log Windows Event Log error retrieval · service restart with timeout
handling and health verification.

**Bash (6 scripts):** Linux system health report with CPU/memory/disk/network/process analysis ·
timestamped backup with archive integrity verification and retention cleanup · user provisioning
with regex validation, group checks, secure password handling, and 90-day expiry policy ·
log cleanup with dry-run mode and gzip compression · disk usage analysis identifying largest
directories and recently created large files · service monitor with auto-restart mode for cron.

Every script: input validation before acting · typed confirmation for destructive operations ·
timestamped logging · before/after state reporting · human-readable colour-coded output.

`PowerShell` `Bash` `CompTIA A+` `CompTIA Network+`

---

### 🏗️ [homelab-documentation](https://github.com/YOUR-USERNAME/homelab-documentation)
> Complete build documentation for a six-VM enterprise home lab built from scratch on Proxmox VE

The repo that proves everything else. A working enterprise simulation running:
**Windows Server 2022** with AD DS, DNS, DHCP, and Group Policy ·
**pfSense** with three-VLAN segmentation (Work/Guest/Management), inter-VLAN firewall
rules, and WireGuard VPN · **Azure hybrid identity** via AD Connect ·
**Splunk Free** SIEM with Universal Forwarder from the DC, SPL security dashboards ·
**Nessus Essentials** with CVSS-based remediation workflow ·
**Microsoft Intune** device compliance and Conditional Access.

Full architecture diagrams with traffic flow examples, complete VLAN firewall rule tables
with per-rule justifications, AD Connect sync flow diagram, and a cert-to-lab mapping
document showing which specific lab component validates each A+, Network+, Security+,
AZ-900, AZ-104, and ITIL 4 exam objective.

The troubleshooting log documents 8 real issues encountered during the build — each with
investigation steps, root cause, and fix. Including: DNS service startup type changed by
mistake · pfSense rule order blocking AD Connect sync · DHCP relay missing in a routed
VLAN environment · Splunk inputs.conf without outputs.conf causing silent data loss ·
Nessus returning false-zero results because Windows Firewall blocked the scanner ·
SYSVOL permissions broken by a Proxmox snapshot rollback.

`Proxmox` `Windows Server 2022` `pfSense` `Splunk` `Nessus` `Intune` `All Certs`

---

## 🔬 Lab Environment

```
Hypervisor  : Proxmox VE 8.x
Domain      : contoso.local (Windows Server 2022)
Firewall    : pfSense 2.7 — VLAN 10/20/99, WireGuard VPN
SIEM        : Splunk Free (Ubuntu 22.04, VLAN 99)
Scanner     : Nessus Essentials (Ubuntu 22.04, VLAN 10)
Kali Linux  : VLAN 20 (isolated) — pen testing, attack simulation
Azure       : Free trial + M365 Dev E5 Sandbox
              VNet 10.20.0.0/16, Bastion, Log Analytics, Intune
```

---

## 📜 Certifications (in progress / completed)

| Cert | Status |
|------|--------|
| CompTIA A+ | ✅ Trained — Cengage curriculum (665+ hrs total across all certs) |
| CompTIA Network+ | ✅ Trained |
| CompTIA Security+ | ✅ Trained |
| ITIL 4 Foundation | ✅ Trained — AXELOS + Sybex |
| Microsoft AZ-900 | ✅ Trained — Microsoft Press |
| Microsoft AZ-104 | ✅ Trained — Microsoft Press |

---

## 💡 What Separates This Portfolio

**The troubleshooting logs.** Every repo where something could go wrong has a documented
record of what actually went wrong, how it was diagnosed, and what fixed it. DNS service
startup type misconfigured. pfSense rule order blocking Azure sync. DHCP relay missing
in a routed network. Splunk outputting nowhere because outputs.conf was absent. Nessus
returning zero findings because Windows Firewall blocked the scan.

These are not made-up scenarios. They are things that happened during the build and were
diagnosed in real time. That is the difference between reading about IT and doing IT.

**The design decisions.** Every architectural choice has a written justification. Why
Password Hash Sync over Pass-Through Authentication. Why Azure Bastion over public RDP.
Why RBAC at resource group scope not subscription scope. Why Splunk is on the management
VLAN rather than the corporate VLAN. These are interview questions — answered in the code.

**The lab is operational, not theoretical.** AD Connect syncs. The Splunk dashboard shows
real Windows Security events. The Nessus scan returns real findings. The Intune compliance
policy evaluates a real enrolled device. The pfSense VLAN rules are verified with connectivity
tests. Everything described is deployed and working.

---

## 📬 Get in Touch

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-LINKEDIN)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:your.email@example.com)

---

<sub>All scripts and playbooks were built and tested in a working lab environment. Nothing here is copied from documentation or generated without hands-on validation. The troubleshooting logs in each repository are the evidence of that.</sub>