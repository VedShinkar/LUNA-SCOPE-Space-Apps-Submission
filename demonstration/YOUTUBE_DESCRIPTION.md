# LUNA-SCOPE — Lunar Landing Site Navigator 🌕
**NASA Space Apps Challenge 2026 | Team VayuTej**

How should we evaluate candidate landing regions near the lunar south pole? LUNA-SCOPE (Lunar Unified Navigation, Analysis & Site Optimization) brings terrain, celestial geometry and mission-level analysis into one interactive environment to help users explore and compare lunar south-polar landing-site candidates.

## What this demonstration covers

1. **Global Lunar Survey** — explore the Moon through an interactive 3D view and navigate toward the south-polar region.
2. **Landing-site navigation** — explore candidate regions: Shackleton Rim (Site 04), de Gerlache Rim (Site 11), and Malapert Massif (Site 23). Data coverage is not identical across regions.
3. **3D terrain analysis** — inspect Site 04 elevation-based relief and its terrain-analysis workspace.
4. **Terrain metrics** — explore elevation, slope, aspect, roughness, data-quality/uncertainty and preliminary hazard screening where available. Preliminary hazard screening is decision support, not certified landing safety.
5. **Solar access and Earth communication** — examine Sun position and illumination, Earth position, geometric and terrain-aware visibility, and potential operating windows. Solar analysis is preliminary, not a validated spacecraft power budget; geometric visibility does not guarantee a complete communications link.
6. **Mission intelligence and scenarios** — inspect mission profiles, equipment configurations, feasibility checks, weighted scenario comparisons and candidate-site assessments. Some illustrative assessments use synthetic fixtures; they are not NASA-derived rankings, validated landing probabilities or certified mission assessments.
7. **AI Mission Copilot concept** — the deck describes deterministic question routing, not a live LLM.

## Scientific data and technology

- NASA Lunar Orbiter Laser Altimeter (LOLA) regional elevation products.
- NASA/JPL SPICE via NAIF for celestial geometry.
- NASA/JPL Horizons for ephemeris queries and reference checks.
- Python, FastAPI, React, TypeScript and SpiceyPy.

## Project links

- Submission repository: https://github.com/VedShinkar/LUNA-SCOPE-Space-Apps-Submission
- Main source-code repository: https://github.com/VedShinkar/LUNA-SCOPE
- Scientific data sources: https://github.com/VedShinkar/LUNA-SCOPE-Space-Apps-Submission/blob/main/scientific-references/DATA-SOURCES.md

## Team VayuTej

Ved Shinkar · Anushka Jadhav · Mahathi Tippavajhula

LUNA-SCOPE is a research and hackathon prototype, not a certified landing-safety system.

#NASASpaceApps #LUNASCOPE #LunarExploration #SpaceTechnology #NASA #LunarSouthPole #SpaceResearch #TerrainAnalysis #AerospaceEngineering
