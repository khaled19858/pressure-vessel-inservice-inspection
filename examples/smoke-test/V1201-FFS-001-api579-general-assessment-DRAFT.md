================================================================================
TEST / DRAFT / NOT FOR ISSUE
This document is a smoke-test example only. All equipment data, personnel names,
measurement values, and site references are FICTIONAL. This document has not been
reviewed or approved and shall not be used for any engineering, operational, or
regulatory purpose. Calculations are incomplete pending resolution of MISSING
DATA items listed in Section 8 and in the associated Input Data Sheet
V1201-FFS-001-IDS (DRAFT).
================================================================================

# API 579-1 / ASME FFS-1 Fitness-For-Service Assessment Report
## General Assessment Template

---

## DOCUMENT CONTROL

| Field                  | Entry                                              |
|------------------------|----------------------------------------------------|
| Document Number        | V1201-FFS-001                                      |
| Revision               | 0 -- DRAFT                                         |
| Date                   | [PLACEHOLDER: date of issue]                       |
| Prepared By            | [PLACEHOLDER: name and qualification]              |
| Reviewed By            | [PLACEHOLDER: name and qualification]              |
| Approved By            | [PLACEHOLDER: name and qualification]              |
| Plant / Site           | Al-Wadi Refinery (FICTIONAL -- TEST DATA ONLY)     |
| Unit / Process Area    | Crude Distillation Unit (CDU), Train A             |
| Supersedes             | N/A -- original issue                              |
| Next Review / Expiry   | [PLACEHOLDER: determine from remaining life result] |

---

## 1. EXECUTIVE SUMMARY

**Equipment Item:**
V-1201, Sour Gas Inlet Separator, Al-Wadi Refinery (FICTIONAL), CDU Train A.
Vertical pressure vessel, ASME Section VIII Division 1.

**Assessment Trigger:**
Local thin area (LTA) detected at CML SC2-06 during UT thickness survey.
Minimum measured thickness at this location is [PLACEHOLDER: t_meas mm] against
nominal wall thickness of 22.0 mm with original corrosion allowance of 3.0 mm.
A possible UT velocity anomaly at this location raises the question of
HIC/SOHIC in addition to general metal loss. An engineering review was
initiated. This FFS assessment addresses the local metal loss component.
HIC/SOHIC characterization is addressed separately (see Recommendation Note
V1201-REC-001, DRAFT).

**Damage Type:**
Local metal loss (local thin area); possible contribution from HIC-related
material degradation -- HIC not yet confirmed (pending TOFD/PAUT scan).

**Assessment Part (API 579-1/ASME FFS-1):**
Part 5 -- Local Metal Loss (Local Thin Area)

NOTE: If HIC or SOHIC is confirmed by follow-up NDE (TOFD/PAUT), the
assessment scope will expand to include Part 7 (Hydrogen Blistering, HIC, SOHIC).
This assessment is conditional on the LTA being attributable to general metal
loss only. The assessment SHALL NOT be concluded until HIC/SOHIC has been
formally assessed or excluded.

**Assessment Level:**  [x] Level 1   [ ] Level 2   [ ] Level 3
(Level 1 attempted. Level 2 may be required depending on LTA geometry inputs
-- see Step 3 in Section 11. Level selection cannot be finalized until LTA
dimensions are confirmed from inspection data.)

**Finding:**
[PLACEHOLDER: cannot be stated until t_req is calculated and LTA dimensions
are characterized. See Sections 7 and 11 for calculation workflow.]

**Acceptability:**
[ ] Acceptable for continued operation
[ ] Not acceptable
[ ] Acceptable with restrictions

PLACEHOLDER -- acceptability cannot be determined until all missing data items
in the Input Data Sheet (V1201-FFS-001-IDS, DRAFT) are resolved and calculations
in Section 11 are completed.

**Key Restrictions or Conditions (if any):**
[PLACEHOLDER: to be determined from assessment results]

**Remaining Life Estimate:**
[PLACEHOLDER: requires confirmed corrosion rate -- see Missing Data Register,
Section 8]

**Recommended Action:**
[PLACEHOLDER: to be finalized following completion of calculations and HIC/SOHIC
NDE results]

**Next Required Assessment or Inspection Date:**
[PLACEHOLDER: to be determined from remaining life result]

