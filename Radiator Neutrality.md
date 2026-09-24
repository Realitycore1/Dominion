---
title: Radiator Neutrality Code v1.0 — Heat Rights, Markets & Emergency Use
Status: CANON
version: 1.0
tags: [Dominion, HeatEconomy, Safety, Ports, Governance, NLPG, Corridors]
links: [[MOT_Operations_And_Safety_Dials_v1]], [[Seat_Sanctum_SOP_v1.0]], [[Nullity_Ops_v1.0]], [[I - Pleroma Archive/Knowledge/Axiom Anchors|Axiom_Anchors_v1.0]]
Category: Archive Infrastructure
Complexity: Tier 1
Prerequisites:
  - "[[Archive Index]]"
Related Notes:
  - "[[Archive Index]]"
  - "[[MOT_Operations_And_Safety_Dials_v1]]"
  - "[[Seat_Sanctum_SOP_v1.0]]"
  - "[[Nullity_Ops_v1.0]]"
  - "[[I - Pleroma Archive/Knowledge/Axiom Anchors|Axiom_Anchors_v1.0]]"
  - "[[Key]]"
  - "[[Rights]]"
Recommended Reading:
  - "[[Archive Index]]"
  - "[[Public Reader Path - Pleroma Archive]]"
Last Reviewed: 2026-06-18
---


# Radiator Neutrality Code v1.0 — Heat Rights, Markets & Emergency Use

> **Principle.** **Radiators** are life-safety infrastructure for Σ rejection after rites, corridors, and Null exits. When **neutral**, they are protected like hospitals: accessible, audit-logged, and outside factional control.

## 1) Definitions

- **Neutral Radiator:** a licensed reject-area with posted capacity, signage, and public telemetry.  
- **Reject-Area Unit:** **m²/MW** equivalent (Ops Dials: space **0.8 m²/MW**, atmo **5.0 m²/MW**).  
- **Σ Dump:** logged conversion of stored entropy into heat at a neutral radiator.  
- **Heat Market:** posted capacity/prices for non-emergency Σ dumping.

## 2) Neutrality Rules

- **Scope:** applies to all neutral radiators, their buffers, feeds, and control rooms.  
- **Marking:** high-contrast beaconing; *no* factional livery.  
- **Access:** first-come within **priority tiers**, no political tests.  
- **Protections:** no weapons discharge, no rites/choirs beyond safety ops; monitored by RAC/Harmonic.

## 3) Priority Tiers (descending)

1) **Life-safety:** hospitals, SAR, emergency vessel Σ after Null exits  
2) **Stability-critical:** gate anchors, sancta cool-downs, corridor Σ deficits  
3) **Civic:** utilities, transit hubs  
4) **Commercial:** scheduled industrial Σ dumps

## 4) Posting & Booking

- Ports publish **hourly capacity** and **queue times**; API + public board.  
- **Booking window:** up to **72 h** ahead (Tiers 3–4); **on-demand** for Tiers 1–2.  
- **PFN logs:** radiator controllers hash state every **60 s** under load.

## 5) Market Conduct

- **Price bands:** bounded by posted **cost floor** and **cap** per MW·h; bands tighten during incidents.  
- **Anti-hoarding triggers:** if **available capacity < 20%** for > 2 h, auto-freeze commercial bookings; civil authority may **requisition** up to **30%** private capacity at cap price.  
- **Dump smoothing:** stagger large dumps to avoid thermal spikes; baffles engaged.

## 6) Emergency Rationing

- **Declaration:** RAC issues **Heat Emergency** when Σ queues exceed **30 min** for Tiers 1–2.  
- **Measures:** suspend auctions; commandeer idle arrays; reroute traffic; deploy **portable radiators**.  
- **Termination:** automatic when queues < **10 min** for 3 consecutive hours; AAR in **72 h**.

## 7) Compliance & Penalties

