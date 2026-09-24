---
title: "Gravity Harness"
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
  - "[[New Readers Start Here/I - Pleroma Archive/World/Civilizations/Dominion/Dominion]]"
  - "[[Verseon]]"
  - "[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]]"
  - "[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]"
  - "[[Chapter (The Old War)|Chapter (The Old War)]]"
  - "[[Time]]"
Recommended Reading:
  - "[[Locations Portal]]"
  - "[[Public Reader Path - Pleroma Archive]]"
Last Reviewed: 2026-06-18
---
What it does

Personal rig that gives the wearer a controllable down-vector (0–1 g) in microgravity. Primary use cases: hands-free work, injury-safe movement, and stable shooting/repair posture.

Core architectures (pick per setting/era)

Grid-Coupled Grav (GCG) — ties into a ship/station’s gravity grid.

Waist/back plate contains a field coupler that locks to the deck’s grav lines (encrypted, low-power).

Pros: minimal power draw, silent, strong hold. Cons: only works where grav lines exist (decks, ladders).

Local Pseudograv (LPG) — wearable field projectors generate a small gradient around the suit.

Uses gravitomagnetic resonators / mass-driver rings to create a down-force relative to a reference beacon.

Pros: works on bare hulls/asteroids. Cons: higher power, faint hum/heat.

Inertial Vector Harness (IVH) — micro-impeller array creates a constant, gentle acceleration “down.”

Cold-gas or ion microthrusters + reaction wheels; IMU closes the loop to feel like gravity.

Pros: simplest/realistic; great as fallback. Cons: propellant/noise; not true gravity (fluids still float).

[[New Readers Start Here/I - Pleroma Archive/World/Civilizations/Dominion/Dominion]]-era note: GCG can couple via a [[Verseon]] impedance pad (down-vector follows the ship’s grav membrane). Harmonic variants avoid strong fields; they use dephase dampers + low-g LPG. Athearn wayhouses favor hard-certified GCG with audit pings.

Anatomy (common to all)

Back plate: coupler or projector core; heat path to a finned spine.

Hip frames: battery + tether reels; anchor for tool lanyards.

Boot nodes: optional mag/gecko pads (for lock-step mode).

IMU stack: detects gait/swing phase; blends hold vs. free.

Nadir lock: software “down” points to a chosen reference (deck tag, beacon, or local normal).

Operating Modes

Walk (0.[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]]–0.6 g): roll heel→toe; auto-release on swing.

Work (0.1–0.[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]] g): just enough to pin you for fine tasks.

Strap-down (1.0 g spike ≤ [[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]] s): brief max for anchoring/impact.

Free (0 g): inert; uses only IMU + reaction wheels to damp drift.

Ballpark performance

Max effective g: 0.8–1.0 g (GCG/LPG); 0.[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]–0.[[Chapter (The Old War)|Chapter (The Old War)]] g continuous (IVH).

Response [[Time]]: < 25 ms (GCG), < 60 ms (LPG), < 80 ms (IVH).

Power draw: 20–80 W (GCG), 150–500 W (LPG), 30–150 W + propellant (IVH).

Endurance (belt pack): 6–12 h (GCG), 1–[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]] h (LPG), [[Chapter (The Old War)|Chapter (The Old War)]]–8 h (IVH; propellant-limited).

Thermal: keep core < 55 °C; silent mode derates to 0.[[Chapter (The Old War)|Chapter (The Old War)]] g.

Quick force heuristic for LPG projector: 
𝐹
≈
𝑘
 
𝐼
[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]
F≈kI
[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]
 (device-specific). Most rigs target 400–800 N peak hold spread across spine/hips.

Safety & failure Modes

Fail-safe stance: power loss → 0 g and auto-deploy dual tethers; if on ferrous deck, boots auto-mag.

Joint loads: shear limit clamps at ~600 N to prevent knee/hip injury; hard lock requires manual override.

EMI/medical: keep ≥30 cm from implants; Harmonic-grade rigs publish field telemetry for audit.

Heat & snag: radiator mantle is touch-cool; all straps breakaway at 1.5 kN.

SOP (shipboard)

Pair to deck tag (GCG) or beacon (LPG/IVH).

Test 0.[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]] g walk → 0.1 g work → hard-lock for 1 s.

Always rig two tethers on EVA; harness assists, doesn’t replace lines.

Crossing non-gridded zones: switch to LPG/IVH or engage mag pads.

Variants by polity

[[New Readers Start Here/I - Pleroma Archive/World/Civilizations/Dominion/Dominion]] GH-9 “Keel” (fleet): GCG primary, LPG backup; [[Verseon]]-pad handshake; PFN logs footfall for mishap forensics.

Athearn “Proof-Hold”: GCG only; mandatory audit chirps at engage/release; rails everywhere on inspection decks.

Harmonic “QuietFall”: LPG tuned ≤0.[[Chapter (The Old War)|Chapter (The Old War)]] g + de-escalation dampers; publishes live field map; no strong EM spikes.

Integrations & accessories

Nadir beacons (stick-on tags) for hull work; set local down.

Tool lanyard hub (auto-reel) synced to gait.

Med-assist mode: ramps g slowly (≤0.05 g/s) for fragile patients.

Dracomari kit: tail-balance fin + radiator-safe straps (no wing pinch).

[[Ameise]] kit: tarsal adapters; scent-rail safe materials.

---

> [!info] Original Vault Path
> `I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Technology/Tools/Gravity Harness.md`
