================================================================================
TEST / DRAFT / NOT FOR ISSUE
This document is a smoke-test example only. All equipment data, personnel names,
measurement values, and site references are FICTIONAL. This document has not been
reviewed or approved and shall not be used for any engineering, operational, or
regulatory purpose.
================================================================================

# RBI and Inspection Planning Template
## Risk-Based Inspection Planning Support

---

## DOCUMENT CONTROL

| Field                  | Entry                                              |
|------------------------|----------------------------------------------------|
| Document Number        | V1201-RBI-001                                      |
| Revision               | 0 -- DRAFT                                         |
| Date                   | [PLACEHOLDER: date of issue]                       |
| Prepared By            | [PLACEHOLDER: name and qualification]              |
| Reviewed By            | [PLACEHOLDER: name and qualification]              |
| Approved By            | [PLACEHOLDER: name and qualification]              |
| Plant / Site           | Al-Wadi Refinery (FICTIONAL -- TEST DATA ONLY)     |
| Unit / Process Area    | Crude Distillation Unit (CDU), Train A             |
| Supersedes             | N/A -- original issue                              |
| Next Review Due        | [PLACEHOLDER: per RBI program cycle; typically 5 years maximum or on significant change] |

---

## 1. EQUIPMENT LIST

This document covers V-1201 only. Additional equipment in CDU Train A to be
covered by separate RBI documents per the site RBI program.

| Item No. | Tag Number | Equipment Type           | Service / Fluid                       | P&ID Ref         | Year Installed | Design Code          |
|----------|-----------|--------------------------|---------------------------------------|------------------|----------------|----------------------|
| 1        | V-1201    | Vertical pressure vessel | Wet sour hydrocarbon gas/liquid separator | P&ID-CDU-A-101 (FICTIONAL) | [PLACEHOLDER] | ASME VIII Div. 1 |

---

## 2. PROCESS UNIT AND SERVICE DESCRIPTION

**Process Unit:**
Crude Distillation Unit (CDU), Train A, Al-Wadi Refinery (FICTIONAL).

**Operating Function:**
V-1201 receives sour hydrocarbon overhead vapors from the crude distillation
column and separates entrained liquid from the gas phase. The separated gas
proceeds to downstream sour gas treating. The separated liquid drains to
[PLACEHOLDER: confirm destination].

**Fluid Inventory:**
Gas phase: sour hydrocarbon gas containing H2S, CO2, light hydrocarbons.
Liquid phase: sour hydrocarbon condensate and produced water.
H2S content: [PLACEHOLDER -- MISSING DATA]. Free water phase: present.
Vessel volume: [PLACEHOLDER: confirm from drawing] m3.
Total fluid inventory under operating conditions: [PLACEHOLDER] kg.

**Toxic / Flammable Classification:**
Toxic and flammable. H2S is classified as a toxic gas above threshold limit
values. All releases require regulatory notification. Consequence classification
is HIGH for personnel and environmental impact.

**Unit Operating Mode:**  [x] Continuous   [ ] Batch   [ ] Intermittent

**Normal Throughput / Capacity:**
[PLACEHOLDER: confirm from process flow diagram (PFD) and operating data]

**Key process upsets or abnormal conditions documented:**
[PLACEHOLDER: document known slugging events, high-H2S exceedances, water hammer
history, or other process upsets that could affect inspection interval or
damage mechanism activity]

---

## 3. DAMAGE MECHANISM REVIEW SUMMARY

Reference full DMR document V1201-DMR-001 (DRAFT) for detailed discussion.

**DMR Reference Document:**
V1201-DMR-001, Revision 0 -- DRAFT (not approved).

