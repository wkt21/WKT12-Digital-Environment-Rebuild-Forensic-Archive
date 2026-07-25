# Shortcuts — Live Analytics Upload System

This document explains the custom Shortcuts workflow used to extract, normalize,
and upload live analytics from the App Privacy Report into the Analyzer system.

---

## 1. Purpose

Shortcuts automate:
- extraction of App Privacy Report
- normalization of sensor/domain events
- tagging of app-initiated contacts
- uploading into the Analyzer workflow

This creates a **live telemetry pipeline**.

---

## 2. Workflow Overview

### Step 1 — Extract Report
Shortcut pulls:
- sensors
- domains
- app-initiated contacts
- permission changes

### Step 2 — Normalize Data
Shortcut:
- removes duplicates
- tags domains
- categorizes events
- timestamps entries

### Step 3 — Upload to Analyzer
Shortcut sends normalized data to:
`docs/app-privacy-report-analyzer/`

### Step 4 — Archive Daily Snapshot
Daily snapshots stored in:
`docs/app-privacy-report-analyzer/daily/`

---

## 3. Shortcut Components

### 3.1 Data Extraction Block
- Reads App Privacy Report JSON
- Filters by app
- Extracts domain groups

### 3.2 Normalization Block
- Converts raw entries → structured objects
- Tags:
  - Apple frameworks
  - Tailscale nodes
  - abnormal domains
  - Google-linked traffic

### 3.3 Upload Block
- Saves to local repo folder
- Optionally syncs to iCloud Drive

---

## 4. Live Telemetry Benefits

Shortcuts provide:
- real-time visibility
- daily baselines
- anomaly detection
- reinfection prevention
- forensic-grade logging

---

## 5. Integration With Other Systems

Shortcuts feed:
- App Privacy Report Analyzer
- Tailscale baseline validation
- Threat actor mapping
- Recovery notes

---

## 6. Conclusion

Shortcuts create a reliable, automated telemetry pipeline that ensures the
rebuilt environment remains clean and observable.
