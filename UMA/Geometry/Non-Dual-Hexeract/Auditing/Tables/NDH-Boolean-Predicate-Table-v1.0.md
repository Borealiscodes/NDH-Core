### NDH Boolean Predicate Table v1.0  
**Placement:**  
`/UMA/Geometry/Non-Dual-Hexeract/Auditing/Tables/NDH-Boolean-Predicate-Table-v1.0.md`

---

#### 1. Purpose  
This table enumerates each Boolean predicate that gates the nine states of the Thicketry Algebraic State Machine, including inputs, meaning, and failure semantics.

---

#### 2. Predicate table

```markdown
# NDH Boolean Predicate Table v1.0

| Predicate | Step                          | Inputs                                           | Condition (True)                                                | Failure Semantics                          |
|----------|-------------------------------|--------------------------------------------------|------------------------------------------------------------------|--------------------------------------------|
| G        | Activate Thicketry Geometry   | N₀ (nodes), E₀ (edges)                          | N₀ > 0 ∧ E₀ ≥ 0                                                 | No valid geometry → σE                     |
| D        | Apply Divergence Rules        | B_pre, B_post, B_max                             | B_post ≥ B_pre ∧ B_post ≤ B_max                                 | Over/under-divergence → σE                 |
| C        | Apply Convergence Rules       | M (merged set), S_merge (success flag)          | |M| > 0 ∧ S_merge = true                                         | Convergence stall/failure → σE             |
| B        | Apply Braid Logic             | P (paths), C_cycles, C_max                      | |P| ≥ 2 ∧ C_cycles ≤ C_max                                      | Excess cycles / invalid braid → σE         |
| T        | Apply Tangle Density          | ρ (density), ρ_max                              | ρ ≤ ρ_max                                                       | Tangle overload → σE                       |
| R        | Resolve into Detect           | R_paths, U_paths                                 | |R_paths| > 0 ∧ |U_paths| = 0                                   | Unresolved paths / incomplete mapping → σE |
| S        | Bind to Workflow Spine v1.1   | contract_valid, binding_success                 | contract_valid ∧ binding_success                                | Spine bind error → σE                      |
| A        | Bind to Temporal Animation    | t_expected, t_actual, δ (tolerance)             | |t_actual − t_expected| ≤ δ                                     | Temporal drift / misalignment → σE         |
| P        | Bind to Production Order v1.3 | lineage_valid, binding_success                  | lineage_valid ∧ binding_success                                 | Production bind gap / lineage break → σE   |
```

---

