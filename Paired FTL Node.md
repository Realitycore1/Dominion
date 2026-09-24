---
title: Paired FTL Node
tags:
  - draft
  - location
  - tier-2
  - pleroma-archive
Status: DRAFT
Category: Location
Complexity: Tier 2
Prerequisites:
  - "[[Archive Index]]"
  - "[[Locations Portal]]"
Related Notes:
  - "[[Locations Portal]]"
  - "[[Colonial Union]]"
  - "[[Origin]]"
  - "[[law]]"
  - "[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Colonies]]"
  - "[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Yauturn Sovereignty/System|System]]"
  - "[[Time]]"
  - "[[Continuity]]"
Recommended Reading:
  - "[[Locations Portal]]"
  - "[[Public Reader Path - Pleroma Archive]]"
Last Reviewed: 2026-06-18
---
## Summary

FTL Comms —
Hub-and-spoke topology: each colon
y has exactly one Paired FTL Node (PFN) linked to the [[Colonial Union]] Relay at Sol (CU-Relay–Sol).

Throughput: narrowband (e.g., ~64 kbps sustained per PFN, configurable by era). Bulk data still rides sub-FTL ships.

Daily queue with five priority classes, enforced at CU-Relay–Sol:

P0 Safety-of-Life (SoL) — distress, medical, nav hazards
– Preemptive; zero-latency slot; free.

P2 Governance & Courts — laws, warrants, injunctions, arbitration filings
– 30-minute slots; subsidized.

P3 Market & Finance — auctions, exchange ticks, customs, insurance
– 15-minute slots; metered.

P4 Routine & Personal — mail, academic, cultural
– 5–10-minute slots; metered cheapest.

Fairness: proportional fair queuing; no exclusive leases (outside declared disasters).

Clock: CU-Relay provides canonical UTC; PFNs correct drift daily.

Privacy & Cryptography

Content seizure only by court order ([[Origin]] colony court + CU Appeals concurrence).

SoL anonymity permitted; all other classes require accountable [[Origin]].

Formats & Restrictions

Allowed: text, compressed data, cryptographic proofs, control signals.

Transparency & Audit

Public dashboards: utilization, wait times, class breakdown, drop/deny stats.

Immutable tamper logs (publicly verifiable).

Quarterly independent technical + process audits.

Sanctions & Remedies (CURA tools)

Rate-limits by class; embargoes (P3–P4 only); escrow of disputed P2/P3 payloads; temporary suspension for tampering/abuse.

Appeals: CU Relay Tribunal—24h (P2–P3) / 7d (P4).

Whitelisting: P0–P1 cannot be throttled or embargoed.

Emergency Provisions

Disaster posture: P0/P1 expand to ≥60% of capacity; P3/P4 curtailed.

Mutual aid: CU can reassign surplus Sol capacity to the affected PFN(s).

Blackout protocol: if a colony PFN fails, CU opens Public Broadcasts for safety bulletins; couriers carry bulk relief data.

Anti-Abuse & Security

Spoofing SoL = felony (permanent P4 cap + fines on conviction).

Fees (reference schedule)

P0 SoL: free

P1 Public Safety: free

P2 Governance/Courts: 0.02 credits/kB (first 5 MB/day free)

P3 Market/Finance: 0.05 credits/kB (standing micro-slots ≤10% total cap)

P4 Routine: 0.01 off-peak / 0.03 peak credits/kB

Surcharges for investigations or emergency overuse beyond quota.

Governance & Jurisdiction

Operator: CU-Relay Authority (CURA) under the [[Colonial Union]] Assembly.

Neutrality: CURA barred from content-based discrimination outside court orders and class rules.

[[law]]: [[Origin]] colony’s [[law]] governs content legality; CU Tribunal governs relay operations.

Operational notes (how it plays at the table)

Info sovereignty = leverage. CU can embargo/slow P3/P4 to pressure bad actors while keeping SoL/Public Safety flowing.

Governance happens over P2. Injunctions, warrants, standards, and arbitration ride FTL quickly; everything else waits for ships.

Black markets emerge. Expect stego attempts, physical dead-drops, and courier networks between neighboring [[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Colonies]] to dodge CU switching.
 Paired FTL Node (PFN) [[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Yauturn Sovereignty/System|System]] (v1.0)
Architecture (what it is)

Only FTL in this era is messaging. No FTL travel.

No colony↔colony FTL. All cross-colony traffic is switched at Sol.

Pair-bound hardware: each PFN is cryptographically and physically paired to CU-Relay–Sol; tamper-evident seals; rotating hardware-rooted session keys.

Scheduling & QoS (how [[Time]] on the link is allocated)

P1 [[Continuity]] & Public Safety — epidemiology, disaster alerts, debris warnings
– 15-minute cap per session; free.

