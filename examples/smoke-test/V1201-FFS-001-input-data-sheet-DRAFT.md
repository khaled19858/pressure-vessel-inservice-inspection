================================================================================
TEST / DRAFT / NOT FOR ISSUE
This document is a smoke-test example only. All equipment data, personnel names,
measurement values, and site references are FICTIONAL. This document has not been
reviewed or approved and shall not be used for any engineering, operational, or
regulatory purpose.
================================================================================

# FFS Assessment Input Data Sheet
## API 579-1 / ASME FFS-1 -- Pre-Assessment Data Collection

---

## DOCUMENT CONTROL

| Field                  | Entry                                              |
|------------------------|----------------------------------------------------|
| Document Number        | V1201-FFS-001-IDS                                  |
| Revision               | 0 -- DRAFT                                         |
| Date Completed         | [PLACEHOLDER: date of completion]                  |
| Completed By           | [PLACEHOLDER: name and qualification]              |
| Reviewed By            | [PLACEHOLDER: name and qualification]              |
| Plant / Site           | Al-Wadi Refinery (FICTIONAL -- TEST DATA ONLY)     |
| Unit / Process Area    | Crude Distillation Unit (CDU), Train A             |
| Associated FFS Report  | V1201-FFS-001 (DRAFT)                              |

---

## PURPOSE

This sheet collects all required inputs before a formal FFS assessment is
started. Missing data items are identified in the Missing Data Register
(Section 14). Do not proceed to assessment without resolving or formally
accepting each missing data item.

The FFS assessment triggered is for a local thin area (LTA) at CML SC2-06
on Shell Course 2 of V-1201. The assessment covers API 579-1/ASME FFS-1,
Part 5 (Local Metal Loss). An additional concern for HIC/SOHIC (Part 7)
has been flagged and is pending TOFD/PAUT NDE results.

---

## 1. EQUIPMENT IDENTIFICATION

| Field                          | Entry                                              |
|--------------------------------|----------------------------------------------------|
| Equipment Tag / Item Number    | V-1201                                             |
| Equipment Description          | Sour Gas Inlet Separator                           |
| Equipment Type                 | Vertical pressure vessel                           |
| Service / Fluid                | Wet sour hydrocarbon gas/liquid (H2S, CO2, water)  |
| Vessel Orientation             | Vertical                                           |
| Year Fabricated                | [PLACEHOLDER: confirm from nameplate]              |
| Year Placed in Service         | [PLACEHOLDER: confirm from installation records]   |
| Design Code and Edition        | ASME Section VIII Division 1, [PLACEHOLDER: edition from MDR] |
| Manufacturer                   | [PLACEHOLDER: confirm from nameplate]              |
| National Board Number          | [PLACEHOLDER: confirm from nameplate]              |
| Nameplate MAWP                 | [PLACEHOLDER: confirm from nameplate] kPa(g)       |
| Nameplate MDMT                 | [PLACEHOLDER: confirm from nameplate] deg C        |
| Drawing Reference              | V1201-GA-001 Rev 3 (FICTIONAL)                     |
| Inspection History Reference   | [PLACEHOLDER: list all prior inspection report numbers] |

---

## 2. DESIGN DATA