---

## 2. EQUIPMENT DATA

| Field                          | Entry                                              |
|--------------------------------|----------------------------------------------------|
| Equipment Tag / Item Number    | V-1201                                             |
| Equipment Description          | Sour Gas Inlet Separator                           |
| Equipment Type                 | Vertical pressure vessel                           |
| Service / Fluid                | Wet sour hydrocarbon gas/liquid (H2S, CO2, water)  |
| Vessel Orientation             | Vertical                                           |
| Year Fabricated / Installed    | [PLACEHOLDER: confirm from nameplate and records]  |
| Design Code                    | ASME Section VIII Division 1                       |
| Code Edition / Addenda         | [PLACEHOLDER: confirm from Manufacturer Data Report] |
| Manufacturer                   | [PLACEHOLDER: confirm from nameplate]              |
| National Board Number          | [PLACEHOLDER: confirm from nameplate]              |
| P&ID Reference                 | P&ID-CDU-A-101 (FICTIONAL)                         |
| Drawing Reference              | V1201-GA-001 Rev 3 (FICTIONAL)                     |

---

## 3. ASSESSMENT SCOPE

**Location of Flaw or Damage:**
Shell Course 2 (SC-2), 6 o'clock position, approximately 2,400 mm from
bottom tangent line (BTL). CML designation: SC2-06.

**Component Assessed:**  [x] Shell   [ ] Head   [ ] Nozzle   [ ] Other

**Assessment boundary:**
This assessment covers the local thin area at CML SC2-06 and the surrounding
zone in Shell Course 2. The assessment does not cover Shell Course 1, heads,
nozzles, or any other components unless findings at those locations trigger
separate assessment. Bottom head is excluded from this assessment scope.

**Driving reason for assessment:**
- [x] Thickness below original CA limit (confirmed or suspected at SC2-06)
- [ ] Flaw or crack detected
- [ ] Pitting or local metal loss (possible but not confirmed as primary mechanism)
- [ ] Blistering / HIC / SOHIC (suspected but not confirmed -- separate NDE required)
- [ ] General metal loss beyond original CA
- [ ] Post-upset evaluation
- [x] Other: Possible UT velocity anomaly at CML SC2-06 during routine survey

---

## 4. DAMAGE MECHANISM

**Primary Damage Mechanism:**
Local metal loss attributed to aqueous corrosion in wet sour hydrocarbon service
(H2S, CO2, and free water in contact with carbon steel shell). General CO2/H2S
aqueous corrosion producing area-averaged thinning with possible localized
acceleration.

**API 571 / API 579 Classification:**
General/local metal loss; aqueous corrosion; wet H2S damage family (HIC/SOHIC
to be confirmed or excluded by TOFD/PAUT -- see Assessment Scope, Section 3).

**Description of how damage manifests for this equipment:**
Aqueous CO2 and H2S corrosion produces general thinning of the carbon steel
shell, accelerated at the liquid/vapor interface, at low points, and in zones
of high turbulence. The 6 o'clock position at approximately 2,400 mm from BTL
places CML SC2-06 in the lower portion of the upper shell course, consistent
with accumulated aqueous phase and a region susceptible to general corrosion
and pitting. The possible UT velocity anomaly suggests a layered or cracked
microstructure that could indicate HIC, warranting TOFD/PAUT follow-up.

**Active or historical:**  [x] Active   [ ] Historical   [ ] Unknown

**Expected progression rate:**
[PLACEHOLDER: planning corrosion rate not established (insufficient UT history
at this CML). Estimated rate per process/materials engineering input:
[PLACEHOLDER] mm/yr. This is a CRITICAL MISSING DATA item.]

---

## 5. ASSESSMENT LEVEL SELECTION

| Factor                          | Assessment Level Selected | Basis                                              |
|---------------------------------|--------------------------|-----------------------------------------------------|
| Data availability               | Level 1 attempted         | Minimum data required; some inputs still MISSING    |
| Complexity of damage            | Level 1 / 2 (TBD)        | LTA dimensions not yet fully characterized          |
| Access to required inputs       | Level 1 (partial)         | t_meas available; LTA extent, S, and CR are MISSING |
| Governing API 579 Part          | Part 5                    | Local metal loss (LTA)                              |

