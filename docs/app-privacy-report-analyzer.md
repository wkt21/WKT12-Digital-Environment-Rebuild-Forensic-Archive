# App Privacy Report Analyzer — Live Data & Interpretation

This document explains how the App Privacy Report Analyzer is used to monitor,
interpret, and validate the behavior of the rebuilt Apple-only environment.

It includes:
- daily sensor/domain usage
- collapse of Google-linked tracking
- stabilization of Apple frameworks
- integration with Shortcuts for live analytics
- interpretation of normal vs. abnormal behavior

---

## 1. Purpose

The App Privacy Report Analyzer provides continuous visibility into:
- app-initiated network contacts
- sensor usage
- domain frequency
- permission changes
- abnormal spikes or collapses

It is the primary telemetry source for confirming that:
- Google Ads, Maps, Photos, and Location traffic dropped to 0%
- Apple frameworks replaced all Google-linked behavior
- no poisoned SDKs or exploit chains remain active

---

## 2. Key Observations After Rebuild

### 2.1 Collapse of Google Tracking

After migrating all accounts from Gmail → Apple:
- **Google Ads: 0%**
- **Google Maps: 0%**
- **Google Photos: collapsed**
- **Google Location: collapsed**

This indicates:
- no ad-based payload delivery
- no malicious SDK calls
- no background tracking
- no exploit-chain triggers

### 2.2 Stabilization of Apple Frameworks

Normal increases observed:
- Safari Photos ↑ 1052%
- Apple Photos ↑
- Apple Location ↑
- Contacts usage by Photos (face recognition)

These are expected behaviors in a clean Apple environment.

---

## 3. Daily Report Structure

Each daily report includes:
- Sensors per day
- Domains per day
- App-initiated domain groups
- Permission changes
- Newly observed domains

These are archived in:
`docs/app-privacy-report-analyzer/`

---

## 4. Integration With Shortcuts

Shortcuts automate:
- extraction of App Privacy Report
- normalization of events
- tagging of domains
- uploading into the Analyzer workflow

See: `docs/shortcuts-live-analytics.md`

---

## 5. Interpretation Rules

### Normal Behavior
- Apple Photos accessing contacts
- Safari requesting location
- Tailscale contacting DERP nodes
- iCloud syncing metadata

### Abnormal Behavior
- Google Ads traffic
- Google Maps location calls
- offshore ASNs (Ghana, Belgium, Spain, Japan)
- repeated unknown domains
- background installs

---

## 6. Conclusion

The App Privacy Report Analyzer confirms:
- the environment is clean
- the rebuild succeeded
- no reinfection vectors remain
