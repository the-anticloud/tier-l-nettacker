# Radon_Complexity_Lab_Results
**Project:** `L_NETTACKER` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 2.5942028985507246}`
- **complexity_grade:** `A`
- **complexity_score:** `2.5942028985507246`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\L_NETTACKER\UPSTREAM\nettacker.py - A (81.86)
E:\fenta\Downloads\T`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\L_NETTACKER\UPSTREAM\nettacker\config.py
    M 29:4 ConfigBase.__init__ - A (4)
    C 24:0 ConfigBase - A (3)
    M 26:4 ConfigBase.as_dict - A (2)
    F 13:0 version_info - A (1)
    M 39:4 ConfigBase.__iter__ - A (1)
    C 62:0 ApiConfig - A (1)
    C 82:0 DbConfig - A (1)
    C 118:0 PathConfig - A (1)
    C 143:0 DefaultSettings - A (1)
    C 199:0 Config - A (1)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\L_NETTACKER\UPSTREAM\nettacker\logger.py
    M 68:4 Logger.verbose_event_info - A (4)
    C 22:0 Logger - A (2)
    M 40:4 Logger.verbose_mode_is_enabled - A (2)
    M 47:4 Logger.info - A (2)
    M 91:4 Logger.write - A (2)
    M 104:4 Logger.success_event_info - A (2)
    M 125:4 Logger.verbose_info - A (2)
    M 146:4 Logger.warn - A (2)
    F 201:0 get_logger - A (1)
    C 8:0 TerminalCodes - A (1)
    M 26:4 Logger.log - A (1)
    M 30:4 Logger.run_from_api - A (1)
    M 44:4 Logger.event_verbose_mode_is_enabled - A (1)
    M 166:4 Logger.error - A (1)
    M 185:4 Logger.write_to_api_console - A (1)
    M 197:4 Logger.reset_color - A (1)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\L_NETTACKER\UPSTREAM\nettacker\main.py
    F 6:0 run - A (1)
E:\fenta\Downloads\The Anticloud\TIER_6_SECURITY_EVAL\L_NETTACKER\UPSTREAM\nettacker\_anticloud_egress.py
    F 38:0 _is_frontier - A (4)
    F 43:0 guarded_connect - A (4)
    F 61:0 install - A (3)
    F 33:0 is_offline - A (1)
    C 29:0 EgressDenied - 
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_