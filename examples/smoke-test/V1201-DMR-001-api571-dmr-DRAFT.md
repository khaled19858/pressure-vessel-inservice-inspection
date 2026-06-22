================================================================================
TEST / DRAFT / NOT FOR ISSUE
This document is a smoke-test example only. All equipment data, personnel names,
measurement values, and site references are FICTIONAL. This document has not been
reviewed or approved and shall not be used for any engineering, operational, or
regulatory purpose.
================================================================================

# API 571 Damage Mechanism Review
## Pressure Vessels and Pressure-Boundary Equipment

---

## DOCUMENT CONTROL

| Field                  | Entry                                              |
|------------------------|----------------------------------------------------|
| Document Number        | V1201-DMR-001                                      |
| Revision               | 0 -- DRAFT                                         |
| Date                   | [PLACEHOLDER: date of issue]                       |
| Prepared By            | [PLACEHOLDER: name and qualification]              |
| Reviewed By            | [PLACEHOLDER: name and qualification]              |
| Approved By            | [PLACEHOLDER: name and qualification]              |
| Plant / Site           | Al-Wadi Refinery (FICTIONAL -- TEST DATA ONLY)     |
| Unit / Process Area    | Crude Distillation Unit (CDU), Train A             |
| Supersedes             | N/A -- original issue                              |
| Next Review Due        | [PLACEHOLDER: determine per inspection plan]       |

---

## 1. EQUIPMENT IDENTIFICATION

| Field                        | Entry                                              |
|------------------------------|----------------------------------------------------|
| Equipment Tag / Item Number  | V-1201                                             |
| Equipment Description        | Sour Gas Inlet Separator                           |
| Equipment Type               | Vertical pressure vessel, two-phase gas/liquid     |
| Year Installed / Fabricated  | [PLACEHOLDER: confirm from nameplate and records]  |
| Design Code                  | ASME Section VIII Division 1                       |
| Manufacturer                 | [PLACEHOLDER: confirm from nameplate]              |
| National Board Number        | [PLACEHOLDER: confirm from nameplate]              |
| Vessel Orientation           | Vertical                                           |
| Drawing Reference            | V1201-GA-001 Rev 3 (FICTIONAL)                     |

---

## 2. PROCESS AND SERVICE DESCRIPTION

**Service / Fluid:**
Wet sour hydrocarbon gas and associated liquids. Two-phase (gas/liquid) separation
of crude overhead vapors. H2S is present. CO2 is present. Free water is present at
operating conditions (wet sour service per NACE MR0175 criteria -- confirmed by
process description; quantitative H2S and pH data are MISSING DATA items).

**Process Function:**
V-1201 receives sour gas from the crude distillation column overhead and separates
entrained liquid from the gas phase prior to downstream gas treating.

**Upset or Abnormal Conditions:**
[PLACEHOLDER: document known process upsets, slugging events, water hammer history,
and any known H2S exceedances from DCS historian.]

**Startup / Shutdown Conditions:**
[PLACEHOLDER: document steam-out practice (relevant to polythionic acid SCC
screening for any stainless steel internals), cooldown rate, and pressurization
procedure.]

**Injection Points or Chemical Additions:**
[PLACEHOLDER: confirm whether corrosion inhibitor, antifoam, or other chemicals
are injected upstream of V-1201. Chemical injection points require dedicated CML
coverage.]

**Connected Equipment:**
Inlet from CDU overhead line. Outlet vapor to sour gas treating unit. Liquid
outlet to [PLACEHOLDER: confirm destination]. Boot drain to [PLACEHOLDER].

---

## 3. MATERIALS OF CONSTRUCTION

| Component              | Material Specification | Grade / UNS | Heat Treatment        | Notes                                  |
|------------------------|------------------------|-------------|-----------------------|----------------------------------------|
| Shell                  | SA-516                 | Grade 70    | [PLACEHOLDER: N or SR?] | PWHT status CRITICAL MISSING DATA    |
| Heads                  | SA-516                 | Grade 70    | [PLACEHOLDER: N or SR?] | 2:1 Ellipsoidal                      |
| Nozzles                | [PLACEHOLDER]          | [PLACEHOLDER] | [PLACEHOLDER]       | Confirm from fabrication drawing       |
| Internals              | [PLACEHOLDER]          | [PLACEHOLDER] | N/A                 | Confirm type and material              |
| Cladding / Overlay     | None confirmed         | N/A           | N/A                 | [PLACEHOLDER: verify -- no cladding assumed] |
| Fasteners              | [PLACEHOLDER]          | [PLACEHOLDER] | [PLACEHOLDER]       | Confirm from bill of materials         |
| Gaskets                | [PLACEHOLDER]          | [PLACEHOLDER] | N/A                 | Confirm type for wet H2S service       |

**Weld Filler Metal:**
[PLACEHOLDER: confirm from weld procedure records and CMTR. Critical for SSC
susceptibility assessment in wet H2S service.]

**PWHT Applied:**  [ ] Yes   [ ] No   [x] Unknown
-- NOTE: PWHT status is a CRITICAL MISSING DATA item for this assessment.
   PWHT is required by NACE MR0175 for certain carbon steel welds in wet H2S
   service. Absence of PWHT significantly increases SSC and SOHIC susceptibility.
   Confirm from fabrication data report before finalizing this DMR.

**Impact Tested:**  [ ] Yes   [ ] No   [x] Unknown
-- [PLACEHOLDER: confirm from Manufacturer Data Report (MDR) and CMTRs.]