| Damage Mechanism               | Credible? | Susceptibility     | Active / Potential | Key Susceptible Equipment Tags |
|--------------------------------|-----------|--------------------|--------------------|-------------------------------|
| HIC (Hydrogen-Induced Cracking) | [x]      | H (provisional)    | Active (presumed)  | V-1201 shell and heads        |
| SOHIC                          | [x]       | H (provisional)    | Active (presumed)  | V-1201 welds and HAZ          |
| Hydrogen blistering            | [x]       | H (provisional)    | Active (presumed)  | V-1201 shell and heads        |
| SSC (Sulfide Stress Cracking)  | [x]       | M (provisional)    | Potential          | V-1201 welds; PWHT status unknown |
| General corrosion (CO2/H2S)    | [x]       | H                  | Active             | V-1201 shell, heads, boot     |
| Pitting corrosion              | [x]       | M                  | Potential          | V-1201 interface zone, low points |
| Erosion-corrosion              | [x]       | M                  | Potential / Active | V-1201 inlet nozzle zone      |
| CUI                            | [x]       | L--M               | Potential          | V-1201 external (if insulated) |

**Susceptibility key:**  H = High   M = Medium   L = Low
NOTE: All susceptibility ratings in the DMR are PROVISIONAL pending receipt of
confirmed chemistry data (H2S, CO2, pH) and confirmation of PWHT status.

**Summary of dominant damage mechanisms for this unit:**
V-1201 is dominated by wet H2S damage mechanisms (HIC, SOHIC, hydrogen blistering)
and active aqueous corrosion (CO2/H2S). Both mechanism families are confirmed
credible based on the service description. The dominant mechanisms drive a
HIGH risk profile for this vessel, requiring enhanced NDE methods (TOFD/PAUT)
beyond standard UT A-scan thickness monitoring.

---

## 4. CONSEQUENCE SCREENING

### 4.1 Consequence Category

| Tag Number | Fluid Hazard Level | Estimated Inventory | Release Type              | Personnel Impact | Environmental Impact | Production Impact | Consequence Category |
|------------|--------------------|---------------------|---------------------------|------------------|----------------------|-------------------|-----------------------|
| V-1201     | HIGH -- sour gas, H2S toxic, flammable | [PLACEHOLDER] kg | Vapor and liquid release on failure | HIGH: H2S fatality potential; confined space entry hazard | HIGH: H2S release; regulatory notification required | HIGH: CDU shutdown | HIGH / A          |

**Consequence category key:**
Category A (High) -- toxic release with fatality potential and significant
environmental impact; full unit shutdown.
(Category assignment per site consequence matrix -- confirm against site-specific
criteria per API 580/581.)

**Screening methodology used:**  [ ] API 581   [x] API 580   [ ] Site-specific   [ ] Other
NOTE: Quantitative API 581 consequence calculation has not been performed for
this smoke-test document. Qualitative consequence screening per API 580 principles
is used here. A full API 581 consequence calculation is required for the formal
RBI program.

**Assumptions in consequence screening:**
1. H2S concentration is sufficient to constitute a toxic hazard. Quantitative
   confirmation PENDING (MISSING DATA).
2. A full rupture or large leak is considered the bounding release scenario for
   consequence assessment.
3. Populated areas and sensitive environmental receptors are [PLACEHOLDER: describe
   proximity from site plot plan].

---

## 5. LIKELIHOOD SCREENING

### 5.1 Damage Factor Inputs

| Tag Number | Dominant Mechanism    | Corrosion Rate Basis   | Years in Service | Last Inspection Date | Last t_measured (mm) | t_required (mm) | Remaining Life | Damage Factor Basis |
|------------|-----------------------|------------------------|------------------|----------------------|-----------------------|-----------------|----------------|---------------------|
| V-1201     | General corrosion; HIC/SOHIC | [PLACEHOLDER -- MISSING] | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER] mm at SC2-06 | [PLACEHOLDER] | [PLACEHOLDER] | Estimated -- MISSING DATA MD-9 |

**Corrosion rate basis:**
[ ] Measured short-term   [ ] Measured long-term   [ ] Estimated   [ ] Literature   [x] Unknown
-- NOTE: Corrosion rate is a CRITICAL MISSING DATA item (MD-9 in Input Data Sheet).
   The likelihood calculation cannot be completed until a measured corrosion rate
   is established at CML SC2-06. An interim conservative estimate shall be used
   for planning purposes only.

