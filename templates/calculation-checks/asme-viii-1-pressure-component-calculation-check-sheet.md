# ASME Section VIII Division 1 - Pressure Component Calculation Check Sheet

---

## 1. Document Control

| Field | Entry |
|---|---|
| Document No. | |
| Revision | |
| Date | |
| Project / Plant | |
| Equipment Tag No. | |
| Equipment Description | |
| Prepared By | |
| Checked By | |
| Approved By | |
| Code Edition / Addenda | ASME Section VIII Division 1, Edition: _______ |
| Calculation Purpose | [ ] New design [ ] Rerating [ ] FFS support [ ] Post-repair [ ] Other: _______ |

---

## 2. Equipment Data

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Vessel orientation | - | [ ] Vertical [ ] Horizontal | - |
| Inside diameter (shell, nominal) | D | | mm / in |
| Shell inside radius (nominal) | R | | mm / in |
| Shell nominal thickness | t\_nom | | mm / in |
| Measured / corroded thickness (shell) | t\_meas | | mm / in |
| Head type (top) | - | [ ] Ellip. [ ] Torisp. [ ] Hemi. [ ] Conical | - |
| Head type (bottom) | - | [ ] Ellip. [ ] Torisp. [ ] Hemi. [ ] Conical | - |
| Head nominal thickness | t\_h | | mm / in |
| Measured / corroded head thickness | t\_h\_meas | | mm / in |
| Torispherical head: crown radius | L | | mm / in |
| Torispherical head: knuckle radius | r | | mm / in |
| Ellipsoidal head: inside depth of head | h | | mm / in |
| Conical section: half apex angle | alpha | | deg |
| Vessel total height (vertical) / ID (horizontal) | H | | mm / in |
| Service fluid | - | | - |
| Fluid specific gravity | SG | | - |

---

## 3. Design Conditions

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Design pressure (internal) | P\_design | | kPa / psi |
| Design temperature | T\_design | | deg C / deg F |
| Hydrostatic test temperature | T\_test | | deg C / deg F |
| Full-fluid hydrostatic head at design conditions | P\_static | | kPa / psi |
| Total design pressure (P\_design + P\_static) | P\_total | | kPa / psi |

> **Note:** P\_total is the governing pressure used in all thickness and MAWP calculations below.

---

## 4. Static Head Calculation

*Governed by vessel orientation. See CLAUDE.md governing instruction.*

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Liquid column height (H for vertical; D for horizontal) | h\_liq | | mm / in |
| Fluid specific gravity | SG | | - |
| Static head pressure | P\_static = SG x rho\_w x g x h\_liq | | kPa / psi |

**Orientation applied:** [ ] Vertical - using vessel height  [ ] Horizontal - using vessel inside diameter  [ ] Orientation not stated - static head neglected

---

## 5. Material Properties

| Component | Material Spec. | P-No. | Allowable Stress at Design Temp (S) | Allowable Stress at Test Temp (S\_test) | UTS (S\_u) | Yield (S\_y) |
|---|---|---|---|---|---|---|
| Shell | | | | | | |
| Top head | | | | | | |
| Bottom head | | | | | | |

| Field | Value |
|---|---|
| Source of allowable stresses | [ ] ASME II Part D Table 1A [ ] Other: _______ |
| Material in corroded condition assumed same | [ ] Yes [ ] No |

---

## 6. Joint Efficiency

| Weld Joint | Category | Type | Examination | Joint Efficiency (E) |
|---|---|---|---|---|
| Shell longitudinal seam | A | | [ ] Full [ ] Spot [ ] None | |
| Shell-to-head (circumferential) | B | | [ ] Full [ ] Spot [ ] None | |
| Head seam (if applicable) | A | | [ ] Full [ ] Spot [ ] None | |

**E applied for shell thickness (longitudinal joint):** ___________

**E applied for head thickness:** ___________

> Joint efficiencies shall be consistent with the radiographic examination actually performed or credited. Do not assign a higher efficiency than the examination supports.

---

## 7. Corrosion Allowance

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Specified corrosion allowance | CA | | mm / in |
| Corroded inside radius (shell) | R\_c = R + CA | | mm / in |
| Corroded inside diameter (shell) | D\_c = D + 2CA | | mm / in |
| Corroded head inside radius / dimension | per component below | | mm / in |
| Corroded shell thickness | t\_c = t\_meas - CA | | mm / in |
| Corroded head thickness | t\_hc = t\_h\_meas - CA | | mm / in |