---

## 4. OPERATING CONDITIONS

### 4.1 Design Conditions

| Parameter                  | Value   | Units     |
|----------------------------|---------|-----------|
| Design Pressure (internal) | 2,500   | kPa(g)    |
| Design Pressure (external) | N/A     | --        |
| Design Temperature (max)   | 120     | deg C     |
| Design Temperature (min)   | [PLACEHOLDER: confirm MDMT from nameplate] | deg C |
| MDMT Stamped               | [PLACEHOLDER: confirm from nameplate]      | deg C |
| Joint Efficiency           | 1.0     | --        |
| Corrosion Allowance (OCA)  | 3.0     | mm        |

### 4.2 Normal Operating Conditions

| Parameter              | Value                               | Units   |
|------------------------|-------------------------------------|---------|
| Operating Pressure     | 2,000 nominal                       | kPa(g)  |
| Operating Temperature  | 50 nominal                          | deg C   |
| Flow Rate              | [PLACEHOLDER: confirm from process data] | --  |
| Phase                  | Two-phase gas/liquid                | --      |

NOTE: Operating conditions stated above are NOMINAL values from process design
documents. Actual operating ranges, including maximum excursions, shall be
confirmed from DCS historian records before finalizing this DMR.

### 4.3 Process Chemistry

| Parameter              | Value                          | Units | Source / Date                        |
|------------------------|--------------------------------|-------|--------------------------------------|
| H2S Content            | [PLACEHOLDER -- CRITICAL]      | mol%  | [PLACEHOLDER: latest lab sample date] |
| CO2 Content            | [PLACEHOLDER]                  | mol%  | [PLACEHOLDER]                        |
| HCl / Chloride Level   | [PLACEHOLDER]                  | ppmw  | [PLACEHOLDER]                        |
| pH                     | [PLACEHOLDER -- CRITICAL]      | --    | [PLACEHOLDER]                        |
| Water / Moisture       | Free water present             | --    | Process description                  |
| Oxygen Content         | Not expected -- [PLACEHOLDER: confirm] | ppmv | Process description             |
| Amine Type / Conc.     | None expected -- [PLACEHOLDER: confirm] | -- | Process description             |
| H2 Partial Pressure    | Not applicable at low temperature | --  | Screening judgment                   |
| Sulfur Content         | [PLACEHOLDER]                  | wt%   | [PLACEHOLDER]                        |
| Other                  | [PLACEHOLDER: check for HCN, mercaptans if applicable] | -- | -- |

**Chemistry data quality:**  [ ] Measured   [ ] Estimated   [x] Unknown
-- NOTE: Chemistry data is a CRITICAL MISSING DATA item. All wet H2S damage
   mechanism susceptibility ratings in this review are PROVISIONAL pending
   receipt of confirmed process chemistry data with dates. This DMR SHALL NOT
   be finalized without confirmed chemistry data.

---

## 5. DAMAGE MECHANISM SCREENING TABLE

Use this table to record each mechanism evaluated. Assign susceptibility per the
criteria in API 571. Susceptibility ratings below are PROVISIONAL pending
confirmation of chemistry data (see Section 4.3).

| #  | Damage Mechanism (API 571)              | Credible | Susceptibility | Basis for Decision                                          |
|----|------------------------------------------|----------|----------------|-------------------------------------------------------------|
| 1  | HIC (Hydrogen-Induced Cracking)          | [x]      | H (provisional) | Wet H2S service, CS, free water; susceptibility pending PWHT confirmation |
| 2  | SOHIC (Stress-Oriented HIC)              | [x]      | H (provisional) | Wet H2S, CS welds and HAZ; PWHT unknown -- critical gap     |
| 3  | Hydrogen blistering                      | [x]      | H (provisional) | Wet H2S, CS shell and heads; free water confirmed           |
| 4  | Sulfide stress cracking (SSC)            | [x]      | M (provisional) | Wet H2S, CS; susceptibility reduced if PWHT; PWHT unknown  |
| 5  | General corrosion (CO2/H2S aqueous)      | [x]      | H              | Wet sour service, CS, aqueous phase; confirmed by service   |
| 6  | Pitting corrosion                        | [x]      | M              | H2S/CO2 environment; liquid/vapor interface; low-point zones |
| 7  | Erosion-corrosion                        | [x]      | M              | Two-phase impingement at inlet nozzle; confirm velocity     |
| 8  | Corrosion under insulation (CUI)         | [x]      | L--M           | Insulation status [PLACEHOLDER]; operating temp ~50 deg C   |
| 9  | Microbiologically influenced corrosion   | [x]      | L              | Water phase present; stagnant low-point zones possible      |
| 10 | HTHA (High-Temp Hydrogen Attack)         | [ ]      | N              | Operating temp 50 deg C; design temp 120 deg C; below Nelson curve threshold for CS |
| 11 | Creep                                    | [ ]      | N              | Temperature well below creep range for carbon steel          |
| 12 | Polythionic acid SCC                     | [ ]      | N              | No sensitized austenitic SS identified in vessel shell or heads |
| 13 | Chloride SCC                             | [ ]      | N              | Carbon steel shell; not susceptible to chloride SCC          |
| 14 | Amine stress corrosion cracking          | [ ]      | N (pending)    | No amine in feed confirmed; reassess if amine detected       |
| 15 | Thermal fatigue                          | [ ]      | N (pending)    | No rapid thermal cycling documented; reassess if steam-out is practiced |

