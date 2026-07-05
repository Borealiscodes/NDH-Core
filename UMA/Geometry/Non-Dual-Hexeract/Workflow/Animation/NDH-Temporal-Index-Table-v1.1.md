### Temporal Index Table v1.1  
**Placement:**
`/UMA/Geometry/Non-Dual-Hexeract/Workflow/Animation/NDH-Temporal-Index-Table-v1.1.md`

---

### 1. Purpose  
The **Temporal Index Table v1.1** formalizes the timing of the **Temporal Phase Animation v1.1** so Production Order v1.3 can treat workflow phases as **governed, time‑indexed operations** rather than just visuals.

---

### 2. Core Table  

```markdown
# NDH Temporal Index Table v1.1

| Phase    | Start (s) | End (s) | Duration (s) | Primary System Focus                  | Key Layers Involved                                      |
|----------|-----------|---------|--------------|----------------------------------------|----------------------------------------------------------|
| Detect   | 0.0       | 1.0     | 1.0          | Deviation sensing & audit triggering   | Workflow Phases, Audit Layer, Execution Spine, SID Cortex |
| Protect  | 1.0       | 2.0     | 1.0          | Fallback stabilization & loop safety   | Safety Net Layer, Workflow Phases, Execution Spine       |
| Flex     | 2.0       | 3.0     | 1.0          | Constraint flexion & SID tension       | SID Cortex (AFL), Workflow Phases, Dual-Spine Rails      |
| Balance  | 3.0       | 4.0     | 1.0          | Load redistribution & CLB balancing    | SID Cortex (CLB), Workflow Phases, Execution+Validation  |
| Validate | 4.0       | 5.0     | 1.0          | Dual-spine reconciliation (DSR)        | SID Cortex (DSR), Validation Spine, Execution Spine      |
| Evolve   | 5.0       | 6.0     | 1.0          | Dimensional & teleological update      | Hexeract Core, 6D Beams, Meta Plane Boundary, Workflow   |
```

Total loop duration: **6.0 seconds**.

---

### 3. Integration Notes  

- **Production Order v1.3 – Step 4** must respect these exact start/end times for each phase.  
- SID layers (AFL, CLB, DSR) are **expected to react** within their assigned windows.  
- Audit and Safety Net triggers are **bound** to Detect and Protect respectively.  
- Dimensional updates (beams, hexeract, boundary glow) are **bound** to Evolve.

---

