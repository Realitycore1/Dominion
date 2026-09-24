---
title: Multi-Link FTL Node
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
  - "[[Relays]]"
  - "[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]"
  - "[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Colonies]]"
  - "[[Time]]"
  - "[[Continuity]]"
  - "[[Origin]]"
Recommended Reading:
  - "[[Locations Portal]]"
  - "[[Public Reader Path - Pleroma Archive]]"
Last Reviewed: 2026-06-18
---
## Summary

Still hub-a
PFN v2 — Multi-Link FTL Comms (Hub
-Controlled Multihoming)
What changed vs PFN v1

From one link → many: each colony may operate multiple paired FTL links (“ports”) instead of a single pair.

Regional [[Relays]] allowed: CU certifies a few Regional [[Relays]] (e.g., Proxima, Epsilon Indi) to take overflow and local disputes, but they ultimately synchronize with Sol.

Topology (three approved Modes)
         [CU-Relay–Sol]  ← Root of trust & global scheduler
            /   |   \
         L1    L2    L3    (PFN trunks to certified Regional [[Relays]])
         |      \     \
 [Regional Relay] \    \___
    (Proxima)      \        \
                    \        \
                 [Colony A]  [Colony B] ... (each multi-homed)

Multi-home to Sol (mandatory baseline):

Each colony runs ≥[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]] PFN ports directly to CU-Relay–Sol.

Gives capacity + hot-failover without changing governance.

Regional [[Relays]] (optional, CU-certified):

CU may authorize Regional [[Relays]] for load-balancing and local cases.

[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Colonies]] can add ports to one or more Regional [[Relays]].

Packets require a Sol attestation token; without it the link won’t carry user traffic.

Typical use: disaster mutual-aid, arbitration fast-paths, standards dissemination.

CU can [[Time]]-box the authorization and revoke instantly.

Capacity & Classes

Per-port bandwidth: narrowband (e.g., ~64 kbps sustained; era-configurable).

Aggregate: colony capacity = Σ(ports). PFN v2 supports link-aggregation and per-class minimums.

Priority classes (unchanged):

P0 Safety-of-Life (SoL) – preemptive, free

P1 [[Continuity]]/Public Safety – free

P2 Governance & Courts – subsidized

P3 Market/Finance – metered

P4 Routine/Personal – metered (cheapest)

New in v2: Per-class floor guarantees across all ports (e.g., P0+P1 reserve ≥30% aggregate at all times).

Routing & Control (how CU keeps the reins)

CRP (Colonial Relay Protocol): a lightweight control protocol (think BGP-lite) where:

[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Colonies]] announce which ports they have (to Sol and any Regional Relay).

Sol publishes slot calendars and class caps per port.

All cross-colony routes carry a Route-of-Record = Sol, even if the packet transits a Regional Relay.

Loop & abuse prevention: route TTLs, signed ledgers, Merkle proofs for slot allocations, per-class rate governors on every port.

Scheduling (v2 refinements)

Proportional fair queuing across all active ports, not just one.

Burst windows for P2 (courts/arbitration) to keep legal matters timely.

Standing micro-slots (≤10% of aggregate) allowed for exchange ticks under P3—revocable on abuse.

Security & Privacy

End-to-end encryption permitted; headers ([[Origin]]/dest, class, byte counts, port) public for audit.

SoL anonymity still honored.

Regional [[Relays]] undergo the same quarterly independent audits as Sol.

Sanctions & Safeguards (what CU can do)

Per-port throttles (class-specific), port suspensions, or full embargo on P3/P4 while P0/P1 remain inviolate.

Escrow at Sol for disputed P2/P3 payloads.

Revocation of inter-colony authorizations with immediate tear-down.

Fees (reference; additive across ports)

P0/P1: free.

P2: 0.02 credits/kB (first 5 MB/day free per colony, not per port).

P3: 0.05 credits/kB; standing micro-slots bill monthly.

P4: 0.01 off-peak / 0.03 peak credits/kB.

Port license surcharge: modest annual fee per extra port to discourage wasteful hoarding.

Typical v2 builds (examples)