**Susceptibility key:**  H = High   M = Medium   L = Low   N = Not susceptible

---

## 6. CREDIBLE DAMAGE MECHANISMS

---

### Mechanism 1: Hydrogen-Induced Cracking (HIC)

**API 571 Classification:**
Hydrogen-induced cracking (HIC); environment-assisted cracking; wet H2S damage family.

**Description:**
Atomic hydrogen generated by the corrosion of carbon steel in wet H2S environments
enters the steel and diffuses to internal defects (inclusions, laminations). Hydrogen
recombines at these sites forming molecular hydrogen at high local pressure, causing
planar cracks parallel to the plate surface. HIC does not require external stress.

**Affected Components / Locations:**
Shell courses SC-1 and SC-2, particularly in the liquid zone and at the liquid/vapor
interface. Bottom head. Boot/sump. Welds and HAZ are not the primary sites for
classical HIC (HAZ cracking is more associated with SOHIC and SSC), but base metal
quality (low sulfur, Ca-treated steel) is critical.

**Susceptibility Factors Present:**
- [x] Fluid / environment: H2S present; free water present; wet sour service
- [x] Material susceptibility: SA-516 Gr 70 carbon steel; HIC resistance depends
      on sulfur content and steel cleanliness; [PLACEHOLDER: confirm steel grade
      and heat specification -- was HIC-resistant plate (low S, Ca-treated, per
      NACE MR0175 or NACE TM0284) specified at fabrication?]
- [ ] Temperature range: temperature not a strong driver for HIC; relevant at
      ambient and low-temperature ranges (current operating temp in range)
- [x] Stress condition: not required for HIC (distinguishes from SOHIC/SSC)
- [x] Other: Free water at operating conditions confirmed; H2S partial pressure
      quantification PENDING (see Section 4.3)

**Susceptibility Level:**  [x] High (provisional)

**Typical Morphology / Location:**
Step-wise cracking in plate base metal parallel to the rolling direction.
Most common in regions exposed to aqueous phase (below liquid/vapor interface)
and at low points where water accumulates.

**Evidence from Inspection History:**
[PLACEHOLDER: review all prior inspection reports for UT velocity anomalies,
TOFD or PAUT scans, or visual evidence of blistering. This is a MISSING DATA item.]

**Evidence from Process Chemistry:**
H2S confirmed present in process stream. Free water phase confirmed.
Quantitative H2S and pH data MISSING (see Section 4.3).

**Rate Estimate or Trend:**
[PLACEHOLDER: HIC is not a thickness-loss mechanism. Detection requires volumetric
NDE methods capable of detecting planar defects parallel to the surface, such as
TOFD, PAUT, or shear-wave UT. RT (radiography) is generally not effective for
detecting HIC laminar cracking.]

**CML Evidence:**
[PLACEHOLDER: review CML SC2-06 UT velocity anomaly flagged in current inspection
round -- investigate whether this represents HIC or lamination.]

**NDE Evidence:**
[PLACEHOLDER: current inspection UT data shows possible velocity anomaly at
CML SC2-06. TOFD or PAUT scan of the affected zone is recommended before
concluding on HIC presence or absence.]

**Active or Potential:**  [x] Active (presumed, pending NDE confirmation)

---

### Mechanism 2: Stress-Oriented HIC (SOHIC)

**API 571 Classification:**
Stress-oriented hydrogen-induced cracking (SOHIC); wet H2S damage family.

**Description:**
SOHIC occurs when HIC cracks align and propagate through-wall under the influence
of applied or residual stress, particularly at welds and heat-affected zones.
SOHIC can cause rapid through-wall cracking in HAZ regions and is more dangerous
than classical HIC because it can progress toward a throughwall leak or rupture.

**Affected Components / Locations:**
Welds and heat-affected zones on shell courses and heads, particularly:
- Longitudinal welds in the liquid zone
- Circumferential (girth) welds
- Nozzle-to-shell welds in the liquid zone
- Any weld where PWHT was not applied or was inadequate

**Susceptibility Factors Present:**
- [x] Fluid / environment: wet H2S service (same as HIC)
- [x] Stress condition: HIGH -- residual weld stresses are the primary driver;
      PWHT status UNKNOWN -- this is the critical susceptibility question
- [x] Material susceptibility: carbon steel weld HAZ
- [x] Other: if PWHT was NOT applied, susceptibility is significantly elevated

**Susceptibility Level:**  [x] High (provisional -- pending PWHT confirmation)

**Typical Morphology / Location:**
Through-thickness step-wise cracking at or adjacent to weld HAZ, typically
perpendicular to the weld line in its overall orientation but with individual
HIC cracks at staggered depths. Can appear as through-wall cracks in severe cases.

**Evidence from Inspection History:**
[PLACEHOLDER: no documented SOHIC findings in inspection history reviewed.
History is incomplete -- see Section 9.]

**Evidence from Process Chemistry:**
Wet H2S service confirmed (quantitative data PENDING).

**Rate Estimate or Trend:**
[PLACEHOLDER: SOHIC is not characterized by a uniform corrosion rate.
Propagation can be slow or rapid depending on stress intensity and H2S activity.
Active SOHIC requires continuous monitoring and periodic volumetric NDE.]

**CML Evidence:**
[PLACEHOLDER: UT data at weld locations has not been reviewed in detail.
Recommend TOFD or PAUT scan of all welds in liquid zone.]

