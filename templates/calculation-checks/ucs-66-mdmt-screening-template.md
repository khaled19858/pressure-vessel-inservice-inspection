# ASME Section VIII Division 1 - MDMT / Impact Test Exemption Screening (UCS-66)

**CONTROLLED DOCUMENT - SCREENING WORKSHEET.**
This worksheet structures the toughness / minimum design metal temperature (MDMT)
screening for carbon and low-alloy steel pressure components per ASME Section VIII
Division 1, Part UCS. It records the procedure and the inputs/outputs. It does
**not** reproduce the UCS-66 exemption curves, the UCS-66 figure values, or the
UCS-66.1 reduction values: those shall be read directly from the controlling code
edition. Do not enter curve temperatures or reduction values from memory.

This worksheet covers UCS materials only. For other material groups (e.g., UHA
austenitic stainless steels under UHA-51, UNF non-ferrous, UHT) use the applicable
Part and its impact-test rules.

---

## 1. Document Control

| Field | Entry |
|---|---|
| Document No. | |
| Revision | |
| Date | |
| Equipment Tag No. | |
| Component(s) screened | |
| Code Edition / Addenda | ASME Section VIII Division 1, Edition: _______ |
| Prepared By | |
| Checked By | |
| Approved By | |

---

## 2. Required MDMT (service basis)

| Parameter | Value | Unit | Source |
|---|---|---|---|
| Minimum design metal temperature required by service | | degC / degF | process / data sheet / lowest expected metal temp |
| Includes upset / depressuring / autorefrigeration cases? | [ ] Yes [ ] No | - | identify cases below |
| Governing low-temperature case | | - | |

> The **required MDMT** is the coldest metal temperature the component must tolerate
> at a coincident pressure, including startup, shutdown, upset, and any
> autorefrigeration or depressuring scenario. The screening must demonstrate the
> permitted MDMT is at or below this required value.

---

## 3. Component and material data (per component)

Complete one row per material/component (shell, each head, nozzles, flanges,
reinforcing pads, etc.). MDMT is established for **each** pressure component; the
warmest permitted MDMT among them governs the vessel unless treated by component.

| Component | Material spec / grade | UCS-66 curve (A/B/C/D) | Governing thickness (UCS-66 basis) | Nominal thk | Notes |
|---|---|---|---|---|---|
| Shell | | | | | |
| Top head | | | | | |
| Bottom head | | | | | |
| Nozzle(s) | | | | | |
| Flanges / bolting | | | | | |

> **Curve assignment:** assign each material to exemption curve A, B, C, or D per
> the material list and notes in UCS-66. Do not assume a curve; read it from the
> code for the exact specification, grade, and product form.
>
> **Governing thickness:** determine the governing thickness for each welded part
> per the UCS-66 definition of governing thickness (it accounts for the controlling
> thickness at welds and is not always the nominal plate thickness). Read the
> definition from the controlling edition.

---

## 4. Step 1 - Exemption without impact testing

Check the exemption paths in the controlling edition and mark which, if any, apply:

- [ ] **UG-20(f) exemption** — the component meets all of the UG-20(f) conditions
  (material, thickness, service, and temperature conditions as listed in the code).
  If every condition is met, impact testing is not required by this path. Record
  the basis. Do not apply UG-20(f) unless **all** stated conditions are satisfied.
- [ ] **UCS-66(a) / Figure UCS-66 exemption** — using the assigned curve and the
  governing thickness, the permitted MDMT read from Figure UCS-66 is at or below
  the required MDMT (before or after any Step 2 reduction).
- [ ] **Other exemption provision in UCS-66** (e.g., specific thickness/temperature
  provisions). Cite the clause.

If an exemption path is fully satisfied, record it in Section 7 and impact testing
is not required by that path.

---

## 5. Step 2 - MDMT from Figure UCS-66 and reduction per UCS-66.1

For each component not otherwise exempt:

