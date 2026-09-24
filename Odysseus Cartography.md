---
title: "Odysseus Galaxy — Scientific Cartography Spec (v1.0)"
tags:
  - canon
  - location
  - tier-2
  - pleroma-archive
Status: CANON
Category: Location
Complexity: Tier 2
Prerequisites:
  - "[[Archive Index]]"
  - "[[Locations Portal]]"
Related Notes:
  - "[[Locations Portal]]"
  - "[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Yauturn Sovereignty/System|System]]"
Recommended Reading:
  - "[[Locations Portal]]"
  - "[[Public Reader Path - Pleroma Archive]]"
Last Reviewed: 2026-06-18
---
# Odysseus Galaxy — Scientific Cartography Spec (v1.0)

This document defines a **science-first, 3D coordinate and tiling [[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Yauturn Sovereignty/System|System]]** for mapping the Odysseus cD galaxy (≈ 8 Mly across). It is camera-independent and reproducible.

---

## 1) Reference Frame

- **Origin (O):** SMBH at the quasar core.
- **ẑ (polar axis):** unit vector along the net angular-momentum vector of the accretion disk (parallel to the twin jets). Defines **North (+z)** and **South (−z)**.
- **x̂ (zero-meridian):** chosen in the equatorial plane (z=0). Recommended options (pick one and keep it):
  - Major axis of the inner cD isophotes (stellar mass ellipse), projected to z=0.
  - Direction to the brightest inbound filament at the core.
- **ŷ:** completes a right‑handed system via **ŷ = ẑ × x̂**.

> Publish the chosen x̂ definition (e.g., “inner isophote major axis PA = 28.0° from ICRS east”) so all maps agree.

---

## 2) Coordinate Systems

### Cartesian (x, y, z) [kpc]
- For dynamics, simulation, spatial indexing.

### Cylindrical (R, φ, z) [kpc, deg]
- **R = sqrt(x² + y²)**
- **φ = atan2(y, x)** (0° at +x̂, increasing toward +ŷ; store in [0°, 360°)).
- **z** as defined above.
- Best for rings/sectors and transit lanes.

### Spherical (r, θ, φ) [kpc, deg]
- **r = sqrt(x² + y² + z²)**
- **θ = arccos(z / r)** (polar; 0° at +ẑ)
- **φ** as above.

### Galactic‑like (longitude/latitude)
- **Longitude λ ≡ φ**
- **Latitude β ≡ arcsin(z / r)**

---

## 3) Tiling (Rings, Sectors, Belts)

### Rings (by cylindrical R)
- **R0 Core:** 0–50 kpc
- **R1 Bright Envelope:** 50–300 kpc
- **R2 Inner Halo:** 300–1000 kpc
- **R3 Ghost Halo:** 1000–3000 kpc
- **R4 Frontier:** 3000–4000 kpc (≈ 8 Mly diameter total)

> Adjust thresholds as data improves; keep IDs stable (R0…R4).

### Latitude Belts (by |z|)
- **Z0 Equatorial:** |z| < 50 kpc
- **Z1 Mid‑lat:** 50–200 kpc
- **Z2 Polar:** |z| ≥ 200 kpc

### Azimuthal Sectors (by φ)
- Choose **N = 32** (11.25° per wedge) or **N = 16** (22.5°). Default: **N = 32**.
- Sector ID: **S00…S31**, where S00 covers φ∈[0°, 11.25°), S01: [11.25°, 22.5°), …

### Composite Cell ID
`<Ring>-<Sector>-<Belt>` e.g., **R2-S07-Z1**.

---

## 4) Navigational Layers

- **Filament Routes:** polyline graphs in (R, φ, z); e.g., Arm of Ilythar.
- **Jet Corridors:** two polar cones, e.g., θ ≤ 20° (North), θ ≥ 160° (South).
- **Hazards:** volumes (spheres/cylinders/polyhedra) for X‑ray cavities, radio lobes, AGN zones.
- **No‑go shells:** isodanger contours around the quasar core (Eddington-limited radiation fields).

---

## 5) Physical/Political/Ceremonial Overlays

- **Physical:** rings/sectors/belts + routes + hazards.
- **Political:** provinces (former galactic nuclei) stored as named regions mapped onto the grid.
- **Ceremonial (optional):** “Four Choirs” (quadrants) as φ ranges:
  - **Choir A:** 0°–90°, **B:** 90°–180°, **C:** 180°–270°, **D:** 270°–360°.
  - Ceremonial only — does not override physical tiling.

---

## 6) Units & Conventions

- **Distance:** kpc (display Mly as needed; 1 Mly ≈ 306.6 kpc).
- **Angles:** store degrees; radians in code if preferred.
- **Velocities (optional):** cylindrical **(v_R, v_φ, v_z)** in km/s.
- **Epoch:** define a fixed epoch for any time‑varying features (e.g., AGN state).

---

## 7) Data Objects (summary; see JSON schema)

- **SectorCell**: `{ringId, sectorId, beltId, bbox}`
- **Province**: named polygon or multipatch mapped to one or many SectorCells; includes metadata.
- **Route**: named polyline (filament/jet lane) with waypoints in (R, φ, z) or (x, y, z).
- **Hazard**: volumetric region with type and parameters (sphere/cylinder/poly).
- **POI** (point of interest): system/world/station with position + tags.

---

## 8) Display Defaults

- **Color map:** Core (orange), Radiant (gold), Ghost (grey), Frontier (red dotted), Arms (turquoise), Jets (violet/blue).
- **Labeling:** use short IDs on base map; expand to full names on hover/click.
- **Scale bars:** show both kpc and Mly.

---

## 9) Validation

- All φ in [0°, 360°).
- Ring/sector/belt IDs must be valid enumerations.
- Geometry must be given in **one** coordinate system per object (declare it).

---

## 10) Provenance

- `frameDefinition`: textual note describing x̂ choice and jet axis derivation.
- `version`: increment on any breaking change to IDs/boundaries.

---

> [!info] Original Vault Path
> `I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Ho'oleilana/Boo╠êtes Supercluster/Odysseus Galaxy/Odysseus Cartography.md`
