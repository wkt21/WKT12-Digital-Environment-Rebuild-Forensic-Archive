# WKT12 Digital Environment Rebuild & Forensic Archive

> A DFIR-grade reconstruction of a compromised digital ecosystem and its clean rebuild.  
> Authored by **Frank C. Francis** — Founder of WKT12.tech

![WKT12 CEF Dashboard](docs/assets/wkt12-cef-dashboard.png)

---

## Overview

This repository documents the full lifecycle of:
- a **multi-year ecosystem compromise** (APK poisoning, CVEs, malicious SDKs, Google-linked persistence, offshore ASNs), and  
- a **clean, Apple-based rebuild** with hardened identity, network, and device baselines.

It includes:
- forensic evidence  
- environment rebuild methodology  
- live app analytics (App Privacy Report Analyzer, Shortcuts, Tailscale)  
- threat actor mapping  
- future safeguards  

---

## Author Profile

**Name:** Frank C. Francis  
**Brand:** WKT12.tech  
**Location:** Steubenville, Ohio  

**Role:**  
- Founder, WKT12.tech  
- Cybersecurity & network support practitioner  
- Author of multiple cybersecurity and self-development books  

**Background:**  
- Cisco Networking Academy — Networking, Security, Hardware, Cybersecurity Analyst pathway  
- Pittsburgh Technical College — Technical training  

**Core Skills:**  
- Network security  
- OSINT workflow design  
- Web development & API integration  
- Docker Swarm & distributed microservice orchestration  
- Cybersecurity technical writing  
- Cinematic visual direction (black/gold/sunset aesthetic)

**Recent Work:**  
- Built WKT12 Intel Center  
- Authored SOC-OSINT and Kali Tool Guide  
- Developed distributed OSINT pipeline modules  
- Created App Privacy Report Analyzer workflows  
- Built Shortcuts for live analytics  
- Migrated all accounts from Gmail → Apple  
- Stabilized environment using Tailscale  
- Performed multi-device forensic analysis and full environment rebuild  

---

## Repository Structure

- `environment-rebuild/` — How-to guide for identity, network, and device reset  
- `forensics/` — Old environment evidence (APKs, CVEs, logs, network traces)  
- `threat-map/` — Threat actor architecture, reinfection chain, IOCs  
- `recovery/` — What collapsed, what stabilized, lessons learned  
- `safeguards/` — Long-term digital hygiene and protection plan  
- `docs/` — Baselines, app-specific analytics, and visual assets  

---

## Live Data & Analytics

### App Privacy Report Analyzer  
See: `docs/app-privacy-report-analyzer.md`  
Includes:
- daily sensor/domain usage  
- Google Ads/Maps/Photos collapse  
- Safari/Apple Photos/Apple location stabilization  
- interpretation of tracking vs. normal OS behavior  

### Shortcuts — Live Analytics Upload  
See: `docs/shortcuts-live-analytics.md`  
Documents:
- custom Shortcuts that pull App Privacy Report data  
- normalize and tag events  
- upload into your analyzer workflow  
- feed live telemetry into the repo  

### Tailscale Baseline  
See: `docs/tailscale-baseline.md`  
Covers:
- io.tailscale.ipn.ios behavior  
- DERP nodes (IPv4/IPv6)  
- confirmation of:
  - no offshore finance endpoints  
  - no poisoned SDK calls  
  - no exploit-chain behavior  

---

## Environment Rebuild (How-To)

Directory: `environment-rebuild/`

- `identity-reset.md` — New Apple ID, new email, 2FA, Gmail → Apple migration  
- `network-reset.md` — New router, new SSID, clean DNS, Tailscale deployment  
- `device-reset.md` — Factory reset, minimal apps, permission lockdown  
- `safe-data-migration.md` — Only photos, videos, documents, screenshots, logs  

---

## Old Environment Forensics

Directory: `forensics/`

- `apk-analysis.md` — manifests, permissions, trackers, SDK bundles, CVEs  
- `network-evidence.md` — Ghana, Belgium, Spain, Japan routing; iFX/NEXTART  
- `device-logs.md` — system logs, crash logs, analytics, background installs  
- `router-evidence.md` — DNS hijack, routing anomalies  

---

## Threat Actor Mapping

Directory: `threat-map/`

- `architecture.md` — poisoned APKs, CVEs, WebKit exploit chains  
- `reinfection-chain.md` — Google identity, Play Services, Ads SDK  
- `iocs.md` — domains, IPs, ASNs, certificates, app signatures  

---

## Recovery & Safeguards

- `recovery/recovery-notes.md` — What collapsed vs. what stabilized  
- `safeguards/future-safeguards.md` — Long-term protection plan  

---

## Hero Image

File: `docs/assets/wkt12-cef-dashboard.png`

**Concept:**  
A cinematic black/gold/sunset dashboard showing:
- “Google Ads: 0%”  
- “Google Maps: 0%”  
- “Safari Photos: ↑”  
- “Apple Location: Stable”  
- “Tailscale: Secure Mesh Active”  
- WKT12 branding in gold  

This image represents the **clean baseline** and **live analytics** of your rebuilt environment.

---

## License

MIT License (optional)