1. **Base permitted MDMT** — read from Figure UCS-66 using the assigned curve and
   the governing thickness. Record the value read (do not interpolate from memory).

2. **Coincident ratio for reduction** — compute the ratio used by UCS-66(b) /
   Figure UCS-66.1. In general terms this ratio compares the required thickness
   (for pressure, adjusted for E) to the available nominal thickness less
   corrosion allowance, i.e. a measure of how lightly stressed the component is at
   the coincident condition. Use the exact ratio definition and stress basis from
   the controlling edition.

3. **Temperature reduction** — read the permitted reduction from Figure UCS-66.1
   using the computed ratio. Apply it to the base permitted MDMT to obtain the
   adjusted permitted MDMT.

| Component | Base permitted MDMT (Fig UCS-66) | Coincident ratio | Reduction (Fig UCS-66.1) | Adjusted permitted MDMT |
|---|---|---|---|---|
| Shell | | | | |
| Top head | | | | |
| Bottom head | | | | |
| Nozzle(s) | | | | |

> Record the figure/clause and the values **as read from the code**. Enter the
> ratio definition and any limits (e.g., maximum permitted reduction) from the
> controlling edition.

---

## 6. Step 3 - Optional additional credits (verify applicability)

- [ ] **UCS-68(c) PWHT credit** — where postweld heat treatment is applied and is
  **not** otherwise required by the rules, UCS-68(c) permits a reduction in the
  MDMT for the applicable materials (historically a 17 degC (30 degF) reduction for
  the eligible P-No. 1 material groups). Confirm eligibility, the exact reduction,
  and any conditions in the controlling edition before taking this credit.

| Credit applied | Clause | Reduction taken | Resulting permitted MDMT |
|---|---|---|---|
| | | | |

---

## 7. Result and disposition

| Component | Required MDMT | Permitted MDMT (after Steps 1-3) | Permitted <= Required? | Impact testing required? |
|---|---|---|---|---|
| Shell | | | [ ] Yes [ ] No | [ ] Yes [ ] No |
| Top head | | | [ ] Yes [ ] No | [ ] Yes [ ] No |
| Bottom head | | | [ ] Yes [ ] No | [ ] Yes [ ] No |
| Nozzle(s) | | | [ ] Yes [ ] No | [ ] Yes [ ] No |

**Governing component (warmest permitted MDMT):** ___________

**Vessel MDMT disposition:** [ ] Acceptable for required MDMT without impact testing
[ ] Impact testing required (specify materials/components) [ ] Operating
restriction or further evaluation required

> If the permitted MDMT for any component is warmer than the required MDMT and no
> further credit applies, the component requires impact testing per UG-84, an
> operating restriction (minimum pressurizing temperature / coincident
> pressure-temperature limit), a material change, or an FFS brittle-fracture
> assessment per API 579-1/ASME FFS-1 Part 3.

---

## 8. Assumptions and limitations

| No. | Item |
|---|---|
| 1 | This is an MDMT/impact-exemption **screening** worksheet, not a substitute for the full UCS-66/UCS-66.1 evaluation against the controlling edition. |
| 2 | Curve assignments, figure values, and reduction values are read from the code; none are reproduced here as fixed values. |
| 3 | Covers UCS (carbon and low-alloy steel) materials only. Other material Parts use their own impact rules. |
| 4 | The required MDMT must reflect all credible low-temperature cases, including upset and autorefrigeration, at coincident pressure. |
| 5 | For existing equipment, confirm whether the original construction code edition or a current evaluation basis applies. |

---

## 9. Approval Block

| Role | Name | Signature | Date |
|---|---|---|---|
| Prepared By | | | |
| Checked By | | | |
| Approved By (Engineer of Record) | | | |

---

*Governed by ASME Section VIII Division 1, Part UCS (UCS-66, UCS-66.1, UCS-68,
UG-20(f), UG-84). Read all curve assignments, figure values, and reduction values
from the controlling edition. Do not enter code chart values from memory.*
