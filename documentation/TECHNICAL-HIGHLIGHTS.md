# Technical highlights

This page summarizes the engineering approach and the verification evidence currently recorded for LUNA-SCOPE. It deliberately separates implemented/tested capabilities from items that still require live or manual verification.

## Terrain processing

- NASA LOLA terrain products are used for the documented terrain-analysis workflow.
- The Site04 Shackleton-region bundle includes surface elevation, slope, and associated uncertainty/derived products.
- The inspected Site04 rasters are 3,200 × 3,200 pixels at 5 m per pixel (approximately 16 km × 16 km).
- The broader terrain workflow includes derived terrain layers such as slope, aspect, roughness, hazards, and uncertainty where corresponding data are available.

## Celestial geometry

- The application includes a celestial geometry subsystem using NAIF SPICE kernels.
- The project includes a Horizons comparison/validation subsystem and an offline benchmark catalogue.
- A recorded validation run reports 25/25 benchmark catalogue cases passing locally.
- Project notes explicitly distinguish offline validation fixtures from live Horizons capture. A passing offline test must not be presented as proof of a completed live capture.

## Solar illumination

- Solar analysis combines Sun geometry with local terrain context.
- The point-illumination workflow includes ray-based terrain-horizon analysis rather than relying only on a flat-horizon approximation.
- Interpretation depends on the selected site, observer location, time interval, terrain model, and the assumptions configured in the analysis.

## Earth visibility and communications

- The communication workflow evaluates Earth visibility from a local lunar observer.
- Antenna minimum-elevation requirements are represented as a mission/configuration constraint.
- Geometric visibility should not be confused with a complete end-to-end communications link budget; RF performance, hardware, and operational constraints require separate analysis.

## Mission timeline and decision support

- The timeline subsystem generates time-sampled environmental/mission outputs; project verification notes describe a 25-sample timeline workflow.
- The mission assessment subsystem uses configurable criteria and weights, including terrain slope, terrain roughness, illumination, and communication availability.
- Assessment results should be interpreted as decision-support outputs whose ranking depends on the selected weights, thresholds, equipment configuration, and input availability.

## Automated verification recorded in project notes

A project verification report records:

- Backend API smoke checks returning successful responses for core terrain, celestial, illumination, communication, and timeline routes.
- A frontend production build completing successfully.
- 25 frontend unit tests passing in one recorded test run.
- 216 backend tests passing in a separate recorded test run.
- 25/25 local Horizons benchmark catalogue cases passing.

These figures are snapshots from recorded project runs, not a guarantee about the current state of every branch or the latest commit. Re-run tests against the submission commit before relying on them as current release status.

## Known scope and verification limits

- A full manual browser workflow was not confirmed by the cited headless verification report.
- The Horizons subsystem was described as pilot-ready pending an authorized live capture; do not claim a completed live NASA Horizons pilot unless a later verified run exists.
- A verification snapshot dated November 15, 2026 described the AI Copilot as a stub/not implemented at that point. Confirm the current main branch before describing it as a working feature.
- Synthetic test fixtures must remain clearly labelled as synthetic.
