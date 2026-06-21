# API 579-1/ASME FFS-1 Pitting Assessment Template
## Part 6 — Assessment of Pitting Corrosion

---

## 1. Executive Summary

| Item | Entry |
|------|-------|
| Equipment ID | |
| Equipment Description | |
| Assessment Date | |
| Assessed By | |
| Reviewed By | |
| Assessment Level | Level 1 / Level 2 / Level 3 |
| Damage Mechanism | Pitting Corrosion |
| Assessment Result | ACCEPTABLE / NOT ACCEPTABLE / FURTHER EVALUATION REQUIRED |
| Recommended Action | |

---

## 2. Equipment Data

### 2.1 Vessel Identification

| Parameter | Value | Source |
|-----------|-------|--------|
| Equipment Tag | | |
| Equipment Name | | |
| Service | | |
| Year Built | | |
| Design Standard | ASME Section VIII Division 1 | |
| Jurisdiction Number / NB Number | | |
| P&ID Reference | | |
| Unit / Plant | | |

### 2.2 Design Data

| Parameter | Symbol | Value | Unit |
|-----------|--------|-------|------|
| Design Pressure (internal) | P_d | | kPa (g) / psi (g) |
| Design Pressure (external) | | | kPa (g) / psi (g) |
| Design Temperature (max) | T_max | | °C / °F |
| Design Temperature (min) | T_min | | °C / °F |
| MAWP (stamped) | MAWP_stamp | | kPa (g) / psi (g) |
| MDMT (stamped) | MDMT_stamp | | °C / °F |
| Operating Pressure | P_op | | kPa (g) / psi (g) |
| Operating Temperature | T_op | | °C / °F |
| Vessel Orientation | Vertical / Horizontal | | |

### 2.3 Component Geometry — Affected Component

| Parameter | Symbol | Value | Unit |
|-----------|--------|-------|------|
| Component Type | | Shell / Head / Nozzle | |
| Shell Inside Diameter (nominal) | D_i | | mm / in |
| Nominal Thickness | t_nom | | mm / in |
| Nominal Corrosion Allowance (original) | CA_orig | | mm / in |
| Future Corrosion Allowance | FCA | | mm / in |
| Mill Undertolerance (UTP) | UTL | | mm / in |
| Weld Joint Efficiency | E | | — |
| Head Type (if applicable) | | Ellipsoidal / Torispherical / Hemispherical / Conical | |
| Crown Radius L (torispherical) | L | | mm / in |
| Half-apex Angle (conical) | α | | degrees |

### 2.4 Material

| Parameter | Value |
|-----------|-------|
| Material Specification | |
| P-Number | |
| Grade / Class | |
| UNS Number | |
| Yield Strength S_y (min, from code) | |
| Ultimate Tensile Strength S_u (min, from code) | |
| Allowable Stress S at Operating Temperature | |
| Code Year / Edition | |

---

## 3. Inspection Findings

### 3.1 Inspection Summary

| Item | Entry |
|------|-------|
| Inspection Date | |
| Inspection Method(s) | UT thickness / VT / PT / WFMT / AUT / PAUT / RT |
| Inspector Name / Cert Level | |
| Inspection Report Reference | |
| Location of Pitting (clock position, elevation, axial zone) | |
| Area Covered by Inspection | |
| Accessibility Limitations | |

### 3.2 Pitting Survey Data

Record all pits within the assessment zone. For extensive pitting, grid-map and report representative worst-case and statistical values.

| Pit ID | Location (axial / circ) | Pit Depth w_i (mm / in) | Pit Diameter d_i (mm / in) | Pit Spacing s_i (mm / in) | Notes |
|--------|--------------------------|--------------------------|----------------------------|---------------------------|-------|
| P-01 | | | | | |
| P-02 | | | | | |
| P-03 | | | | | |
| P-04 | | | | | |
| P-05 | | | | | |
| (add rows as needed) | | | | | |

### 3.3 Thickness Readings in Pitting Zone

| Reading ID | Location | Measured Thickness t_meas (mm / in) | Pit Depth w (mm / in) | Remaining Thickness t_rem = t_meas − w (mm / in) |
|------------|----------|--------------------------------------|------------------------|---------------------------------------------------|
| | | | | |
| | | | | |
| | | | | |

