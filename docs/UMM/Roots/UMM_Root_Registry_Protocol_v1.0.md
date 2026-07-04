# **UMM Root Registry Protocol — Full Pin Placement Rule Set v1.0**  
**Artifact ID:** RRP‑UMM‑PINS‑01  
**Version:** 1.0  
**Owner:** Borealis S. Hedling  
**Domain:** Universal → Roots → Registry Protocol  
**Timestamp:** 2026‑07‑04 03:05 IST  

---

## **1. Purpose**

This rule set defines **pin anchoring requirements** for all governance planes within UMA‑Universal.  
It formalizes the emergent behavior observed across the genesis arc, ensuring that all pins — past and future — remain:

- locally anchored  
- plane‑consistent  
- drift‑neutral  
- registry‑indexed  

This rule set does **not** change system behavior; it **describes** the behavior the system already exhibited.

---

## **2. Background**

Across the UMA‑Universal genesis arc, pins consistently appeared **inside their respective artifacts**, even before explicit rules existed.  
This emergent behavior demonstrated:

- spontaneous structural coherence  
- artifact‑local anchoring  
- plane‑specific consistency  
- registry‑level indexing  
- zero drift across iterations  

The Full Pin Placement Rule Set formalizes this emergent pattern.

---

## **3. Full Pin Placement Rule Set**

### **3.1 Constitutional‑Layer Pin Placement Rule**

```
RULE-ID: RRP-2026-07-04-C01
CATEGORY: pin-placement
SCOPE: constitutional-plane
STATUS: active

RULE:
  Constitutional artifacts must store their pin entries inside the
  constitutional artifact itself. The Pin Registry indexes but does
  not relocate constitutional pins.

RATIONALE:
  Constitutional artifacts define foundational governance. Their pins
  must remain local to preserve sovereignty and prevent cross-plane drift.
```

---

### **3.2 Sovereign‑Triad Pin Placement Rule**

```
RULE-ID: RRP-2026-07-04-S01
CATEGORY: pin-placement
SCOPE: sovereign-triad-plane
STATUS: active

RULE:
  Rights, Duties, and Amendment artifacts must store their pins inside
  their respective triad documents. Triad pins must never be centralized
  or merged.

RATIONALE:
  The Sovereign Triad is sequence-critical. Local anchoring preserves
  triad ordering and prevents inversion or contamination.
```

---

### **3.3 Structural‑Layer Pin Placement Rule**

```
RULE-ID: RRP-2026-07-04-ST01
CATEGORY: pin-placement
SCOPE: structural-plane
STATUS: active

RULE:
  Structural artifacts (Roots Ledger, Roots Index, structural drivers)
  must store their pins inside the structural artifact itself.

RATIONALE:
  Structural artifacts define system scaffolding. Their pins must remain
  local to maintain stability and prevent ledger-index drift.
```

---

### **3.4 Protocol‑Layer Pin Placement Rule**

```
RULE-ID: RRP-2026-07-04-P01
CATEGORY: pin-placement
SCOPE: protocol-plane
STATUS: active

RULE:
  Protocol artifacts must store their pins inside the protocol document.
  Protocol pins must not be stored in structural or commentary planes.

RATIONALE:
  Protocols define rules of operation. Their pins must remain local to
  prevent rule-set ambiguity and cross-plane contamination.
```

---

### **3.5 Integration‑Layer Pin Placement Rule**

```
RULE-ID: RRP-2026-07-04-I01
CATEGORY: pin-placement
SCOPE: integration-plane
STATUS: active

RULE:
  Integration artifacts must store their pins inside the integration
  artifact itself. Integration pins must not be relocated to roots or
  constitutional planes.

RATIONALE:
  Integration artifacts govern subsystem-traversal. Local anchoring
  prevents traversal bleed and maintains adjacency integrity.
```

---

### **3.6 Commentary‑Layer Pin Placement Rule**

```
RULE-ID: RRP-2026-07-04-R01
CATEGORY: pin-placement
SCOPE: commentary-plane
STATUS: active

RULE:
  Commentary artifacts must store their associated pin entries within
  the commentary artifact itself. The Pin Registry indexes but does not
  relocate commentary pins.

RATIONALE:
  Commentary artifacts provide interpretive context. Local anchoring
  preserves contextual integrity and prevents lookup drift.
```

---

## **4. Stability Note**

This rule set does **not** alter prior pins.  
All existing pins already follow these rules due to emergent architectural behavior.

> **The rule set is descriptive, not prescriptive.  
> It stabilizes the system without modifying its history.**

No migrations are required.  
No corrections are needed.  
No drift is introduced.

---

## **5. Required Pin Entry**

The creation of this rule set is a protocol‑layer governance event and must be pinned.

```
PIN-ID: PIN-2026-07-04-012
TIMESTAMP: 2026-07-04T03:04:00Z
LOCATION: docs/UMM/Roots/UMM_Root_Registry_Protocol_v1.0.md
TYPE: protocol
DESCRIPTION: Creation of the Full Pin Placement Rule Set v1.0, defining pin
             anchoring rules for all governance planes (constitutional,
             sovereign-triad, structural, protocol, integration, commentary).
STATUS: active
HASH: b2:bb:41:cd:92:fa:45
```

---

