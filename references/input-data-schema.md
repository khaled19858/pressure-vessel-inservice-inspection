# Structured Input Data Convention (YAML Front-Matter)

Controlled reference. Defines an optional, machine-readable input block that may be
placed at the top of a calculation or assessment instance so that inputs can be
validated before any calculation proceeds. This is a documentation convention; it
does not change any code formula or acceptance criterion.

The intent is traceability: every input that drives a result is declared once, in
one place, with its unit and source. The worked example in `examples/` demonstrates
the convention in use.

---

## 1. Placement and format

Place a single YAML block, delimited by `---`, at the very top of the instance
file (a filled-out copy of a template), before the title. Keys use lower_snake_case.
Every physical quantity is an object with `value`, `unit`, and `source`. Leave
`value` null when not yet known; an unresolved (null) value that feeds a result is
a hold point — the calculation must not proceed until it is resolved.

---

## 2. Schema (fields)

```yaml
---
document:
  number: null            # controlled document number
  revision: 0
  date: null
  prepared_by: null
  checked_by: null
  approved_by: null
  status: draft           # draft | issued_for_review | issued | superseded

equipment:
  tag: null
  description: null
  code_of_construction: ASME VIII-1
  code_edition: null      # edition/addenda actually used
  orientation: null       # vertical | horizontal

design:
  pressure:   { value: null, unit: kPa,  source: null }   # gauge
  temperature:{ value: null, unit: degC, source: null }
  mdmt:       { value: null, unit: degC, source: null }

materials:
  shell:
    spec: null
    allowable_stress_design: { value: null, unit: MPa, source: ASME II-D }
    allowable_stress_test:   { value: null, unit: MPa, source: ASME II-D }
  head:
    spec: null
    allowable_stress_design: { value: null, unit: MPa, source: ASME II-D }

geometry:
  inside_diameter_nominal: { value: null, unit: mm, source: null }
  shell_thickness_nominal: { value: null, unit: mm, source: null }
  head_type: null         # ellipsoidal_2_1 | torispherical | hemispherical | conical
  head_thickness_nominal:  { value: null, unit: mm, source: null }

corrosion:
  ca:  { value: null, unit: mm, source: null }   # corrosion allowance
  fca: { value: null, unit: mm, source: null }   # future corrosion allowance

joint_efficiency:
  shell: { value: null, source: UW-12_and_RT_credited }
  head:  { value: null, source: UW-12_and_RT_credited }

inspection:
  date: null
  shell_t_measured: { value: null, unit: mm, source: UT }
  head_t_measured:  { value: null, unit: mm, source: UT }
  t_previous:       { value: null, unit: mm, source: null }
  previous_date: null

corrosion_rate:
  cr_long_term:  { value: null, unit: mm/yr, source: computed }
  cr_short_term: { value: null, unit: mm/yr, source: computed }
  cr_governing:  { value: null, unit: mm/yr, source: null }

verification:
  edition_confirmed: false        # code edition/addenda confirmed for all clauses
  allowables_confirmed: false     # S values confirmed against ASME II-D
  api579_constants_confirmed: false  # any Part 6 screening constants verified
---
```

---

## 3. Validation rules

Before any result is computed from a structured instance:

- `equipment.code_edition` is set, and `verification.edition_confirmed` is true.
- Every `value` that feeds a result is non-null with a `unit` and a `source`.
- Allowable stresses are confirmed against ASME II Part D for the stated edition
  (`verification.allowables_confirmed`).
- If an API 579 Part 6 assessment is performed, any embedded screening constant is
  verified against the controlling edition
  (`verification.api579_constants_confirmed`).
- Units within a single formula are consistent (no mixed SI / US customary).

Any null value that drives a result is a hold point. Record it in the instance's
missing-data register and resolve it before calculating.

---

## 4. Cross-references

- `references/symbols-and-conventions.md`
- `examples/worked-example-vertical-vessel-mawp-remaining-life.md`