| Parameter                            | Value    | Units  | Source / Document                        |
|--------------------------------------|----------|--------|------------------------------------------|
| Design Pressure (internal)           | 2,500    | kPa(g) | Process design document / drawing        |
| Design Pressure (external, if any)   | N/A      | --     | Not applicable                           |
| Full Vacuum Design?                  | [x] No   |        | Confirm from design records              |
| Design Temperature (maximum)         | 120      | deg C  | Process design document / drawing        |
| Design Temperature (minimum / MDMT)  | [PLACEHOLDER] | deg C | Confirm from nameplate and design records |
| Stamped MDMT                         | [PLACEHOLDER] | deg C | Confirm from nameplate                   |
| Joint Efficiency (E)                 | 1.0      | --     | Full radiography per design records      |
| Radiography Category                 | Full RT  | --     | Design records                           |
| Original Corrosion Allowance (OCA)   | 3.0      | mm     | Drawing V1201-GA-001 (FICTIONAL)         |
| Supplemental loads considered?       | [ ] Yes  [x] No | -- | Wind and seismic loads not considered in this LTA assessment; confirm no supplemental loads govern at this location |
| Wind / seismic loads applicable?     | [ ] Yes  [x] No (for FFS scope only) | -- | Confirm no wind/seismic effect at SC2-06 |
| Cyclic service?                      | [ ] Yes  [x] No | -- | No documented cyclic pressure service; confirm |
| Lethal service?                      | [ ] Yes  [x] No | -- | Toxic (H2S) -- not classified as lethal service per ASME VIII-1 UW-2; confirm with owner/operator |

---

## 3. OPERATING DATA

| Parameter                             | Value                | Units  | Source / Document                   |
|---------------------------------------|----------------------|--------|-------------------------------------|
| Current Operating Pressure            | 2,000 nominal        | kPa(g) | Process design (confirm from DCS)   |
| Maximum Operating Pressure            | [PLACEHOLDER]        | kPa(g) | DCS historian -- MISSING DATA MD-3  |
| Minimum Operating Pressure            | [PLACEHOLDER]        | kPa(g) | DCS historian                       |
| Current Operating Temperature         | 50 nominal           | deg C  | Process design (confirm from DCS)   |
| Maximum Operating Temperature         | [PLACEHOLDER]        | deg C  | DCS historian                       |
| Minimum Operating Temperature         | [PLACEHOLDER]        | deg C  | DCS historian                       |
| Fluid Phase                           | Two-phase gas/liquid | --     | Process description                 |
| Fluid Density (for static head calc)  | [PLACEHOLDER]        | kg/m3  | MISSING DATA MD-4 -- required for static head at SC2-06 |
| Process Chemistry (key parameters)    | H2S present; CO2 present; free water present -- quantitative data MISSING | -- | Process description; lab data MISSING MD-1 and MD-2 |
| Startup / Shutdown conditions noted?  | [x] No (not documented) | -- | [PLACEHOLDER: confirm from procedures] |
| Upset history documented?             | [ ] Yes  [x] No (incomplete) | -- | [PLACEHOLDER: review DCS alarms and logs] |

---

## 4. MATERIAL DATA

| Parameter                          | Value                | Units | Source / Document                   |
|------------------------------------|----------------------|-------|-------------------------------------|
| Material Specification             | SA-516               | --    | Drawing / MDR                       |
| Grade / UNS Number                 | Grade 70             | --    | Drawing / MDR                       |
| Product Form                       | Plate                | --    | Drawing / MDR                       |
| Heat Treatment Condition           | [PLACEHOLDER]        | --    | MDR -- MISSING DATA MD-5            |
| PWHT Applied                       | [x] Unknown -- CRITICAL MISSING DATA MD-5 | | Fabrication records required |
| Impact Tested                      | [x] Unknown          | --    | CMTRs -- MISSING DATA MD-6          |
| Impact Test Temperature            | [PLACEHOLDER]        | deg C | CMTRs -- MISSING DATA MD-6          |
| Allowable Stress at Design Temp (S)| [PLACEHOLDER]        | MPa   | ASME II Part D, Table 1-A -- MISSING DATA MD-7; code edition must be confirmed |
| Allowable Stress at Op. Temp       | [PLACEHOLDER]        | MPa   | ASME II Part D, Table 1-A -- MISSING DATA MD-7 |
| Yield Strength (Sy) at Temp        | [PLACEHOLDER]        | MPa   | ASME II Part D for SA-516 Gr 70    |
| Ultimate Tensile Strength (Su)     | [PLACEHOLDER]        | MPa   | ASME II Part D for SA-516 Gr 70    |
| Young's Modulus (E_mat) at Temp    | [PLACEHOLDER]        | GPa   | ASME II Part D for SA-516 Gr 70    |
| Fracture Toughness (KIC or MAT)    | Not required at Level 1 Part 5 | -- | If SOHIC / crack-like flaw confirmed, KIC becomes required for Part 7 or Part 9 |
| Fracture toughness basis           | Not applicable at this level | -- | See note above |
| Cladding / overlay material        | None confirmed       | --    | Drawing / MDR                       |