Small colony ([[Austro Guard]]):

[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]× Sol ports (capacity + failover).

Optional 1× Regional (Proxima) for local arbitration overflow.

Arbitration hub ([[Proxima Commonwealth]]):

[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]× Sol + [[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]× Regional (Alpha Cen/Prox);

[[Time]]-boxed inter-colony pairs to litigants during active cases.

Trade node ([[United Authority of Systems]]):

[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]]× Sol for market feeds; small Regional port for nearby disputes.

Migration from v1 → v2 (playbook)

[[Key]] ceremony: CU-supervised multi-port keying (two-[[Man]] rule, sealed logs).

Policy binding: colony picks class floors and standing micro-slot contracts (if any).

Regional enrollment (optional): apply for a Regional Relay port; CU certifies after audit.

(If needed) Inter-colony license: request [[Time]]-boxed authorization; Sol issues capability tokens; schedule appears on public ledger.

Cutover: enable link-aggregation; publish new Daily Queue; monitor via public dashboards.

Failure Modes & resilience (what happens when things break)

Single-port failure: traffic instantly reflows; P0/P1 floors preserved.

Regional Relay outage: sessions reroute to Sol, with P3/P4 throttled as needed.

[[Key]] compromise suspected: instant token revocation; out-of-band courier delivers new seeds; audit publishes incident within 24h.
nd-spoke: Sol remains root-of-trust and switch-of-record. Even when a colony has other links, [[Colonial Union]] (CU) keys are required for any cross-colony session.

All sessions are still signed and versioned by Sol (periodic ledger sync).

Permissioned inter-colony pairs (rare, licensed):

Direct colony↔colony PFN pairs are allowed only with CU escrow keys.

Token gating: every session carries a Sol-minted capability token (scope: [[Origin]], destination, class, duration). Regional [[Relays]] and inter-colony pairs must verify it before passing traffic.

Two-[[Man]] rule for rekeying multi-port chassis; hardware pair integrity checks per session.

Chassis upgrade: install a PFN v2 multi-port chassis (hot-add bays).

## Details

## References


## Legacy Content

> Automated segregation run completed.
> Moved to Summary: 7 block(s).
> Moved to Details: 66 block(s).

PFN v2 — Multi-Link FTL Comms (Hub-Controlled Multihoming)
What changed vs PFN v1

From one link → many: each colony may operate multiple paired FTL links (“ports”) instead of a single pair.

Still hub-and-spoke: Sol remains root-of-trust and switch-of-record. Even when a colony has other links, [[Colonial Union]] (CU) keys are required for any cross-colony session.

Regional [[Relays]] allowed: CU certifies a few Regional [[Relays]] (e.g., Proxima, Epsilon Indi) to take overflow and local disputes, but they ultimately synchronize with Sol.

Topology (three approved Modes)
         [CU-Relay–Sol]  ← Root of trust & global scheduler
            /   |   \
         L1    L2    L3    (PFN trunks to certified Regional [[Relays]])
         |      \     \
 [Regional Relay] \    \___
    (Proxima)      \        \
                    \        \
                 [Colony A]  [Colony B] ... (each multi-homed)


Multi-home to Sol (mandatory baseline):

Each colony runs ≥[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]] PFN ports directly to CU-Relay–Sol.

Gives capacity + hot-failover without changing governance.

Regional [[Relays]] (optional, CU-certified):

CU may authorize Regional [[Relays]] for load-balancing and local cases.

[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Colonies]] can add ports to one or more Regional [[Relays]].

All sessions are still signed and versioned by Sol (periodic ledger sync).

Permissioned inter-colony pairs (rare, licensed):

Direct colony↔colony PFN pairs are allowed only with CU escrow keys.

Packets require a Sol attestation token; without it the link won’t carry user traffic.

Typical use: disaster mutual-aid, arbitration fast-paths, standards dissemination.

CU can [[Time]]-box the authorization and revoke instantly.

Capacity & Classes

Per-port bandwidth: narrowband (e.g., ~64 kbps sustained; era-configurable).

Aggregate: colony capacity = Σ(ports). PFN v2 supports link-aggregation and per-class minimums.

