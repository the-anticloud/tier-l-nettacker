# Developer Cookbook — L_NETTACKER
**Stack:** Python 3.11, OWASP NetTacker, PAX 27B, AIOSS_FORMAT
**Domain:** NetTacker: authorized network reconnaissance for Anticloud infrastructure

## Authorized network scan
```python
from l_nettacker import NetTackerAssessor

assessor = NetTackerAssessor(
    pax_model="./pax-27b-q4.gguf",
    authorized_scope=["192.168.1.0/24"],
    aioss_chain="./nettacker.aioss"
)

assessor.verify_scope_authorization()  # checks AIOSS auth entry

result = assessor.scan(
    modules=["port_scan", "service_detection", "ssl_audit"]
)
print(f"Hosts found: {len(result.hosts)}")
print(f"Critical findings: {result.critical_count}")
print(f"PAX remediation plan: {result.pax_plan}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