CRITICAL NOTE: The allowable stress S is required for the t_req calculation
in the FFS report (V1201-FFS-001). It SHALL be taken from the current edition
of ASME Section II Part D, Table 1-A, at the appropriate assessment temperature.
It SHALL NOT be assumed or estimated. The code edition used must match the
edition applicable to the vessel's design code of record where practicable,
or the current edition if a more conservative result is obtained. Document the
specific code edition and table used when this value is confirmed.

---

## 5. GEOMETRY

| Parameter                          | Value                | Units | Source / Document                   |
|------------------------------------|----------------------|-------|-------------------------------------|
| Inside Diameter (nominal)          | 1,500                | mm    | Drawing V1201-GA-001 (FICTIONAL)    |
| Outside Diameter (nominal)         | 1,500 + 2 x 22.0 = 1,544 (nominal) | mm | Calculated from ID and t_nom; confirm from drawing |
| Nominal Wall Thickness             | 22.0                 | mm    | Drawing V1201-GA-001 (FICTIONAL)    |
| Mill under-tolerance               | [PLACEHOLDER]        | mm    | Material specification for SA-516   |
| Minimum as-ordered thickness       | [PLACEHOLDER]        | mm    | Purchase order / mill order records |
| Head Type                          | 2:1 Ellipsoidal      | --    | Drawing V1201-GA-001 (FICTIONAL)    |
| Head Crown Radius (L)              | N/A (ellipsoidal)    | mm    | --                                  |
| Head Knuckle Radius (r)            | N/A (ellipsoidal)    | mm    | --                                  |
| Cone Half-Apex Angle (alpha)       | N/A                  | deg   | --                                  |
| Total Shell / Head Length (T-T)    | [PLACEHOLDER]        | mm    | Drawing V1201-GA-001 (FICTIONAL) -- required for static head calculation |
| Weld Joint Type at Flaw Location   | [PLACEHOLDER]        | --    | Drawing -- confirm whether SC2-06 is near a longitudinal or circumferential weld |
| Nozzle details at flaw location    | N/A (shell zone, no nozzle at SC2-06) | -- | Confirm from drawing |
| Reinforcement pad                  | N/A at flaw location | --    | Confirm from drawing                |

---

## 6. CORROSION ALLOWANCE

| Parameter                              | Value          | Units | Basis                                 |
|----------------------------------------|----------------|-------|---------------------------------------|
| Original Corrosion Allowance (OCA)     | 3.0            | mm    | Drawing V1201-GA-001 (FICTIONAL)      |
| Corrosion Allowance Used to Date       | [PLACEHOLDER]  | mm    | t_nominal - t_measured = 22.0 - [PLACEHOLDER] |
| Remaining Original CA                  | [PLACEHOLDER]  | mm    | OCA - CA used to date                 |
| Future Corrosion Allowance (FCA)       | [PLACEHOLDER]  | mm    | MISSING DATA MD-8; CR x remaining interval |
| FCA basis (interval x rate)            | [PLACEHOLDER]  | --    | Pending corrosion rate (MD-9)         |
| Planning corrosion rate used for FCA   | [PLACEHOLDER]  | mm/yr | MISSING DATA MD-9                     |
| FCA basis: rate source                 | [PLACEHOLDER]  | --    | MISSING DATA -- see MD-9              |

