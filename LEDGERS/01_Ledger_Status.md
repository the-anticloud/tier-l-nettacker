# Ledger Status

**Project:** `L_NETTACKER`  
**Tier:** TIER_6_SECURITY_EVAL  
**Identity:** Upstream `OWASP/Nettacker` @ `cee419f8f815` (Apache-2.0)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `OWASP/Nettacker` |
| Commit | `cee419f8f8152419c9275bcb092707d8b270dc7b` |
| Upstream licence | Apache-2.0 |
| Licence class | permissive |
| Clone size | 10.99 MB |
| Ledger | 0 blocks, chain verified |
| Current TRL | NOT YET MEASURED |
| Post-optimisation TRL | NOT YET MEASURED |
| II budget cap | 1500.0 IIU |
| Verified upstream edits | 1 |

- Blocks: **0**
- Head digest: `None`
- Chain verification: **verified**

## Independent verification

The chain is verifiable without trusting this project's tooling:

```
anticloud ledger verify
anticloud ledger export > ledger.jsonl
```

Each block carries the previous block's digest, so removing or reordering an
entry invalidates every block after it. That property is the reason the
ledger can stand in for a claim of what happened.
