# DACS Research Explorer

An interactive, searchable overview of the research of the faculty of the
[Department of Advanced Computing Sciences (DACS)](https://www.maastrichtuniversity.nl/research/department-advanced-computing-sciences)
at Maastricht University.

**Live site:** https://maastrichtu-ids.github.io/dacs-research-explorer/

## What it shows

- **People** — every faculty member with a short research overview, career publication metrics and their most-cited works
- **Research clusters** — seven methodology clusters: Physical Intelligence; Security, Privacy & Distributed Systems;
  Computing Paradigms; Learning, Reasoning & Discovery; Responsible Data Science; Human-centered AI;
  Mathematical & Decision Sciences
- **Application areas** — cross-cutting tags: Health & Life Sciences; Planetary Health & Sustainability;
  Education & Learning; Law, Governance & Policy; Industry, Agri-Food & Logistics
- **Clusters × applications matrix**, a publication browser and department-level trends

## Data and method

- **Roster:** the *Faculty* section of the department's public staff page (November 2026).
- **Publications and topics:** [OpenAlex](https://openalex.org) (CC0). Each person was matched to an OpenAlex author record
  by surname and Maastricht University affiliation, then checked against initials, topics and institution.
- **Placement:** each person's OpenAlex topic profile is scored against keyword definitions for every cluster and
  application area; the highest-scoring cluster is primary, and an application tag applies at ≥15% of topic weight.
  A small number of placements are set by hand and flagged in the interface.
- **Research overviews** summarise each person's publication record and may not reflect current or unpublished work.

Metrics are indicative, not evaluative. Author disambiguation in OpenAlex is automated and can merge or split records;
known issues are flagged on the affected profiles. Corrections are welcome via issues or pull requests.

## Files

| Path | Contents |
|---|---|
| `index.html` | The self-contained site, with the full dataset embedded (no build step, no external dependencies) |
| `data/roster.tsv` | Roster with the matched OpenAlex author IDs |
| `data/narratives.json` | The per-person research overviews |
