# Cybersecurity Resources & Tools Checklist

A curated collection of cybersecurity resources, Blue Team tools, threat intelligence feeds, and analysis utilities used for SOC operations, malware analysis, and DFIR investigations.

---

## Navigation & Index

- [Resources](#-resources)
  - [MITRE Frameworks & Research](#mitre-frameworks--research)
  - [SIEM & Detection Platforms](#siem--detection-platforms)
- [Blue Team Tools](#️-blue-team-tools)
  - [Threat Intelligence & IP Lookup](#threat-intelligence--ip-lookup)
  - [Email Header & Security Analysis](#email-header--security-analysis)
  - [Sandbox & Malware Analysis](#sandbox--malware-analysis)
- [DFIR & Data Utilities](#-dfir--data-utilities)
- [Quick Investigation Workflow](#-quick-investigation-workflow)

---

## Resources

### MITRE Frameworks & Research
* [MITRE D3FEND – Credential Rotation](https://d3fend.mitre.org/technique/d3f:CredentialRotation/) — Countermeasure knowledge graph for defensive tactics.
* [MITRE CTID](https://ctid.mitre.org/) — Center for Threat-Informed Defense research and tools.

### SIEM & Detection Platforms
* [Wazuh](https://wazuh.com/) — Open-source SIEM and XDR security monitoring platform.
* [Splunk Sign-Up](https://www.splunk.com/en_us/form/sign-up.html) — Enterprise SIEM platform (Free trial & Splunk Free 500MB/day available).

---

## Blue Team Tools

### Threat Intelligence & IP Lookup
| Tool | Description |
| :--- | :--- |
| [AbuseIPDB](https://www.abuseipdb.com/) | IP address abuse reporting and reputation database. |
| [Cisco Talos Intelligence](https://talosintelligence.com/reputation_center/) | Comprehensive threat intelligence and IP/domain reputation center. |
| [IPinfo](https://ipinfo.io/) | IP geolocation, ASN, and network details lookup. |

### Email Header & Security Analysis
| Tool | Description |
| :--- | :--- |
| [Google Message Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/analyzeheader) | Analyze email headers for hop delays and routing issues. |
| [Azure Message Header Analyzer (MHA)](https://mha.azurewebsites.net/) | Web-based RFC 822 email header parser. |
| [DMARCian – DKIM Selectors](https://dmarcian.com/dkim-selectors/) | Guide and lookup tools for DKIM selector records. |
| [DMARCian – DMARC Videos](https://dmarcian.com/videos-on-all-things-dmarc/) | Video tutorials covering DMARC, SPF, and DKIM concepts. |
| [Microsoft Docs – S/MIME in Exchange](https://learn.microsoft.com/en-us/exchange/security-and-compliance/smime-exo/smime-exo) | Documentation for S/MIME message signing and encryption. |

### Sandbox & Malware Analysis
| Tool | Description |
| :--- | :--- |
| [ANY.RUN](https://app.any.run/) | Interactive cloud sandbox for real-time malware analysis. |
| [VirusTotal](https://www.virustotal.com/gui/home/upload) | Multi-engine file, hash, and URL scanner. |
| [Hybrid Analysis](https://hybrid-analysis.com/) | Free automated malware analysis service powered by Falcon Sandbox. |
| [Joe Sandbox Windows](https://www.joesandbox.com/#windows) | Deep automated malware analysis on Windows environments. |
| [URLScan.io](https://urlscan.io/) | Web site scanner for analyzing HTTP requests, redirects, and DOM. |

---

## DFIR & Data Utilities

* [CyberChef](https://gchq.github.io/CyberChef/) — GCHQ's web app for encoding, decoding, parsing, and data manipulation.
* [WhereGoes](https://wheregoes.com/) — Trace the entire redirect path of any shortened or hidden URL.
* [ConvertCSV URL Extractor](https://www.convertcsv.com/url-extractor.htm) — Extract URLs from unstructured text files or data lists.

---

## Quick Investigation Workflow

```text
[ Suspicious Indicator / Email Received ]
                  │
                  ├──► 1. Parse Email Headers ► (Google Header Analyzer / Azure MHA)
                  │
                  ├──► 2. Check IP / Domain Reputation ► (AbuseIPDB / Talos / IPinfo)
                  │
                  ├──► 3. Inspect URLs & Links ► (WhereGoes / URLScan.io)
                  │
                  └──► 4. Analyze File / Hash ► (VirusTotal / ANY.RUN / Hybrid Analysis)

```

---
