---
title: C.U Relay Charter
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
  - "[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Estela Integralism/Identity|Identity]]"
  - "[[Origin]]"
  - "[[Key]]"
  - "[[law]]"
  - "[[Continuity]]"
  - "[[Time]]"
Recommended Reading:
  - "[[Locations Portal]]"
  - "[[Public Reader Path - Pleroma Archive]]"
Last Reviewed: 2026-06-18
---
## Summary

Purpose. De
[[Colonial Union]] Relay (PFN) Cha
rter (v1.0)

Operator: CU-Relay Authority (CURA) under the [[Colonial Union]] Assembly.

Topology: Star-of-Sol hub-and-spoke. Each colony maintains exactly one PFN joined only to CU-Relay–Sol.

II. [[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Estela Integralism/Identity|Identity]], Keys, & Trust

Mutual attestation at session start (post-quantum signatures).

Public audit proofs (Merkle attestations) for slot allocation and message headers (not content).

III. Scheduling & QoS

P0 Safety-of-Life (SoL) – distress, medical, navigational hazards. Preemptive; 0-latency slot; free.

P2 Governance & Courts – laws, warrants, injunctions, arbitration filings. 30-min slots; subsidized.

P3 Market & Finance – auctions, exchange ticks, customs, insurance. 15-min slots; metered.

P4 Routine & Personal – mail, academic, cultural. 5–10-min slots; metered cheapest.

Baseline capacity per PFN: narrowband, e.g. 64 kbps sustained (configurable by era).

Slot fairness: Proportional fair queuing; no exclusive leases except disaster periods (see §VIII).

Timekeeping: CU-Relay provides canonical UTC; PFNs must correct drift daily.

IV. Formats & Restrictions

Compression & dedupe mandatory; content-hashing for caching at Sol.

V. Privacy & Cryptography

Content seizure only via court order (colony court + CU Appeals concurrence).

Anonymity: SoL may be anonymous; all others require accountable [[Origin]].

VI. Transparency & Audit

Public dashboards: per-PFN utilization, wait times, drop/deny stats, class breakdown.

Tamper logs: immutable, publicly verifiable.

Quarterly independent audits (technical + process).

VII. Sanctions & Remedies

CURA may impose:

Rate-limits (by class),

Embargoes (class P3–P4 only),

Escrow of disputed governance/market payloads pending tribunal,

Temporary suspension for tampering or abuse.

Whitelists: P0–P1 cannot be throttled or embargoed.

VIII. Emergency Provisions

Disaster Posture: P0/P1 expand to absorb ≥60% of capacity; P3/P4 curtailed.

Mutual Aid: CURA may reassign surplus Sol capacity to affected PFNs.

Blackout Protocol: if a colony’s PFN fails, Sol opens Public Boardcasts (PB) for safety bulletins; couriers carry bulk relief data.

IX. Anti-Abuse & Security

Steganography bans in P0/P1; cryptographic watermarks required.

Spoofing SoL: felony; permanent P4 cap and fines on conviction.

X. Fees & Tariffs (reference schedule)

P0 SoL: free.

P1 Public Safety: free.

P2 Governance/Courts: 0.02 credits/kB; first 5 MB per day free.

P3 Market/Finance: 0.05 credits/kB; exchange feeds may contract for standing micro-slots (≤10% total capacity).

P4 Routine: 0.01 credits/kB off-peak; 0.03 peak.

Surcharges: abuse investigations, emergency overuse beyond quota.

XI. Interop & Backups

Laser tight-beam gateways at Sol mirror [[Key]] governance docs to courier packets (non-FTL fallback).

Disaster caches: standardized “PFN-lite” message sets for ships.

XII. Governance & Jurisdiction

CU Assembly sets policy; CU Relay Tribunal adjudicates disputes; Colony courts retain [[Origin]]-side [[law]] for content legality.
fine lawful operation of Paired FTL Nodes (PFNs) linking each colony to the [[Colonial Union]] Relay at Sol (CU-Relay–Sol); ensure safety-of-life traffic, fair access, privacy, auditability, and sanction tools.

I. Authority & Scope

Exclusivity: No colony-to-colony FTL; all cross-colony FTL is switched at Sol.

Hardware pair-binding at manufacture; tamper-evident seals.

Rotating session keys per slot; hardware-rooted ephemeral keys.

Traffic is slotted; each PFN publishes a Daily Queue (UTC) with five priority classes:

P1 [[Continuity]] & Public Safety – epidemiology, disaster alerts, debris warnings. Hard 15-min cap/session; free.

Content types: text, compressed data, cryptographic proofs, control signals. No bulk media; no executable uploads that alter PFN firmware.

End-to-end encryption permitted; header metadata (sender/receiver, class, slot [[Time]], byte counts) is public for audit.

Appeals: summary appeal to CU Relay Tribunal within 24 h (P2–P3) / 7 d (P4).

Malware / exploit payloads: lifetime ban + shared signatures.

