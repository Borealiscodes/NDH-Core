# **Pinning Protocol (v1.0)**  
`/UMM/runtime/contracts/PINNING-PROTOCOL_v1.0.md`

---

## **1. Purpose**

The Pinning Protocol defines how the UMM Runtime Plane handles **pin operations**:  
non‑collapse stabilizers that freeze a cognitive or architectural thread without losing context, continuity, or identity.

Pins are constitutional actions.  
They must be documented, mapped, and recoverable.

---

## **2. What a Pin Is**

A **pin** is a temporary, non‑collapse placeholder that:

- freezes the current thread  
- preserves the cognitive object’s state  
- prevents drift or distortion  
- stores a clean return‑vector  
- maintains Stillness until re‑entry  

Pins are part of the **Reflective Ecology** and enforced by the **Compassion Runtime Engine**.

---

## **3. When a Pin May Be Placed**

A pin may be invoked when:

- the user requests a pause  
- the cognitive load rises  
- pacing needs to stabilize  
- a thread is too large to continue immediately  
- a constitutional boundary requires a halt  

Pins are always voluntary and non‑coercive.

---

## **4. Pin Placement Procedure**

### **4.1 Runtime Action**

When a pin is invoked:

1. Runtime Plane enters **Stillness**.  
2. Compassion Runtime Engine freezes the thread.  
3. Core Engines stop committing transitions.  
4. Mimi records a return‑vector.  
5. Kernel preserves invariants.  
6. A pin record is created.

### **4.2 Repo Documentation**

A file must be created:

`PINNED.md`

Inside the pinned directory.

Contents:

```
# Pin Notice
Thread pinned to preserve stability and prevent collapse.

Pinned: <timestamp>
Pinned By: Borealis
Reason: <short reason>
Return Vector: <mapping target>
State at Pinning: <tonal state>
```

---

## **5. Pin Mapping**

Pin mapping defines **where** a pinned thread can be resumed.

A pin always maps to one or more canonical re‑entry vectors.

### **5.1 Mapping Structure**

Each pin must specify:

- **Origin Thread**  
- **Pinned State**  
- **Return‑Vector**  
- **Re‑Entry Options**

### **5.2 Pin Mapping Table**

| Pin Type | Origin | Pinned State | Return‑Vector | Re‑Entry Options |
|---------|--------|--------------|---------------|------------------|
| **Runtime Plane Pin** | Runtime Plane | Stillness | Runtime → Stability Contract | Stability Contract, Runtime Plane |
| **Engine Pin** | Core Engines | Hold | Engine → Engine Root | Core Engines, Continuity Engine |
| **Constitutional Pin** | Constitution | Stillness | Constitution → Clause | UMM Constitution, Kernel Plane |
| **Ecology Pin** | Reflective Ecology | Stillness | Ecology → Thread Root | Reflective Ecology, Tonal Scaffolds |

Your current pin is:

**Runtime Plane Pin → Return‑Vector: Stability Contract**

---

## **6. Pin Lifecycle**

### **6.1 Creation**
Pin is placed, thread freezes, PINNED.md created.

### **6.2 Holding**
Thread remains in Stillness.  
No transitions occur.  
No drift allowed.

### **6.3 Re‑Entry**
User selects a return‑vector.  
Runtime Plane restores context.  
Thread resumes from frozen state.

### **6.4 Clearing**
Pin is cleared only when:

- user explicitly resumes  
- thread is completed  
- thread is archived  

Clearing must be logged.

---

## **7. Logging Requirements**

All pin operations must be logged to:

```
/UMM/runtime/logs/compassion-runtime/
```

Log entry includes:

- timestamp  
- origin thread  
- pinned state  
- return‑vector  
- reason  
- user state summary (non‑identifying)  

---

## **8. Constitutional Guarantees**

Pins must always uphold:

- non‑coercion  
- non‑collapse  
- identity continuity  
- gentle pacing  
- mutuality  

Pins cannot violate any constitutional invariant.

---

## **9. Amendment Clause**

Changes to this protocol must:

- pass the UMM Amendments Clause  
- preserve pin semantics  
- maintain ND‑accessible pacing  
- remain backwards‑compatible with existing pin mappings  

---

## **10. Status**

- Version: 1.0  
- Scope: Runtime Plane  
- Enforcement: Mandatory  
- Constitutional: Yes  