**Corrosion rate source:**  [ ] Measured short-term   [ ] Measured long-term   [ ] Estimated   [ ] Literature   [x] Unknown
-- MISSING DATA MD-9: insufficient inspection history for a measured rate.
   Two UT data points at the same CML with known elapsed time are required.
   Currently only one inspection data point exists at CML SC2-06.
   An interim estimated rate from process/materials engineering shall be used
   as a conservative interim planning value pending the second data point.

---

## 7. INSPECTION READINGS

### 7.1 UT Thickness Readings

| Reading ID | CML ID | Location Description                   | Component | Clock Position | t_nominal (mm) | t_measured (mm) | t_minimum (mm) | t_required (mm) | Date Measured | Instrument / Probe | Inspector |
|------------|--------|----------------------------------------|-----------|----------------|----------------|-----------------|----------------|-----------------|---------------|--------------------|-----------|
| R-01       | SC2-06 | SC-2, 6 o'clock, ~2400 mm from BTL    | Shell SC-2 | 06:00         | 22.0           | [PLACEHOLDER -- ALERT] | [PLACEHOLDER min of all R-xx readings in zone] | [PLACEHOLDER from FFS Step 1] | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] |
| R-02       | SC2-06 | Adjacent above SC2-06                  | Shell SC-2 | 06:00         | 22.0           | [PLACEHOLDER]   | --             | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] |
| R-03       | SC2-06 | Adjacent below SC2-06                  | Shell SC-2 | 06:00         | 22.0           | [PLACEHOLDER]   | --             | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] |
| R-04       | SC2-06 | Adjacent circumferential (3 o'clock of zone) | Shell SC-2 | 03:00   | 22.0           | [PLACEHOLDER]   | --             | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] |
| R-05       | SC2-06 | Adjacent circumferential (9 o'clock of zone) | Shell SC-2 | 09:00   | 22.0           | [PLACEHOLDER]   | --             | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] |

NOTE: Minimum t_measured in the LTA zone is [PLACEHOLDER] mm at reading [PLACEHOLDER].
A close-interval grid (spacing [PLACEHOLDER] mm) is required to map the LTA extent.

**UT method:**  [x] Contact A-scan   [ ] Immersion   [ ] Phased Array UT   [ ] Other
NOTE: Contact A-scan is used for thickness at CML grid points. A-scan is NOT
adequate for HIC/SOHIC detection. TOFD or PAUT angle-beam is required additionally.

**Calibration reference:**
[PLACEHOLDER: document calibration block number, material, and calibration date]

**Reading repeatability / uncertainty:**
[PLACEHOLDER: document multiple readings at SC2-06 and report range of readings.
Velocity anomaly at this CML must be documented in the UT data sheet.]

### 7.2 Profile Radiography or Other Mapping Data

| Scan ID | Location    | Scan Type | Min. Thickness Found | Area of Damage (approx.) | Date | Reference |
|---------|-------------|-----------|----------------------|--------------------------|------|-----------|
| --      | SC2-06 zone | TOFD/PAUT (PENDING) | [PLACEHOLDER -- not yet performed] | [PLACEHOLDER] | [PLACEHOLDER] | V1201-NDE-[PLACEHOLDER] |

NOTE: TOFD or PAUT scan of the SC2-06 zone and adjacent weld HAZ is PENDING.
Results will update this data sheet when available. The FFS assessment (Part 5)
cannot be concluded until the HIC/SOHIC question is resolved by this NDE.

---

## 8. FLAW DIMENSIONS

| Flaw ID | Flaw Type     | Location          | Component  | Nearest Weld (distance) | Length (2c or l) | Depth (a) | Width (s) | Area       | Orientation | NDE Method Used |
|---------|---------------|-------------------|------------|------------------------|-----------------|-----------|-----------|------------|-------------|-----------------|
| LTA-001 | Local metal loss (LTA) | SC-2, 06:00, ~2400 mm from BTL | Shell SC-2 | [PLACEHOLDER -- CRITICAL] | [PLACEHOLDER] | [PLACEHOLDER: = t_nom - t_min_meas] | [PLACEHOLDER] | [PLACEHOLDER] | N/A (area of metal loss) | UT A-scan grid (to be supplemented by TOFD/PAUT) |

**Flaw characterization basis:**
UT A-scan thickness grid at CML SC2-06 and adjacent readings. LTA axial and
circumferential extent has not been fully characterized. A close-interval UT
grid survey of the SC2-06 zone (proposed 50 mm x 50 mm grid or closer) is
required to fully map the LTA boundary.

**Flaw sizing uncertainty:**
High. Current characterization is based on spot UT readings only. LTA extent
could be significantly larger or smaller than implied by the available readings.
Close-interval grid mapping is required.

---

## 9. NDE METHOD AND COVERAGE

| NDE Method Used | Coverage Achieved       | Standard Reference | Inspector Qualification | Date | Report Reference |
|-----------------|-------------------------|--------------------|------------------------|------|-----------------|
| UT A-scan (thickness) | CML grid per inspection plan | [PLACEHOLDER: NDE procedure no.] | [PLACEHOLDER: Level II UT, SNT-TC-1A or equivalent] | [PLACEHOLDER] | [PLACEHOLDER: inspection report no.] |
| TOFD or PAUT   | PENDING -- not yet performed | -- | -- | -- | PENDING |

**Coverage limitations or access restrictions:**
[PLACEHOLDER: document any insulation on SC-2, scaffold requirements, and
surface condition (scale, deposits) affecting UT coupling]

**NDE indications not yet characterized:**  [x] Yes
-- Velocity anomaly at CML SC2-06 requires TOFD/PAUT follow-up for HIC/SOHIC
   assessment. This is a CRITICAL outstanding item.

---

## 10. DAMAGE TYPE CLASSIFICATION

**Primary Damage Type:**
- [x] Local thin area (LTA)

**API 579-1 Part applicable to primary damage:**
Part 5 -- Assessment of Local Metal Loss

**Secondary damage types identified:**
- Possible HIC/SOHIC (suspected based on UT velocity anomaly; NOT YET CONFIRMED)
  -- Part 7 will be added to scope if confirmed by TOFD/PAUT
- Possible pitting within LTA zone (not yet confirmed; to be evaluated at internal inspection)
  -- Part 6 will be added to scope if confirmed

---

## 11. TEMPERATURE AND PRESSURE (ASSESSMENT SPECIFIC)

| Parameter                              | Value          | Units  |
|----------------------------------------|----------------|--------|
| Assessment temperature (metal temp)    | 120            | deg C  |
| Assessment pressure (governing)        | 2,500          | kPa(g) |
| Static head pressure at flaw location  | [PLACEHOLDER]  | kPa    |
| Total pressure at flaw location        | [PLACEHOLDER]  | kPa(g) |

NOTE: The assessment temperature is the maximum design temperature (120 deg C)
as the allowable stress basis. The governing assessment pressure is the design
pressure (2,500 kPa(g)) plus static head contribution.

Static head at CML SC2-06 (approximately 2,400 mm from BTL, vertical vessel):
   P_sh = rho x g x h
   rho = [PLACEHOLDER] kg/m3 (fluid density -- MISSING DATA MD-4)
   g   = 9.81 m/s2
   h   = [PLACEHOLDER] m (height of liquid column above SC2-06 elevation;
         depends on normal liquid level set point -- confirm from process data)
   P_sh = [PLACEHOLDER] kPa (MISSING DATA)

Total assessment pressure P_total = 2,500 + [PLACEHOLDER] = [PLACEHOLDER] kPa(g)

---

## 12. WELD DETAILS

| Parameter                          | Entry                                              |
|------------------------------------|----------------------------------------------------|
| Is flaw at or near a weld?         | [x] Unknown -- confirm from drawing and field check |
| Weld joint type                    | [PLACEHOLDER: confirm from drawing -- long. or circ. seam?] |
| Weld joint category (per code)     | [PLACEHOLDER: Category A or B per ASME VIII-1]     |
| Joint efficiency at flaw location  | 1.0 (full RT, applied uniformly -- confirm for seam at SC2-06) |
| Weld examined at fabrication?      | [x] Unknown -- [PLACEHOLDER: confirm from MDR]     |
| Weld RT / UT type at fabrication   | Full RT per design records; confirm from MDR        |
| PWHT of weld joint                 | [x] Unknown -- CRITICAL MISSING DATA MD-5          |
| Distance of flaw from weld toe     | [PLACEHOLDER -- MISSING DATA: measure in field]    |
| Distance of flaw from weld centerline | [PLACEHOLDER -- MISSING DATA: measure in field] |

NOTE: Distance of LTA from nearest weld is a CRITICAL parameter for Part 5
Level 1 screening criteria. This dimension MUST be measured in the field and
confirmed from the drawing before the Level 1 criteria can be applied.

---

## 13. TOUGHNESS AND CYCLIC SERVICE SCREENING

**Toughness screening required?**  [ ] Yes   [x] No (for Part 5 Level 1 LTA assessment)
-- If SOHIC or crack-like flaw is confirmed by TOFD/PAUT, toughness screening
   becomes required for Part 7 or Part 9 assessment.

**Basis for toughness requirement:**
Not required for Part 5 (local metal loss) Level 1 assessment. Required if
Part 7 or Part 9 scope is added.

| Parameter                          | Value          | Units  | Source                              |
|------------------------------------|----------------|--------|-------------------------------------|
| Minimum operating temperature      | [PLACEHOLDER]  | deg C  | DCS / process data                  |
| MDMT (stamped or calculated)       | [PLACEHOLDER]  | deg C  | Nameplate -- MISSING DATA           |
| Reference temperature              | N/A at this level | --  | Not required for Part 5 Level 1     |
| Charpy impact energy               | [PLACEHOLDER]  | J      | CMTRs -- MISSING DATA MD-6          |
| KIC or equivalent                  | N/A at this level | --  | Not required for Part 5 Level 1     |

**Brittle fracture concern:**  [ ] Yes   [ ] No   [x] Screening required if HIC/SOHIC confirmed

**Cyclic service screening:**

| Parameter                             | Value          | Units  | Source            |
|---------------------------------------|----------------|--------|-------------------|
| Number of full pressure cycles        | [PLACEHOLDER]  | --     | DCS historian     |
| Operating temperature cycles (range)  | [PLACEHOLDER]  | --     | DCS historian     |
| Startup / shutdown cycles per year    | [PLACEHOLDER]  | --     | Operations records |
| Fatigue assessment required?          | [x] Screening required -- confirm cycle count | | |

NOTE: Cyclic service screening should be completed before concluding this
assessment. If significant pressure cycling is identified, a fatigue life
check may be required.

---

## 14. MISSING DATA REGISTER

List every input required for the assessment that is not available. Each item
must be resolved before the FFS assessment in V1201-FFS-001 is finalized.

| Item No. | Required Input                               | Why Required                                    | Current Status | Proposed Resolution                            | Responsible Party   | Target Date   |
|----------|----------------------------------------------|-------------------------------------------------|----------------|------------------------------------------------|---------------------|---------------|
| MD-1     | H2S concentration (mol% or ppmv)             | NACE MR0175 screening; HIC/SSC driving force     | MISSING        | Obtain from latest process lab sample          | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-2     | CO2 concentration (mol% or ppmv)             | CO2 corrosion rate basis                         | MISSING        | Obtain from latest process lab sample          | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-3     | Maximum operating pressure (from DCS)        | Confirm assessment pressure basis                | MISSING        | DCS historian review                           | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-4     | Fluid density at operating conditions        | Static head calculation at SC2-06 elevation      | MISSING        | Process engineering / PVT data                 | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-5     | PWHT status (applied / not applied)          | SSC and SOHIC susceptibility; weld details       | MISSING        | Fabrication data report (MDR) review           | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-6     | Impact test results (CMTRs)                  | MDMT confirmation; toughness screening           | MISSING        | Retrieve CMTRs from material file              | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-7     | Allowable stress S for SA-516 Gr 70          | t_req and MAWP calculations; code edition must be confirmed | MISSING | ASME II Part D, Table 1-A; confirm code edition | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-8     | Future corrosion allowance (FCA)             | t_available and MAWP at end of interval          | MISSING        | Depends on MD-9 (corrosion rate)               | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-9     | Measured corrosion rate at CML SC2-06        | Remaining life; FCA; inspection interval         | MISSING        | Second UT data point at next inspection        | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-10    | LTA dimensions: length and width of LTA zone | Part 5 Level 1 or Level 2 screening criteria     | MISSING        | Close-interval UT grid map of SC2-06 zone      | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-11    | Distance from LTA to nearest weld             | Part 5 Level 1 structural discontinuity criteria | MISSING        | Drawing review and field measurement            | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-12    | TOFD / PAUT results for SC2-06 and HAZ       | Exclude or confirm HIC/SOHIC                     | PENDING NDE    | Schedule TOFD/PAUT at next inspection          | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-13    | Vessel total height (T-T)                    | Static head column height for vertical vessel     | MISSING        | Drawing V1201-GA-001 (to be confirmed)          | [PLACEHOLDER]       | [PLACEHOLDER] |
| MD-14    | Normal liquid level set point in V-1201      | Static head height above CML SC2-06             | MISSING        | Process operations / instrumentation records   | [PLACEHOLDER]       | [PLACEHOLDER] |

**Missing data items that could materially affect the assessment outcome:**
MD-7 (allowable stress S): determines t_req and MAWP.
MD-9 (corrosion rate): determines remaining life and inspection interval.
MD-10 (LTA dimensions): determines whether Level 1 screening criteria are met.
MD-11 (distance to weld): determines Level 1 structural discontinuity criterion.
MD-12 (TOFD/PAUT): if HIC/SOHIC is confirmed, Part 7 assessment supersedes Part 5.

---

## 15. ASSUMPTIONS

1. Design pressure of 2,500 kPa(g) and joint efficiency of 1.0 are taken from
   process design documentation. These shall be confirmed from the nameplate and
   MDR before this data sheet is approved.
2. Inside diameter of 1,500 mm and nominal shell thickness of 22.0 mm are taken
   from the drawing. No field verification has been performed.
3. The LTA at CML SC2-06 is assumed to be attributable to aqueous corrosion
   (general metal loss) unless HIC/SOHIC is confirmed by TOFD/PAUT. This is a
   PROVISIONAL assumption.
4. No mill undertolerance deduction has been applied to nominal thickness because
   the mill order records are not available. This is conservative if the actual
   as-delivered thickness was at or above nominal.
5. The vessel is not in cyclic service based on available information.
   This assumption shall be confirmed from DCS cycle count records.
6. The assessment temperature for allowable stress lookup is taken as the
   maximum design temperature (120 deg C) as a conservative basis.

---

## 16. REVIEWER SIGN-OFF

The undersigned confirms that this data sheet has been reviewed, that inputs are
traceable to the sources noted, that missing data items have been identified, and
that the data sheet is suitable to proceed with FFS assessment subject to
resolution of MISSING DATA items listed in Section 14.

| Role                          | Name | Signature | Date |
|-------------------------------|------|-----------|------|
| Data Sheet Prepared By        | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Data Sheet Reviewed By        | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Assessment Engineer Acceptance| [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |

---

*Template reference: API 579-1/ASME FFS-1, current edition. Completeness and
accuracy of this data sheet directly affects the validity of the subsequent FFS
assessment. This template does not substitute for engineering judgment.*

================================================================================
TEST / DRAFT / NOT FOR ISSUE
Smoke-test example document V1201-FFS-001-IDS -- Al-Wadi Refinery (FICTIONAL)
All data is fictional and for template demonstration only.
================================================================================