**Minimum measured thickness in pitting zone:** `t_mm` = ________ mm / in

**Minimum remaining thickness (below deepest pit):** `t_rem_min` = ________ mm / in

---

## 4. Damage Mechanism Review

**Primary Damage Mechanism:** Pitting Corrosion

**API 571 Reference:** Section 5.1.2 (Uniform Corrosion) / Section 5.1.6 (Pitting Corrosion)

| Item | Description |
|------|-------------|
| Corrosive Agent | |
| Pitting Morphology | Isolated / Widespread / Localized zone |
| Pitting Pattern | Random / Linear / Directional |
| Associated Damage Mechanisms | HIC / SCC / Erosion / Cavitation / MIC |
| Corrosion Rate (historical or estimated) | mm/yr or mpy |
| Basis for Corrosion Rate | UT history / Coupon / Literature |
| Is pitting active or dormant? | |

---

## 5. Applicable Code Basis

- **FFS Standard:** API 579-1/ASME FFS-1, Edition: ________
- **Part 6:** Assessment of Pitting Corrosion
- **Design Code:** ASME Section VIII Division 1, Edition: ________
- **Allowable Stress Source:** ASME II Part D, Table 1-A, Edition: ________

---

## 6. Input Data Table

| Parameter | Symbol | Value | Unit | Source / Remark |
|-----------|--------|-------|------|-----------------|
| Design pressure | P | | kPa / psi | Nameplate / drawing |
| Allowable stress at operating temperature | S | | MPa / psi | ASME II Part D |
| Weld joint efficiency | E | | — | Nameplate / drawing |
| Nominal thickness | t_nom | | mm / in | Drawing |
| Mill undertolerance | UTL | | mm / in | Material spec |
| Future corrosion allowance | FCA | | mm / in | Process/materials eng |
| Minimum measured thickness (sound metal) | t_mm | | mm / in | UT inspection |
| Minimum remaining thickness below pit | t_rem_min | | mm / in | UT inspection |
| Maximum pit depth | w_max | | mm / in | Inspection |
| Representative pit diameter | d | | mm / in | Inspection |
| Pit spacing (nearest neighbor) | s | | mm / in | Inspection |
| Inside radius (nominal) | R_i | | mm / in | Drawing |
| Inside radius (corroded) | R_c = R_i + FCA | | mm / in | Calculated |

---

## 7. Assumptions and Limitations

1. Thickness readings are representative of the component condition at the time of inspection.
2. The corrosion rate used for future corrosion allowance is ________ mm/yr, based on ________.
3. Assessment is limited to the pitting zone identified; areas not inspected are assumed to be at the nominal design condition.
4. No credit is taken for any remaining original corrosion allowance beyond the FCA stated.
5. Weld joint efficiency `E` = ________ is assumed uniform in the assessment zone.
6. No external pressure, cyclic loading, or elevated-temperature creep conditions are present unless noted.
7. [Add additional assumptions specific to this assessment]

---

## 8. Calculations

### 8.1 Remaining Thickness Ratio (RTR) — API 579-1 Part 6 Screening

**Structural thickness available for pressure containment:**

```
t_available = t_mm − FCA
```

| Parameter | Value | Unit |
|-----------|-------|------|
| t_mm (minimum measured in sound metal) | | mm / in |
| FCA | | mm / in |
| t_available = t_mm − FCA | | mm / in |

### 8.2 Required Thickness (Pressure Design)

**Cylindrical shell — ASME VIII-1, UG-27(c)(1):**

```
t_req = P × R_c / (S × E − 0.6 × P)
```

**Torispherical head — ASME VIII-1, UG-32(d):**

```
t_req = 0.885 × P × L / (S × E − 0.1 × P)
```

**Ellipsoidal head (2:1) — ASME VIII-1, UG-32(c):**

```
t_req = P × D_c / (2 × S × E − 0.2 × P)
```

*(Use the formula applicable to this component.)*

| Parameter | Value | Unit |
|-----------|-------|------|
| P (design pressure) | | kPa / psi |
| R_c (corroded inside radius = R_i + FCA) | | mm / in |
| D_c (corroded inside diameter = D_i + 2×FCA) | | mm / in |
| S | | MPa / psi |
| E | | — |
| **t_req (calculated)** | | **mm / in** |

