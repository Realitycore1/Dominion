---
title: "Mag Boots"
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
  - "[[Man]]"
  - "[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]"
  - "[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]]"
  - "[[New Readers Start Here/I - Pleroma Archive/World/Civilizations/Dominion/Dominion]]"
Recommended Reading:
  - "[[Locations Portal]]"
  - "[[Public Reader Path - Pleroma Archive]]"
Last Reviewed: 2026-06-18
---
What they’re for

Controlled locomotion in micro-g on ferrous decks/rails.

Hands-free work-holding on hulls and inside bays.

Emergency “stick” when a tether fails or a blowdown gust hits.

Core designs (pick per hull material)

Electromagnet soles (EM)

Coils pull against ferromagnetic steel/ferrite in the deck.

Pros: variable force, fast release. Cons: draws power when on; EMI to manage.

Electro-permanent magnets (EPM)

Hybrid AlNiCo/NeFeB blocks toggled by a brief pulse; zero hold power.

Pros: no idle draw, fail-safe hold on power loss. Cons: needs ferrous target; add pry tabs for manual release.

Rail-coupled shoes

Boots couple to embedded steel strips/pebbled ferrite tiles along passageways.

Pros: cheap decks, strong grip where needed. Cons: off-rail areas need handholds.

Gecko pads (van der Waals)

Micro-fibrillar soles for composites/CFRP/aluminum.

Pros: vacuum-friendly, low EMI. Cons: hates dust/oils; needs periodic cleaning.

Electroadhesive pads

High-voltage, low-current “electrostatic cling” on dielectrics.

Pros: works on many plastics/paint. Cons: arcing risk if sharp edges; use with HV interlocks.

Micro-spike cleats

Retractable ceramic/diamondlike spikes for ice/regolith or textured gratings.

Pros: works when nothing else does. Cons: damages surfaces; last-resort only.

For aluminum hull plates: EM won’t hold; use gecko/electroadhesive or install ferrous rails along corridors and service rings. “Eddy-current” tricks are great for braking a moving foot, not for static hold.

Control & ergonomics

Heel/Toe zones: independent pads so you can roll a step (heel off → swing → toe plant).

IMU gait assist: detects swing phase; auto-modulates hold.

Dead-[[Man]]: spring toe switch + glove kill-switch; long-press to hard-release both soles.

Quiet mode: soft-start field to avoid slamming plates; noise < 40 dBA.

EMI hygiene: μ-metal shoe cans + twisted-pair drive leads; keep <5 mG at avionics height.

Ballpark performance (useful numbers)

Hold force target (per boot): 400–800 N (≈40–80 kgf) adjustable.

Response: on/off < 30–50 ms (EM), < 10 ms (EPM toggle).

Energy: EM 5–25 W while engaged (duty-cycled with gait); EPM ≈ 0 W hold, ~[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]–5 J per toggle.

Sole area (active pad): ~25–40 cm² per zone.

Simple force estimate (EM on steel):

𝐹
≈
𝐵
[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]
 
𝐴
[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]
𝜇
0
F≈
2μ
0
	​

B
[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]
A
	​


Example: 
𝐵
=
0.6
 T
B=0.6 T, 
𝐴
=
[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]].5
×
10
−
[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]]
 m
[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]
⇒
𝐹
≈
360
 N/pad
A=[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]].5×10
−[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]]
 m
[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]
⇒F≈360 N/pad. Two pads ≈ 700 N per boot.

Safety & failure Modes

Power-off behavior: EM releases; EPM stays latched (good for brownouts—add pry tabs).

Trip / ankle load: set a max shear so a violent snag releases before twisting a knee.

Contamination: gecko/electroadhesive degrade with dust/oils → carry a dry cleaning roller or swap pads.

Arc discipline: electroadhesive HV interlocked to vacuum rating and sharp-edge detection.

Mag hazards: label keep-out around implantable devices and mag-sensitive tools.

Maintenance

Swap pad modules in < 60 s; check coil resistance weekly (EM).

Geckos: solvent wipe + lint-free roller; replace at ~10⁴ steps on gritty decks.

EPM: cycle test monthly; verify pry tabs and lock LEDs.

[[New Readers Start Here/I - Pleroma Archive/World/Civilizations/Dominion/Dominion]] / Athearn / Harmonic flavors (for your setting)

[[New Readers Start Here/I - Pleroma Archive/World/Civilizations/Dominion/Dominion]] MB-9 (fleet standard): EPM+gecko hybrid. Ferrous walk strips in corridors, gecko pads for composite bays. IMU-assisted gait and PFN-logged footfall telemetry for accident forensics.

Athearn Wayhouse boots: Heavy rail-coupled EPM, big safety margin, loud audit beeps on engage/release; rails are everywhere on inspection decks.

Harmonic “QuietStep”: Gecko + electroadhesive only (minimal EMI), soft-start HV, and a chorus-chime when both feet free (crew etiquette cue).

SOP (shipboard)

Blue light = free; amber = one foot latched; green = both latched.

Never move both feet “red” (override latch) unless stationary & braced.

Crossing a non-ferrous zone: flip to Gecko Mode or “rails only.”

EVA: boots supplement tethers, they don’t replace them. Always rig two points.

---

> [!info] Original Vault Path
> `I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Technology/Tools/Mag Boots.md`