> All pressure calculations below use corroded geometry (R\_c, D\_c, t\_c, t\_hc) unless otherwise stated.

---

## 8. Cylindrical Shell - Internal Pressure (UG-27)

### 8.1 Required Thickness

**Circumferential stress (governs longitudinal weld seam):**

```
t_req = P_total x R_c / (S x E - 0.6 x P_total)
```

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Total design pressure | P\_total | | kPa / psi |
| Corroded inside radius | R\_c | | mm / in |
| Allowable stress | S | | MPa / psi |
| Joint efficiency | E | | - |
| **Required thickness (circ. stress)** | **t\_req\_c** | | **mm / in** |

**Longitudinal stress (governs circumferential weld seam):**

```
t_req = P_total x R_c / (2 x S x E + 0.4 x P_total)
```

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| **Required thickness (long. stress)** | **t\_req\_L** | | **mm / in** |

**Governing required shell thickness:**

```
t_req = max(t_req_c, t_req_L)
```

| Governing t\_req | | mm / in |
|---|---|---|
| Required nominal thickness (t\_req + CA) | | mm / in |
| Actual nominal thickness (t\_nom) | | mm / in |
| **Adequacy** | [ ] ADEQUATE (t\_nom >= t\_req + CA) [ ] INADEQUATE | |

### 8.2 Shell MAWP (corroded condition)

**Circumferential stress:**

```
MAWP_c = S x E x t_c / (R_c + 0.6 x t_c)
```

**Longitudinal stress:**

```
MAWP_L = 2 x S x E x t_c / (R_c - 0.4 x t_c)
```

| | Value | Unit |
|---|---|---|
| MAWP\_c (circumferential) | | kPa / psi |
| MAWP\_L (longitudinal) | | kPa / psi |
| **Governing Shell MAWP (corroded)** | | **kPa / psi** |

---

## 9. Ellipsoidal Head - Internal Pressure (UG-32(c))

*Applies to 2:1 semi-ellipsoidal heads. D is the corroded inside diameter.*

```
t_req = P_total x D_c / (2 x S x E - 0.2 x P_total)
```

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Total design pressure | P\_total | | kPa / psi |
| Corroded inside diameter | D\_c | | mm / in |
| Allowable stress | S | | MPa / psi |
| Joint efficiency | E | | - |
| **Required head thickness** | **t\_req\_h** | | **mm / in** |
| Required nominal thickness (t\_req\_h + CA) | | | mm / in |
| Actual nominal head thickness (t\_h) | | | mm / in |
| **Adequacy** | [ ] ADEQUATE [ ] INADEQUATE | | |

**MAWP (corroded):**

```
MAWP_ellip = 2 x S x E x t_hc / (D_c + 0.2 x t_hc)
```

| **Ellipsoidal Head MAWP (corroded)** | | kPa / psi |
|---|---|---|

---

## 10. Torispherical Head - Internal Pressure (UG-32(d))

*L = corroded inside crown radius. Default: L = D\_c.*

```
t_req = 0.885 x P_total x L / (S x E - 0.1 x P_total)
```

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Total design pressure | P\_total | | kPa / psi |
| Corroded inside crown radius | L | | mm / in |
| Knuckle radius | r | | mm / in |
| Allowable stress | S | | MPa / psi |
| Joint efficiency | E | | - |
| **Required head thickness** | **t\_req\_h** | | **mm / in** |
| Required nominal thickness (t\_req\_h + CA) | | | mm / in |
| Actual nominal head thickness (t\_h) | | | mm / in |
| **Adequacy** | [ ] ADEQUATE [ ] INADEQUATE | | |

**MAWP (corroded):**

```
MAWP_tori = S x E x t_hc / (0.885 x L + 0.1 x t_hc)
```

| **Torispherical Head MAWP (corroded)** | | kPa / psi |
|---|---|---|

---

## 11. Hemispherical Head - Internal Pressure (UG-32(e))

*L\_h = corroded inside radius of hemispherical head.*

```
t_req = P_total x L_h / (2 x S x E - 0.2 x P_total)
```

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Total design pressure | P\_total | | kPa / psi |
| Corroded inside radius of head | L\_h | | mm / in |
| Allowable stress | S | | MPa / psi |
| Joint efficiency | E | | - |
| **Required head thickness** | **t\_req\_h** | | **mm / in** |
| Required nominal thickness (t\_req\_h + CA) | | | mm / in |
| Actual nominal head thickness (t\_h) | | | mm / in |
| **Adequacy** | [ ] ADEQUATE [ ] INADEQUATE | | |

**MAWP (corroded):**

