---
title: "Generated Stub Cleanup Report - 2026-06-19"
tags:
  - canon
  - archive-infrastructure
  - tier-1
  - archive-management
Status: CANON
Category: Archive Infrastructure
Complexity: Tier 1
Prerequisites:
  - "[[Archive Index]]"
Related Notes:
  - "[[Missing Notes Recovery Index]]"
  - "[[Retained Generated Stubs - Public Link Review]]"
Recommended Reading:
  - "[[Archive and Canon FAQ]]"
  - "[[Retained Generated Stubs - Public Link Review]]"
Last Reviewed: 2026-06-19
---
# Generated Stub Cleanup Report - 2026-06-19

## Purpose Summary

This cleanup reduced bloat created by automated missing-note recovery. The recovery pass had correctly prevented broken note links, but many generated stubs represented glossary placeholders, common words, table fragments, or malformed import text rather than real canon concepts.

## Cleanup Rule

A generated stub was removed when it had no non-glossary public lore links. Its incoming links were converted back into plain readable text before deletion.

A generated stub was retained when at least one real lore or reader-facing page still links to it. Retained stubs require manual review before promotion, redirect, merge, or deletion.

## Results

| Measure | Count |
| --- | ---: |
| Generated stubs before cleanup | 6164 |
| Generated stubs removed | 6082 |
| Generated stubs retained for review | 82 |
| Markdown files modified | 28 |
| Stub links converted to plain text | 6377 |
| Generated stubs remaining | 82 |

## Removed Stub Buckets

| Bucket | Removed |
| --- | ---: |
| glossary generic single word removed | 83 |
| glossary malformed fragment removed | 52 |
| glossary only possible term removed | 5792 |
| glossary table artifact removed | 43 |
| orphan malformed fragment removed | 88 |
| orphan management only removed | 23 |

## Verification

| Check | Result |
| --- | ---: |
| Markdown notes after cleanup | 3048 |
| Missing note targets | 0 |
| Missing note link occurrences | 0 |
| Malformed wiki-link occurrences | 0 |
| Notes missing required metadata | 0 |
| Missing attachment targets | 409 |
| Missing attachment occurrences | 952 |

## Retained Public-Linked Stubs

The retained stubs are listed in [[Retained Generated Stubs - Public Link Review]]. These should be reviewed as actual editorial decisions, not bulk-deleted.

