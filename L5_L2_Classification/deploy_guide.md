# Deploy Guide — L_NETTACKER
**Tier:** TIER_6_SECURITY_EVAL | **Stack:** Python 3.11, OWASP NetTacker, PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, owasp-nettacker 0.x, PAX 27B. AUTHORIZED SCOPE REQUIRED.

## Environment
CPU-only for network scanning. GPU for PAX analysis. AUTHORIZED TEST ENVIRONMENT ONLY.

## AIOSS Integration
```bash
aioss init --module L_NETTACKER --output ./l_nettacker.aioss
aioss append --chain ./l_nettacker.aioss --payload ./output.bin --module L_NETTACKER
aioss verify --chain ./l_nettacker.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_NETTACKER",
    aioss_chain="./L_NETTACKER.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_NETTACKER.aioss --verbose
python -m L_NETTACKER.tests.smoke
```
