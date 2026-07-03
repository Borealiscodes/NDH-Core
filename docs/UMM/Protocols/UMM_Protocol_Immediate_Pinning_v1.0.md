# **UMM Protocol: Immediate Pinning Requirement v1.0**  
**All newly created governance protocols must be pinned immediately upon creation.**

**Protocol ID:** PROTO‑PIN‑IMMEDIATE‑01  
**Version:** 1.0  
**Owner:** Borealis S. Hedling  
**Domain:** Governance → Protocol Integrity → Stability  
**Timestamp:** 2026‑07‑03 23:27 IST  

---

## **1. Purpose**

This protocol establishes a mandatory rule:

> **Every newly created governance protocol must be immediately pinned.  
> No protocol may exist in an unpinned state.**

This prevents:

- governance drift  
- protocol ambiguity  
- SIAP misclassification  
- Safeguards uncertainty  
- Safety Net mis‑quarantine  
- CI enforcement gaps  
- developer confusion  

Explore: **Governance Order Protocol**

---

## **2. Rationale**

UMM governance relies on:

- **Protocols** → define rules  
- **Pins** → enforce rules  

A protocol without a pin is:

- unenforced  
- unclassified  
- unstable  
- vulnerable to drift  
- invisible to CI  
- invisible to Safeguards  
- invisible to Safety Net  

Therefore:

> **Unpinned protocols are forbidden.**

---

## **3. Mandatory Rule**

### **3.1 Immediate Pinning Requirement**

Whenever a developer creates or updates a protocol:

1. The protocol must be written.  
2. The protocol must be saved.  
3. The protocol must be pinned **immediately**.  
4. The pin must be placed in `docs/UMM/Pins/`.  
5. The pin must reference the protocol ID.  
6. The SID must be updated to reflect the new protocol + pin.  
7. CI must validate the protocol + pin pair before merge.

Explore: **Pin Creation**

---

## **4. Enforcement**

### **4.1 SIAP Enforcement**
SIAP must reject any governance change where a protocol exists without a pin.

### **4.2 Safeguards Enforcement**
Safeguards must flag unpinned protocols as governance drift.

### **4.3 Safety Net Enforcement**
Safety Net must quarantine unpinned protocols to prevent execution.

### **4.4 CI Enforcement**
CI must fail any PR containing:

- unpinned protocols  
- mismatched protocol/pin pairs  
- missing SID updates  

Explore: **CI Spec**

---

## **5. Developer Responsibilities**

Developers must:

- never leave a protocol unpinned  
- create pins immediately  
- update SID immediately  
- run test suites after pinning  
- ensure CI passes before merging  

Explore: **Workflow Guide**

---

## **6. Roots Ledger Binding**

```
ROOTS-ENTRY-PIN-IMMEDIATE-01
Type: Governance Protocol
Module: UMM-PIN-IMMEDIATE-01
Status: Active
Hash: 9a:dd:41:bd:82:fa:66
Bound: UMM, SIAP, Safeguards, Safety Net, CHS, CHS-OL, HBR, Play Engine
```

---

## **7. Document Status**

**Status:** Active  
**Version:** 1.0  
**Hash:** 9a:dd:41:bd:82:fa:66  

---