```
MAWP_hemi = 2 x S x E x t_hc / (L_h + 0.2 x t_hc)
```

| **Hemispherical Head MAWP (corroded)** | | kPa / psi |
|---|---|---|

---

## 12. Conical Section Without Transition Knuckle - Internal Pressure (UG-32(f))

*D = corroded inside diameter at the large end of the cone. alpha = half apex angle. UG-32(f) applies when alpha <= 30 deg; verify applicability for larger angles.*

```
t_req = P_total x D_c / [2 x cos(alpha) x (S x E - 0.6 x P_total)]
```

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Total design pressure | P\_total | | kPa / psi |
| Corroded inside diameter at large end | D\_c | | mm / in |
| Half apex angle | alpha | | deg |
| cos(alpha) | cos(alpha) | | - |
| Allowable stress | S | | MPa / psi |
| Joint efficiency | E | | - |
| **Required cone thickness** | **t\_req\_cone** | | **mm / in** |
| Required nominal thickness (t\_req\_cone + CA) | | | mm / in |
| Actual nominal cone thickness | | | mm / in |
| **Adequacy** | [ ] ADEQUATE [ ] INADEQUATE | | |

**MAWP (corroded):**

```
MAWP_cone = 2 x S x E x t_cc x cos(alpha) / [D_c + 1.2 x t_cc x cos(alpha)]
```

where t\_cc = corroded cone thickness.

| **Conical Section MAWP (corroded)** | | kPa / psi |
|---|---|---|

---

## 13. MAWP Summary and Governing Component

| Component | MAWP (corroded) (kPa / psi) | Governing? |
|---|---|---|
| Cylindrical shell (circumferential stress) | | |
| Cylindrical shell (longitudinal stress) | | |
| Top head | | |
| Bottom head | | |
| Conical section (if applicable) | | |
| **Governing Equipment MAWP (corroded)** | | **YES** |

**MAWP vs. Design Pressure check:**

| | Value | Unit |
|---|---|---|
| Governing MAWP (corroded) | | kPa / psi |
| Total design pressure (P\_total) | | kPa / psi |
| Margin (MAWP - P\_total) | | kPa / psi |
| Margin (%) | | % |
| **Acceptable for continued operation?** | [ ] YES - MAWP >= P\_total [ ] NO - action required | |

---

## 14. Hydrostatic Test Pressure (UG-99)

*Standard hydrostatic test pressure as a function of MAWP and stress ratio between test and design temperature.*

```
P_test = 1.3 x MAWP_corroded x (S_test / S_design)
```

| Parameter | Symbol | Value | Unit |
|---|---|---|---|
| Governing MAWP (corroded) | MAWP | | kPa / psi |
| Allowable stress at test temperature | S\_test | | MPa / psi |
| Allowable stress at design temperature | S\_design | | MPa / psi |
| Stress ratio | S\_test / S\_design | | - |
| **Minimum required hydrostatic test pressure** | **P\_test** | | **kPa / psi** |
| Actual test pressure applied (if known) | P\_test\_actual | | kPa / psi |
| Test medium | | [ ] Water [ ] Other: _______ | |
| Test temperature | T\_test | | deg C / deg F |

> Verify that P\_test does not exceed the limits for any component. For pneumatic testing (UG-100), a different multiplier and risk assessment apply - do not use this section for pneumatic tests.

---

## 15. Assumptions

List all assumptions made in this calculation. Each assumption must be justified or flagged for verification.

| No. | Assumption | Basis / Justification |
|---|---|---|
| A1 | Division 1 rules apply | Vessel designed/registered under ASME VIII-1 |
| A2 | Corroded inside radius and diameter used throughout | Conservative; CLAUDE.md governing rule |
| A3 | Corrosion allowance applies uniformly to all components | Per design specification or inspection data |
| A4 | Joint efficiency per weld examination credited above | Consistent with NDE records |
| A5 | Static head per governing orientation rule | Per CLAUDE.md static head rule |
| A6 | | |
| A7 | | |

---

## 16. Limitations

| No. | Limitation |
|---|---|
| L1 | This check sheet covers internal pressure only. External pressure, wind, seismic, nozzle loads, and combined loading are not addressed here. |
| L2 | Nozzle reinforcement is not evaluated in this check sheet. |
| L3 | UG-32(f) conical section formula is valid without transition knuckles. If knuckles are present, UG-32(g) (toriconical) applies and this sheet does not apply. |
| L4 | Ellipsoidal head formula (UG-32(c)) as presented is for a standard 2:1 (h = D/4) head. Non-standard ratios require additional factors per the code. |
| L5 | Allowable stresses are taken at the stated design temperature. If temperature varies along the vessel, each zone requires separate evaluation. |
| L6 | This check sheet does not replace a full code calculation package. It is a structured verification aid only. |
| L7 | Material toughness, impact test exemption, and MDMT are not addressed here. |
| L8 | | |