### 8.3 Minimum Allowable Remaining Thickness

```
t_min_allow = t_req   (for structural adequacy, per API 579-1 Part 6)
```

| Parameter | Value | Unit |
|-----------|-------|------|
| t_req | | mm / in |
| t_min_allow | | mm / in |

### 8.4 Level 1 Screening — API 579-1 Part 6, para. 6.4

**Criterion 1 — Sound metal thickness:**

```
t_available ≥ t_min_allow
```

| Check | Value | Limit | Pass / Fail |
|-------|-------|-------|-------------|
| t_available | | ≥ t_min_allow | |

**Criterion 2 — Remaining thickness ratio (RTR):**

```
RTR = (t_rem_min − FCA) / t_req
```

The Level 1 acceptance criterion is:

```
RTR ≥ 0.20
```

| Parameter | Value | Unit |
|-----------|-------|------|
| t_rem_min | | mm / in |
| FCA | | mm / in |
| t_req | | mm / in |
| **RTR = (t_rem_min − FCA) / t_req** | | — |
| Criterion: RTR ≥ 0.20 | | Pass / Fail |

**Criterion 3 — Pit dimension limit (Level 1):**

```
d ≤ 0.2 × √(D_c × t_nom)
```

| Parameter | Value | Unit |
|-----------|-------|------|
| D_c | | mm / in |
| t_nom | | mm / in |
| √(D_c × t_nom) | | mm / in |
| 0.2 × √(D_c × t_nom) | | mm / in |
| d (largest pit diameter) | | mm / in |
| Criterion: d ≤ limit | | Pass / Fail |

**Criterion 4 — Pit spacing (Level 1):**

```
s ≥ 2 × √(D_c × t_nom)
```

| Parameter | Value | Unit |
|-----------|-------|------|
| 2 × √(D_c × t_nom) | | mm / in |
| s (minimum pit spacing) | | mm / in |
| Criterion: s ≥ limit | | Pass / Fail |

**Level 1 Overall Result:** PASS / FAIL

*If Level 1 fails, proceed to Level 2.*

---

### 8.5 Level 2 Assessment — API 579-1 Part 6, para. 6.5

*Complete this section only if Level 1 was not satisfied.*

#### 8.5.1 Pitting Chart Approach (para. 6.5.2)

Step 1 — Determine the average pit depth ratio (ρ):

```
ρ = w_avg / t_mm
```

| Parameter | Value |
|-----------|-------|
| w_avg (average pit depth) | |
| t_mm | |
| ρ | |

Step 2 — Determine pitting density (number of pits per unit area in the survey zone):

```
Pit density = N_pits / A_survey
```

| Parameter | Value | Unit |
|-----------|-------|------|
| N_pits (count in survey area) | | — |
| A_survey (survey area) | | mm² / in² |
| Pit density | | pits/mm² or pits/in² |

Step 3 — Enter API 579-1 Part 6 Figure 6.10 (or Table 6.2) with `ρ` and pit density to obtain allowable remaining strength factor RSF_a for pitting:

```
RSF_pit = f(ρ, pit density)   [from Figure 6.10 / Table 6.2]
```

| Parameter | Value |
|-----------|-------|
| ρ | |
| Pit density | |
| RSF_pit (from chart / table) | |

Step 4 — Evaluate acceptability:

```
RSF_pit ≥ RSF_a   where RSF_a = 0.90 (default, ASME VIII-1)
```

| Check | Value | Criterion | Pass / Fail |
|-------|-------|-----------|-------------|
| RSF_pit | | ≥ 0.90 | |

#### 8.5.2 Equivalent General Metal Loss (Alternative — para. 6.5.3)

If pitting is modeled as equivalent uniform corrosion:

```
t_eq_loss = ρ × t_mm
t_rem_eq = t_mm − t_eq_loss
```

Assess using Part 4 (general metal loss) methodology:

```
MAWP_pit = S × E × (t_rem_eq − FCA) / (R_c + 0.6 × (t_rem_eq − FCA))
```

| Parameter | Value | Unit |
|-----------|-------|------|
| t_eq_loss | | mm / in |
| t_rem_eq | | mm / in |
| MAWP_pit | | kPa / psi |
| Operating pressure P_op | | kPa / psi |
| Criterion: MAWP_pit ≥ P_op | | Pass / Fail |