**Assessment Part selected (API 579-1/ASME FFS-1):**
Part 5 -- Assessment of Local Metal Loss

**Justification for assessment level:**
Level 1 is the starting point per API 579 Part 5 because it requires minimum
data (principal flaw dimensions and wall thickness). Level 2 will be required
if Level 1 screening criteria are not met or if the LTA is near a weld.

**Limitations of selected level:**
Level 1 does not account for the interaction of multiple damage mechanisms.
If HIC/SOHIC is confirmed, a Level 2 or Level 3 assessment per Part 7 will
supersede this assessment. Level 1 Part 5 also does not account for pitting
superimposed on the LTA.

---

## 6. APPLICABLE ASSESSMENT PART SELECTION

- [ ] Part 4 - General Metal Loss
- [x] Part 5 - Local Metal Loss (primary -- LTA at CML SC2-06)
- [ ] Part 6 - Pitting Corrosion
- [ ] Part 7 - Hydrogen Blistering, HIC, SOHIC, and HTHA
         NOTE: Part 7 to be added to scope if HIC/SOHIC confirmed by TOFD/PAUT
- [ ] Part 8 - Weld Misalignment and Shell Distortions
- [ ] Part 9 - Crack-Like Flaws
- [ ] Part 10 - Creep Damage
- [ ] Part 11 - Fire Damage
- [ ] Part 12 - Dent and Gouge
- [ ] Part 13 - Laminations
         NOTE: to be evaluated if velocity anomaly at SC2-06 is confirmed to
         represent a lamination rather than HIC
- [ ] Part 14 - Fatigue Damage

**Secondary Parts considered:**
Part 4 (general metal loss) -- if LTA is shown to be widespread, upgrade to Part 4.
Part 6 (pitting) -- if pitting is confirmed within the LTA zone at internal inspection.
Part 7 (HIC/SOHIC) -- pending TOFD/PAUT results.

---

## 7. INPUT DATA

### 7.1 Design Data

| Parameter                      | Value   | Units   | Source                                |
|--------------------------------|---------|---------|---------------------------------------|
| Design Pressure (internal)     | 2,500   | kPa(g)  | Process design / nameplate            |
| Design Pressure (external)     | N/A     | --      | Not applicable                        |
| Design Temperature (max)       | 120     | deg C   | Process design / nameplate            |
| Design Temperature (min / MDMT)| [PLACEHOLDER] | deg C | Confirm from nameplate             |
| Joint Efficiency (E)           | 1.0     | --      | Full radiography per design records   |
| Original Corrosion Allowance   | 3.0     | mm      | Drawing V1201-GA-001 (FICTIONAL)      |
| Radiography Category           | Full RT | --      | Design records                        |

### 7.2 Operating Data

| Parameter                     | Value              | Units   | Source                              |
|-------------------------------|--------------------|---------|-------------------------------------|
| Current Operating Pressure    | 2,000 nominal      | kPa(g)  | Process design (confirm from DCS)   |
| Maximum Operating Pressure    | [PLACEHOLDER]      | kPa(g)  | Confirm maximum excursion from DCS  |
| Current Operating Temperature | 50 nominal         | deg C   | Process design (confirm from DCS)   |
| Maximum Operating Temperature | [PLACEHOLDER]      | deg C   | Confirm from DCS                    |
| Fluid Phase                   | Two-phase gas/liquid | --    | Process description                 |

### 7.3 Geometry

| Parameter                | Value                | Units | Source                              |
|--------------------------|----------------------|-------|-------------------------------------|
| Inside Diameter (nominal)| 1,500                | mm    | Drawing V1201-GA-001 (FICTIONAL)    |
| Nominal Wall Thickness   | 22.0                 | mm    | Drawing V1201-GA-001 (FICTIONAL)    |
| Head Type                | 2:1 Ellipsoidal      | --    | Drawing V1201-GA-001 (FICTIONAL)    |
| Weld Joint Type at SC2-06 | [PLACEHOLDER: confirm if near a seam weld] | -- | Drawing review required |
| Orientation              | Vertical             | --    | Equipment identification            |

### 7.4 Material Data

