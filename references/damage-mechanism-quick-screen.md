# Damage Mechanism Quick-Screen Matrix

Controlled reference and **screening aid only**. This matrix lists commonly
associated damage mechanisms by service condition to support the damage mechanism
review (DMR). It does **not** replace API 571 or the full DMR template
(`templates/damage-mechanism-review/`). Every mechanism flagged here must be
confirmed against API 571 and the equipment's actual materials, process chemistry,
temperatures, and history before it is carried into a report. Absence from this
table is not evidence that a mechanism is not credible.

> Mechanism applicability depends strongly on material, temperature, concentration,
> pH, velocity, stress, and the presence of water/condensation. Use the temperature
> ranges, susceptibility factors, and exclusions in the controlling API 571 edition.
> Do not assert that a mechanism is active or absent without that basis.

---

## 1. Service / condition to candidate mechanism associations

| Service or condition | Candidate mechanisms to screen (confirm per API 571) |
|---|---|
| Wet H2S (per NACE definition) | Hydrogen blistering; hydrogen-induced cracking (HIC); stress-oriented HIC (SOHIC); sulfide stress cracking (SSC) |
| Chlorides + austenitic stainless steel + temperature | Chloride stress corrosion cracking (Cl-SCC) |
| Caustic (NaOH/KOH) service | Caustic stress corrosion cracking (caustic embrittlement); caustic corrosion |
| Amine treating units | Amine stress corrosion cracking; amine corrosion |
| Carbonate-containing alkaline sour water | Alkaline carbonate stress corrosion cracking (ACSCC) |
| CO2 + water | Carbon dioxide (CO2) corrosion |
| Hydrofluoric (HF) acid alkylation | HF acid corrosion; relevant environmental cracking in HF service |
| Sulfuric acid service | Sulfuric acid corrosion |
| High-temperature hydrogen partial pressure (carbon/low-alloy steel) | High temperature hydrogen attack (HTHA) — screen against the relevant material/temperature/H2 partial-pressure limits |
| Elevated temperature, long-term (above the creep threshold for the material) | Creep / stress rupture |
| Insulated equipment in the susceptible external temperature band | Corrosion under insulation (CUI) |
| Austenitic stainless steel exposed to sensitizing temperatures | Sensitization / intergranular attack; polythionic acid stress corrosion cracking (PASCC) on shutdown |
| Cyclic pressure or thermal loading | Mechanical and thermal fatigue |
| High-velocity / two-phase / impingement flow | Erosion / erosion-corrosion |
| Dead legs, low points, intermittent wetting | Localized / under-deposit corrosion; microbiologically influenced corrosion (MIC) |
| Injection and mixing points | Localized corrosion/erosion at the point of injection |
| Soil-to-air or buried interfaces, supports, and contact points | External / galvanic / crevice corrosion at contact points |
| Carbon steel in oxygenated water | General/oxygen corrosion; pitting |

---

## 2. How to use

1. List the equipment's actual materials, fluids, concentrations, temperatures,
   pressures, and operating history.
2. For each row that matches the service, screen the candidate mechanisms against
   API 571 (temperature ranges, susceptibility factors, required conditions).
3. Carry credible mechanisms into the API 571 DMR template with the basis for each.
4. Record mechanisms considered and screened out, with the reason.
5. Set CML placement and NDE method selection from the credible mechanisms
   (damage-mechanism-first placement, per `CLAUDE.md`).

---

## 3. Cross-references

- `templates/damage-mechanism-review/api-571-damage-mechanism-review-template.md`
- `templates/CML-UT-mapping/cml-ut-thickness-mapping-template.md`
- `CLAUDE.md` — governing standards list and CML placement guidance.
