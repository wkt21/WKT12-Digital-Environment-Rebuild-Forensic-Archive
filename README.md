# WKT12-Digital-Environment-Rebuild-Forensic-Archive
A complete DFIR‑grade repository documenting the rebuild of a compromised digital ecosystem, authored by Frank C. Francis.

# WKT12 Digital Environment Rebuild & Forensic Archive

> A DFIR-grade, real-world reconstruction of a compromised digital ecosystem and its clean rebuild.  
> Authored by **Frank C. Francis** — Founder of WKT12.tech

![WKT12 CEF Dashboard](docs/assets/wkt12-cef-dashboard.png)

---

## Overview

This repository documents the full lifecycle of:
- a **multi-year ecosystem compromise** (APK poisoning, CVEs, malicious SDKs, Google-linked persistence, offshore ASNs), and  
- a **clean, Apple-based rebuild** with hardened identity, network, and device baselines.

It combines:
- **forensic evidence**
- **environment rebuild methodology**
- **live app analytics** (App Privacy Report Analyzer, Shortcuts, Tailscale)
- **threat actor mapping**
- **future safeguards**

---

## Author Profile

**Name:** Frank C. Francis  
**Brand:** WKT12.tech  
**Location:** Steubenville, Ohio, USA  

**Role:**  
- Founder, WKT12.tech  
- Cybersecurity & network support practitioner  
- Author of multiple cybersecurity and self-development books  

**Background:**  
- Cisco Networking Academy — Networking, Security, Hardware, Cybersecurity Analyst pathway  
- Pittsburgh Technical College — Technical training  

**Core Skills:**  
- **Network security & support** (Cisco-trained)  
- **OSINT workflow design**  
- **Web development & API integration**  
- **Docker Swarm & distributed microservice orchestration**  
- **Cybersecurity technical writing**  
- **Cinematic visual direction (black/gold/sunset aesthetic)**  

**Recent Work:**  
- Built **WKT12 Intel Center** (malware feed, exploit feed, Shodan search, DNS tools, killfeed)  
- Authored **WKT12 SOC-OSINT** and **Kali Tool Guide**  
- Developed **distributed OSINT pipeline** study modules  
- Created **App Privacy Report Analyzer workflows** and **Shortcuts** for live analytics  
- Performed **multi-device forensic analysis** and **full environment rebuild**  
- Stabilized environment using **Tailscale** and Apple-only identity

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

File: `docs/app-privacy-report-analyzer.md`

Includes:
- daily **sensor/domain usage**  
- **Google Ads / Maps / Photos collapse** after identity migration  
- **Safari / Apple Photos / Apple location** stabilization  
- interpretation of **tracking vs. normal OS behavior**

### Shortcuts — Live Analytics Upload

File: `docs/shortcuts-live-analytics.md`

Documents:
- custom **Shortcuts** that:
  - pull **App Privacy Report** data  
  - normalize and tag events  
  - upload into your analyzer workflow  
- how these Shortcuts feed **live telemetry** into the repo

### Tailscale Baseline

File: `docs/tailscale-baseline.md`

Covers:
- **io.tailscale.ipn.ios** behavior  
- DERP nodes (IPv4/IPv6) and why they’re **normal**  
- confirmation of:
  - no offshore finance endpoints  
  - no poisoned SDK calls  
  - no exploit-chain behavior  
- how Tailscale fits into the **clean network baseline**

---

## Environment Rebuild (How-To)

Directory: `environment-rebuild/`

- `identity-reset.md`  
  - New Apple ID  
  - New email  
  - 2FA  
  - Full migration of accounts from **Gmail → Apple**  
  - Removal of all Google accounts and tokens  

- `network-reset.md`  
  - New router  
  - New SSID & password  
  - Remote management disabled  
  - Clean DNS (ISP / Cloudflare)  
  - Tailscale deployment  

- `device-reset.md`  
  - Factory reset  
  - New Apple ID  
  - No restored backups  
  - Minimal app set  
  - Permission lockdown  

- `safe-data-migration.md`  
  - Only photos, videos, documents, screenshots, logs  
  - No APKs, app data, config files, or executables  

---

## Old Environment Forensics

Directory: `forensics/`

- `apk-analysis.md` — manifests, permissions, trackers, SDK bundles, WebKit components, CVEs  
- `network-evidence.md` — Ghana, Belgium, Spain, Japan routing; iFX / NEXTART; offshore ASNs  
- `device-logs.md` — system logs, crash logs, analytics, background installs, OTA-style behavior  
- `router-evidence.md` — DNS hijack, routing anomalies, repeated malicious endpoints  

---

## Threat Actor Mapping

Directory: `threat-map/`

- `architecture.md` — poisoned APKs, CVEs, WebKit exploit chains, malicious SDK bundles  
- `reinfection-chain.md` — Google identity, Play Services, Ads SDK, Photos/Maps/Location, cloud sync  
- `iocs.md` — domains, IPs, ASNs, certificates, app signatures  

---

## Recovery & Safeguards

- `recovery/recovery-notes.md`  
  - What collapsed: Google Ads/Maps/Photos/Location, poisoned SDK ecosystem  
  - What stabilized: Safari, Apple Photos, Apple location, Tailscale, App Privacy Report Analyzer  

- `safeguards/future-safeguards.md`  
  - Avoid trading/offshore broker/signal apps  
  - Avoid APK sideloading  
  - Avoid Google identity reuse  
  - Maintain Apple-only baseline  
  - Keep router secure  
  - Monitor network behavior regularly  

---

## Hero Image Concept (`docs/assets/wkt12-cef-dashboard.png`)

Design this image to match your aesthetic and the repo’s purpose:

- **Style:** cinematic, highly realistic  
- **Palette:** black, gold, sunset tones  
- **Content:**  
  - a **dashboard-style UI** showing:
    - “Google Ads: 0%”  
    - “Google Maps: 0%”  
    - “Safari Photos: ↑”  
    - “Apple Location: Stable”  
    - “Tailscale: Secure Mesh Active”  
  - subtle **network graph** with clean Apple-only nodes  
  - WKT12 branding in gold in a corner  

This becomes the visual anchor for the repo and signals “live data, real analysis, clean rebuild.”

---
