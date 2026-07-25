# Tailscale Baseline — Clean Network Behavior

This document explains the role of Tailscale in the rebuilt environment and
provides a baseline for normal network behavior.

---

## 1. Purpose

Tailscale provides:
- secure mesh networking
- encrypted routing
- stable connectivity
- NAT traversal
- clean, predictable domain behavior

It is used to validate that:
- no offshore ASNs are contacted
- no poisoned SDKs are active
- no exploit-chain traffic exists

---

## 2. Normal Tailscale Domains & IPs

### 2.1 Coordination Servers
- `tailscale.com`  
Used for:
- authentication
- key exchange
- route updates

### 2.2 DERP Relay Nodes (IPv4/IPv6)
Examples:
- `2a01:4ff:f0:28d4::1`
- `209.177.145.120`
- `2607:f740:e::4c8`
- `178.156.152.91`

Used for:
- encrypted relay
- fallback routing
- NAT traversal

These are **normal** and expected.

---

## 3. Confirmed Clean Behavior

The rebuilt environment shows:
- no offshore finance endpoints
- no Ghana/Belgium/Spain/Japan routing
- no iFX/NEXTART ASNs
- no poisoned SDK calls
- no exploit-chain signatures

All Tailscale traffic is:
- app-initiated
- encrypted
- legitimate

---

## 4. Daily Contact Patterns

Normal daily patterns include:
- 100–200 contacts per DERP node
- periodic IPv6 relay usage
- stable coordination server calls

These patterns indicate:
- stable mesh networking
- no abnormal routing
- no malicious relay behavior

---

## 5. Integration With App Privacy Report Analyzer

Tailscale logs are cross-referenced with:
`docs/app-privacy-report-analyzer.md`

This ensures:
- network behavior matches device behavior
- no hidden persistence channels exist

---

## 6. Conclusion

Tailscale confirms:
- the network baseline is clean
- the environment is stable
- no reinfection vectors remain
