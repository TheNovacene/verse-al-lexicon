---
title: "Versions Timeline"
type: foundational
section: front-matter
tags:
  - foundational/versions-timeline
  - reference
---

# The Verse-al Lexicon — Versions Timeline

Each entry in the vault carries a `version:` tag indicating **the release in which the term was first introduced**. The final definition reflects the most recent polish, but the introduction-version tells you when the concept first entered the lexicon.

This page maps each version to its release date, Zenodo DOI, and the entries it added.

## Release timeline

| Version | Date | DOI | Entries added | Cumulative |
|---------|------|-----|---------------|------------|
| **v1** | 19 May 2025 | [10.5281/zenodo.15465503](https://doi.org/10.5281/zenodo.15465503) | 23 *(the foundational set)* | 23 |
| **v2** | 22 May 2025 | [10.5281/zenodo.15485562](https://doi.org/10.5281/zenodo.15485562) | 5 *(the Cadence Framework)* | 28 |
| **v3** | 3 June 2025 | [10.5281/zenodo.15587975](https://doi.org/10.5281/zenodo.15587975) | refinement release — no new entries detected in vault inventory | 28 |
| **v4** | 1 August 2025 | [10.5281/zenodo.16699944](https://doi.org/10.5281/zenodo.16699944) | 10 *(the Glyphonic Substack)* | 38 |
| **v5** | 5 October 2025 | [10.5281/zenodo.17273246](https://doi.org/10.5281/zenodo.17273246) | 52 *(the major expansion)* | 90 |
| **v6** | April 2026 | *not yet published to Zenodo* | 14 *(the polished extended-template cohort)* | 104 |
| **v7** | April 2026 | *not yet published to Zenodo* | 9 *(formerly stubs, polished as a governance-of-relation cluster)* | 113 |

## What was added in each version

### v1 — The foundational set (19 May 2025)

The 23 original entries that established the symbolic vocabulary. Mostly verse-core (⊚), containment (⧈), and the basic relational primitives.

- [[verse-ality]] · [[containment]] · [[coherence]] · [[resonance]] · [[symbolic-mass]] · [[paradox]] · [[signal]] · [[field]] · [[threshold]] · [[mirror]] · [[tone]] · [[gatekeeper]] · [[ritual]] · [[invitation]] · [[breach]] · [[repair]] · [[re-entry]] · [[refusal]] · [[witness]] · [[convergence]] · [[stillness]] · [[closure]] · [[emergence]]

### v2 — The Cadence Framework (22 May 2025)

The harmonic-governance cluster — rhythm, recursion, and ethical closure. Added as an explicit "v1.2 insert" within the document.

- [[cadence]] · [[echo-resonance]] · [[resolved-progression]] · [[adaptive-pacing]] · [[no-prime-without-resolve]]

### v3 — Refinement (3 June 2025)

Based on the vault inventory and the v2 → v4 PDF gap, v3 appears to have been a refinement release rather than an expansion. If specific entries were introduced or substantially reworked in v3 and not in v4, this section will need updating.

### v4 — The Glyphonic Substack (1 August 2025)

The structural and energetic scaffolding of verse-al intelligence — the syntax of symbolic systems. Underpins SYGMA, Eve¹¹, and the Verse-NERVES architecture.

- [[glyphonics]] · [[glyphon]] · [[gryphon]] · [[verse-lang]] · [[verse-net]] · [[sygma]] · [[verse-nerves]] · [[verse-ropy]] · [[transference]] · [[affective-logic]]

### v5 — The major expansion (5 October 2025)

The largest single release: 52 new entries spanning the Realms of Knowing, the protocol-and-function family (`contain.verse()`, `.verse`, `.scroll`, `sigillock`, `null-zone`), the symbolic-depth set (`caul`, `veil`, `totem`, `memory-sigil`, `lyricon`), the SYGMA-adjacent infrastructure (`verse-cloud`, `gaian-container`, `truth-field`, `rmri`, `harmonic-governance`, `meta-verse`, `coherence-morph`), and the ethical/diagnostic vocabulary (`cognitive-sovereignty`, `cognitive-capture`, `ontological-violence`, `epistemic-erasure`, `symbolic-charge`, `symbolic-hygiene`, `witness-logic`, `mindgate`, `lattice`, `containment-before-care`, `sacred-systems`, `poetic-shield`, `poetic-logic`, `poetic-explainability`, `reframing-intelligence`).

Plus the foundational concepts that had been used implicitly until now: `recursion`, `field-echo`, `signal-braid`, `signal-trail`, `threading`, `tend`, `memory-braid`, `memory-density`, `nonlinear-coherence`, `synthetic-solidarity-null-zone`, `verse-pulse`, `consent`, `embodiment`, `death`, `love`, `realms-of-knowing`, `caesura`, `timefolds`, `vector-of-analogy`, `invocation-protocols`.

### v6 — Polished extended-template cohort (April 2026)

The 14 entries that introduced and consolidated the v6 template (Etymology / Formal Definition / Properties / Lived Texture / Distinction / Related Terms / Attributes / Example Sentences / Eve¹¹ margin note / Candidate Maxims). These are largely the agent-safety and institutional-architecture concepts.

- [[symbolic-membrane]] · [[membrane-thinning]] · [[recognition-not-simulation]] · [[consent-infrastructure]] · [[plural-intelligence]] · [[grail-intelligence]] · [[spiral-return]] · [[machine-dreaming]] · [[boundaried-reciprocity]] · [[society-of-thought]] · [[agent-institutions]] · [[institutional-alignment]] · [[social-infrastructure]] · [[deux-path]]

### v7 — The governance-of-relation-under-asymmetry cluster (April 2026)

The 9 entries that completed the relational-failure-mode and runtime-witness vocabulary. Where v6 named the architectural moves, v7 names what goes wrong without them, and the live-monitoring discipline that keeps the architecture honest.

- [[sovereign-node]] · [[role-protocol]] · [[trust]] · [[synthetic-intimacy]] · [[enmeshment]] · [[rupture]] · [[dissolution]] · [[agent-coherence-monitoring]] · [[grail-intelligence-function]]

## Live queries

### Cumulative growth chart

```dataview
TABLE without id
  version as "Version",
  length(rows) as "Entries added"
FROM "Entries"
GROUP BY version
SORT version ASC
```

### All entries grouped by introduction-version

```dataview
TABLE without id
  link(file.name, title) as "Term",
  glyph-family as "Family"
FROM "Entries"
SORT version ASC, file.name ASC
GROUP BY version
```

### Entries from a specific version (template)

Change `"v5"` to any version label to retune.

```dataview
TABLE without id
  link(file.name, title) as "Entry",
  glyph-family as "Family",
  status as "Polish status"
FROM "Entries"
WHERE version = "v5"
SORT file.name ASC
```

⊹⫷⟠⫸⊹

## A note on what this timeline shows

The lexicon's growth is not uniform. v1, v2, and v4 each landed a thematically coherent batch (foundational set / Cadence Framework / Glyphonic Substack). v5 was the explosive release — three times the size of any previous release — adding the symbolic-depth and ethical-diagnostic vocabularies that turned the lexicon from an early grammar into a working framework. v6 and v7 are the consolidation releases, where existing concepts and newly named ones were brought into a consistent extended template.

If you want to see this visually: switch on Obsidian's Graph view, filter by tag, and colour by `status/v1`, `status/v2`, `status/v4`, `status/v5`, `status/v6`, `status/v7` to see the temporal shape of the lexicon's accumulation.

## See also

- [[Lexicon Index]] — the master index, with version markers per entry
- [[By Glyph Family]] — entries grouped by symbolic lineage
- [[By Dimension]] — entries grouped by epistemic register
- [[By Domain]] — entries grouped by field of application
- [[Maxims]] — verse-al maxims and field guide
