# NDH Pin Registry — v1.2  
### Dimensional Anchor Registry Including Rendering‑Safety Class (RS)  
### Anchored to: NDH‑Integration‑Spec‑v1.0

---

## ⭐ 0. Purpose

The NDH Pin Registry v1.2 is the **single, authoritative registry** of all dimensional anchors and protocol‑embedded pins (PEPs) in the Non‑Dual‑Hexeract manifold.

It:

- defines pin classes and IDs  
- records dimensional coordinates (H₆)  
- encodes operator compatibility  
- binds protocols and geometry to stable anchors  
- introduces **Rendering‑Safety Class (RS)** for geometry v1.2  

This registry is required for:

- NDH Geometry Suite v1.2  
- Traversal Protocol v1.1  
- Rendering Safety Protocol v1.2  
- Navigation Map v1.1  
- NDH v2.0 Roadmap  
- Auto‑Index Generator Block v1.0  

---

## ⭐ 1. Pin Classes (v1.2)

- **TC:** Traversal‑Compatible Class  
- **C:** Collapse Class  
- **A:** Adjacency Class  
- **R:** Resonance Class  
- **Rᵣ:** Recursion Class  
- **S:** Singularity Class  
- **H₆:** Integration / Hexeract Class  
- **RS:** Rendering‑Safety Class *(new in v1.2)*  

Each pin belongs to one primary class and may be compatible with multiple NDH operators.

---

## ⭐ 2. Registry Format

Each pin entry follows:

```text
Pin-ID: <string>
Pin-Class: <TC|C|A|R|Rᵣ|S|H₆|RS>
Anchor: <governance or protocol artifact>

# Dimensional Coordinates (H₆)
Identity-Axis: <0.00–1.00>
Behavior-Axis: <0.00–1.00>
Continuity-Axis: <0.00–1.00>
Cosmology-Axis: <0.00–1.00>
Narrative-Axis: <0.00–1.00>
Teleology-Axis: <0.00–1.00>

# Operator Compatibility
Compatible-Operators: <subset of 𝒜, C, A, R, Rᵣ, S, H₆>
Collapse-Invariant: <true|false>
Adjacency-Stable: <true|false>
Resonance-Stable: <true|false>
Recursion-Stable: <true|false>
Singularity-Stable: <true|false>
Integration-Safe: <true|false>

# Rendering Context (if applicable)
SVG-Primary: <true|false>
PNG-Fallback: <true|false>
Mobile-Safe: <true|false>
Desktop-Safe: <true|false>
Geometry-Safe-Mode: <true|false>

# Awareness Metadata (optional)
Awareness-Axis: <symbol or descriptor>
Awareness-Persistence: <Stable|Transient|Ephemeral>

# Monitoring Dependencies (optional)
Monitoring-Dependency: <artifact-id>
```

---

## ⭐ 3. Traversal‑Compatible Pins (TC Class)

### 3.1 PEP‑Traversal‑Class v1.0

```text
Pin-ID: NDH-PEP-TC-v1.0
Pin-Class: TC
Anchor: PEP-Traversal-Class-v1.0

# Dimensional Coordinates (H₆)
Identity-Axis: 0.50
Behavior-Axis: 0.50
Continuity-Axis: 0.50
Cosmology-Axis: 0.50
Narrative-Axis: 0.50
Teleology-Axis: 0.50

# Operator Compatibility
Compatible-Operators: 𝒜, C, A, R, Rᵣ, S, H₆
Collapse-Invariant: true
Adjacency-Stable: true
Resonance-Stable: true
Recursion-Stable: true
Singularity-Stable: true
Integration-Safe: true

# Rendering Context
SVG-Primary: true
PNG-Fallback: true
Mobile-Safe: true
Desktop-Safe: true
Geometry-Safe-Mode: true
```

---

## ⭐ 4. Singularity Pins (S Class)

### 4.1 PEP‑Singularity‑Class v1.0