Neutrality: CURA is barred from content-based discrimination outside court orders and class rules.

## Details

## References


## Legacy Content

> Automated segregation run completed.
> Moved to Summary: 12 block(s).
> Moved to Details: 49 block(s).


[[Colonial Union]] Relay (PFN) Charter (v1.0)

Purpose. Define lawful operation of Paired FTL Nodes (PFNs) linking each colony to the [[Colonial Union]] Relay at Sol (CU-Relay–Sol); ensure safety-of-life traffic, fair access, privacy, auditability, and sanction tools.

I. Authority & Scope

Operator: CU-Relay Authority (CURA) under the [[Colonial Union]] Assembly.

Topology: Star-of-Sol hub-and-spoke. Each colony maintains exactly one PFN joined only to CU-Relay–Sol.

Exclusivity: No colony-to-colony FTL; all cross-colony FTL is switched at Sol.

II. [[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Estela Integralism/Identity|Identity]], Keys, & Trust

Hardware pair-binding at manufacture; tamper-evident seals.

Mutual attestation at session start (post-quantum signatures).

Rotating session keys per slot; hardware-rooted ephemeral keys.

Public audit proofs (Merkle attestations) for slot allocation and message headers (not content).

III. Scheduling & QoS

Traffic is slotted; each PFN publishes a Daily Queue (UTC) with five priority classes:

P0 Safety-of-Life (SoL) – distress, medical, navigational hazards. Preemptive; 0-latency slot; free.

P1 [[Continuity]] & Public Safety – epidemiology, disaster alerts, debris warnings. Hard 15-min cap/session; free.

P2 Governance & Courts – laws, warrants, injunctions, arbitration filings. 30-min slots; subsidized.

P3 Market & Finance – auctions, exchange ticks, customs, insurance. 15-min slots; metered.

P4 Routine & Personal – mail, academic, cultural. 5–10-min slots; metered cheapest.

Baseline capacity per PFN: narrowband, e.g. 64 kbps sustained (configurable by era).

Slot fairness: Proportional fair queuing; no exclusive leases except disaster periods (see §VIII).

Timekeeping: CU-Relay provides canonical UTC; PFNs must correct drift daily.

IV. Formats & Restrictions

Content types: text, compressed data, cryptographic proofs, control signals. No bulk media; no executable uploads that alter PFN firmware.

Compression & dedupe mandatory; content-hashing for caching at Sol.

V. Privacy & Cryptography

End-to-end encryption permitted; header metadata (sender/receiver, class, slot [[Time]], byte counts) is public for audit.

Content seizure only via court order (colony court + CU Appeals concurrence).

Anonymity: SoL may be anonymous; all others require accountable [[Origin]].

VI. Transparency & Audit

Public dashboards: per-PFN utilization, wait times, drop/deny stats, class breakdown.

Tamper logs: immutable, publicly verifiable.

Quarterly independent audits (technical + process).

VII. Sanctions & Remedies

CURA may impose:

Rate-limits (by class),

Embargoes (class P3–P4 only),

Escrow of disputed governance/market payloads pending tribunal,

Temporary suspension for tampering or abuse.

Appeals: summary appeal to CU Relay Tribunal within 24 h (P2–P3) / 7 d (P4).

Whitelists: P0–P1 cannot be throttled or embargoed.

VIII. Emergency Provisions

Disaster Posture: P0/P1 expand to absorb ≥60% of capacity; P3/P4 curtailed.

Mutual Aid: CURA may reassign surplus Sol capacity to affected PFNs.

Blackout Protocol: if a colony’s PFN fails, Sol opens Public Boardcasts (PB) for safety bulletins; couriers carry bulk relief data.

IX. Anti-Abuse & Security

Steganography bans in P0/P1; cryptographic watermarks required.

Malware / exploit payloads: lifetime ban + shared signatures.

Spoofing SoL: felony; permanent P4 cap and fines on conviction.

X. Fees & Tariffs (reference schedule)

P0 SoL: free.

P1 Public Safety: free.

P2 Governance/Courts: 0.02 credits/kB; first 5 MB per day free.

P3 Market/Finance: 0.05 credits/kB; exchange feeds may contract for standing micro-slots (≤10% total capacity).

P4 Routine: 0.01 credits/kB off-peak; 0.03 peak.

Surcharges: abuse investigations, emergency overuse beyond quota.

XI. Interop & Backups

Laser tight-beam gateways at Sol mirror [[Key]] governance docs to courier packets (non-FTL fallback).

Disaster caches: standardized “PFN-lite” message sets for ships.

XII. Governance & Jurisdiction

CU Assembly sets policy; CU Relay Tribunal adjudicates disputes; Colony courts retain [[Origin]]-side [[law]] for content legality.

Neutrality: CURA is barred from content-based discrimination outside court orders and class rules.

---

> [!info] Original Vault Path
> `I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/C.U Relay Charter.md`