| Retained Stub | Public Links | Review Bucket | Sample Sources |
| --- | ---: | --- | --- |
| Dominion Omniverse | 28 | public linked retained | I - Pleroma Archive/Structure/Economy & Infrastructure/Megastructures/2 Astronomical/Substellar Compressor.md<br>I - Pleroma Archive/Structure/Economy & Infrastructure/Megastructures/3 Stellar/Celestial Printer.md |
| Independent | 21 | public linked retained | I - Pleroma Archive/Structure/Science/Species/Ameise/Ameise.md<br>I - Pleroma Archive/Structure/Science/Species/Haldra/Haldra.md |
| MOT_Physics | 8 | public linked retained | I - Pleroma Archive/Structure/Science/Exotic Matter/Aether.md<br>I - Pleroma Archive/Structure/Science/Physics/MOT/MOT_Advanced_Systems.md |
| Aether_Field_Guide | 6 | public linked retained | I - Pleroma Archive/Structure/Science/Physics/Methods/Symbols_Legend.md<br>I - Pleroma Archive/Structure/Science/Physics/MOT/MOT.md |
| Vitality Magic – Blood Magic | 6 | public linked retained | III - Arcanum Omniversalis/Interfaces of Magic.md<br>III - Arcanum Omniversalis/Taxonomy.md |
| Particles_and_Fields_Registry | 5 | public linked retained | I - Pleroma Archive/Structure/Science/Exotic Matter/Aether.md<br>I - Pleroma Archive/Structure/Science/Physics/MOT/MOT.md |
| Federal Branch | 4 | public linked retained | I - Pleroma Archive/World/Civilizations/Dominion/Doctrine/Continuity Code.md<br>I - Pleroma Archive/World/Civilizations/Dominion/Government/Dominion Institutions.md |
| Immutable Pattern | 4 | public linked retained | I - Pleroma Archive/Structure/Science/Cosmic Phenomenon/Structures Hub.md<br>I - Pleroma Archive/Structure/Science/Physics/Verse Field Framework Hub.md |
| Tempus Profundus | 4 | public linked retained | I - Pleroma Archive/World/Historical Eras/VI - Severance Era (Akasha)/Conditional Eternalism.md |
| Consent_Key_Log_Template | 3 | public linked retained | I - Pleroma Archive/Structure/Science/Physics/Methods/Math_and_Methods.md<br>I - Pleroma Archive/Structure/Science/Physics/MOT/MOT_Mind_Systems.md |
| Cosmology Index | 3 | public linked retained | I - Pleroma Archive/Structure/Science/Cosmic Phenomenon/Stars/Stars.md |
| Dracosian Gateway | 3 | public linked retained | I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Ho'oleilana/Boötes Supercluster/Odysseus Galaxy/Systems/Carneliam System.md |
| Legio Praetoria | 3 | public linked retained | I - Pleroma Archive/World/Civilizations/Dominion/Military/Royal Military/Legions/Verarch/Aurelion Custivar.md |
| Lozenge-class World Stations | 3 | public linked retained | I - Pleroma Archive/Structure/Economy & Infrastructure/Megastructures/2 Astronomical/Megastructures Hub.md<br>I - Pleroma Archive/World/Civilizations/Dominion/Military/Orders & Commands/Intergalactic Warfare.md |
| Particles Index | 3 | public linked retained | I - Pleroma Archive/Structure/Science/Physics/Particles/Particles.md |
| The Cosmic City | 3 | public linked retained | I - Pleroma Archive/World/Civilizations/Zek'razzar Veyrth/Locations/Zar'astor Urth.md |
| unnamed ([[Chapter XXIX (Verse Concursus) | 3 | public malformed fragment retained | I - Pleroma Archive/Characters/Dominion/Amber Andreia Zohair/Amber Andreia Zohair.md<br>I - Pleroma Archive/World/Civilizations/Dominion/Locations/Velorum R-9.md |
| VFF MOT Index | 3 | public linked retained | I - Pleroma Archive/I - Pleroma Archive.md |
| Workshop | 3 | public linked retained | I - Pleroma Archive/Structure/Economy & Infrastructure/Megastructures/2 Astronomical/Demiurge Forge.md |
| Aether Tables | 2 | public linked retained | I - Pleroma Archive/World/Locations/Eos Multiverse/The Aphotic Zone/Concordia/Concordia Master Summary.md |
| Archive Gate Authority | 2 | public linked retained | I - Pleroma Archive/World/Civilizations/Galactic Federation/Government/Leaders.md |
| Aurathene | 2 | public linked retained | I - Pleroma Archive/Structure/Science/Species/Symmorph/Symmorph.md |
| Black Holes | 2 | public linked retained | I - Pleroma Archive/Structure/Science/Cosmic Phenomenon/Stars/Stars Hub.md |
| Boson Star Clusters | 2 | public linked retained | I - Pleroma Archive/Structure/Science/Cosmic Phenomenon/Cosmic Phenomena Hub.md |
| Church Register | 2 | public linked retained | I - Pleroma Archive/World/Locations/Eos Multiverse/The Aphotic Zone/Concordia/Concordia Master Summary.md |
| Confluencia Tethers | 2 | public linked retained | I - Pleroma Archive/Structure/Science/Physics/Verse Field Framework Hub.md |
| Cryonics | 2 | public linked retained | I - Pleroma Archive/World/Locations/Eos Multiverse/The Dark Forest Zone/Local Cluster/Totum/Verse Structure/Superclusters/Laniakea/Milky Way Galaxy/Sol System/Earth (Terra)/2079-4000/Colonial Union/Technology/Tools/Human Cryonics.md |
| Dyson Swarm | 2 | public linked retained | I - Pleroma Archive/Structure/Economy & Infrastructure/Megastructures/2 Astronomical/Megastructures Hub.md |
| Elemental Aether Table | 2 | public linked retained | I - Pleroma Archive/World/Locations/Eos Multiverse/The Aphotic Zone/Concordia/Concordia Master Summary.md |
| Frayzones | 2 | public linked retained | I - Pleroma Archive/Structure/Science/Cosmic Phenomenon/Structures Hub.md |

## Editorial Recommendation

Most generated recovery stubs should not become public archive notes. A term deserves a note only when it is a canon concept, being, civilization, place, technology, doctrine, material, event, or recurring system. Common words and glossary table fragments should remain glossary text until canon material exists.

## Backup Location

Backups for deleted stubs and modified Markdown files are stored under:

`.codex-vault-backups/2026-06-19-generated-stub-cleanup`

## Machine Manifest

Detailed machine-readable cleanup data is stored at:

`generated-stub-cleanup-manifest.json`


## Final Verification File

`post-generated-stub-cleanup-verification.json`

---

> [!info] Original Vault Path
> `I - Pleroma Archive/_Pleroma Archive Management/Missing Note Recovery/Generated Stub Cleanup Report - 2026-06-19.md`