**NDE Evidence:**
[PLACEHOLDER: standard UT A-scan for thickness is NOT adequate to detect SOHIC.
TOFD or angle-beam PAUT is required for weld HAZ scanning.]

**Active or Potential:**  [x] Active (presumed, pending NDE)

---

### Mechanism 3: General Corrosion -- CO2 / H2S Aqueous Corrosion

**API 571 Classification:**
Uniform/general corrosion; aqueous corrosion; CO2 corrosion (carbonic acid
corrosion); H2S aqueous corrosion.

**Description:**
In the presence of free water, dissolved CO2 forms carbonic acid (H2CO3) and
dissolved H2S forms hydrosulfuric acid. Both reduce pH and accelerate corrosion
of carbon steel. The corrosion manifests as general wall thinning, typically
affecting the entire wetted surface, with accelerated attack at areas of flow
turbulence, high velocity, or elevated temperature.

**Affected Components / Locations:**
All internal wetted surfaces in contact with the aqueous phase:
- Shell SC-1 and SC-2 (liquid zone and splash zone)
- Bottom head and boot/sump
- Inlet nozzle bore and reinforcement zone
- Low-point locations and water accumulation zones

**Susceptibility Factors Present:**
- [x] Fluid / environment: H2S and CO2 both present; free water confirmed
- [x] Temperature range: 50 deg C operating -- moderate corrosion rate expected
- [x] Material susceptibility: carbon steel; no corrosion-resistant cladding
- [ ] Stress condition: not a driver for general corrosion
- [x] Other: injection points and turbulence zones (inlet nozzle) increase rate

**Susceptibility Level:**  [x] High

**Typical Morphology / Location:**
Uniform thinning across wetted surfaces. Accelerated at turbulence zones
(inlet nozzle, impingement area). Pitting may coexist at H2S/CO2 ratios
favoring localized attack.

**Evidence from Inspection History:**
[PLACEHOLDER: UT thickness readings show measurable thinning at CML SC2-06.
Corrosion rate cannot be calculated without minimum two inspection data points
with known elapsed time -- see Missing Data Register, Section 21.]

**Evidence from Process Chemistry:**
CO2 and H2S both present. Specific concentrations PENDING (see Section 4.3).

**Rate Estimate or Trend:**
[PLACEHOLDER: cannot calculate corrosion rate without two UT data points.
Planning corrosion rate assumed at [PLACEHOLDER] mm/yr based on
[PLACEHOLDER: process/materials engineering input] pending actual measurement.]

**CML Evidence:**
[PLACEHOLDER: see CML table in Section 11. Minimum measured thickness at
CML SC2-06 is [PLACEHOLDER] mm against nominal 22.0 mm, requiring engineering
review.]

**NDE Evidence:**
[PLACEHOLDER: UT A-scan grid survey conducted. Results in Section 11.]

**Active or Potential:**  [x] Active

---

### Mechanism 4: Pitting Corrosion

**API 571 Classification:**
Pitting corrosion; localized corrosion.

**Description:**
Localized electrochemical corrosion resulting in small-diameter, relatively
deep penetrations in the steel. In H2S/CO2 sour service, pitting typically
occurs at the liquid/vapor interface and in areas where water accumulates and
stagnates. Pitting is more aggressive than general corrosion in terms of local
remaining thickness.

**Affected Components / Locations:**
- Liquid/vapor interface zone on shell courses
- Low-point accumulation zones and boot
- Inlet zone below inlet nozzle (impingement/splash)
- Deadlegs and stagnant sections of piping associated with V-1201

**Susceptibility Factors Present:**
- [x] Fluid / environment: H2S and CO2 with free water; salts or chlorides
      may concentrate at the liquid/vapor interface
- [x] Geometry or configuration: interface zone, low-flow zones

**Susceptibility Level:**  [x] Medium

**Typical Morphology / Location:**
Isolated or clustered pits at and below the liquid/vapor interface. May
be obscured by scale or deposit. Requires close-interval UT grid or pit
gauge measurement during internal inspection for detection and characterization.

**Evidence from Inspection History:**
[PLACEHOLDER: review internal inspection records for visual pitting evidence.]

**Evidence from Process Chemistry:**
H2S, CO2, and free water: conditions support pitting. Chloride level UNKNOWN.

**Rate Estimate or Trend:**
[PLACEHOLDER: pitting rate cannot be estimated without historical pit depth data.]

**CML Evidence:**
[PLACEHOLDER: CML coverage at liquid/vapor interface zone to be confirmed.]

**NDE Evidence:**
[PLACEHOLDER: standard UT grid may not detect all pits; recommend pit gauge
during internal inspection.]

**Active or Potential:**  [x] Active (assumed)

---

### Mechanism 5: Erosion-Corrosion

**API 571 Classification:**
Erosion-corrosion; mechanical damage plus corrosion.

**Description:**
Combined mechanical erosion (from two-phase impingement) and corrosion
accelerating metal loss beyond that of either mechanism alone. Particularly
severe at inlet nozzles in two-phase gas/liquid service where liquid droplets
and solid particles (if present) impact the nozzle bore and impingement zone.

**Affected Components / Locations:**
- Inlet nozzle bore and nozzle-to-shell zone
- Internal impingement plate or baffle (if present -- confirm from drawing)
- Shell wall opposite inlet nozzle (confirm orientation from drawing)

