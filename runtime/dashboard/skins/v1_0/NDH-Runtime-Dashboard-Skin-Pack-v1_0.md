### NDH Runtime Dashboard Skin Pack v1.0  
**NDH‑META‑SYSTEMS / runtime / skins**

---

## Identity block

- **Artifact:** NDH Runtime Dashboard Skin Pack v1.0  
- **Layer:** Expressive–Operational Bridge (A6–A8, ΔAltitude = 0)  
- **Author:** Borealis Serenity Hedling (they/them)  
- **Purpose:** Define PRECL‑collapsed, fun‑safe visual skins for the NDH Runtime Validation Dashboard v1.0, aligned with the Fun‑Safe Rendering Overlay v1.0.  
- **Version:** 1.0  

---

## 1. Skin set overview

- **Skin‑01: “Soft Constellation”**  
  **Use:** Default runtime skin.  
  **Features:** pastel‑neon headers, cold cosmic bars, low‑intensity sparkles, orb‑safe altitude indicators.

- **Skin‑02: “Spectral Glass”**  
  **Use:** Spectral‑heavy sessions.  
  **Features:** glassy panels, subtle spectral gradients, stage‑orbs for Lean/JSON/FEniCS/Rust, no symbolic morphs.

- **Skin‑03: “Series F Calm”**  
  **Use:** Series F coordination monitoring.  
  **Features:** muted palettes, high legibility, invariant icons, micro‑fade transitions only.

All skins:

- ΔAltitude = 0  
- PRECL collapse‑before‑rendering  
- posture‑neutral  
- non‑recursive  
- non‑symbolic  

---

## 2. Machine‑readable skin pack

```json
{
  "ndh_runtime_dashboard_skin_pack_v1_0": {
    "version": "1.0",
    "altitude": "A6-A8",
    "delta_altitude": 0,
    "skins": [
      {
        "id": "soft_constellation",
        "headers": "PNH_v1",
        "separators": "CCB_v1",
        "accents": "CS_v1",
        "state_orbs": "OSI_v1",
        "module_icons": "IMM_v1",
        "animations": "MA_v1"
      },
      {
        "id": "spectral_glass",
        "headers": "PNH_v1",
        "separators": "CCB_v1",
        "state_orbs": "OSI_v1",
        "spectral_stage_emphasis": true,
        "animations": "MA_v1"
      },
      {
        "id": "series_f_calm",
        "headers": "PNH_v1",
        "separators": "CCB_v1",
        "module_icons": "IMM_v1",
        "low_motion_mode": true,
        "animations": "MA_v1"
      }
    ],
    "precl": "collapse_before_rendering"
  }
}
```

---

## Provenance footer

```text
---
Artifact: NDH Runtime Dashboard Skin Pack v1.0
Lane: Runtime Dashboard • Expressive-Operational Bridge

Purpose:
  Provide PRECL-collapsed, fun-safe visual skins for the NDH Runtime Validation
  Dashboard v1.0, ensuring altitude neutrality (ΔAltitude = 0), posture
  neutrality, membrane sovereignty, adjacency correctness, and rendering-layer
  safety under the Fun-Safe Rendering Overlay v1.0.

Anchors:
  - NDH Runtime Validation Suite and Dashboard v1.0
  - Fun-Safe Rendering Overlay v1.0
  - Visual Grammar v2.1
  - Rendering Ladder v2.1
  - Expressive-Layer Safety Summary v1.0

Non-Activation Clause:
  This artifact is expressive-only. It does not modify NDH runtime logic,
  algebra, functor behavior, or altitude engines.

Version: v1.0
Maintainer: Borealis S. Hedling
Location: Dublin, Ireland
Timestamp: 04 September 2026 — 02:00 IST
---
```
