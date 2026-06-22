# Pressure Vessel Inservice Inspection

Controlled engineering workspace for pressure vessel in-service inspection, API 510 inspection planning, API 579-1/ASME FFS-1 fitness-for-service assessments, ASME Section VIII Division 1 pressure calculations, damage mechanism review, CML/UT mapping, and inspection reporting.

## Project scope

This repository is intended for:

- API 510 pressure vessel inspection work
- API 579-1/ASME FFS-1 assessments
- ASME Section VIII Division 1 pressure-boundary calculations
- API 571 damage mechanism review
- RBI and inspection planning support
- CML/UT thickness mapping templates
- Fitness-for-service reports
- Inspection recommendations and technical notes

## Repository control

This repository shall be treated as a controlled engineering workspace. Engineering calculations, assumptions, inputs, and outputs must be traceable.

## Controlled Templates

The following templates are maintained in this repository. Each template is a Markdown file structured for direct use in engineering reports and calculations.

| Template | Path | Intended Use |
|---|---|---|
| API 579 Pitting Assessment | templates/FFS/api-579-pitting-assessment-template.md | Level 1 and Level 2 pitting and local metal loss fitness-for-service assessment per API 579-1/ASME FFS-1. |
| API 579 General FFS Assessment Report | templates/FFS/api-579-general-ffs-assessment-report-template.md | General fitness-for-service assessment report covering all API 579-1/ASME FFS-1 Parts, including assessment level selection, input data, calculation workflow, results, and acceptability statement. |
| FFS Assessment Input Data Sheet | templates/FFS/ffs-assessment-input-data-sheet.md | Pre-assessment data collection sheet capturing design data, operating data, material data, geometry, corrosion allowance, inspection readings, flaw dimensions, NDE method, weld details, toughness/cyclic screening, and missing data register. |
| API 510 Inspection Report | templates/inspection-plan/api-510-pressure-vessel-inspection-report-template.md | Structured inspection reporting per API 510 including damage mechanism review, thickness data, MAWP check, and recommendations. |
| RBI and Inspection Planning | templates/inspection-plan/rbi-inspection-planning-template.md | Risk-based inspection planning covering equipment list, damage mechanism review summary, consequence screening, likelihood screening, risk ranking, inspection strategy, CML strategy, NDE method selection, interval basis, and deferral triggers. |
| ASME VIII-1 Calculation Check Sheet | templates/calculation-checks/asme-viii-1-pressure-component-calculation-check-sheet.md | Pressure-boundary calculations for shells, heads, and nozzles per ASME Section VIII Division 1 including MAWP and hydrotest. |
| CML / UT Thickness Mapping | templates/CML-UT-mapping/cml-ut-thickness-mapping-template.md | CML placement, UT reading tables, and clock-position mapping for corrosion monitoring programs. |
| API 571 Damage Mechanism Review | templates/damage-mechanism-review/api-571-damage-mechanism-review-template.md | Damage mechanism review for pressure vessels and pressure-boundary equipment covering credible and non-credible mechanisms, susceptibility factors, inspection history, inspection effectiveness, CML/UT evidence, NDE evidence, process chemistry evidence, active versus potential mechanisms, and FFS triggers. |
| Inspection Recommendation and Technical Note | templates/recommendations/inspection-recommendation-technical-note-template.md | Technical note for inspection findings and recommendations covering issue statement, inspection finding, technical basis, risk consideration, options, recommended action, priority, due date, shutdown or online requirements, follow-up inspection, and responsible party. |

## Workflow

To create or update a template:

  1. Create or edit the template file in the appropriate subdirectory under templates/.
  2. Review the content for accuracy against the applicable code or standard.
  3. Run:  git status
  4. Stage the file:  git add <file path>
  5. Commit with a descriptive message:  git commit -m "message"
  6. Push to remote:  git push