**Susceptibility Factors Present:**
- [x] Fluid / environment: two-phase gas/liquid at inlet
- [x] Geometry or configuration: inlet nozzle impingement zone
- [ ] Temperature range: not a primary driver
- [x] Other: solid particle content [PLACEHOLDER: confirm]

**Susceptibility Level:**  [x] Medium

**Typical Morphology / Location:**
Smooth, scalloped or grooved metal loss at impingement zone.
Metal loss rate higher than adjacent areas measured by UT.

**Evidence from Inspection History:**
[PLACEHOLDER: review inlet nozzle UT data and internal inspection records.]

**Evidence from Process Chemistry:**
Two-phase inlet confirmed. Particle content unknown.

**Rate Estimate or Trend:**
[PLACEHOLDER: requires dedicated CML coverage at inlet impingement zone.]

**CML Evidence:**
[PLACEHOLDER: confirm whether inlet nozzle zone CMLs are included in inspection plan.]

**NDE Evidence:**
[PLACEHOLDER: targeted UT at inlet nozzle zone required.]

**Active or Potential:**  [x] Active

---

## 7. NON-CREDIBLE DAMAGE MECHANISMS

| Damage Mechanism                  | Reason Not Credible                                          |
|-----------------------------------|--------------------------------------------------------------|
| HTHA (High-Temp Hydrogen Attack)  | Operating temp ~50 deg C; design temp 120 deg C. Below Nelson curve threshold for carbon steel. No high-temperature hydrogen service. |
| Creep                             | Temperature well below creep threshold for carbon steel (generally above 370 deg C). Not applicable at this service. |
| Polythionic acid SCC              | No sensitized austenitic stainless steel identified in vessel shell or heads. If SS internals are present, this mechanism shall be re-evaluated. |
| Chloride SCC                      | Carbon steel (SA-516 Gr 70) shell and heads. Chloride SCC is specific to austenitic stainless steels and certain nickel alloys. CS not susceptible. |
| Amine stress corrosion cracking   | No amine confirmed in feed stream to V-1201. Reassess if upstream amine treating or contamination is identified. |
| Thermal fatigue                   | No documented rapid thermal cycling. Routine steam-out or cooldown practices shall be reviewed if identified (potential concern for any stainless internals). |
| Caustic corrosion                 | No caustic in process stream expected. pH of water phase UNKNOWN but not expected to be alkaline above ~9 -- confirm from chemistry data. |

---

## 8. SUSCEPTIBILITY FACTORS SUMMARY

**Material susceptibility factors:**
SA-516 Grade 70 carbon steel is susceptible to all wet H2S damage mechanisms
(HIC, SOHIC, SSC, hydrogen blistering). Susceptibility is strongly influenced
by plate sulfur content, cleanliness, and PWHT status. PWHT status is a CRITICAL
MISSING DATA item and must be confirmed before this DMR is finalized.

**Process / environment susceptibility factors:**
Wet H2S service with free water is the primary driver. CO2 corrosion is a
secondary driver. H2S partial pressure and pH -- the key NACE MR0175 threshold
parameters -- are MISSING DATA items.

**Mechanical / stress susceptibility factors:**
Residual weld stresses are the primary driver for SOHIC and SSC at welds.
PWHT would reduce residual stresses significantly. PWHT status unknown.

**Geometry or configuration factors:**
Vertical orientation: water and heavy liquids accumulate at the bottom.
Boot/sump and lower shell are highest-risk zones for aqueous corrosion.
Inlet nozzle is highest-risk zone for erosion-corrosion.
Liquid/vapor interface is highest-risk zone for pitting and concentrated attack.

**Operating history factors:**
[PLACEHOLDER: document any known process excursions, water slugging events,
high-H2S upsets, or unexpected corrosion findings from process records.]

---

## 9. INSPECTION HISTORY

| Inspection Date     | Type                  | Method              | Inspector / Firm | Findings Summary                       | Reference              |
|---------------------|-----------------------|---------------------|------------------|----------------------------------------|------------------------|
| [PLACEHOLDER]       | [PLACEHOLDER]         | UT, VT              | [PLACEHOLDER]    | [PLACEHOLDER]                          | [PLACEHOLDER: report no.] |
| [PLACEHOLDER]       | [PLACEHOLDER]         | UT                  | [PLACEHOLDER]    | [PLACEHOLDER]                          | [PLACEHOLDER: report no.] |

**Years in service at time of this review:**
[PLACEHOLDER: calculate from year installed to current date]

**Last internal inspection date:**
[PLACEHOLDER: confirm from inspection records]

**Last external inspection date:**
[PLACEHOLDER: confirm from inspection records]

**Open inspection recommendations from prior inspections:**
[PLACEHOLDER: review all prior inspection reports and list open items with
original recommendation, due date, and current status]

NOTE: Inspection history is INCOMPLETE for this smoke-test document. All
placeholder entries above must be replaced with actual data before this DMR
is issued for use.

---

## 10. INSPECTION EFFECTIVENESS

