# HF_Leaderboard_Lab_Results

**Project:** `L_NETTACKER`  
**Tier:** `TIER_6_SECURITY_EVAL`  
**Slug:** `OWASP/Nettacker`  
**Commit:** `cee419f8f815`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **44.43 ms** |
| Min latency | 38.6 ms |
| Max latency | 49.53 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **40** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5859 |
| Classification latency | 131.58 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_NETTACKER (OWASP/Nettacker) — 867 files, 14317 source lines, licence Apache-2.0, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'net', '##ta', '##cker', '(', 'ow', '##as', '##p', '/', 'net', '##ta', '##cker', ')', '—', '86', '##7', 'files', ',']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_