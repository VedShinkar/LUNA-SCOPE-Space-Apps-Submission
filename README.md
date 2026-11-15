# LUNA-SCOPE — Lunar Landing Site Navigator

**NASA Space Apps Challenge 2026 | Team VayuTej**

LUNA-SCOPE (Lunar Unified Navigation, Analysis & Site Optimization) is an interactive lunar exploration and decision-support platform designed to help users explore and compare lunar south-polar landing-site candidates. It brings terrain, celestial geometry and mission-level analysis into one environment.

> This public repository is the submission hub for judges and reviewers. The application source code remains in the main project repository: [VedShinkar/LUNA-SCOPE](https://github.com/VedShinkar/LUNA-SCOPE).

## Judge quick links

| Submission item | Link / status |
|---|---|
| **Demonstration video** | [Watch LUNA-SCOPE on YouTube](https://youtu.be/1WInFyLfS4M) |
| **Project presentation** | Final 7-page PDF and editable PowerPoint prepared; binary upload to this repository is pending |
| Application source code | [LUNA-SCOPE source repository](https://github.com/VedShinkar/LUNA-SCOPE) |
| Technical overview | [Project overview](documentation/PROJECT-OVERVIEW.md) |
| System architecture | [System architecture](documentation/SYSTEM-ARCHITECTURE.md) |
| Technical highlights | [Technical highlights](documentation/TECHNICAL-HIGHLIGHTS.md) |
| Scientific data provenance | [Data sources and references](scientific-references/DATA-SOURCES.md) |
| YouTube description | [Demonstration page](demonstration/README.md) |

## The problem

Choosing a lunar landing site is more than finding flat ground. Four factors interact, and they change with location and time:

1. **Terrain** — elevation, slope, roughness and preliminary hazards.
2. **Solar access** — when sunlight may reach a candidate site.
3. **Earth communication** — where Earth sits, and when it may be seen.
4. **Mission feasibility** — mission profiles and equipment assumptions.

## LUNA-SCOPE workflow

1. Select a lunar candidate site.
2. Explore the terrain using 3D relief and terrain-analysis layers.
3. Analyze Sun and Earth geometry relative to the local horizon.
4. Examine operational windows with solar illumination, Earth visibility and operations timeline views.
5. Compare mission scenarios using Mission Intelligence and scenario comparison.

## Candidate regions

| Candidate region | Site ID |
|---|---|
| Shackleton Rim | Site 04 |
| de Gerlache Rim | Site 11 |
| Malapert Massif | Site 23 |

**Data coverage is not identical across regions.** The high-resolution terrain inspection evidence is specifically documented for Site 04 (Shackleton Rim); consult the source repository and data catalogue for per-region coverage.

## Scientific data and technology

- NASA Lunar Orbiter Laser Altimeter (LOLA) regional elevation products.
- NASA/JPL SPICE via NAIF for celestial geometry.
- NASA/JPL Horizons for ephemeris queries and reference checks.
- Python, FastAPI, React, TypeScript and SpiceyPy.

The project distinguishes source NASA products, locally processed data, synthetic test fixtures and modelled outputs. Some illustrative mission assessments use synthetic fixtures; these are not NASA-derived rankings, validated landing probabilities or certified mission assessments.

## Application screenshots

The gallery index and target file names are documented in [assets/screenshots](assets/screenshots/README.md). The original screenshots and the YouTube thumbnail are also included in the downloadable [submission media bundle](https://github.com/VedShinkar/LUNA-SCOPE-Space-Apps-Submission) once the binary assets have been committed.

## Team VayuTej

- Ved Shinkar
- Anushka Jadhav
- Mahathi Tippavajhula

## Repository contents

```text
.
├── README.md
├── presentation/
│   └── README.md
├── demonstration/
│   └── README.md
├── scientific-references/
│   └── DATA-SOURCES.md
├── documentation/
│   ├── PROJECT-OVERVIEW.md
│   ├── SYSTEM-ARCHITECTURE.md
│   └── TECHNICAL-HIGHLIGHTS.md
└── assets/
    └── screenshots/
        └── README.md
```

## Main source repository

For implementation details, code, tests and development history, visit:

**[https://github.com/VedShinkar/LUNA-SCOPE](https://github.com/VedShinkar/LUNA-SCOPE)**

---

*The demo is published on YouTube. The final PDF, PowerPoint, application screenshots and YouTube thumbnail are prepared in the submission media bundle; their binary upload to this repository remains pending.*
