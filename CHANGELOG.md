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

## [v0.2.0] - 2026-06-28

Integrity-hardening release. Closes a code-correctness gap (UG-16(b) minimum
thickness), adds a reference/convention layer and a fully worked example, adds an
MDMT screening template, and flags edition-dependent FFS constants for
verification. No fabricated clause numbers, formulas, allowable stresses, or
acceptance constants were introduced; values that must come from the code are left
as fields or hold points with read-from-code pointers.

### Added

#### Controlled reference documents

- `references/symbols-and-conventions.md`
  Single source of truth for symbol definitions, sign conventions, and units used
  across all templates. Establishes that `t_req` always means the governing
  required thickness, not the pressure value alone.

- `references/minimum-thickness-governing-logic.md`
  Defines the governing required thickness as `max(t_pressure, t_UG16b, t_struct)`
  and documents the ASME VIII-1 UG-16(b) minimum-thickness floor (1.5 mm / 1/16 in.
  exclusive of corrosion allowance), including its exclusions and service-specific
  provisions to be read from the controlling edition.

- `references/corrosion-rate-and-interval-conventions.md`
  Defines short-term and long-term corrosion-rate formulas, governing-rate
  selection, remaining life, and the API 510 interval basis (lesser of half
  remaining life or the prescriptive maximum), with edition-dependent limits
  flagged for verification.

- `references/input-data-schema.md`
  Optional YAML front-matter input convention so inputs are declared once with
  unit and source, plus validation rules and hold-point handling before any
  calculation proceeds.

- `references/damage-mechanism-quick-screen.md`
  Service-to-mechanism screening aid to support the API 571 damage mechanism
  review. Explicitly a screening aid only; every flagged mechanism is to be
  confirmed against API 571.

#### Controlled templates

- `templates/calculation-checks/ucs-66-mdmt-screening-template.md`
  MDMT / impact-test exemption screening worksheet per ASME VIII-1 UCS-66,
  UCS-66.1, UCS-68(c), UG-20(f), and UG-84. Provides the procedure and fields
  only; curve assignments, figure values, and temperature reductions are read
  from the controlling edition and never entered from memory.

#### Worked example

- `examples/worked-example-vertical-vessel-mawp-remaining-life.md`
  End-to-end worked example (vertical vessel, 2:1 ellipsoidal head) demonstrating
  corroded geometry, the UG-16(b) governing-thickness check, circumferential and
  longitudinal shell checks, governing MAWP, UG-99(b) hydrotest pressure, and
  remaining life with the half-life interval basis. All arithmetic verified. The
  allowable stress used is labeled as illustrative and is not a code lookup.

#### Governance and tooling

- `CONTRIBUTING.md`
  Document-control rules, revision/status convention, branch and pull-request
  workflow, and the technical-accuracy review checklist.

- `.github/pull_request_template.md`
  Pull-request template with a required technical-accuracy checklist.

### Changed

- `CLAUDE.md`
  Added governing rules for: the UG-16(b) minimum-thickness floor and governing
  required thickness; restriction of the simplified UG-32(c) formula to 2:1
  ellipsoidal heads (Appendix 1-4(c) otherwise); UG-99(b) hydrotest using the
  lowest stress ratio across all materials with the multiplier flagged as
  edition-dependent; MDMT/UCS-66 screening instead of silently skipping toughness;
  treating API 579 numeric screening constants as edition-dependent and verifying
  them; and a rounding / significant-figures convention. Added cross-references to
  the new `references/` documents. All original content preserved.

- `templates/calculation-checks/asme-viii-1-pressure-component-calculation-check-sheet.md`
  Added Section 7A (Minimum Thickness Floor and Governing Required Thickness,
  UG-16(b)); updated the shell and each head/cone section to report the governing
  required thickness as `max(t_pressure, t_UG16b, t_struct)`; restricted the
  simplified UG-32(c) ellipsoidal formula to 2:1 heads; updated the hydrostatic
  test section to use the lowest stress ratio (LSR) across all materials with the
  multiplier flagged as edition-dependent; added a UG-16(b) reviewer-checklist
  subsection and updated related checklist items and limitations. All original
  content preserved.

- `templates/FFS/api-579-pitting-assessment-template.md`
  Added a prominent code-verification notice; reworded the Level 1 and Level 2
  numeric screening constants (remaining-thickness-ratio threshold, pit
  diameter/spacing limits, pitting-chart/RSF approach) as edition-dependent values
  to be verified rather than asserted; added a non-2:1 ellipsoidal head note and a
  UG-16(b) cross-reference; and added an explicit cross-check that any acceptable
  result is consistent with corroded MAWP >= operating pressure. No screening
  constants were changed to fabricated alternatives. All original content
  preserved.

### Notes

- The API 510 inspection report template (`templates/inspection-plan/`) was not
  modified in this release. Its required-thickness basis is now governed by
  `references/minimum-thickness-governing-logic.md` and the `CLAUDE.md` rule. An
  inline UG-16(b) cross-reference note in that report can be added as a small
  follow-up change once the style of this release is reviewed.

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

[Unreleased]: https://github.com/khaled19858/pressure-vessel-inservice-inspection/compare/v0.2.0...HEAD
[v0.2.0]: https://github.com/khaled19858/pressure-vessel-inservice-inspection/compare/v0.1.0...v0.2.0
[v0.1.0]: https://github.com/khaled19858/pressure-vessel-inservice-inspection/releases/tag/v0.1.0