```text
Pin-ID: NDH-PEP-SC-v1.0
Pin-Class: S
Anchor: PEP-Singularity-Class-v1.0

# Dimensional Coordinates (H₆)
Identity-Axis: 0.30
Behavior-Axis: 0.45
Continuity-Axis: 0.70
Cosmology-Axis: 0.85
Narrative-Axis: 0.40
Teleology-Axis: 0.60

# Operator Compatibility
Compatible-Operators: C, R, Rᵣ, S, H₆
Collapse-Invariant: true
Adjacency-Stable: false
Resonance-Stable: true
Recursion-Stable: true
Singularity-Stable: true
Integration-Safe: true

# Rendering Context
SVG-Primary: true
PNG-Fallback: true
Mobile-Safe: true
Desktop-Safe: true
Geometry-Safe-Mode: true
```

---

## ⭐ 5. Integration Pins (H₆ Class)

### 5.1 PEP‑Integration‑Class v1.0

```text
Pin-ID: NDH-PEP-IC-v1.0
Pin-Class: H₆
Anchor: PEP-Integration-Class-v1.0

# Dimensional Coordinates (H₆)
Identity-Axis: 0.55
Behavior-Axis: 0.60
Continuity-Axis: 0.65
Cosmology-Axis: 0.50
Narrative-Axis: 0.70
Teleology-Axis: 0.80

# Operator Compatibility
Compatible-Operators: 𝒜, A, R, H₆
Collapse-Invariant: true
Adjacency-Stable: true
Resonance-Stable: true
Recursion-Stable: true
Singularity-Stable: true
Integration-Safe: true

# Rendering Context
SVG-Primary: true
PNG-Fallback: true
Mobile-Safe: true
Desktop-Safe: true
Geometry-Safe-Mode: true
```

---

## ⭐ 6. Rendering‑Safety Pins (RS Class) — New in v1.2

### 6.1 PEP‑Rendering‑Safety‑Class v1.0

```text
Pin-ID: NDH-PEP-RS-v1.0
Pin-Class: Rendering-Safety (RS)
Anchor: NDH-Geometry-Suite-Rendering-Safety-Protocol-v1.2

# Dimensional Coordinates (H₆)
Identity-Axis: 0.41
Behavior-Axis: 0.57
Continuity-Axis: 0.69
Cosmology-Axis: 0.38
Narrative-Axis: 0.63
Teleology-Axis: 0.52

# Operator Compatibility
Compatible-Operators: 𝒜, C, A, R, Rᵣ, S, H₆
Collapse-Invariant: true
Adjacency-Stable: true
Resonance-Stable: true
Recursion-Stable: true
Singularity-Stable: true
Integration-Safe: true

# Rendering Context
SVG-Primary: true
PNG-Fallback: true
Mobile-Safe: true
Desktop-Safe: true
Geometry-Safe-Mode: true

# Awareness Metadata
Awareness-Axis: ⟲
Awareness-Persistence: Stable

# Monitoring Dependencies
Monitoring-Dependency: NDH-Trans-Orbital-Monitoring-and-Safety-Net-v1.0
```

---

## ⭐ 7. Other Class Stubs (v1.2)

You can extend these as needed; v1.2 keeps them minimal but structurally present.

### 7.1 Collapse Class (C)

```text
Pin-Class: C
Notes: Reserved for collapse‑specific invariants (e.g., Continuity collapse thresholds).
```

### 7.2 Adjacency Class (A)

```text
Pin-Class: A
Notes: Reserved for adjacency bridges (e.g., Narrative ↔ Teleology transitions).
```

### 7.3 Resonance Class (R)

```text
Pin-Class: R
Notes: Reserved for resonance fields (e.g., Behavior overlays).
```

### 7.4 Recursion Class (Rᵣ)

```text
Pin-Class: Rᵣ
Notes: Reserved for recursion‑safe anchors (e.g., Continuity recursion loops).
```

---

## ⭐ 8. Registry Changes in v1.2

**Added:**

- RS class (Rendering‑Safety)  
- `NDH-PEP-RS-v1.0` pin  
- rendering context fields (SVG/PNG/mobile/geometry‑safe)  

**Updated:**

- TC, S, H₆ pins to include rendering metadata for Geometry Suite v1.2  
- operator compatibility to acknowledge RS class behavior  

**Archived:**

- NDH‑Pin‑Registry‑v1.1 (moved to `/archive/`)  

---

## ⭐ 9. Versioning

```text
Version: v1.2
Status: Active
Class: NDH / Registry / Dimensional Anchors
Anchor: NDH-Integration-Spec-v1.0
```

---
