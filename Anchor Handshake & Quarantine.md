---
title: Anchor Handshake & Quarantine v1.0
Status: CANON
version: 1.0
tags: [MOT, Anchors, Nullity, Quarantine, Governance, AIF]
links: [[I - Pleroma Archive/Knowledge/Axiom Anchors|Axiom_Anchors_v1.0]], [[Nullity_Ops_v1.0]], [[MOT_Operations_And_Safety_Dials_v1]], [[I - Dominion Omniverse/Knowledge/Verse Collision Field|Verse_Collision_Field_SOP_v1.0]]
Category: Archive Infrastructure
Complexity: Tier 1
Prerequisites:
  - "[[Archive Index]]"
Related Notes:
  - "[[Archive Index]]"
  - "[[I - Pleroma Archive/Knowledge/Axiom Anchors|Axiom_Anchors_v1.0]]"
  - "[[Nullity_Ops_v1.0]]"
  - "[[MOT_Operations_And_Safety_Dials_v1]]"
  - "[[I - Dominion Omniverse/Knowledge/Verse Collision Field|Verse_Collision_Field_SOP_v1.0]]"
Recommended Reading:
  - "[[Archive Index]]"
  - "[[Public Reader Path - Pleroma Archive]]"
Last Reviewed: 2026-06-18
---


# Anchor Handshake & Quarantine v1.0

> **Purpose.** Define the **admission protocol** between a verse-side **Axiom Anchor (pier)** and an incoming **Axiom Anchor Sheath (AAS)**—plus the **quarantine & reimposition** procedures for cross-axiom cargo, code, and minds.

## 1) Handshake — Five Steps (T+00:00 to T+00:10)

**Step 1 — Scan & Compile (≤2 s)**  
- Anchor compiles current **axiom map** from Φ, η, ℓᶜ, Ζₑ, 𝒦.  
- Vessel compiles **compatibility proof** against cached map.

**Step 2 — Exchange Proofs (≤1 s)**  
- Swap **AIF** fingerprints + **continuity seals** (triplicate clocks: *ship • anchor • escrow*).  
- Verify seal freshness (≤ 24 h) and clock consistency (Δt ≤ 50 ms).

**Step 3 — Micro-Reimposition (3 s)**  
- Spin a **micro-sheath** at the interface; run **Null-Verse Test** on EM, clocks, and chemistry.  
- Accept if *EM carriers present*, *clock skew < 10 ms*, *bench assay passes* (see §3).

**Step 4 — Admit (1–3 s)**  
- Open **window** (HAG) or sustain **sheath bubble** (tear).  
- Begin **Σ ledger** reconciliation scheduling; reserve neutral radiator area.

**Step 5 — Log & Notify (≤1 s)**  
- Publish **PFN-equivalent proof hashes** to the port log.  
- Trigger **quarantine routing** as needed.

**Deny conditions:** stale/invalid seals, Σ bank full, radiator shortage, invasive-reality signature, failed bench assay, or policy blocklist.

---

## 2) Continuity Seals (Design)

- **Structure:** Merkle chain over: axiom map ID • AIF bundle hash • Σ ledger digest • nav vector • crew κ-keys (blinded).  
- **Clocks:** *ship • anchor • escrow*; accept with any **2-of-3** concurrence.  
- **Drift handling:** if one clock deranges, freeze its branch and proceed with remaining two; flag for arbitration.

---

## 3) Reimposition Test Matrix (3 s budget)

| Channel | Test | Pass Criteria | Notes |
|---|---|---|---|
| **EM** | Carrier check | stable EM modes present | If fail → sandbox as *rite* |
| **Time** | Clock sync | skew < 10 ms | Uses escrow as tie-break |
| **Chem** | Bench assay | stoichiometry within 0.5% of anchor reference | Uses buffered micro-sheath |
| **Memory** | Continuity poke | hash ring returns prior state | Non-destructive |
| **PFN** | Hash emit | cadence live @ 60 s | If fail → read-only admission |

*If any fail:* route to **Sandbox Quarantine** (see §4).

---

## 4) Quarantine Classes (Q1–Q3)

- **Q1 — Same-Axiom Intake (24 h):** clean bills for human/code/matter; observe, log, exit after Σ dump + final PFN.  
- **Q2 — Cross-Axiom Standard (72 h):** apply **Reimposition** battery (daily micro-sheath checks, error-corrected drift).  
- **Q3 — High-Risk / DE Adjacency (168 h):** isolated **Veil** suites; no choirs; no rites; daily *Null-certified* timebox arbitration.

**Sandbox rules (any class):** artifacts that only operate inside the visitor’s sheath count as **rites** → remain sandboxed until a native-port **Null-Verse Test** passes.

---

## 5) Allowed vs Sandboxed Artifacts

**Allowed (post-Q2):**  
- Native-operable machinery (passes EM/Chem/Time).  
- AIF proof objects and **Witness Capsules**.  
- Human minds and code-persons that pass **Personhood Triad** with local anchors.

**Sandboxed (until explicit clearance):**  
- Sheath-dependent devices/rites.  
- Choir-fused artifacts.  
- Any item with **Σ leakage** exceeding posted radiator reservation.

---

## 6) Templates

### 6.1 Handshake Record (port log)
```
HANDSHAKE — {PORT} — {UTC}
Axiom Map: {id}
Seals: Ship {ok/fail}, Anchor {ok}, Escrow {ok/fail}
Micro-Reimposition: EM {ok} | Time {ok} | Chem {ok} | Memory {ok}
Σ Ledger: {bank %, scheduled dump slot UTC}
Routing: {Q1/Q2/Q3} | Sandbox: {yes/no}
PFN Hash: {hash}
```

### 6.2 Quarantine Intake
```
Subject: {vessel/cargo/person}
Class: {Q1/Q2/Q3}
Duration: {hrs}
Tests: {set}
Radiator Booking: {MW·h @ UTC}
Exit Conditions: {criteria}
Ombuds: {name/comm}
```

---

## 7) Captain’s Quick Card (front)

**Before berth**  
- AIF proofs sealed • Σ bank < 70% • radiator slot booked • crew κ-keys in order.

**During handshake**  
- Watch EM/Time/Chem triad; if *any* fail, request SANDBOX route.

**After berth**  
- Dump Σ on **neutral radiators** • sign quarantine class • publish proof hashes.

---

**Cross-refs:** [[Axiom Anchors|Axiom_Anchors_v1.0]] • [[Nullity_Ops_v1.0]] • [[MOT_Operations_And_Safety_Dials_v1]] • [[Verse Collision Field|Verse_Collision_Field_SOP_v1.0]]

---

> [!info] Original Vault Path
> `I - Pleroma Archive/Knowledge/Anchor Handshake & Quarantine.md`