**Level 2 Overall Result:** PASS / FAIL

---

### 8.6 Maximum Allowable Working Pressure (MAWP) at Current Condition

```
MAWP_corroded = S × E × t_available / (R_c + 0.6 × t_available)
```

*(Use appropriate head formula if applicable.)*

| Parameter | Value | Unit |
|-----------|-------|------|
| S | | MPa / psi |
| E | | — |
| t_available = t_mm − FCA | | mm / in |
| R_c | | mm / in |
| **MAWP_corroded** | | **kPa / psi** |
| Operating pressure P_op | | kPa / psi |
| MAWP_corroded ≥ P_op? | | Yes / No |

---

### 8.7 Remaining Life and Next Inspection Interval

```
t_remaining_life = (t_available − t_req) / CR
```

| Parameter | Value | Unit |
|-----------|-------|------|
| t_available | | mm / in |
| t_req | | mm / in |
| Corrosion rate CR | | mm/yr |
| **Remaining life** | | **years** |
| Inspection interval (½ remaining life, max per API 510) | | years |
| Next inspection due date | | |

---

## 9. Results Summary

| Assessment Item | Criterion | Actual Value | Result |
|----------------|-----------|--------------|--------|
| t_available ≥ t_min_allow | t_available ≥ t_req | | Pass / Fail |
| RTR ≥ 0.20 (Level 1) | ≥ 0.20 | | Pass / Fail |
| Pit diameter criterion (Level 1) | d ≤ 0.2√(D_c t_nom) | | Pass / Fail |
| Pit spacing criterion (Level 1) | s ≥ 2√(D_c t_nom) | | Pass / Fail |
| RSF_pit ≥ RSF_a (Level 2, if applicable) | ≥ 0.90 | | Pass / Fail |
| MAWP_corroded ≥ P_op | ≥ P_op | | Pass / Fail |

---

## 10. Acceptability Statement

> **Assessment Level:** ________
>
> Based on the API 579-1/ASME FFS-1 Part 6 Level __ assessment, the pitting corrosion on **[Component]** of **[Equipment ID]** is **[ACCEPTABLE / NOT ACCEPTABLE]** for continued operation at the current MAWP of **________ kPa (g) [psi (g)]** and operating temperature of **________ °C [°F]**.
>
> The corroded MAWP is **________ kPa (g) [psi (g)]**, which [exceeds / does not exceed] the operating pressure of **________ kPa (g) [psi (g)]**.

---

## 11. Recommendations

| # | Recommendation | Priority | Target Date |
|---|---------------|----------|-------------|
| 1 | | High / Medium / Low | |
| 2 | | | |
| 3 | | | |

**Recommended inspection method for follow-up:** UT thickness survey / PAUT / AUT / Grid UT

**CMLs to add or revise:** [List by location and method]

**Monitoring:** [Specify if online monitoring, coupon, or periodic UT is recommended]

**Repair options (if not acceptable):**
- Weld repair per ASME VIII-1 and applicable NBIC / jurisdictional requirements
- Overlay / clad repair
- Full or partial shell replacement
- Rerate to reduced MAWP

---

## 12. Inspection Interval or Follow-up Actions

| Item | Value |
|------|-------|
| Half-life date (internal inspection due) | |
| External inspection due | |
| Next API 510 internal inspection | |
| Condition monitoring frequency | |
| Pressure test requirement | Yes / No |
| Operating restrictions pending repair | |

---

## 13. References

- API 579-1/ASME FFS-1, Fitness-For-Service, Edition: _________, Part 6
- ASME Section VIII Division 1, Edition: _________
- ASME Section II Part D, Edition: _________
- API 510, Pressure Vessel Inspection Code, Edition: _________
- API 571, Damage Mechanisms Affecting Fixed Equipment in the Refining Industry, Edition: _________
- Inspection Report No.: _________
- UT Data Sheet No.: _________
- Drawing No.: _________

---

## 14. Signature Block

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Assessed By | | | |
| Reviewed By (API 510 Inspector / CWI) | | | |
| Approved By (Owner-User Engineer) | | | |

---

*This assessment is valid for the stated operating conditions and inspection data only. Any change in service, operating pressure, operating temperature, or discovery of additional damage requires reassessment.*
