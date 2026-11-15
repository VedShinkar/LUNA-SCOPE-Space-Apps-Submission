# LUNA-SCOPE — Lunar Landing Site Navigator

**NASA Space Apps Challenge 2026 | Project submission**

LUNA-SCOPE is a lunar landing-site analysis and decision-support application designed to help evaluate candidate locations near the lunar south pole. It brings terrain context, solar illumination, Earth visibility, mission timelines, and comparative assessment into a single exploration workflow.

> This repository is the public-facing **submission hub** for judges and reviewers. The application source code remains in the main project repository: [VedShinkar/LUNA-SCOPE](https://github.com/VedShinkar/LUNA-SCOPE).

## Judge quick links

| Submission item | Link |
|---|---|
| **Demonstration video** | [Watch the LUNA-SCOPE demo on YouTube](https://youtu.be/1WInFyLfS4M) |
| **Project presentation** | _PPT/PDF will be added here_ |
| Application source code | [LUNA-SCOPE source repository](https://github.com/VedShinkar/LUNA-SCOPE) |
| Technical overview | [Project overview](documentation/PROJECT-OVERVIEW.md) |
| System architecture | [System architecture](documentation/SYSTEM-ARCHITECTURE.md) |
| Technical highlights | [Technical highlights](documentation/TECHNICAL-HIGHLIGHTS.md) |
| Scientific data provenance | [Data sources and references](scientific-references/DATA-SOURCES.md) |

## What LUNA-SCOPE does

Lunar landing-site selection is a multi-factor problem. A candidate site needs terrain that can support a safe landing and surface operations, useful periods of sunlight for power, and viable communication opportunities with Earth.

LUNA-SCOPE organizes these questions into a connected workflow:

1. **Explore candidate regions** using lunar terrain context and elevation-derived analysis.
2. **Inspect terrain conditions** through slope, aspect, roughness, hazard, and uncertainty layers where available.
3. **Evaluate solar geometry** and local illumination, including terrain-horizon effects.
4. **Evaluate Earth visibility** and communication opportunities, including antenna elevation constraints.
5. **Review mission timelines** to understand how environmental conditions change over time.
6. **Compare candidate sites** and assess mission suitability using configurable criteria.

## Candidate sites represented in the current application

The application configuration and technical verification records identify these candidate areas:

- **Shackleton region** — Site04
- **de Gerlache region** — Site11
- **Malapert region** — Site23

The current terrain inspection and high-resolution LOLA processing evidence specifically documents Site04. Do not interpret every layer or numerical result as equally validated across all sites; consult the technical documentation and source repository for dataset details.

## Application screenshots

Selected interface screenshots will be placed in [assets/screenshots](assets/screenshots/README.md). The gallery documentation identifies the recommended order and content.

## Scientific integrity and limitations

- NASA LOLA terrain products are used for the documented terrain workflow. Dataset products and processing details are listed in [DATA-SOURCES.md](scientific-references/DATA-SOURCES.md).
- The celestial geometry subsystem uses NASA/JPL NAIF SPICE kernels and is designed with Horizons comparison/validation support.
- Offline synthetic fixtures and test data are not NASA observations. They must be labelled as synthetic wherever shown.
- Horizons comparison tests or a benchmark catalogue do not, by themselves, establish that a live NASA Horizons capture has been completed.
- Mission-scoring outputs depend on configured criteria, thresholds, and available input data. They are decision-support aids, not certified landing-safety determinations.
- Browser-level manual verification and the current status of optional Copilot functionality must be checked against the latest source repository before being claimed as completed.

See [Technical highlights](documentation/TECHNICAL-HIGHLIGHTS.md) for a status-aware description.

## Team

LUNA-SCOPE is developed by a three-member team:

- Ved Shinkar
- Anushka
- Mahati

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

For implementation details, setup instructions, code, tests, and ongoing development, visit:

**[https://github.com/VedShinkar/LUNA-SCOPE](https://github.com/VedShinkar/LUNA-SCOPE)**

---

*The demonstration video is published on YouTube. The final presentation files will be added to `presentation/`.*
