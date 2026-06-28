---
document:
  number: EX-001
  revision: 0
  date: null
  prepared_by: null
  checked_by: null
  approved_by: null
  status: draft
equipment:
  tag: EX-V-1001
  description: Illustrative vertical pressure vessel (worked example)
  code_of_construction: ASME VIII-1
  code_edition: ILLUSTRATIVE - confirm in real work
  orientation: vertical
design:
  pressure:    { value: 1000, unit: kPa, source: illustrative }
  temperature: { value: 150,  unit: degC, source: illustrative }
materials:
  shell:
    spec: ILLUSTRATIVE
    allowable_stress_design: { value: 138, unit: MPa, source: ILLUSTRATIVE - not a code lookup }
  head:
    spec: ILLUSTRATIVE
    allowable_stress_design: { value: 138, unit: MPa, source: ILLUSTRATIVE - not a code lookup }
geometry:
  inside_diameter_nominal: { value: 2000, unit: mm, source: illustrative }
  shell_thickness_nominal: { value: 20,   unit: mm, source: illustrative }
  head_type: ellipsoidal_2_1
  head_thickness_nominal:  { value: 20,   unit: mm, source: illustrative }
corrosion:
  ca:  { value: 3.0, unit: mm, source: illustrative }
  fca: { value: 3.0, unit: mm, source: illustrative }
joint_efficiency:
  shell: { value: 1.0, source: full RT (illustrative) }
  head:  { value: 1.0, source: full RT (illustrative) }
inspection:
  date: null
  shell_t_measured: { value: 18.0, unit: mm, source: UT (illustrative) }
  t_previous:       { value: 18.6, unit: mm, source: UT (illustrative) }
verification:
  edition_confirmed: false
  allowables_confirmed: false
  api579_constants_confirmed: false
---

# Worked Example - Vertical Vessel: Governing Thickness, MAWP, and Remaining Life

> **READ THIS FIRST.** This is a teaching example. The numbers are chosen to make
> the method clear, not to represent any real vessel. In particular, the allowable
> stress `S = 138 MPa` is an **illustrative value only** and is **not** a lookup
> from ASME II Part D. In real work, read `S` from ASME II Part D for the actual
> material, temperature, and code edition. All formulas used are ASME Section VIII
> Division 1 formulas as referenced; all arithmetic below has been checked.

The example demonstrates the repository conventions: corroded geometry throughout,
the **governing required thickness** rule including the UG-16(b) floor, the
circumferential and longitudinal shell checks, a 2:1 ellipsoidal head, the
governing MAWP, the UG-99(b) hydrotest pressure, and remaining life with the
half-life interval basis.

---

## 1. Given data (illustrative)

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Orientation | - | Vertical | - |
| Design pressure (incl. static head) | P | 1000 | kPa(g) = 1.0 MPa |
| Inside diameter (nominal) | D | 2000 | mm |
| Inside radius (nominal) | R | 1000 | mm |
| Shell nominal thickness | t_nom | 20.0 | mm |
| Current measured shell thickness | t_meas | 18.0 | mm |
| Head type | - | Ellipsoidal 2:1 | - |
| Head nominal / measured thickness | t_h | 20.0 / 18.0 | mm |
| Corrosion allowance | CA | 3.0 | mm |
| Future corrosion allowance | FCA | 3.0 | mm |
| Allowable stress (ILLUSTRATIVE) | S | 138 | MPa |
| Joint efficiency | E | 1.0 | - |

Static head note: vessel is vertical, so the static-head column would be the vessel
height per the governing rule. For this example the design pressure of 1000 kPa is
taken as already inclusive of static head (P = P_total).

---

## 2. Corroded geometry

```
R_c = R + CA = 1000 + 3.0 = 1003.0 mm
D_c = D + 2*CA = 2000 + 2(3.0) = 2006.0 mm
t_c = t_meas - FCA = 18.0 - 3.0 = 15.0 mm   (thickness available for pressure)
```

---

## 3. Shell required thickness (UG-27)

**Circumferential stress, UG-27(c)(1)** (governs the longitudinal seam):

```
t_pressure,circ = P*R_c / (S*E - 0.6*P)
               = 1.0*1003.0 / (138*1.0 - 0.6*1.0)
               = 1003.0 / 137.4
               = 7.30 mm
```

**Longitudinal stress, UG-27(c)(2)** (governs the circumferential seam):

```
t_pressure,long = P*R_c / (2*S*E + 0.4*P)
               = 1.0*1003.0 / (2*138 + 0.4*1.0)
               = 1003.0 / 276.4
               = 3.63 mm
```

**Pressure-governing:** t_pressure = max(7.30, 3.63) = **7.30 mm** (circumferential
stress governs, as expected for a cylinder).

**UG-16(b) floor:** 1.5 mm exclusive of CA. Since 7.30 mm > 1.5 mm, **pressure
governs**, not the code floor. (On a thinner, larger-diameter, or lower-pressure
shell the 1.5 mm floor could govern — that check must always be made.)

**Structural minimum:** none additional assumed for this example (N/A).

**Governing required thickness:**

```
t_req = max(t_pressure, t_UG16b, t_struct) = max(7.30, 1.5, N/A) = 7.30 mm
Required nominal = t_req + CA = 7.30 + 3.0 = 10.30 mm
```

Actual nominal 20.0 mm >= 10.30 mm -> **ADEQUATE** (new condition).
Current measured 18.0 mm >= 7.30 mm -> **ADEQUATE** (in-service).

---

## 4. Shell MAWP (corroded condition)

