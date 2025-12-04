# 🛡️ Cyber Intelligence Playbooks, Hunting, Enrichment, and Reporting (CIPHER)  
**A Structured, Scalable, and Actionable CTI Knowledge System**

This repository contains a complete **Cyber Threat Intelligence (CTI) Obsidian vault framework** designed to support analysts, incident responders, threat hunters, and security leaders. This vault provides a modular, highly structured system for documenting, analyzing, and maintaining intelligence using Obsidian’s markdown-based knowledge management model.

It includes **MITRE ATT&CK capsules**, **threat actor profiles**, **campaign tracking**, **malware documentation**, **IOC lifecycle management**, CTI briefings, and daily/weekly analytic workflows — all optimized for clarity, repeatability, and operational value.

---

## 📌 Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Vault Structure](#vault-structure)
- [Templates Included](#templates-included)
- [Core Concepts](#core-concepts)
- [MITRE ATT&CK Capsules](#mitre-attck-capsules)
- [Threat Actor Capsules](#threat-actor-capsules)
- [Malware Notes](#malware-notes)
- [Campaign Tracking](#campaign-tracking)
- [IOC Lifecycle Tracking](#ioc-lifecycle-tracking)
- [Analyst Workflow Templates](#analyst-workflow-templates)
- [How to Use This Vault](#how-to-use-this-vault)
- [Recommended Plugins](#recommended-plugins)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)

---

## 🔎 Overview
The CIPHER vault represents a **full CTI knowledge ecosystem** purpose-built for Obsidian. It allows analysts to create structured, interconnected CTI content that supports:

- Standardized, metadata-driven intelligence notes  
- Consistency through YAML templates  
- Rapid navigation via backlinks and graph views  
- Dataview-powered dashboards  
- MITRE ATT&CK alignment across the vault  
- Integration with SOC analysis, IR workflows, and threat hunting  

This system is built upon atomic, reusable note structures that promote **clarity**, **repeatability**, and **actionability**.

---

## ⭐ Key Features

- MITRE ATT&CK Tactic and Technique dashboards  
- Threat Actor profiles with TTP mappings and industry relevance  
- Malware family notes with behaviors, hashes, and detection rules  
- IOC lifecycle tracking with confidence, tagging, and relationships  
- Campaign tracking for actor activity, infrastructure, and IOCs  
- Daily and Weekly analysis templates  
- CTI briefing/reporting templates  
- Dataview-enabled dashboards for indexing and analysis  
- Structured folder hierarchy for CTI operations  
- Designed to scale into long-term intelligence repositories  

---

## 📁 Vault Structure

Below is the recommended folder structure:

```
.
├── _Templates/
|   ├── Briefing_Template
|   ├── Campaign_Template
|   ├── Daily_Analysis_Journal
|   ├── IOC_Template
|   ├── Malware_Template
|   ├── MITRE_Technique_Template
|   ├── Tactic_Dashboard_Template
│   └── Vulnerability_Template
├── 00_Dashboard & Index/
│   ├── Daily_Notes_Index
│   ├── Map_of_Content
|   ├── TA0001 - Initial Access Dashboard
|   ├── TA0002 - Execution Dashboard
|   ├── TA0003 - Persistence Dashboard
|   ├── TA0004 - Privilege Escalation Dashboard
|   ├── TA0005 - Defense Evasion Dashboard
|   ├── TA0006 - Credential Access Dashboard
|   ├── TA0007 - Discovery Dashboard
|   ├── TA0008 - Lateral Movement Dashboard
|   ├── TA0009 - Collection Dashboard
|   ├── TA0010 - Exfiltration Dashboard
|   ├── TA0011 - Command and Control Dashboard
|   ├── TA0040 - Impact Dashboard
|   ├── TA0042 - Resource Development Dashboard
│   └── TA0043 - Reconnaisance Dashboard
├── 01_Intelligence_Program/
|   ├── Metrics & Reporting
|   ├── PIRs
|   ├── Requirements
|   ├── Stakeholders
|   ├── Strategy
│   └── Workflows & SOPs
├── 02_Collections/
|   ├── Dark Web
|   ├── Government_ISACs
|   ├── Internal_Telemetry
|   ├── OSINT
│   └── Vendor_Feeds
├── 03_Threat_Actors/
├── 04_Campaigns/
├── 05_Malware & Tools/
├── 06_Vulnerabilities & CVEs/
│   ├── Exploitation_Chains
│   ├── KEV_Tracking
│   └── Patch_Timelines
├── 07_TTP Library (MITRE ATT&CK)/   
├── 08_Indicators & Observables
│   ├── Domains
│   ├── Hashes
│   ├── IPs
│   └── URLs
├── 09_IOCs/
├── 10_Analysis & Reporting/
│   └── Hyphotheses
├── 11_Intel_Requirements & PIRs/
│   ├── Business_Risks
│   ├── Customer_Personas
│   └── PIRs
├── 12_Training & Tradecraft/
│   └── CTI_Methodologies
├── 98_News_Articles/
└── 99_Attachments/



```

---

## 🧩 Templates Included

### MITRE Templates
- Tactic dashboard template  
- Technique capsule template for Txxxx and sub-techniques  
- Dataview tables for technique indexing  

### Threat Actor Template
Includes YAML for:
- Names and aliases  
- Country and motivations  
- Targeting focus  
- Associated TTPs  
- Malware used  
- Infrastructure  
- IOCs  
- Reporting history  
- Confidence levels  

### IOC Template
Includes fields for:
- Indicator type  
- Value  
- First/last seen  
- Confidence  
- Source  
- Tags  
- Related threat actor  
- Related malware or technique  
- Expiration and suppression  

### Malware Template
Includes:
- Family and type  
- Hashes  
- Behaviors and TTPs  
- Sandbox links  
- Detection rules (YARA, SIGMA, KQL)  
- Actor and campaign relationships  

### Campaign Template
Includes:
- Campaign ID  
- Threat actor  
- Sector targeting  
- MITRE mapping  
- Timeline  
- Infrastructure  
- Malware and IOCs  
- Key judgments  

### Briefing Template
Includes:
- Executive Summary  
- Key Judgments  
- Impact Assessment  
- TTP Breakdown  
- Recommended Actions  
- Appendix  

### Analyst Workflow Templates
- Daily Intelligence Journal  
- Weekly CTI Roll-Up  

---

## 🧠 Core Concepts

This vault is built on the following principles:

### Atomic Notes
Each concept is a standalone file:
- One actor  
- One technique  
- One malware family  
- One campaign  
- One IOC  

### YAML Metadata
Used for:
- Dataview queries  
- Cross-note consistency  
- Automated dashboards  
- Sorting, grouping, filtering  

### Relationship-Driven Intelligence
Use Obsidian links to tie notes together:
- Actors ↔ Campaigns  
- Campaigns ↔ Techniques  
- Techniques ↔ Malware  
- Malware ↔ IOCs  
- IOCs ↔ Campaigns  

### MITRE-First Model
Techniques act as the backbone for:
- Detection engineering  
- Threat hunting  
- Attribution  
- Reports  

### Dataview Dashboards
Enable automatic:
- Index pages  
- Tables  
- Lists of new entities  
- Technique/sub-technique grouping  
- IOC lifespan tracking  

---

## 🔢 MITRE ATT&CK Capsules

The vault includes:

- All 14 MITRE ATT&CK tactics (TA0001–TA0011, TA0040-TA0049)  
- Technique capsules for all techniques and sub-techniques you add  

Each technique capsule includes:
- YAML metadata  
- Summary and description  
- Detection guidance  
- Linked threat actors  
- Linked malware  
- Linked campaigns  
- Dataview blocks  

Example Dataview block:

```
TABLE ID, Name, Tactic, Status
FROM "07_TTP Library (MITRE ATT&CK)"
WHERE contains(Tactic, "TA0006")
SORT ID ASC
```

---

## 👤 Threat Actor Capsules

Threat actor profiles include:
- Summary  
- Target sectors and industries  
- Known TTPs  
- Infrastructure  
- IOCs  
- Malware families  
- Regional or geopolitical context  
- Intelligence gaps  
- Confidence assessments  

These profiles are designed to integrate seamlessly with techniques, campaigns, and IOCs.

---

## 🦠 Malware Notes

Each malware note includes:
- Family overview  
- Behavior and capabilities  
- ATT&CK mappings  
- Indicators and hashes  
- Associated threat actors  
- Associated campaigns  
- Detection content (YARA/SIGMA/KQL)  
- External references and sandbox analysis  

---

## 🎯 Campaign Tracking

Campaign notes track:
- Actor(s) involved  
- Target sectors/regions  
- Timeline  
- Infrastructure changes  
- Techniques used  
- Malware deployed  
- IOCs observed  
- Impact and industry-specific concerns  
- Defensive recommendations  

Campaign notes function as the central hub of multi-entity relationships.

---

## 🎣 IOC Lifecycle Tracking

Each IOC file includes:
- Type (IP, domain, hash, etc.)  
- Value  
- Source  
- First/Last seen  
- Confidence rating  
- Expiration  
- Relationships to techniques, malware, campaigns, actors  

Using Dataview, you can automatically generate:
- IOC dashboards  
- Recently added indicators  
- Low/high confidence indicators  
- Expired or soon-to-expire indicators  

---

## 📅 Analyst Workflow Templates

### Daily Intelligence Journal
Used for recording:
- Key observations  
- Hypotheses  
- Leads  
- Behavioral anomalies  
- New threats or shifts  

### Weekly CTI Roll-Up
Used for:
- Summarizing overall trends  
- Campaign updates  
- Threat actor movements  
- New malware discoveries  
- Strategic insights  
- Next week’s priorities  

---

## 🧠 How to Use This Vault

1. Use templates to create standardized notes.  
2. Link notes aggressively for strong relationship mapping.  
3. Maintain daily and weekly logs to build analytic continuity.  
4. Use Dataview dashboards to surface insights automatically.  
5. Over time, grow this into a **long-term, living intelligence repository**.  

---

## 🔌 Recommended Plugins

- Dataview  
- Templater
- Tasks
- Calendar  
- Iconize
- Outliner
- File Explorer Note Count
- Periodic Notes  
- Code Styler
- Paste Image Rename  
- Tag Wrangler
- Pixel Banner
- Chronos Timeline  

---

## 🛣️ Roadmap

- Full MITRE Technique coverage  
- Add SIGMA detection packs  
- Add YARA rule sets  
- Add more KQL hunting queries  
- Example campaign bundles  
- Add Dataview-powered dashboards  
- AI-assisted note generation scripts  

---

## 🤝 Contributing

Contributions are welcome!  
Please submit pull requests for:

- New templates  
- Expanded MITRE coverage  
- Additional threat actor capsules  
- Detection content  
- Vault organization or documentation improvements  

---

## 📄 License

GNU Public License 3.

