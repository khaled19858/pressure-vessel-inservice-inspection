# Changelog

All notable changes to this repository are documented in this file.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased]

### Added

#### Controlled templates

- `templates/damage-mechanism-review/api-571-damage-mechanism-review-template.md`
  API 571 damage mechanism review template for pressure vessels and
  pressure-boundary equipment. Covers document control, equipment
  identification, process and service description, materials of construction,
  operating conditions, process chemistry, damage mechanism screening table,
  credible and non-credible mechanisms, susceptibility factors, inspection
  history, inspection effectiveness, CML and UT evidence, NDE evidence,
  process chemistry evidence, active versus potential mechanisms, consequence
  notes, recommended inspection methods, recommended CML locations, mitigation
  and monitoring actions, FFS triggers, assumptions, limitations, and approval
  block.

- `templates/FFS/api-579-general-ffs-assessment-report-template.md`
  General fitness-for-service assessment report template per API
  579-1/ASME FFS-1. Covers document control, executive summary, equipment
  data, assessment scope, damage mechanism, assessment level selection,
  applicable Part selection (Parts 4 through 14), input data (design,
  operating, geometry, material, inspection readings, flaw dimensions),
  assumptions, required thickness basis, inspection data, structured
  calculation workflow (required thickness, damage characterization, remaining
  thickness, MAWP, remaining life), results table, sensitivity checks, MAWP
  impact, acceptability statement, limitations, recommendations, and approval
  block.

- `templates/FFS/ffs-assessment-input-data-sheet.md`
  Pre-assessment input data collection sheet for API 579-1/ASME FFS-1. Covers
  equipment identification, design data, operating data, material data,
  geometry, corrosion allowance and future corrosion allowance, UT inspection
  readings, flaw dimensions, NDE method and coverage, damage type
  classification, assessment temperature and pressure, weld details, toughness
  and cyclic service screening, missing data register, assumptions, and
  reviewer sign-off. Requires resolution of all missing data before assessment
  proceeds.

- `templates/inspection-plan/rbi-inspection-planning-template.md`
  Risk-based inspection planning template per API 580 and API 581. Covers
  document control, equipment list, process unit and service description,
  damage mechanism review summary, consequence screening (fluid hazard,
  inventory, personnel and environmental impact), likelihood screening
  (damage factor inputs and inspection effectiveness factor), risk ranking
  table, inspection history and open items, current inspection effectiveness
  assessment, recommended inspection strategy, CML strategy (existing and
  proposed CMLs), NDE method selection, inspection interval basis (remaining
  life, regulatory limits, safety factors), deferral and escalation triggers
  (including chemistry exceedance parameters), data quality notes, assumptions,
  limitations, and approval block.

- `templates/recommendations/inspection-recommendation-technical-note-template.md`
  Inspection recommendation and technical note template. Covers document
  control, background, issue statement, inspection finding (location,
  dimensions, NDE method, classification), technical basis (damage mechanism,
  corrosion rate and trend, required and retirement thickness, code basis),
  risk consideration (safety, environmental, production), options considered,
  recommended action, priority classification, due date basis, required
  shutdown or online action scope, follow-up inspection and interim monitoring,
  responsible party table, assumptions, limitations, approval block, and
  revision history.

---

## [v0.1.0] - 2026-06-20

### Initial controlled pressure vessel inspection workspace baseline

#### Repository structure

- Created top-level directory layout with placeholder `.gitkeep` files to
  establish the folder hierarchy under version control:
  - `admin/`
  - `calculations/` with sub-folders: `external-pressure/`, `hydrotest/`,
    `local-thin-area/`, `MAWP/`, `pitting-assessment/`, `pressure-vessel/`,
    `remaining-life/`
  - `examples/`
  - `references/`
  - `reports/` with sub-folders: `API-510/`, `FFS/`, `inspection/`,
    `recommendations/`
  - `standards/` with sub-folders: `API-510/`, `API-571/`, `API-572/`,
    `API-579/`, `API-580-581/`, `ASME-IX/`, `ASME-V/`, `ASME-VIII-1/`,
    `NACE/`, `NBIC/`
  - `templates/` with sub-folders: `calculation-checks/`, `CML-UT-mapping/`,
    `FFS/`, `inspection-plan/`
- Added `.gitignore` covering common operating-system, editor, and
  office-document artifact patterns.

#### Project governance

- Added `CLAUDE.md` defining the AI assistant role, governing standards
  (API 510, API 579-1/ASME FFS-1, ASME Section VIII Division 1, ASME
  Sections V and IX, API 571, API 572, API 576, API 577, API 578, API 580,
  API 581, NBIC, NACE MR0175/MR0103), calculation conventions, ASME VIII-1
  paragraph map for formed heads, static head rules, FFS assessment
  approach, CML/UT mapping guidance, and engineering report structure.

#### Documentation

- Added `README.md` with project description and a controlled template index
  table listing each template, its revision, and its location in the
  repository.

#### Controlled templates

- `templates/FFS/api-579-pitting-assessment-template.md`
  API 579-1/ASME FFS-1 pitting assessment template covering equipment data,
  damage description, Level 1 and Level 2 pitting assessment inputs,
  calculations, acceptability determination, limitations, and
  recommendations.

- `templates/inspection-plan/api-510-pressure-vessel-inspection-report-template.md`
  API 510 pressure vessel inspection report template covering executive
  summary, equipment data, inspection history, current inspection findings,
  damage mechanism review, code basis, MAWP/remaining-life calculations,
  acceptability statement, and inspection interval recommendation.

- `templates/calculation-checks/asme-viii-1-pressure-component-calculation-check-sheet.md`
  ASME Section VIII Division 1 pressure component calculation check sheet
  covering cylindrical shells, ellipsoidal heads, torispherical heads,
  hemispherical heads, conical sections, and flat heads, with input data
  tables, equation references, unit tracking, and acceptance criteria rows.

- `templates/CML-UT-mapping/cml-ut-thickness-mapping-template.md`
  CML and UT thickness mapping template covering CML location tables by
  component type (shell courses, heads, nozzles, piping), clock-position and
  axial/girth-band grids, damage-mechanism-based placement rationale, and
  thickness reading log format.

---

[Unreleased]: https://github.com/khaled19858/pressure-vessel-inservice-inspection/compare/v0.1.0...HEAD
[v0.1.0]: https://github.com/khaled19858/pressure-vessel-inservice-inspection/releases/tag/v0.1.0