```
MAWP_circ = S*E*t_c / (R_c + 0.6*t_c)
         = 138*1.0*15.0 / (1003.0 + 0.6*15.0)
         = 2070 / 1012.0
         = 2.0455 MPa = 2045.5 kPa(g)

MAWP_long = 2*S*E*t_c / (R_c - 0.4*t_c)
         = 2*138*1.0*15.0 / (1003.0 - 0.4*15.0)
         = 4140 / 997.0
         = 4.1525 MPa = 4152.5 kPa(g)
```

Governing shell MAWP = min(2045.5, 4152.5) = **2045.5 kPa(g)** (circumferential).

---

## 5. Ellipsoidal head (2:1), UG-32(c)

For a standard 2:1 head (h = D/4), using corroded inside diameter D_c:

```
t_pressure,head = P*D_c / (2*S*E - 0.2*P)
              = 1.0*2006.0 / (2*138 - 0.2*1.0)
              = 2006.0 / 275.8
              = 7.27 mm
```

t_req,head = max(7.27, 1.5) = 7.27 mm; required nominal = 7.27 + 3.0 = 10.27 mm.
Actual 20.0 mm -> **ADEQUATE**.

```
MAWP_head = 2*S*E*t_hc / (D_c + 0.2*t_hc),   t_hc = 18.0 - 3.0 = 15.0 mm
         = 2*138*1.0*15.0 / (2006.0 + 0.2*15.0)
         = 4140 / 2009.0
         = 2.0607 MPa = 2060.7 kPa(g)
```

> The simplified UG-32(c) formula above applies to a **2:1** head. For a non-2:1
> ratio, the factor K from Mandatory Appendix 1-4(c) is required; the simplified
> formula must not be used in that case.

---

## 6. Governing MAWP and adequacy

| Component | MAWP (corroded) | kPa(g) |
|---|---|---|
| Shell (circumferential) | governing | 2045.5 |
| Shell (longitudinal) | - | 4152.5 |
| Ellipsoidal head (2:1) | - | 2060.7 |
| **Governing equipment MAWP** | **shell** | **2045.5** |

Governing MAWP 2045.5 kPa(g) >= design pressure 1000 kPa(g) -> **acceptable for
continued operation** at the stated condition. Margin = 1045.5 kPa (about 104.6%
above design).

---

## 7. Hydrostatic test pressure (UG-99(b))

```
P_test = 1.3 * MAWP_corroded * (S_test / S_design)
```

Assuming the test is performed at a temperature where the stress ratio
(S_test / S_design) = 1.0 for the governing material (i.e., LSR = 1.0):

```
P_test = 1.3 * 2045.5 * 1.0 ~= 2659 kPa(g)
```

(Carried from the unrounded MAWP the product is 2659.15 kPa; reported to whole
kPa to avoid implying precision the inputs do not support.)

Notes:
- Use the **lowest stress ratio (LSR)** among **all** pressure-boundary materials,
  not only the governing-MAWP component, per UG-99(b).
- The 1.3 multiplier is the current UG-99(b) basis; older editions used a different
  factor. Confirm the multiplier for the controlling edition.
- Verify the test does not over-stress any component (test-stress limit) and apply
  UG-100 separately if a pneumatic test is used.

---

## 8. Corrosion rate, remaining life, and interval

Illustrative inspection history at the governing shell CML:

| Quantity | Value |
|---|---|
| Original nominal t_nom | 20.0 mm |
| Previous measured t_prev (5 yr ago) | 18.6 mm |
| Current measured t_meas | 18.0 mm |
| Age since new | 15 yr |

```
CR_ST = (t_prev - t_meas) / interval = (18.6 - 18.0) / 5  = 0.120 mm/yr
CR_LT = (t_nom  - t_meas) / age      = (20.0 - 18.0) / 15 = 0.133 mm/yr
CR_gov = max(CR_ST, CR_LT) = 0.133 mm/yr   (conservative)
```

Remaining metal above the governing required thickness:

```
t_meas - t_req = 18.0 - 7.30 = 10.70 mm
RL = (t_meas - t_req) / CR_gov = 10.70 / 0.133 ~= 80 yr
Half-life = RL / 2 ~= 40 yr
```

(With the exact long-term rate 2/15 = 0.1333 mm/yr the result is 80.25 yr; reported
as ~80 yr. Intermediate rounding can shift the last digit, so carry full precision
in real calculations and round only the final reported figure.)

Inspection interval = min(half-life, API 510 prescriptive maximum, RBI-derived).
Here the half-life (~40 yr) far exceeds the API 510 prescriptive maximum, so the
**prescriptive maximum governs** the next internal/on-stream interval. Read that
maximum from the controlling API 510 edition and record the figure used; do not
extend beyond it without RBI or accepted engineering justification.

---

## 9. Summary

| Item | Result |
|---|---|
| Governing required thickness (shell) | 7.30 mm (pressure governs; UG-16(b) floor 1.5 mm checked) |
| Shell adequacy | Adequate (measured 18.0 mm) |
| Governing equipment MAWP (corroded) | 2045.5 kPa(g), set by shell circumferential stress |
| MAWP vs design (1000 kPa) | Acceptable, ~104.6% margin |
| Hydrotest pressure (LSR = 1.0 assumed) | ~2659 kPa(g) |
| Governing corrosion rate | 0.133 mm/yr (long-term) |
| Remaining life / half-life | ~80 yr / ~40 yr |
| Interval basis | API 510 prescriptive maximum governs (half-life is larger) |

> Reminder: replace the illustrative `S = 138 MPa` and the illustrative code
> edition with verified values from ASME II Part D and the controlling code
> editions before using this method on a real vessel.
