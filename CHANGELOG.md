# Changelog

All notable changes to this repository are documented in this file.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased]

No unreleased changes at this time.

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