| Parameter                         | Value                | Units | Source                              |
|-----------------------------------|----------------------|-------|-------------------------------------|
| Material Specification            | SA-516               | --    | Drawing / MDR                       |
| Grade / UNS                       | Grade 70             | --    | Drawing / MDR                       |
| Allowable Stress at Temp (S)      | [PLACEHOLDER]        | MPa   | ASME II Part D, Table 1-A, current edition; value depends on code edition -- DO NOT ESTIMATE |
| Yield Strength (Sy)               | [PLACEHOLDER]        | MPa   | ASME II Part D for SA-516 Gr 70     |
| Ultimate Tensile Strength (Su)    | [PLACEHOLDER]        | MPa   | ASME II Part D for SA-516 Gr 70     |
| Fracture Toughness (KIC or MAT)   | Not required for Part 5 Level 1 | -- | N/A at this level |
| PWHT Applied                      | [PLACEHOLDER -- CRITICAL MISSING DATA] | -- | Fabrication records |
| Impact Tested                     | [PLACEHOLDER]        | --    | MDR / CMTRs                         |

NOTE: The allowable stress (S) for SA-516 Gr 70 at the assessment temperature
shall be taken from the current applicable edition of ASME Section II Part D,
Table 1-A. This value SHALL NOT be assumed or estimated in this document. It
must be obtained from the appropriate code table and documented with the code
edition reference.

### 7.5 Inspection Readings

| CML / Reading ID | Location             | t_measured (mm) | t_minimum (mm) | t_required (mm) | Date Measured | Method          |
|------------------|----------------------|-----------------|----------------|-----------------|---------------|-----------------|
| SC2-06           | SC-2, 6 o'clock, ~2400 mm from BTL | [PLACEHOLDER -- ALERT] | [PLACEHOLDER: minimum of all readings in zone] | [PLACEHOLDER: from Section 11 Step 1] | [PLACEHOLDER] | UT A-scan contact |
| SC2-06-adj-A     | Adjacent to SC2-06 (above) | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] | UT A-scan |
| SC2-06-adj-B     | Adjacent to SC2-06 (below) | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] | UT A-scan |
| SC2-06-adj-C     | Adjacent to SC2-06 (circumferential) | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] | UT A-scan |

### 7.6 Flaw / Damage Dimensions

| Parameter                  | Value          | Units | Source                              |
|----------------------------|----------------|-------|-------------------------------------|
| Flaw Length (2c or l)      | [PLACEHOLDER]  | mm    | Grid UT mapping of LTA zone         |
| Flaw Depth (a)             | [PLACEHOLDER]  | mm    | Minimum measured thickness reading  |
| Flaw Width (s)             | [PLACEHOLDER]  | mm    | Grid UT mapping of LTA zone         |
| Damage Area                | [PLACEHOLDER]  | mm2   | Grid UT mapping                     |
| Local / General Extent     | [PLACEHOLDER]  | --    | To be determined from grid UT       |
| Distance to nearest weld   | [PLACEHOLDER]  | mm    | Drawing review and measurement in field |
| Distance to structural disc| [PLACEHOLDER]  | mm    | Drawing review                      |

NOTE: LTA dimensions are CRITICAL MISSING DATA items. A close-interval UT grid
(100 mm x 100 mm or closer) is required to map the LTA extent before the Part 5
assessment criteria can be applied.

---

## 8. ASSUMPTIONS

1. Design pressure of 2,500 kPa(g) and joint efficiency of 1.0 are taken from
   process design documentation and drawing records. These shall be confirmed
   from the nameplate and MDR before this assessment is finalized.
2. Inside diameter of 1,500 mm is taken from the drawing. No field measurement
   of actual inside diameter has been performed.
3. Original corrosion allowance of 3.0 mm is taken from the drawing.
4. Future corrosion allowance (FCA) for the remaining inspection interval is set
   at [PLACEHOLDER: FCA = CR x interval] and is a MISSING DATA item pending
   confirmed corrosion rate.
5. The local thin area at CML SC2-06 is attributed to general aqueous corrosion.
   This assumption is CONDITIONAL on HIC/SOHIC being excluded by TOFD/PAUT NDE.
   If HIC or SOHIC is confirmed, this assessment is superseded.