---

## 17. Reviewer Checklist

Complete each item before sign-off. Mark N/A if a component is not present.

### 17.1 Document and Data

- [ ] Document number, revision, and date are complete
- [ ] Code edition / addenda is identified
- [ ] Equipment tag number matches the vessel data sheet
- [ ] All design conditions are sourced from the approved data sheet or engineering specification
- [ ] Material specifications are complete and allowable stresses are sourced from ASME II Part D

### 17.2 Geometry and Corrosion Allowance

- [ ] Corroded inside radius and diameter are correctly derived from nominal dimensions plus CA
- [ ] Corroded thickness is nominal minus CA, confirmed against inspection records where applicable
- [ ] Head inside dimensions are consistently corrected for CA
- [ ] Conical half apex angle is confirmed from drawing

### 17.3 Static Head

- [ ] Vessel orientation is confirmed
- [ ] Static head column height is correctly selected (vessel height for vertical; ID for horizontal)
- [ ] P\_static is correctly calculated and added to design pressure to give P\_total
- [ ] If orientation is unknown, static head neglect is documented as an assumption

### 17.4 Shell (UG-27)

- [ ] Both circumferential and longitudinal stress cases are evaluated
- [ ] Correct joint efficiency is applied to each case
- [ ] Governing required thickness is the larger of the two cases
- [ ] Required nominal thickness includes CA
- [ ] Shell MAWP is calculated using corroded thickness and corroded inside radius

### 17.5 Heads

- [ ] Correct UG-32 paragraph is applied for each head type
- [ ] Corrected inside dimensions are used in head calculations
- [ ] Torispherical head: L is the corroded inside crown radius
- [ ] Conical section: half apex angle and cos(alpha) are correctly applied
- [ ] Head MAWP is calculated using corroded head thickness

### 17.6 MAWP Summary

- [ ] All components (shell, heads, cone) appear in MAWP summary table
- [ ] Governing MAWP is the minimum of all component MAWPs
- [ ] Governing MAWP >= total design pressure P\_total; if not, deficiency is flagged

### 17.7 Hydrostatic Test Pressure

- [ ] Test pressure is calculated as 1.3 x MAWP\_corroded x (S\_test / S\_design)
- [ ] Stress ratio is correctly applied; if S\_test / S\_design > 1.0, apply the ratio; if = 1.0, P\_test = 1.3 x MAWP
- [ ] Test pressure does not impose stresses exceeding 90% of yield in any component (verify separately)
- [ ] Test medium and temperature are recorded

### 17.8 General

- [ ] No clause numbers are cited beyond those established in CLAUDE.md or independently verified
- [ ] No values are assumed without being listed in the Assumptions section
- [ ] All equations show substitution with units
- [ ] All results are reported with units
- [ ] Adequacy statements are explicit for every component

---

## 18. Calculation Results Summary

| Component | t\_req (mm/in) | t\_req + CA (mm/in) | t\_actual (mm/in) | MAWP (kPa/psi) | Adequate? |
|---|---|---|---|---|---|
| Cylindrical shell | | | | | [ ] Y [ ] N |
| Top head | | | | | [ ] Y [ ] N |
| Bottom head | | | | | [ ] Y [ ] N |
| Conical section | | | | | [ ] Y [ ] N |
| **Governing MAWP** | - | - | - | | - |
| **Hydrostatic test pressure** | - | - | - | | - |

---

## 19. Approval Block

| Role | Name | Signature | Date |
|---|---|---|---|
| Prepared By | | | |
| Independently Checked By | | | |
| Approved By (Engineer of Record) | | | |
| Client / Owner Review (if applicable) | | | |

**Calculation Status:** [ ] Preliminary [ ] Issued for Review [ ] Issued for Construction / Rerating [ ] Superseded by Rev: _______

---

*This check sheet is governed by ASME Section VIII Division 1. All calculations shall use corroded geometry. Clause references are limited to UG-27 (shells), UG-32(c) (ellipsoidal), UG-32(d) (torispherical), UG-32(e) (hemispherical), UG-32(f) (conical without transition knuckle), and UG-99 (hydrostatic test). Do not apply Division 2 rules unless separately instructed.*