| Damage Mechanism    | Prior NDE Method | Coverage | Effectiveness Rating | Basis                                         |
|---------------------|------------------|----------|----------------------|-----------------------------------------------|
| HIC                 | UT A-scan        | [PLACEHOLDER] | D              | UT A-scan thickness measurement is poorly effective for detecting HIC laminar cracks parallel to the surface |
| SOHIC               | UT A-scan        | [PLACEHOLDER] | D--E           | Requires TOFD or PAUT angle-beam for HAZ scanning; A-scan inadequate |
| General corrosion   | UT A-scan        | [PLACEHOLDER] | B              | Generally effective for area-average thickness loss |
| Pitting             | UT A-scan grid   | [PLACEHOLDER] | C              | Grid may miss isolated pits; pit gauge required during internal inspection |
| Erosion-corrosion   | UT A-scan        | [PLACEHOLDER] | B--C           | Effective if CMLs placed at impingement zone; requires targeted coverage |

**Effectiveness rating key:**
A = Highly effective   B = Usually effective   C = Fairly effective
D = Poorly effective   E = Ineffective

**Summary:**
Current inspection program using UT A-scan thickness measurements is
INADEQUATE to detect HIC and SOHIC. Supplemental TOFD or PAUT scanning
of base metal and weld HAZ is required to adequately address the dominant
damage mechanisms in this wet H2S service. See Section 16 for recommendations.

---

## 11. CML AND UT EVIDENCE

| CML ID      | Location Description               | Clock Position | Axial / Girth Band | t_measured (mm) | t_nominal (mm) | t_required (mm) | Date | Trend | Notes |
|-------------|-------------------------------------|----------------|---------------------|-----------------|----------------|-----------------|------|-------|-------|
| SC1-12      | Shell Course 1, mid-course          | 12:00          | Band A              | [PLACEHOLDER]   | 22.0           | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | Lower shell, gas zone |
| SC1-06      | Shell Course 1, mid-course          | 06:00          | Band A              | [PLACEHOLDER]   | 22.0           | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | Lower shell, liquid zone |
| SC2-12      | Shell Course 2, mid-course          | 12:00          | Band A              | [PLACEHOLDER]   | 22.0           | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | Upper shell |
| SC2-06      | Shell Course 2, ~2400 mm from BTL   | 06:00          | Band A              | [PLACEHOLDER -- ALERT] | 22.0  | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | ALERT: thin reading; engineering review required; possible HIC velocity anomaly noted |
| HD2-CR      | Bottom head, crown                  | --             | Crown               | [PLACEHOLDER]   | 22.0           | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | Bottom head |
| BT-01       | Boot / sump bottom                  | --             | Boot                | [PLACEHOLDER]   | [PLACEHOLDER]  | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | High-risk water accumulation zone |
| N1-NB       | Inlet nozzle bore                   | --             | Nozzle bore         | [PLACEHOLDER]   | [PLACEHOLDER]  | [PLACEHOLDER]   | [PLACEHOLDER] | [PLACEHOLDER] | Erosion-corrosion zone |

**Corrosion rate method used:**
[x] Estimated (insufficient inspection history for measured rate)
-- NOTE: Corrosion rate calculation requires a minimum of two thickness data
   points at the same CML with a known elapsed time. Estimated rate from
   [PLACEHOLDER: process/materials engineering input] is being used as interim
   planning rate pending second inspection data point.

---

## 12. NDE EVIDENCE

| NDE Event Date | Method      | Coverage            | Relevant Findings                          | Accept / Reject | Standard / Criteria Ref         | Inspector |
|----------------|-------------|---------------------|--------------------------------------------|-----------------|---------------------------------|-----------|
| [PLACEHOLDER]  | UT A-scan   | [PLACEHOLDER]       | Thin reading at SC2-06; possible velocity anomaly | Under review | API 510, site inspection plan | [PLACEHOLDER] |
| [PLACEHOLDER]  | VT (internal) | [PLACEHOLDER]     | [PLACEHOLDER]                              | [PLACEHOLDER]   | API 510                         | [PLACEHOLDER] |

---

## 13. PROCESS CHEMISTRY EVIDENCE

| Date         | Parameter   | Measured Value | Specification Limit | Exceedance? | Action Taken |
|--------------|-------------|----------------|---------------------|-------------|--------------|
| [PLACEHOLDER] | H2S (gas phase) | [PLACEHOLDER] | [PLACEHOLDER]  | [PLACEHOLDER] | [PLACEHOLDER] |
| [PLACEHOLDER] | CO2 (gas phase) | [PLACEHOLDER] | [PLACEHOLDER]  | [PLACEHOLDER] | [PLACEHOLDER] |
| [PLACEHOLDER] | pH (water phase) | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] |

**Trend in chemistry conditions:**
[PLACEHOLDER: summarize chemistry trend from available data. All chemistry
entries above are MISSING DATA items -- see Section 21 for missing data register.]

---

## 14. ACTIVE VERSUS POTENTIAL MECHANISMS SUMMARY

| Damage Mechanism       | Active | Potential | Basis                                                        |
|------------------------|--------|-----------|--------------------------------------------------------------|
| HIC                    | [x]    | [ ]       | Wet H2S service active; HIC assumed active pending NDE confirmation |
| SOHIC                  | [x]    | [ ]       | Wet H2S service active; SOHIC at welds assumed active pending NDE |
| Hydrogen blistering    | [x]    | [ ]       | Wet H2S service active; assumed active pending inspection    |
| SSC                    | [ ]    | [x]       | Wet H2S present; SSC potential depends on hardness/PWHT; not confirmed active |
| General CO2/H2S corrosion | [x] | [ ]       | Active: measurable thinning at CML SC2-06                    |
| Pitting                | [ ]    | [x]       | Conditions present; not confirmed by inspection              |
| Erosion-corrosion      | [ ]    | [x]       | Inlet nozzle zone; not confirmed by targeted inspection      |