ADDITIONAL NOTE: HIC and SOHIC are not characterized by a corrosion rate.
Likelihood of HIC/SOHIC damage is assessed qualitatively based on:
- Wet H2S service conditions (HIGH susceptibility driver)
- PWHT status (UNKNOWN -- HIGH risk if not applied)
- Steel cleanliness (UNKNOWN -- HIC-resistant plate specification not confirmed)
- Years in service (PLACEHOLDER -- longer service = greater HIC exposure)

### 5.2 Inspection Effectiveness Factor

| Tag Number | Prior Inspection Type | NDE Method      | Coverage         | Effectiveness | Adjusted DF Basis                  |
|------------|-----------------------|-----------------|------------------|---------------|------------------------------------|
| V-1201     | Periodic UT survey    | UT A-scan       | [PLACEHOLDER]    | D             | UT A-scan is poorly effective for HIC/SOHIC detection; does NOT reduce damage factor for HIC/SOHIC |
| V-1201     | Internal VT           | Visual (if entry) | [PLACEHOLDER]  | B--C          | Effective for surface blistering and pitting; not effective for buried HIC |

**Effectiveness key:**
A = Highly effective   B = Usually effective   C = Fairly effective
D = Poorly effective   E = Ineffective

**Summary:**
Current inspection program (UT A-scan) provides POOR effectiveness for the
dominant damage mechanisms (HIC/SOHIC). The inspection effectiveness factor
does not reduce the likelihood score for these mechanisms. This is the key
driver for recommending enhanced NDE (TOFD/PAUT) in the inspection strategy.

---

## 6. RISK RANKING

| Tag Number | Likelihood Category | Consequence Category | Risk Ranking | Risk Matrix Reference |
|------------|--------------------|-----------------------|--------------|-----------------------|
| V-1201     | [PLACEHOLDER -- HIGH provisional] | HIGH / A | [PLACEHOLDER -- HIGH/A x HIGH = HIGH risk] | Site risk matrix [PLACEHOLDER] |

NOTE: Risk ranking is PROVISIONAL. Likelihood category cannot be finalized until:
(a) Corrosion rate is established (MD-9).
(b) HIC/SOHIC status is confirmed or excluded by TOFD/PAUT (MD-12).
(c) PWHT status is confirmed (MD-5).
(d) Full inspection history is available.

**Risk ranking methodology:**  [ ] API 581   [x] API 580   [ ] Site matrix   [ ] Other
(Qualitative screening per API 580 principles. Quantitative API 581 ranking
is required for the formal site RBI program.)

**Risk matrix attached:**  [ ] Yes   [x] No -- to be attached with formal RBI program document

**Items requiring immediate action (high risk):**
V-1201 is provisionally ranked as HIGH risk due to:
1. Dominant damage mechanisms (HIC/SOHIC) not yet confirmed or excluded.
2. Current inspection program (UT A-scan) is poorly effective for HIC/SOHIC.
3. Wet H2S service with HIGH consequence (toxic sour gas).
4. PWHT status unknown -- increases SSC and SOHIC susceptibility significantly.
5. Thin reading at CML SC2-06 with possible velocity anomaly.

Immediate action: conduct TOFD/PAUT scan of SC2-06 zone and liquid-zone welds
before next operating cycle. See Recommendation Note V1201-REC-001 (DRAFT).

---

## 7. INSPECTION HISTORY

| Tag Number | Inspection Date | Inspection Type   | NDE Method    | Inspector | Coverage          | Summary of Findings                    | Action Taken |
|------------|-----------------|-------------------|---------------|-----------|-------------------|----------------------------------------|--------------|
| V-1201     | [PLACEHOLDER]   | UT survey         | UT A-scan     | [PLACEHOLDER] | [PLACEHOLDER]  | Thin reading at CML SC2-06; possible velocity anomaly | FFS assessment triggered (V1201-FFS-001) |
| V-1201     | [PLACEHOLDER]   | [PLACEHOLDER]     | [PLACEHOLDER] | [PLACEHOLDER] | [PLACEHOLDER]  | [PLACEHOLDER]                          | [PLACEHOLDER] |