6. Joint efficiency E = 1.0 applies uniformly to the assessment zone unless a
   weld seam runs through the LTA zone (confirm from drawing).

---

## 9. REQUIRED THICKNESS OR ALLOWABLE CONDITION BASIS

**Code basis for required thickness calculation:**
ASME Section VIII Division 1, UG-27(c)(1) -- cylindrical shell under internal pressure.
Static head contribution per CLAUDE.md rule: vertical vessel, use vessel height as
static head liquid column. Static head contribution at CML SC2-06 location
(approximately 2,400 mm from BTL) from the liquid above this point is
[PLACEHOLDER: calculate from fluid density and height of liquid above CML location].
Total assessment pressure = design pressure + static head at CML SC2-06 elevation.

**Formula reference:**
ASME VIII-1, UG-27(c)(1):

   t_req = P_total x R_c / (S x E - 0.6 x P_total)

where:
   P_total = design pressure + static head contribution at flaw location [kPa converted to MPa]
   R_c     = corroded inside radius = R_i + FCA [mm]
   R_i     = nominal inside radius = D_i / 2 = 1500 / 2 = 750 mm
   S       = allowable stress at assessment temperature [MPa -- per ASME II Part D, PLACEHOLDER]
   E       = weld joint efficiency = 1.0

**Variables used:**

| Variable   | Symbol    | Value                | Units | Source                                     |
|------------|-----------|----------------------|-------|--------------------------------------------|
| Design pressure | P_d  | 2,500               | kPa(g) | Design document                           |
| Static head at CML elevation | P_sh | [PLACEHOLDER] | kPa  | Vertical vessel; fluid density x g x h_liquid_above_CML |
| Total assessment pressure | P_total | [PLACEHOLDER] | MPa | P_d + P_sh, converted to MPa            |
| Inside radius (nominal) | R_i | 750              | mm    | D_i / 2 = 1500 / 2                        |
| Future corrosion allowance | FCA | [PLACEHOLDER] | mm   | CR x remaining interval -- MISSING DATA    |
| Corroded inside radius | R_c | [PLACEHOLDER]   | mm    | R_i + FCA                                 |
| Allowable stress | S   | [PLACEHOLDER]        | MPa   | ASME II Part D, Table 1-A, for SA-516 Gr 70 at assessment temp -- PLACEHOLDER |
| Joint efficiency | E  | 1.0                  | --    | Full radiography                           |

**Required minimum thickness (t_required):**

   t_required = [PLACEHOLDER: cannot be calculated until S and P_total and R_c are established]

IMPORTANT NOTE FOR REVIEWER: The required thickness calculation above cannot be
completed in this DRAFT document because:
(a) The allowable stress S is not known (code edition not confirmed).
(b) The future corrosion allowance FCA is not known (corrosion rate missing).
(c) The static head contribution is not known (fluid density missing).
These are all listed in the Missing Data Register in the associated Input Data
Sheet V1201-FFS-001-IDS (DRAFT).

**Basis:**
UG-27(c)(1), cylindrical shell under internal pressure, using corroded inside
radius per CLAUDE.md convention.

---

## 10. INSPECTION DATA SUPPORTING THE ASSESSMENT

**NDE method(s) used to characterize the damage:**
UT A-scan contact thickness measurement. Possible velocity anomaly noted at
SC2-06 -- may indicate HIC/SOHIC or lamination (not yet characterized).

**Date of inspection:**
[PLACEHOLDER: confirm from inspection records]

**Inspector qualification:**
[PLACEHOLDER: confirm API 510 certification number and expiry]

**Coverage achieved:**
[PLACEHOLDER: describe UT grid spacing and area covered at SC2-06 zone]

**Repeatability / uncertainty in readings:**
[PLACEHOLDER: document instrument calibration, probe type, and reading repeatability
for the SC2-06 zone. Multiple readings at this CML -- record all readings, not just
minimum.]

**Reference standard / acceptance criteria applied in the field:**
[PLACEHOLDER: document the NDE procedure number and calibration block reference]