---

## 15. CONSEQUENCE NOTES

**Safety consequence of mechanism activation:**
HIC/SOHIC leading to through-wall cracking in wet H2S service would release
toxic and flammable sour gas. Consequences include potential personnel fatalities
and environmental release. Risk is HIGH.

**Environmental consequence:**
Sour gas release would constitute a significant environmental release event
requiring regulatory notification.

**Production / reliability consequence:**
Unplanned shutdown for emergency repair in wet H2S service is operationally
disruptive and commercially significant.

**Potential for sudden versus gradual failure:**
General corrosion: gradual -- detectable by periodic UT.
HIC/SOHIC: can be gradual or sudden; HIC cracking can propagate rapidly to
through-wall under the right stress and environment conditions.
Hydrogen blistering: typically gradual; blisters may cause sudden local failure.

**Risk driver (likelihood, consequence, or both):**
Both: wet H2S service elevates likelihood; sour gas content elevates consequence.

---

## 16. RECOMMENDED INSPECTION METHODS

| Priority | Damage Mechanism Targeted | Recommended NDE Method             | Applicability | Notes                                              |
|----------|---------------------------|------------------------------------|---------------|----------------------------------------------------|
| 1        | HIC, SOHIC, blistering    | TOFD or PAUT (angle-beam)          | Shell and welds in liquid zone | Required at next inspection; current UT A-scan is inadequate |
| 2        | HIC, SOHIC, blistering    | WFMT (Wet Fluorescent MT)          | External weld surfaces after insulation removal | If vessel is accessible for insulation removal |
| 3        | General corrosion, pitting | UT A-scan close-interval grid     | All shell courses, heads, boot | Increase CML density in liquid zone and at interface |
| 4        | Erosion-corrosion         | UT A-scan targeted                 | Inlet nozzle bore and adjacent shell | Dedicated CML required at inlet impingement zone |
| 5        | Pitting                   | Visual + pit gauge (internal)      | All internal wetted surfaces   | Required at next internal inspection entry         |
| 6        | SOHIC, SSC                | PAUT or TOFD                       | Welds and HAZ in liquid zone   | Particularly if PWHT not confirmed                 |

---

## 17. RECOMMENDED CML LOCATIONS

| CML ID (Proposed) | Location Description                  | Component    | Basis (Damage Mechanism) | Measurement Method | Notes                                  |
|-------------------|---------------------------------------|--------------|--------------------------|-------------------|----------------------------------------|
| SC1-06-A          | SC-1, 6 o'clock, lower liquid zone    | Shell SC-1   | General corrosion; pitting | UT A-scan       | High-risk liquid accumulation zone     |
| SC1-06-B          | SC-1, 6 o'clock, interface zone       | Shell SC-1   | General corrosion; pitting | UT A-scan       | Liquid/vapor interface                 |
| SC2-06-A          | SC-2, 6 o'clock, ~2400 mm from BTL   | Shell SC-2   | General corrosion; HIC investigation | UT A-scan + TOFD | Existing alert CML; supplemental TOFD scan required |
| N1-IMP            | Inlet nozzle impingement zone          | Inlet nozzle | Erosion-corrosion          | UT A-scan targeted | New CML required                      |
| FL-01             | Liquid/vapor interface, 360-degree band | Shell       | Pitting; general corrosion | UT A-scan grid   | New zone; interface elevation from process data |
| BT-01             | Boot / sump bottom and sides          | Boot         | General corrosion; pitting | UT A-scan        | High-risk zone                         |
| LP-01             | Low point on liquid outlet line       | Nozzle/piping | Corrosion, pitting         | UT A-scan        | Deadleg potential                      |

---

## 18. MITIGATION AND MONITORING ACTIONS

| Action                                      | Mechanism Addressed        | Responsible Party   | Target Date                   | Status  |
|---------------------------------------------|----------------------------|---------------------|-------------------------------|---------|
| Confirm PWHT status from fabrication records | SSC, SOHIC susceptibility  | [PLACEHOLDER: owner/operator records group] | [PLACEHOLDER] | Open |
| Obtain process chemistry data (H2S, CO2, pH) | All wet H2S mechanisms     | [PLACEHOLDER: process engineering] | [PLACEHOLDER] | Open |
| Conduct TOFD / PAUT scan of liquid-zone welds and SC2-06 zone | HIC, SOHIC | [PLACEHOLDER: NDE contractor] | Next inspection / [PLACEHOLDER] | Open |
| Review corrosion inhibitor program if applicable | General corrosion       | [PLACEHOLDER: process/corrosion engineering] | [PLACEHOLDER] | Open |
| Confirm inlet nozzle impingement zone CML coverage | Erosion-corrosion     | [PLACEHOLDER: inspection group] | Next inspection          | Open |

**Chemical treatment or inhibitor program:**
[PLACEHOLDER: confirm with process and corrosion engineering whether a corrosion
inhibitor program is active for this vessel and whether it is effective.]

**Operating limit changes recommended:**
None recommended at this stage pending completion of FFS assessment and NDE.
Confirm that operating pressure does not exceed MAWP per current corroded condition.

**Material upgrade or replacement recommended:**  [ ] Yes   [x] No   -- pending FFS outcome

---

## 19. FFS TRIGGERS

The following conditions trigger a formal FFS assessment per API 579-1/ASME FFS-1:

