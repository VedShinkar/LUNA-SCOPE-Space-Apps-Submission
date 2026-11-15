# Project overview

## Problem

A lunar landing location must be evaluated against multiple interacting constraints. At the lunar south pole, terrain geometry, long and changing shadows, access to sunlight, and line-of-sight communication with Earth can all influence mission operations.

A map or a single terrain metric cannot answer the full site-selection question. Mission planners need to examine the local surface and the time-varying geometry of the Sun and Earth together.

## Proposed solution

LUNA-SCOPE is an interactive lunar landing-site exploration and decision-support application. It combines:

- Lunar terrain visualization and derived terrain-analysis layers.
- Solar position and terrain-aware illumination analysis.
- Earth visibility and communication geometry.
- Mission timeline simulation.
- Candidate-site comparison and configurable mission assessment.

The aim is to help users understand trade-offs and investigate candidate landing regions through a single workflow.

## Current candidate regions

The current application configuration identifies three candidate areas:

| Site ID | Region |
|---|---|
| Site04 | Shackleton |
| Site11 | de Gerlache |
| Site23 | Malapert |

High-resolution LOLA terrain inspection evidence is specifically documented for Site04. Coverage and confidence should be checked per layer and per site in the source repository.

## Intended workflow

1. Choose a candidate region.
2. Inspect terrain and derived hazard indicators.
3. Evaluate local solar illumination and Sun geometry.
4. Evaluate Earth visibility and communication opportunities.
5. Examine changes over a mission timeline.
6. Compare candidate regions and review the resulting decision-support assessment.

## Intended users

The system is intended for educational, exploratory, and early-stage mission-planning analysis by students, researchers, and teams investigating lunar surface operations.

## Scope boundary

LUNA-SCOPE is a research prototype and decision-support tool. It does not replace mission certification, detailed engineering analysis, operational ephemeris validation, or human review by qualified lunar mission specialists.