**Open items from prior inspections:**

| Item | Tag   | Finding                                 | Recommended Action                          | Due Date      | Status |
|------|-------|-----------------------------------------|---------------------------------------------|---------------|--------|
| OI-1 | V-1201 | Thin reading at CML SC2-06; velocity anomaly | FFS assessment and TOFD/PAUT scan required | [PLACEHOLDER] | Open   |
| OI-2 | V-1201 | PWHT status not confirmed               | Retrieve and confirm from fabrication records | [PLACEHOLDER] | Open   |
| OI-3 | V-1201 | Chemistry data not available            | Obtain from process laboratory              | [PLACEHOLDER] | Open   |

---

## 8. CURRENT INSPECTION EFFECTIVENESS ASSESSMENT

| Tag Number | Mechanism         | Current Inspection Program | Current Effectiveness | Gap                                       | Improvement Required |
|------------|-------------------|----------------------------|-----------------------|-------------------------------------------|----------------------|
| V-1201     | HIC               | UT A-scan thickness grid   | D -- Poorly effective | UT A-scan cannot detect laminar HIC cracks | [x] TOFD or PAUT required |
| V-1201     | SOHIC             | UT A-scan thickness grid   | D-E -- Poorly effective | UT A-scan cannot detect HAZ cracking       | [x] Angle-beam PAUT or TOFD required |
| V-1201     | Hydrogen blistering | UT A-scan; VT internal   | C -- Fairly effective | VT effective for surface blistering; UT may detect thickness increase over large blisters | [x] Confirm internal VT coverage |
| V-1201     | General corrosion | UT A-scan thickness grid   | B -- Usually effective | Coverage must include liquid zone and interface | [x] Confirm CML density and location |
| V-1201     | Pitting           | UT A-scan; VT internal (if entry) | C -- Fairly effective | Grid may miss isolated pits; pit gauge needed | [x] Pit gauge during internal entry |
| V-1201     | Erosion-corrosion | UT A-scan (if CMLs placed at inlet nozzle) | C (if targeted) | CML placement at inlet nozzle zone not confirmed | [x] Confirm inlet nozzle CML coverage |

**Overall effectiveness assessment:**
INADEQUATE for the dominant damage mechanisms (HIC/SOHIC). The current program
using UT A-scan thickness monitoring is not capable of detecting HIC or SOHIC.
The inspection program must be upgraded to include TOFD or PAUT angle-beam
scanning of the shell base metal and weld HAZ in the liquid zone before the
risk profile can be considered managed.

---

## 9. RECOMMENDED INSPECTION STRATEGY

| Tag Number | Risk Ranking      | Dominant Mechanism   | Recommended Inspection Type | Recommended NDE Method                  | Online or Shutdown | Rationale |
|------------|-------------------|----------------------|-----------------------------|-----------------------------------------|--------------------|-----------|
| V-1201     | HIGH (provisional) | HIC, SOHIC          | Shutdown (internal) + targeted NDE | TOFD or PAUT (angle-beam) of shell base metal and all liquid-zone welds | Shutdown           | HIC/SOHIC requires volumetric NDE; vessel entry required for internal VT |
| V-1201     | HIGH (provisional) | General corrosion    | Shutdown (internal)         | Close-interval UT A-scan grid; internal VT with pit gauge | Shutdown           | Corrosion rate establishment; pitting characterization |
| V-1201     | HIGH (provisional) | Erosion-corrosion    | Online (from external) or Shutdown | UT A-scan at inlet nozzle CML zone | Online or Shutdown | Targeted CML addition at inlet impingement zone |
| V-1201     | HIGH (provisional) | Hydrogen blistering  | Shutdown (internal)         | Internal VT; supplemented by UT for blister height | Shutdown           | Surface blisters visible internally; subsurface requires UT |