- **Violations:** denial of access, non-neutral livery, capacity misreporting, sabotage, unauthorized rites, PFN spoofing.  
- **Penalties:** fines (×3 cap price), license suspension, civil liability, criminal referral; in conflict, **neutrality flip** requires Conclave/RAC sign-off + public proof record.

## 8) Engineering & Safety

- **Interlocks:** backflow preventers; thermal surge baffles; isolated power feeds.  
- **Metrology:** calibrated Σ meters; fault-tolerant logging; tamper-evident seals.  
- **Redundancy:** N+1 radiator fields for major ports; portable units on 4 h deployment SLA.  
- **Human factors:** clear egress lanes; heatstroke kits; ombuds presence during emergencies.

## 9) Templates & Forms

### 9.1 Public Capacity Notice
```
NEUTRAL RADIATOR CAPACITY — {PORT}
Space eq: {m²}  |  Atmo eq: {m²}
Booked (next 3h): {MW·h}
Queue (T1/T2): {min}
Status: {NORMAL / HEAT EMERGENCY}
```

### 9.2 Σ Dump Request (Tiers 3–4)
```
Vessel/Facility: {id}
Requested slot: {UTC}
Expected Σ: {MW·h}
PFN hash: {hash}
Safety contact: {name/comm}
```

## 10) KPIs & Audits

- **Queue times** (T1/T2) • **Utilization** (%) • **Σ deficits** averted • **Incidents**/month • **PFN compliance** • **Hoards detected**  
- **Audits:** quarterly RAC audit; random ombuds inspections; after-action within **72 h** of emergencies.

---
**Cross-refs:** [[MOT_Operations_And_Safety_Dials_v1]] • [[Seat_Sanctum_SOP_v1.0]] • [[Nullity_Ops_v1.0]] • [[Axiom Anchors|Axiom_Anchors_v1.0]]

---
title: Window Proof Sheet — Template
status: template
version: 1.0
tags: [Template, MOT, Gates, Engineering, Proof]
---

# Window Proof Sheet — Template

**Port / Gate ID:**  
**UTC:**  
**Operator:**  
**RAC Surveyor:**  

## Survey Inputs
- Φ:  
- η:  
- ℓᶜ:  
- 𝒦 (orientation):  

## Arc Geometry
- **R_a (radius):**  
- **α (tilt):**  
- **b_arc (bandwidth, PFN-eq):**  

## Performance
- **Predicted jitter (95p):**  
- **Spool / Cool:**  
- **Θ_safe (η ceiling):**  

## Budgets
- **G export (GEZ draw/hr):**  
- **Σ (entropy) plan:** radiator booking {MW·h @ UTC}, neutral field: {yes/no}  

## Proofs & Logs
- **PFN hash (current):**  
- **Attachments:** aether-weather map, α/𝒦 diagram, radiator reservation

**Signatures:** Port CE • RAC Surveyor

---
title: Reason Sheet — Template
status: template
version: 1.0
tags: [Template, Governance, MOT, Proof, Policy]
---

# Reason Sheet — Template

**Title:**  
**Context:** (incident / policy / route change)  
**UTC:**  
**Decision owner(s):**  

## Hypothesis
One-line statement of what is believed true and why it matters.

## Plan
- Actions & timelines  
- Ω_c profile (expected duty/cool)  
- Expected ΔS(t) recovery

## Null/Veil Checks
List which operations remain valid under Veil/Null; no acausal threads.

## Risks & Backfire
- Taboos potentially engaged  
- Choir caps & exit-[[Key]] plan  
- Radiator plan (neutrality, bookings)

## KPIs
ΔS • η variance • ℓᶜ recovery • jitter • PFN compliance • [[Rights]]-restoration SLA

**Sign-offs:** Athearn liaison • DVAA representative • RAC auditor

---

> [!info] Original Vault Path
> `I - Pleroma Archive/Knowledge/Radiator Neutrality.md`
