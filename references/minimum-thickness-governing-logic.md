# Governing Minimum Thickness Logic (ASME Section VIII Division 1)

Controlled reference. This document defines how the **governing required
thickness** is determined for pressure-boundary components assessed under ASME
Section VIII Division 1. It applies to all calculation, inspection, and
fitness-for-service templates in this repository.

---

## 1. Why this matters

A pressure component can satisfy the pressure-based thickness formula (UG-27 for
shells, UG-32 for heads) and still be **non-compliant**, because Division 1 also
imposes a minimum-thickness floor that is independent of pressure. This is most
likely to control on thin-wall, large-diameter, or low-pressure components, where
the pressure-required thickness is small.

A required thickness that uses only the pressure formula is therefore incomplete.

---

## 2. Governing required thickness

The governing required thickness used for adequacy checks, MAWP, remaining
corrosion allowance, and remaining life is:

```
t_req = max( t_pressure , t_UG16b , t_struct )
```

where:

- **t_pressure** — required thickness from the applicable pressure formula in the
  corroded condition:
  - Cylindrical shell: UG-27(c)(1) circumferential stress and UG-27(c)(2)
    longitudinal stress; take the larger.
  - Formed heads: the applicable UG-32 paragraph for the head type
    (see `CLAUDE.md` for the paragraph map).
- **t_UG16b** — the code minimum-thickness floor per UG-16(b) (Section 3 below).
- **t_struct** — any additional minimum thickness required for structural,
  handling, support, wind/seismic, nozzle-load, or supplemental-load reasons,
  where such evaluations apply. Determined separately; not covered by the pressure
  formula.

The **required nominal (new) thickness** then adds the corrosion allowance:

```
t_req_nominal = t_req + CA
```

A component is adequate when:

```
t_actual_nominal >= t_req + CA      (design / new condition)
t_measured       >= t_req           (in-service condition, before adding future loss)
```

---

## 3. UG-16(b) minimum thickness floor

ASME Section VIII Division 1, UG-16(b), establishes a minimum permitted thickness
for shells and heads after forming, **exclusive of corrosion allowance**:

- The minimum thickness for shells and heads, regardless of product form and
  dimensions, is **1.5 mm (1/16 in.)**, exclusive of any corrosion allowance.

Important qualifications (read the controlling edition for the exact provisions):

- This minimum **does not include** corrosion allowance; corrosion allowance is
  added on top of it.
- UG-16(b) lists **exclusions and special cases** (for example, it does not apply
  to certain heat-transfer plates, and specific services such as compressed air,
  steam, and water carry their own minimum-thickness provisions). Where the
  service or component falls under such a provision, use that provision instead of
  the general 1.5 mm (1/16 in.) value.
- Other paragraphs may impose their own minima (for example, tube and pipe wall
  provisions). Confirm which minimum applies to the component being assessed.

> Do not state a service-specific minimum from memory. If the component is in a
> service that UG-16(b) treats specially, read the value from the controlling
> code edition and record it as t_UG16b with the clause cited.

---

## 4. Worked logic check (no fabricated values)

For each pressure component:

1. Compute t_pressure in the corroded condition using the correct UG-27/UG-32
   formula.
2. Determine t_UG16b from UG-16(b) for the component and its service.
3. Determine t_struct if any supplemental-load evaluation applies; otherwise mark
   N/A with a reason.
4. Set t_req = max of the applicable values above.
5. Add CA to obtain the required nominal thickness.
6. Compare to the actual / measured thickness and state adequacy explicitly.
7. Record which criterion governs (pressure, UG-16(b), or structural).

If UG-16(b) governs, the report must say so; this is a common and legitimate
outcome on low-pressure or large-diameter equipment and must not be hidden behind
a pressure-only required thickness.

---

## 5. Cross-references

- `references/symbols-and-conventions.md` — symbol definitions.
- `templates/calculation-checks/asme-viii-1-pressure-component-calculation-check-sheet.md`
  — implements this logic in the shell and head sections.
- `CLAUDE.md` — governing instruction requiring this logic in all calculations.
