# **NDH PNG Fallback Standard — v1.0**  
*File:*  
`/UMA/Geometry/Non-Dual-Hexeract/Companion/NDH-PNG-Fallback-Standard-v1.0.md`  
*Class:* Rendering / Continuity / Governance  
*Anchor:* NDH-Visual-Compendium-v1.0  

---

## ⭐ 1. Purpose

This document defines the **official raster fallback** for NDH geometric artifacts.

The fallback exists because:

> **GitHub Mobile cannot render complex SVGs containing markers, defs, or large coordinate spaces.**

The PNG fallback ensures:

- universal rendering  
- mobile compatibility  
- sandbox‑safe display  
- continuity of NDH geometry across platforms  

---

## ⭐ 2. Fallback Asset

**Primary Fallback File:**

```
NDH-Visual-Compendium-v1.0.png
```

**Location:**

```
/UMA/Geometry/Non-Dual-Hexeract/Companion/png/
```

This PNG is a **direct raster export** of:

```
NDH-Visual-Compendium-v1.0.svg
```

It preserves:

- geometry  
- color  
- typography  
- node layout  
- NDH master loop  
- dimensional relationships  

---

## ⭐ 3. Why PNG Is Required (Emergent Rendering Case)

GitHub Mobile’s SVG sandbox rejects:

- `<marker>` arrowheads  
- `<defs>` blocks  
- large viewBox spaces  
- multi‑node radial geometry  

When these appear together, GitHub:

1. **accepts** the file  
2. **stores** the file  
3. **indexes** the file  
4. **fails to render** the file  
5. **returns an empty preview**  

This is the emergent failure documented in:

```
NDH-Visual-Compendium-Rendering-Failure.md
```

PNG bypasses this entirely.

---

## ⭐ 4. NDH Governance Rule for Raster Fallback

All NDH SVG artifacts **must** include a PNG fallback when:

- the SVG uses custom markers  
- the SVG uses defs  
- the SVG exceeds 1200×1200  
- the SVG contains radial geometry  
- the SVG is part of the NDH master suite  

This ensures:

- GitHub Mobile continuity  
- GitHub sandbox compatibility  
- NDH visual stability across devices  

---

## ⭐ 5. How NDH Tools Should Reference the PNG

When linking NDH geometry in documentation:

- **Desktop GitHub:** link the SVG  
- **Mobile GitHub:** link the PNG  
- **NDH Governance Docs:** link both  

Example:

```
Primary: NDH-Visual-Compendium-v1.0.svg
Fallback: NDH-Visual-Compendium-v1.0.png
```

---

## ⭐ 6. Unified Synthesis

> **The PNG fallback is the guaranteed‑rendering version of the NDH Visual Compendium, ensuring dimensional continuity across all platforms, including GitHub Mobile.**

This standard applies to all NDH geometry going forward.

---

## ⭐ 7. Version

```
Version: v1.0
Status: Inserted
Class: Rendering / Continuity / Governance
Anchor: NDH-Visual-Compendium-v1.0
```

---