- [x] Measured thickness below required thickness (CML SC2-06 -- under review)
- [ ] Active pitting or local metal loss detected (not yet confirmed by internal inspection)
- [ ] Crack-like flaw identified (HIC/SOHIC not yet confirmed by TOFD/PAUT)
- [ ] Remaining life estimate below inspection interval (pending corrosion rate data)
- [x] Blistering, HIC, SOHIC, or HTHA indication (suspected at CML SC2-06 -- velocity anomaly noted)
- [ ] Creep damage indication (not applicable)
- [ ] Equipment operating beyond design limits (not identified)
- [ ] Other

**FFS assessment currently required:**  [x] Yes   [ ] No   [ ] Under evaluation
-- FFS triggered by potential thickness below required value at CML SC2-06.
   Reference FFS assessment document V1201-FFS-001 (DRAFT).

**FFS reference (if applicable):**
V1201-FFS-001 (DRAFT) -- API 579 General FFS Assessment Report

---

## 20. ASSUMPTIONS

1. Operating pressure of 2,000 kPa(g) and operating temperature of 50 deg C are
   nominal design-basis values. Actual operating conditions to be confirmed from
   DCS records.
2. Free water is present at operating conditions based on process description.
   Phase diagram confirmation not performed for this DMR.
3. PWHT was NOT applied unless confirmed otherwise. This conservative assumption
   drives higher susceptibility ratings for SSC and SOHIC. If PWHT is confirmed,
   susceptibility ratings shall be revised.
4. H2S is present in sufficient quantity to constitute wet H2S service per NACE
   MR0175. Quantitative confirmation PENDING.
5. No sensitized austenitic stainless steel internals are present. If SS internals
   exist, polythionic acid SCC mechanism must be re-evaluated.
6. Inspection history prior to the most recent inspection is incomplete.
   Susceptibility and rate assessments may change when additional history is available.

---

## 21. LIMITATIONS

1. This DMR is PROVISIONAL and shall not be finalized without resolution of all
   CRITICAL MISSING DATA items: PWHT status, chemistry data (H2S, CO2, pH), and
   complete inspection history.
2. Susceptibility ratings assigned as H, M, L are engineering judgments based on
   the information available at the time of this review. They shall be revised if
   new information changes the basis.
3. This DMR does not constitute an FFS assessment. A separate formal FFS assessment
   per API 579-1/ASME FFS-1 is required and has been triggered (see Section 19).
4. NDE effectiveness assessment in Section 10 is based on the NDE methods used in
   prior inspections as understood from available records. If additional NDE was
   performed that is not captured here, effectiveness ratings may change.
5. No laboratory analysis of corrosion products or steel microstructure has been
   performed to confirm damage mechanism identification.

---

## 22. APPROVAL BLOCK

| Role                              | Name | Signature | Date |
|-----------------------------------|------|-----------|------|
| Prepared By                       | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Technically Reviewed By           | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Approved By                       | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Client Acceptance (if applicable) | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |

---

## MISSING DATA REGISTER

The following data items are required to finalize this DMR. This list shall be
reviewed at each issue cycle and all items resolved before final approval.

| Item | Required Data                              | Why Required                                      | Current Status | Proposed Resolution              | Responsible Party   | Target Date   |
|------|--------------------------------------------|---------------------------------------------------|----------------|----------------------------------|---------------------|---------------|
| MD-1 | PWHT status (applied / not applied)        | Determines SSC and SOHIC susceptibility level      | MISSING        | Obtain from fabrication data report (MDR) | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-2 | H2S concentration (mol% or ppmv)           | NACE MR0175 threshold screening; HIC/SSC driving force | MISSING    | Latest process lab sample        | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-3 | CO2 concentration                          | CO2 corrosion rate estimation                     | MISSING        | Latest process lab sample        | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-4 | pH of water phase                          | Corrosion rate basis; NACE threshold              | MISSING        | Latest process lab sample        | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-5 | Chloride concentration                     | Assess pitting severity; confirm no chloride SCC issue if SS present | MISSING | Latest process lab sample | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-6 | Complete inspection history (all prior reports) | Corrosion rate calculation; trend analysis    | INCOMPLETE     | Retrieve all prior inspection records | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-7 | Corrosion rate (measured)                  | Remaining life calculation; inspection interval determination | MISSING | Second UT data point at next inspection | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-8 | TOFD/PAUT results for SC2-06 and liquid-zone welds | HIC/SOHIC confirmation or exclusion      | PENDING NDE    | Schedule TOFD/PAUT scan          | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-9 | Steel plate CMTRs (sulfur content, Ca-treatment) | HIC susceptibility of base metal          | MISSING        | Obtain from material files or manufacturer | [PLACEHOLDER] | [PLACEHOLDER] |
| MD-10 | Inlet nozzle CML data                     | Erosion-corrosion rate at inlet zone             | MISSING        | Add inlet nozzle CML to inspection plan | [PLACEHOLDER] | [PLACEHOLDER] |

---

*Template reference: API 571, current edition. All damage mechanism descriptions,
susceptibility criteria, and inspection recommendations shall be based on the
current edition of API 571 and the engineer's documented judgment. This template
does not substitute for engineering analysis.*

================================================================================
TEST / DRAFT / NOT FOR ISSUE
Smoke-test example document V1201-DMR-001 -- Al-Wadi Refinery (FICTIONAL)
All data is fictional and for template demonstration only.
================================================================================