**Inspection type key:**
INT = Internal   EXT = External   OTF = On-stream / online   SH = Shutdown

---

## 10. CML STRATEGY

| Tag Number | No. of Existing CMLs | CML Coverage Adequate? | New CMLs Required | Basis for CML Placement   | Reference DMR     |
|------------|----------------------|------------------------|-------------------|---------------------------|-------------------|
| V-1201     | [PLACEHOLDER]        | [x] No                 | Yes               | Liquid zone, interface zone, inlet nozzle, boot -- current CML set does not cover all damage-mechanism-driven zones | V1201-DMR-001 (DRAFT) |

**CML placement basis:**
- [x] Damage-mechanism-first (preferred)
- [x] Prior inspection history
- [x] Process chemistry hot spots (liquid/vapor interface; low points)
- [x] Geometry-driven (deadlegs, low points, inlet impingement zone)
- [ ] Other

**Proposed new CML locations:**

| Tag Number | Proposed CML ID | Location Description                  | Clock Position | Component    | Mechanism Targeted           | NDE Method           |
|------------|-----------------|---------------------------------------|----------------|--------------|------------------------------|----------------------|
| V-1201     | SC2-06-A        | SC-2, 6 o'clock, ~2400 mm from BTL -- existing ALERT location | 06:00 | Shell SC-2 | General corrosion; HIC (TOFD zone) | UT A-scan + TOFD supplement |
| V-1201     | FL-01           | Liquid/vapor interface zone, 06:00    | 06:00          | Shell        | Pitting; general corrosion   | UT A-scan close interval |
| V-1201     | FL-02           | Liquid/vapor interface zone, 12:00    | 12:00          | Shell        | Pitting; general corrosion   | UT A-scan close interval |
| V-1201     | N1-IMP          | Inlet nozzle impingement zone         | --             | Inlet nozzle | Erosion-corrosion            | UT A-scan targeted   |
| V-1201     | BT-01           | Boot / sump bottom                    | --             | Boot         | General corrosion; pitting   | UT A-scan            |
| V-1201     | LP-01           | Low point on liquid outlet line       | --             | Nozzle/pipe  | Corrosion; deadleg           | UT A-scan            |

---

## 11. NDE METHOD SELECTION

| Damage Mechanism   | Applicable NDE Method                   | Coverage Achievable         | Limitation                                                    | Reference |
|--------------------|-----------------------------------------|-----------------------------|---------------------------------------------------------------|-----------|
| HIC                | TOFD; PAUT (pulse-echo with low-angle shear wave) | Full volume of plate in scan zone | Requires dedicated probe setup; surface scan from outside; may be affected by insulation | API 571; ASME V Article 4 (TOFD) |
| SOHIC              | TOFD; angle-beam PAUT                   | Weld HAZ volume             | Requires weld profile compensation; signal interpretation by Level II or III | API 571 |
| General corrosion  | UT A-scan (contact, single element)     | Grid points at CML locations | Spot measurement only; cannot detect pitting between grid points | ASME V Article 5; API 510 |
| Pitting            | UT A-scan close-interval grid + pit gauge (mechanical) | Grid + visual during internal entry | UT alone cannot fully characterize pit depth and density at grid scale | API 579 Part 6 |
| Erosion-corrosion  | UT A-scan targeted at impingement zone  | CML zone coverage           | Requires correct CML placement at impingement point          | API 571   |
| Hydrogen blistering | VT internal + UT for blister dimensions | Surface-accessible blisters | Subsurface (buried) blisters require UT for detection        | API 571   |

**NDE method selection basis:**
Damage-mechanism-first: NDE methods are selected to detect the specific
damage morphology of each credible mechanism. UT A-scan alone is INADEQUATE
for HIC and SOHIC. TOFD or PAUT is required as a supplemental method for
the dominant mechanisms in this wet H2S service.

---

## 12. INSPECTION INTERVAL BASIS

