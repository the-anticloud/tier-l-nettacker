# L5 Narrow / L2 General Classification — L_NETTACKER
**Platform:** Anticloud | **Tier:** TIER_6_SECURITY_EVAL | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
L_NETTACKER integrates OWASP NetTacker for authorized network reconnaissance of Anticloud deployments: identifying active hosts, open services, and network configuration issues. Narrow scope: Anticloud network perimeter — authorized scope only.

## L2 General
L2 General: L_NETTACKER's network reconnaissance applies to all Anticloud deployment tiers as part of authorized security testing. Same reconnaissance framework for hospital LANs and defense networks.

## PAX 27B Integration
PAX 27B synthesizes NetTacker scan results into prioritized remediation plans: 'Port 5555 (ZeroMQ broker) is exposed to 0.0.0.0 — should be bound to 127.0.0.1 only.'

## AIOSS Audit Chain
Every network scan (scope hash + discovered hosts hash + service inventory hash + risk findings hash) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
NIST SP 800-115 (security testing). Authorized use only.
