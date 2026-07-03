# UMM Hook Safety CI Integration Spec v1.0

**Module:** CI‑UMM‑HOOKSAFE‑01  
**Domain:** Governance → Stability → CI Enforcement  
**Version:** 1.0  
**Owner:** Borealis S. Hedling  
**Linked Protocols:** PRO‑UMM‑HOOKSAFE‑01, PRO‑UMM‑DVM‑01  
**Linked Pins:** PIN‑UMM‑HOOKSAFE‑01, PIN‑UMM‑DVM‑01  
**Linked Test Suites:** TEST‑UMM‑HOOKSAFE‑01, TEST‑UMM‑DVM‑01  

---

## 1. CI trigger conditions

Hook Safety CI must run on:

- **Governance‑layer changes:**
  - changes under `docs/UMM/Protocols/`  
  - changes under `docs/UMM/Pins/`  
- **Subsystem hook changes:**
  - any file touching `hooks/` or `HookConfig/`  
- **Safety/governance config changes:**
  - Safeguards, Safety Net, SIAP config files  

No merge to `main` or `stable` is allowed if Hook Safety CI fails.

---

## 2. CI pipeline stages





---

## 3. Branch policy

- **Protected branches:** `main`, `stable`, `release/*`  
- **Required checks:**
  - `CI-UMM-HOOKSAFE-01` (Hook Safety)  
  - `CI-UMM-DVM-01` (Drift Vector Mitigation)  

No direct pushes; only PRs with passing checks may merge.

---

## 4. Failure handling

- **On failure:**
  - CI annotates the PR with:
    - failing test category (Hook Safety / Drift Vector)  
    - specific scenario (e.g., “HRB isolation gate inactive on hook X”)  
  - Developer must:
    - update protocol or pin  
    - re‑run tests  
    - only merge once both suites pass  

---

## 5. Roots ledger entry

```text
ROOTS-ENTRY-CI-HOOKSAFE-01
Type: CI Spec
Module: CI-UMM-HOOKSAFE-01
Artifact: Hook Safety CI Integration Spec v1.0
Status: Active
Hash: 2e:aa:31:bd:62:fa:11
Bound: UMA, UMM, Safeguards, Final Safety Net, SIAP, HRB, CHS-OL, Play Engine
```

---