Priority classes (unchanged):

P0 Safety-of-Life (SoL) – preemptive, free

P1 [[Continuity]]/Public Safety – free

P2 Governance & Courts – subsidized

P3 Market/Finance – metered

P4 Routine/Personal – metered (cheapest)

New in v2: Per-class floor guarantees across all ports (e.g., P0+P1 reserve ≥30% aggregate at all times).

Routing & Control (how CU keeps the reins)

CRP (Colonial Relay Protocol): a lightweight control protocol (think BGP-lite) where:

[[New Readers Start Here/I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Interstellar/Colonies/Colonies]] announce which ports they have (to Sol and any Regional Relay).

Sol publishes slot calendars and class caps per port.

All cross-colony routes carry a Route-of-Record = Sol, even if the packet transits a Regional Relay.

Token gating: every session carries a Sol-minted capability token (scope: [[Origin]], destination, class, duration). Regional [[Relays]] and inter-colony pairs must verify it before passing traffic.

Loop & abuse prevention: route TTLs, signed ledgers, Merkle proofs for slot allocations, per-class rate governors on every port.

Scheduling (v2 refinements)

Proportional fair queuing across all active ports, not just one.

Burst windows for P2 (courts/arbitration) to keep legal matters timely.

Standing micro-slots (≤10% of aggregate) allowed for exchange ticks under P3—revocable on abuse.

Security & Privacy

End-to-end encryption permitted; headers ([[Origin]]/dest, class, byte counts, port) public for audit.

SoL anonymity still honored.

Two-[[Man]] rule for rekeying multi-port chassis; hardware pair integrity checks per session.

Regional [[Relays]] undergo the same quarterly independent audits as Sol.

Sanctions & Safeguards (what CU can do)

Per-port throttles (class-specific), port suspensions, or full embargo on P3/P4 while P0/P1 remain inviolate.

Escrow at Sol for disputed P2/P3 payloads.

Revocation of inter-colony authorizations with immediate tear-down.

Fees (reference; additive across ports)

P0/P1: free.

P2: 0.02 credits/kB (first 5 MB/day free per colony, not per port).

P3: 0.05 credits/kB; standing micro-slots bill monthly.

P4: 0.01 off-peak / 0.03 peak credits/kB.

Port license surcharge: modest annual fee per extra port to discourage wasteful hoarding.

Typical v2 builds (examples)

Small colony ([[Austro Guard]]):

[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]× Sol ports (capacity + failover).

Optional 1× Regional (Proxima) for local arbitration overflow.

Arbitration hub ([[Proxima Commonwealth]]):

[[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]× Sol + [[Chapter XXIX (Verse Concursus)|Chapter XXIX (Verse Concursus)]]× Regional (Alpha Cen/Prox);

[[Time]]-boxed inter-colony pairs to litigants during active cases.

Trade node ([[United Authority of Systems]]):

[[Chapter XXX (Munitum Age)|Chapter XXX (Munitum Age)]]× Sol for market feeds; small Regional port for nearby disputes.

Migration from v1 → v2 (playbook)

Chassis upgrade: install a PFN v2 multi-port chassis (hot-add bays).

[[Key]] ceremony: CU-supervised multi-port keying (two-[[Man]] rule, sealed logs).

Policy binding: colony picks class floors and standing micro-slot contracts (if any).

Regional enrollment (optional): apply for a Regional Relay port; CU certifies after audit.

(If needed) Inter-colony license: request [[Time]]-boxed authorization; Sol issues capability tokens; schedule appears on public ledger.

Cutover: enable link-aggregation; publish new Daily Queue; monitor via public dashboards.

Failure Modes & resilience (what happens when things break)

Single-port failure: traffic instantly reflows; P0/P1 floors preserved.

Regional Relay outage: sessions reroute to Sol, with P3/P4 throttled as needed.

[[Key]] compromise suspected: instant token revocation; out-of-band courier delivers new seeds; audit publishes incident within 24h.

---

> [!info] Original Vault Path
> `I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Technology/FTL/Multi-Link FTL Node.md`
