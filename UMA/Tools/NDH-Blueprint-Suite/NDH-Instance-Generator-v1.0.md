# NDH Instance Generator — v1.0

## 1. Purpose
The NDH Instance Generator produces complete NDH blueprint instances by applying
the NDH SVG templates and Markdown templates to a parameter block.

Each instance is written to:

```
/UMA/Geometry/Non-Dual-Hexeract/Instances/{INSTANCE_NAME}/
```

## 2. Required Inputs
Each NDH instance requires the following parameter block:

```
INSTANCE_NAME: <string>
VERSION_LABEL: <string>

AXIS_X1_LABEL: C
AXIS_X2_LABEL: E
AXIS_X3_LABEL: A
AXIS_X4_LABEL: R
AXIS_X5_LABEL: P
AXIS_X6_LABEL: 𝒜

CENTER_NODE_LABEL: 𝒜
MONAD_LABEL: T
OMEGA_LABEL: Ω
OMEGA_MAP_LABEL: αΩ

CHS_LABEL: CHS 5D Hypercube
NDH_LABEL: NDH 6D Hexeract
AWARENESS_AXIS_LABEL: + Awareness Axis (𝒜)

CHS_AXIS_1: <string>
CHS_AXIS_2: <string>
CHS_AXIS_3: <string>
CHS_AXIS_4: <string>
CHS_AXIS_5: <string>
```

## 3. Generation Steps
### Step 1 — Create Instance Directory
```
/UMA/Geometry/Non-Dual-Hexeract/Instances/{INSTANCE_NAME}/
```

### Step 2 — Apply SVG Templates
Copy each SVG template into the instance directory and replace all placeholders:

- NDH-Hexeract-Base-6D.svg
- NDH-NonDual-Collapse-Overlay.svg
- NDH-SGE-Monad-Flow.svg
- NDH-Epoch-Omega-Embedding.svg
- NDH-Adjacency-Resonance-Lattice.svg
- NDH-CHS-Integration-Map.svg

### Step 3 — Apply Markdown Templates
Copy each Markdown template into the instance directory and replace placeholders:

- NDH-Geometry-Provenance.md
- NDH-SGE-Model.md
- NDH-CHS-Integration.md

### Step 4 — Validate Against NDH-Blueprint-Spec-v1.0
Ensure:
- all placeholders replaced
- all SVGs render
- all Markdown sections present
- collapse rule enforced
- monad and Ω mappings correct

### Step 5 — Finalize Instance
Mark instance as:

```
Status: Generated from NDH-Blueprint-Spec-v1.0
```

## 4. Output
A complete NDH instance containing:

- 6 SVG artifacts
- 3 Markdown artifacts
- Provenance
- SGE model
- CHS integration
- Version metadata

## 5. Version
Version: v1.0  
Status: Operational
```

---