| Tag Number | Risk Ranking | Controlling Mechanism | Remaining Life (calculated) | Safety Factor Applied | Recommended Inspection Interval | Next Inspection Due Date | Regulatory Limit |
|------------|--------------|-----------------------|-----------------------------|-----------------------|---------------------------------|--------------------------|--------------------|
| V-1201     | HIGH (provisional) | General corrosion (interval limit); HIC/SOHIC (drives enhanced NDE scope) | [PLACEHOLDER -- MISSING DATA MD-9] | 1/2 remaining life per API 510 | [PLACEHOLDER -- shorter of calculated or maximum per API 510 or regulatory] | [PLACEHOLDER] | [PLACEHOLDER: confirm jurisdictional limit; typically 10 years maximum internal per API 510 for RBI] |

**Interval basis methodology:**
API 510 half-life rule: next inspection interval shall not exceed the lesser
of half the remaining corrosion allowance life or the maximum interval permitted
by the applicable inspection plan or regulatory requirement.

Because HIC and SOHIC do not follow a standard corrosion-rate-based remaining
life model, the interval for V-1201 is also governed by the requirement to
perform enhanced NDE (TOFD/PAUT) at a frequency that detects and tracks HIC
progression before it reaches a critical size. The interval for TOFD/PAUT
scanning shall be determined by the assessment engineer based on detected
damage extent (from initial TOFD/PAUT results) and growth rate assumptions.

**Maximum interval constraints:**
API 510 maximum internal inspection interval: [PLACEHOLDER -- confirm per API 510
current edition; 10 years with RBI basis is commonly cited but the specific
requirements shall be taken from the current standard].
Regulatory / jurisdictional maximum: [PLACEHOLDER: confirm with local authority].

---

## 13. DEFERRAL AND ESCALATION TRIGGERS

**Conditions requiring immediate escalation:**
- [x] Measured thickness below t_required at any CML (SC2-06 -- currently under FFS review)
- [x] Corrosion rate significantly higher than planning rate (cannot assess until rate established)
- [x] New damage mechanism identified (HIC/SOHIC suspected but not yet confirmed)
- [x] Process chemistry exceedance (H2S chemistry data not available -- escalation trigger if H2S exceeds NACE MR0175 threshold)
- [ ] Equipment operating outside design limits (not identified)
- [ ] Any leak, crack, or visible flaw identified (not identified at this time)
- [ ] Near-miss or integrity event on connected equipment
- [ ] Change in service or operating conditions

**Chemistry exceedance parameters triggering escalation:**

| Parameter   | Normal Limit                    | Escalation Threshold              | Action                                    |
|-------------|---------------------------------|-----------------------------------|-------------------------------------------|
| H2S         | [PLACEHOLDER -- process design] | Any increase above design basis   | Notify inspection and corrosion engineering; reassess DMR and inspection plan |
| CO2         | [PLACEHOLDER]                   | Any increase above design basis   | Reassess CO2 corrosion rate estimate      |
| pH          | [PLACEHOLDER]                   | pH < [PLACEHOLDER] or pH > [PLACEHOLDER] | Notify corrosion engineering; reassess damage mechanism activity |
| Chlorides   | [PLACEHOLDER]                   | Any detection above background    | Assess pitting and SCC potential          |

**Deferral criteria:**
- [x] Remaining life > 2x the deferred interval
- [x] No corrosion rate trend increase
- [x] No new damage mechanism identified
- [x] Formal engineering review completed and documented
- [ ] Regulatory authority consent obtained where required
- [x] Other: HIC/SOHIC must be excluded by TOFD/PAUT before any deferral can be considered

NOTE: Deferral of inspection for V-1201 is NOT RECOMMENDED while:
(a) CML SC2-06 thin reading is under FFS review.
(b) HIC/SOHIC has not been confirmed or excluded by TOFD/PAUT.
(c) PWHT status is unconfirmed.

**Authority for deferral approval:**
[PLACEHOLDER: owner-user inspection engineer per API 510; AI (Authorized Inspector)
concurrence required per jurisdiction]