**As-found condition description:**
CML SC2-06 at Shell Course 2, 6 o'clock position, approximately 2,400 mm from
BTL recorded a minimum measured thickness of [PLACEHOLDER] mm against nominal
22.0 mm. This represents a measured loss of [PLACEHOLDER] mm from nominal.
Adjacent CML readings in the same zone ranged from [PLACEHOLDER] to [PLACEHOLDER] mm.
A possible UT velocity anomaly was noted at this location during the survey,
flagged as requiring further evaluation (see CML flag notation in UT data sheet
reference [PLACEHOLDER]).

---

## 11. CALCULATION WORKFLOW

### Step 1: Establish Required Thickness

```
Formula (ASME VIII-1, UG-27(c)(1)):

   t_req = P_total x R_c / (S x E - 0.6 x P_total)

Variables:
   P_total = [PLACEHOLDER] MPa  (design pressure + static head at CML SC2-06 elevation)
   R_c     = 750 + [FCA -- PLACEHOLDER] mm
   S       = [PLACEHOLDER] MPa  (from ASME II Part D, current edition, SA-516 Gr 70 at design temp)
   E       = 1.0

Substitution:
   t_req = [PLACEHOLDER] x [PLACEHOLDER] / ([PLACEHOLDER] x 1.0 - 0.6 x [PLACEHOLDER])

Result:
   t_req = [PLACEHOLDER] mm

NOTE: This calculation CANNOT be completed in this DRAFT because S and FCA are
MISSING DATA. The structure of the calculation is shown to allow the reviewer
to verify the approach once inputs are available.
```

### Step 2: Characterize the Damage

```
LTA classification (API 579-1, Part 5):

LTA located at SC-2, 6 o'clock, ~2400 mm from BTL.
This location is [PLACEHOLDER: in liquid zone / splash zone / gas zone -- confirm].

Minimum measured thickness (t_mm) at CML SC2-06 = [PLACEHOLDER] mm

Minimum remaining thickness available for pressure design (t_available):
   t_available = t_mm - FCA = [PLACEHOLDER] - [PLACEHOLDER] = [PLACEHOLDER] mm

Critical dimensions for LTA (required for Part 5 Level 1 screening):
   LTA length (l, axial) = [PLACEHOLDER] mm (from grid UT mapping -- MISSING)
   LTA width (s, circumferential) = [PLACEHOLDER] mm (from grid UT mapping -- MISSING)

Distance from nearest weld = [PLACEHOLDER] mm (MISSING -- confirm from drawing
and field measurement)

NOTE: LTA dimensions are MISSING DATA. A close-interval UT grid map of the
SC2-06 zone is required before Step 3 can be completed.
```

### Step 3: Assess Remaining Thickness or Flaw Tolerance

```
API 579-1/ASME FFS-1, Part 5, Level 1 screening criteria:

Criterion 1 -- Minimum remaining thickness:
   t_available >= t_req

   t_available = [PLACEHOLDER] mm
   t_req       = [PLACEHOLDER] mm (from Step 1)
   Result: [PLACEHOLDER -- cannot evaluate until Step 1 is complete]

Criterion 2 -- Distance from structural discontinuity:
   The LTA shall not be located within 1.8 * sqrt(R_c * t_mm) of a weld seam
   or structural discontinuity (per API 579-1, Part 5 Level 1 requirements).

   1.8 * sqrt([PLACEHOLDER] * [PLACEHOLDER]) = [PLACEHOLDER] mm
   Distance to nearest weld = [PLACEHOLDER] mm
   Result: [PLACEHOLDER -- MISSING DATA]

NOTE: The specific Level 1 screening criteria and their numerical limits are
defined in API 579-1/ASME FFS-1, Part 5. The criteria SHALL be applied from
the current edition of the standard and SHALL NOT be reproduced from memory.
Do not fill in criterion limits without referencing the current standard.

Overall Level 1 Screening: [PLACEHOLDER -- incomplete]

If Level 1 fails or cannot be completed, proceed to Level 2 (API 579-1, Part 5).
Level 2 uses the Remaining Strength Factor (RSF) methodology requiring LTA
dimensions as inputs. Level 2 calculations are not shown in this DRAFT.
```

### Step 4: MAWP Determination (if required)