End-to-end encryption allowed; header metadata ([[Origin]]/dest, class, slot [[Time]], byte counts) is public for audit.

Not allowed: bulk media; firmware-altering payloads; P0/P1 steganography (watermarks required).

Malware/exploit signatures shared; lifetime ban lists.

Hardware pair integrity checks at every session; Merkle proofs for slot allocation.

## Details

## References


## Legacy Content

> Automated segregation run completed.
> Moved to Summary: 10 block(s).
> Moved to Details: 43 block(s).


FTL Comms — Paired FTL Node (PFN) [[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Yauturn Sovereignty/System|System]] (v1.0)
Architecture (what it is)

Only FTL in this era is messaging. No FTL travel.

Hub-and-spoke topology: each colony has exactly one Paired FTL Node (PFN) linked to the [[Colonial Union]] Relay at Sol (CU-Relay–Sol).

No colony↔colony FTL. All cross-colony traffic is switched at Sol.

Pair-bound hardware: each PFN is cryptographically and physically paired to CU-Relay–Sol; tamper-evident seals; rotating hardware-rooted session keys.

Throughput: narrowband (e.g., ~64 kbps sustained per PFN, configurable by era). Bulk data still rides sub-FTL ships.

Scheduling & QoS (how [[Time]] on the link is allocated)

Daily queue with five priority classes, enforced at CU-Relay–Sol:

P0 Safety-of-Life (SoL) — distress, medical, nav hazards
– Preemptive; zero-latency slot; free.

P1 [[Continuity]] & Public Safety — epidemiology, disaster alerts, debris warnings
– 15-minute cap per session; free.

P2 Governance & Courts — laws, warrants, injunctions, arbitration filings
– 30-minute slots; subsidized.

P3 Market & Finance — auctions, exchange ticks, customs, insurance
– 15-minute slots; metered.

P4 Routine & Personal — mail, academic, cultural
– 5–10-minute slots; metered cheapest.

Fairness: proportional fair queuing; no exclusive leases (outside declared disasters).

Clock: CU-Relay provides canonical UTC; PFNs correct drift daily.

Privacy & Cryptography

End-to-end encryption allowed; header metadata ([[Origin]]/dest, class, slot [[Time]], byte counts) is public for audit.

Content seizure only by court order ([[Origin]] colony court + CU Appeals concurrence).

SoL anonymity permitted; all other classes require accountable [[Origin]].

Formats & Restrictions

Allowed: text, compressed data, cryptographic proofs, control signals.

Not allowed: bulk media; firmware-altering payloads; P0/P1 steganography (watermarks required).

Transparency & Audit

Public dashboards: utilization, wait times, class breakdown, drop/deny stats.

Immutable tamper logs (publicly verifiable).

Quarterly independent technical + process audits.

Sanctions & Remedies (CURA tools)

Rate-limits by class; embargoes (P3–P4 only); escrow of disputed P2/P3 payloads; temporary suspension for tampering/abuse.

Appeals: CU Relay Tribunal—24h (P2–P3) / 7d (P4).

Whitelisting: P0–P1 cannot be throttled or embargoed.

Emergency Provisions

Disaster posture: P0/P1 expand to ≥60% of capacity; P3/P4 curtailed.

Mutual aid: CU can reassign surplus Sol capacity to the affected PFN(s).

Blackout protocol: if a colony PFN fails, CU opens Public Broadcasts for safety bulletins; couriers carry bulk relief data.

Anti-Abuse & Security

Spoofing SoL = felony (permanent P4 cap + fines on conviction).

Malware/exploit signatures shared; lifetime ban lists.

Hardware pair integrity checks at every session; Merkle proofs for slot allocation.

Fees (reference schedule)

P0 SoL: free

P1 Public Safety: free

P2 Governance/Courts: 0.02 credits/kB (first 5 MB/day free)

P3 Market/Finance: 0.05 credits/kB (standing micro-slots ≤10% total cap)

P4 Routine: 0.01 off-peak / 0.03 peak credits/kB

Surcharges for investigations or emergency overuse beyond quota.

Governance & Jurisdiction

Operator: CU-Relay Authority (CURA) under the [[Colonial Union]] Assembly.

Neutrality: CURA barred from content-based discrimination outside court orders and class rules.

[[law]]: [[Origin]] colony’s [[law]] governs content legality; CU Tribunal governs relay operations.

Operational notes (how it plays at the table)

Info sovereignty = leverage. CU can embargo/slow P3/P4 to pressure bad actors while keeping SoL/Public Safety flowing.

Governance happens over P2. Injunctions, warrants, standards, and arbitration ride FTL quickly; everything else waits for ships.

Black markets emerge. Expect stego attempts, physical dead-drops, and courier networks between neighboring [[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Colonies]] to dodge CU switching.

---

> [!info] Original Vault Path
> `I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Technology/FTL/Paired FTL Node.md`