---

## 14. DATA QUALITY NOTES

| Item | Data Parameter                     | Data Quality | Source                     | Action Required                    |
|------|------------------------------------|-------------|----------------------------|------------------------------------|
| 1    | H2S concentration                  | P -- Poor   | Not measured               | Obtain from process laboratory; CRITICAL |
| 2    | CO2 concentration                  | P -- Poor   | Not measured               | Obtain from process laboratory     |
| 3    | pH of water phase                  | P -- Poor   | Not measured               | Obtain from process laboratory; CRITICAL |
| 4    | Corrosion rate (measured)          | P -- Poor   | Not established            | Two-point UT history required; CRITICAL |
| 5    | PWHT status                        | P -- Poor   | Not confirmed              | Retrieve MDR; CRITICAL             |
| 6    | Inspection history (complete)      | F -- Fair   | Partial -- some records only | Retrieve all prior inspection reports |
| 7    | Allowable stress S                 | P -- Poor   | Code table not confirmed   | Obtain from ASME II Part D current edition |
| 8    | Fluid density                      | P -- Poor   | Not available              | Obtain from process engineering    |

**Data quality key:**  G = Good (measured, verified)   F = Fair (estimated, reasonable)   P = Poor (unknown, assumed)

**Significant data gaps affecting risk ranking or interval:**
The risk ranking and inspection interval for V-1201 are both PROVISIONAL due to
multiple POOR-quality data items. No finalized risk ranking or inspection interval
shall be issued until at minimum MD-1 (H2S), MD-5 (PWHT), MD-9 (corrosion rate),
and MD-12 (TOFD/PAUT results) are resolved.

---

## 15. ASSUMPTIONS

1. V-1201 is in continuous wet sour gas service. This is the basis for HIGH
   susceptibility ratings for wet H2S damage mechanisms.
2. Free water is present at operating conditions in V-1201 based on process
   description. Phase envelope confirmation not performed.
3. PWHT was NOT applied unless confirmed from fabrication records. This is the
   conservative assumption for SSC and SOHIC susceptibility rating.
4. All susceptibility ratings are PROVISIONAL pending confirmed chemistry data.
5. The consequence category of HIGH is based on the presence of toxic H2S in
   the process fluid. Quantitative consequence calculation has not been performed.

---

## 16. LIMITATIONS

1. This RBI document is PROVISIONAL. Risk ranking, inspection strategy, and
   inspection interval are all subject to revision when MISSING DATA items are
   resolved.
2. Quantitative API 581 risk calculation has not been performed. Qualitative
   screening per API 580 is used as an interim basis only.
3. The inspection effectiveness assessment for HIC and SOHIC reflects the
   capability of UT A-scan, which is POOR. Until TOFD/PAUT results are
   available, the inspection effectiveness factor cannot be assigned a value
   that reduces the risk ranking.
4. This document covers V-1201 only. Connected equipment and the broader CDU
   Train A equipment list must be covered by a separate RBI study.
5. This document does not constitute a formal API 581 risk-based inspection
   program. It is a planning-support document only.

---

## 17. APPROVAL BLOCK

| Role                          | Name | Signature | Date |
|-------------------------------|------|-----------|------|
| Prepared By                   | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Technically Reviewed By       | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Approved By                   | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |
| Client / Owner Acceptance     | [PLACEHOLDER] | [PLACEHOLDER -- NOT SIGNED -- DRAFT] | [PLACEHOLDER] |

---

*Template reference: API 580 and API 581, current editions. All risk ranking,
inspection interval determination, and NDE method selection shall be based on
the current editions of API 580 and API 581 or the applicable site RBI methodology.
This template does not substitute for engineering analysis.*

================================================================================
TEST / DRAFT / NOT FOR ISSUE
Smoke-test example document V1201-RBI-001 -- Al-Wadi Refinery (FICTIONAL)
All data is fictional and for template demonstration only.
================================================================================