```
MAWP at current corroded / damaged condition (shell, cylindrical, UG-27(c)(1)):

   MAWP_corroded = S x E x t_available / (R_c + 0.6 x t_available)

Variables:
   S           = [PLACEHOLDER] MPa
   E           = 1.0
   t_available = t_mm - FCA = [PLACEHOLDER] mm
   R_c         = 750 + FCA = [PLACEHOLDER] mm

Result:
   MAWP_corroded = [PLACEHOLDER] MPa = [PLACEHOLDER] kPa(g)

Current operating pressure = 2,000 kPa(g)
MAWP_corroded >= 2,000 kPa(g)? [PLACEHOLDER -- cannot evaluate until inputs confirmed]

NOTE: This calculation cannot be completed in this DRAFT.
```

### Step 5: Remaining Life (if applicable)

```
Remaining life from corrosion allowance:

   RL = (t_available - t_req) / CR

Variables:
   t_available = [PLACEHOLDER] mm
   t_req       = [PLACEHOLDER] mm (from Step 1)
   CR          = [PLACEHOLDER] mm/yr (MISSING DATA -- see Input Data Sheet MD-7)

Result:
   RL = [PLACEHOLDER] years

Inspection interval (per API 510, not to exceed lesser of RL/2 or max interval):
   RL/2 = [PLACEHOLDER] years
   Next inspection due = [PLACEHOLDER] (date)

NOTE: Remaining life cannot be calculated in this DRAFT because the corrosion
rate is a MISSING DATA item.
```

---

## 12. RESULTS

| Result Parameter                        | Value          | Units   | Accept?        |
|-----------------------------------------|----------------|---------|----------------|
| Required minimum thickness (t_req)      | [PLACEHOLDER]  | mm      | N/A (input)    |
| Minimum measured thickness (t_meas)     | [PLACEHOLDER]  | mm      | N/A (measured) |
| Available corrosion allowance remaining | [PLACEHOLDER]  | mm      | [PLACEHOLDER]  |
| MAWP at current condition               | [PLACEHOLDER]  | kPa(g)  | [PLACEHOLDER]  |
| Design / operating pressure             | 2,500 / 2,000  | kPa(g)  | N/A (input)    |
| Remaining life (calculated)             | [PLACEHOLDER]  | years   | N/A            |
| FCA (future corrosion allowance)        | [PLACEHOLDER]  | mm      | N/A (input)    |
| Life limited by (CR, flaw, other)       | [PLACEHOLDER]  | --      | N/A            |

NOTE: All result values are PLACEHOLDERS. This results table cannot be populated
until the missing data items listed in the Input Data Sheet are resolved.

---

## 13. SENSITIVITY CHECKS

Describe the sensitivity of the result to key uncertain inputs.

| Input Parameter   | Nominal Value      | Varied To    | Effect on Result           | Significance |
|-------------------|--------------------|--------------|----------------------------|--------------|
| Corrosion rate CR | [PLACEHOLDER]      | [PLACEHOLDER] | Direct effect on RL        | High         |
| Allowable stress S | [PLACEHOLDER]     | +/- 5%       | Linear effect on t_req     | Medium       |
| FCA               | [PLACEHOLDER]      | +/- 1.0 mm   | Effect on t_available and MAWP | Medium   |
| LTA length        | [PLACEHOLDER]      | [PLACEHOLDER] | Drives Level 1 vs Level 2 boundary | High |

**Overall sensitivity assessment:**
[PLACEHOLDER: cannot assess sensitivity until nominal values are established.
Corrosion rate and LTA dimensions are the highest-sensitivity inputs for this
assessment.]

---

## 14. MAWP IMPACT

**Original design MAWP:**
[PLACEHOLDER: confirm stamped MAWP from nameplate]

**MAWP at current corroded or damaged condition:**
[PLACEHOLDER: see Step 4 in Section 11]

**Reduction in MAWP:**
[PLACEHOLDER: cannot determine until MAWP calculation in Step 4 is completed]

**Current operating pressure vs. revised MAWP:**
[ ] Within limit   [ ] Exceeds revised limit
PLACEHOLDER -- evaluation pending

**Rerating required:**  [ ] Yes   [ ] No
PLACEHOLDER -- evaluation pending

---

## 15. ACCEPTABILITY STATEMENT

Based on the assessment performed:

[ ] ACCEPTABLE for continued operation at current operating conditions without restriction.

[ ] ACCEPTABLE for continued operation subject to the following restrictions and conditions.

[ ] NOT ACCEPTABLE for continued operation. Repair, rerating, or retirement is required.

[x] ACCEPTABILITY CANNOT BE DETERMINED -- Missing data items must be resolved
    before this assessment can be concluded. See Sections 7, 8, and 11, and the
    associated Input Data Sheet V1201-FFS-001-IDS (DRAFT).

ADDITIONALLY: This assessment is conditional on HIC/SOHIC being excluded by
TOFD/PAUT NDE of the SC2-06 zone and adjacent weld HAZ. If HIC or SOHIC is
confirmed, Part 7 assessment is required and this assessment is superseded.

**Applicable API 579 Part and Level:**
Part 5 -- Local Metal Loss, Level 1 (attempted; incomplete)

**Date through which acceptability applies (if life-limited):**
[PLACEHOLDER: to be determined from remaining life calculation]

---

## 16. LIMITATIONS

1. This assessment is INCOMPLETE. All result values are placeholders. This
   document shall not be used to make any run/repair/replace decision.
2. The assessment is conditional on HIC/SOHIC exclusion. If HIC or SOHIC is
   confirmed by follow-up NDE, this FFS report is superseded by a Part 7
   assessment and must be revised.
3. LTA dimensions have not been confirmed by close-interval grid UT. The LTA
   extent assumed for screening is based on the single CML SC2-06 reading only.
   This may understate or overstate the actual LTA geometry.
4. The corrosion rate used in the remaining life calculation is estimated, not
   measured. The remaining life result will have high uncertainty until a second
   UT data point is obtained at the next inspection.
5. Static head contribution has been noted as required per CLAUDE.md but the
   fluid density is a MISSING DATA item and the static head calculation cannot
   be completed.
6. Pitting within the LTA zone has not been characterized. If pitting is found
   during internal inspection, Part 6 (pitting assessment) must be added to scope.

---

## 17. RECOMMENDATIONS

| Priority | Action                                             | Basis                                | Target Date    | Responsible Party |
|----------|----------------------------------------------------|--------------------------------------|----------------|-------------------|
| 1 -- Immediate | Conduct TOFD or PAUT scan of SC2-06 zone and all liquid-zone welds in SC-2 | Exclude or confirm HIC/SOHIC; cannot conclude FFS without this | Before returning to service / next inspection | [PLACEHOLDER] |
| 2 -- Immediate | Confirm PWHT status from fabrication records       | Critical for SSC/SOHIC susceptibility | Before FFS conclusion | [PLACEHOLDER] |
| 3 -- High  | Obtain process chemistry data (H2S, CO2, pH, density) | Required for static head, rate, and mechanism review | [PLACEHOLDER] | [PLACEHOLDER] |
| 4 -- High  | Conduct close-interval UT grid of SC2-06 zone to map LTA extent | Required to complete Level 1 / Level 2 screening | Next inspection / turnaround | [PLACEHOLDER] |
| 5 -- High  | Obtain second UT data point at all shell CMLs to establish measured corrosion rate | Required for remaining life and interval | Next inspection | [PLACEHOLDER] |

**Follow-up inspection recommended:**  [x] Yes

**Follow-up inspection method:**
TOFD or PAUT for HIC/SOHIC; close-interval UT grid for LTA characterization;
UT A-scan at all CMLs for corrosion rate establishment.

**Follow-up inspection interval:**
[PLACEHOLDER: to be determined from remaining life result]

**Repair or rerating required:**  [ ] Yes   [ ] No   [x] Under evaluation

---

## 18. APPROVAL BLOCK

| Role                          | Name | Signature | Date |
|-------------------------------|------|-----------|------|
| Prepared By                   | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Technically Reviewed By       | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Approved By                   | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Client / Owner Acceptance     | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |

---

*Template reference: API 579-1/ASME FFS-1, current edition. All assessment
procedures, acceptance criteria, and remaining life calculations shall be
performed in accordance with the current edition of API 579-1/ASME FFS-1 and
the engineer's documented judgment. This template does not substitute for
engineering analysis.*

================================================================================
TEST / DRAFT / NOT FOR ISSUE
Smoke-test example document V1201-FFS-001 -- Al-Wadi Refinery (FICTIONAL)
All data is fictional and for template demonstration only.
================================================================================
