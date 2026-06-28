# Symbols, Notation, and Engineering Conventions

Controlled reference. This document is the single source of truth for symbol
definitions, sign conventions, and units used across all templates and
calculations in this repository. Where a template uses a symbol, it shall carry
the meaning defined here. If a calculation needs a symbol not listed here, define
it explicitly in that calculation and, where it is reusable, add it to this list
by pull request.

---

## 1. General rules

- All pressure-thickness and MAWP calculations use **corroded geometry** unless a
  code basis requires otherwise (see `CLAUDE.md`).
- Pressures are **gauge** unless explicitly noted as absolute. Tables that mix the
  two shall state which is which.
- SI is the primary unit system; US customary is given in parentheses where
  helpful. Every reported value carries its unit. Mixed-unit substitution is not
  permitted within a single equation.
- Code clause numbers, allowable stresses, material properties, and acceptance
  constants are taken from the controlling edition of the governing code. They are
  never assumed from memory. See `CLAUDE.md`.

---

## 2. Geometry symbols

| Symbol | Definition | Notes |
|---|---|---|
| D | Inside diameter (nominal, uncorroded) | shell or head as stated |
| D_c | Corroded inside diameter = D + 2·CA | used in head and cone formulas |
| R | Inside radius (nominal, uncorroded) | R = D / 2 |
| R_c | Corroded inside radius = R + CA | used in shell formulas |
| L | Inside crown radius of a torispherical head (corroded where applicable) | UG-32(d) |
| r | Inside knuckle radius of a torispherical head | UG-32(d) |
| L_h | Inside radius of a hemispherical head (corroded where applicable) | UG-32(e) |
| h | Inside depth of a formed head | for 2:1 ellipsoidal, h = D / 4 |
| alpha | Half-apex angle of a conical section | degrees; cos(alpha) used in UG-32(f) |
| H | Vessel height (vertical) or inside diameter (horizontal) used as static-head column | per static-head rule in `CLAUDE.md` |

---

## 3. Thickness symbols

| Symbol | Definition |
|---|---|
| t_nom | Nominal (new) thickness from the drawing or data sheet |
| t_meas | Current measured thickness from inspection (e.g., UT) |
| t_prev | Previous measured thickness used for short-term corrosion rate |
| t_c | Corroded thickness available for pressure = t_meas − FCA (or − CA where CA is treated as future loss) |
| CA | Corrosion allowance (as specified) |
| FCA | Future corrosion allowance (metal loss reserved for the next interval) |
| UTL | Mill undertolerance (per material specification) |
| t_pressure | Required thickness from the applicable pressure formula (UG-27 / UG-32), in corroded condition |
| t_UG16b | Code minimum thickness floor per ASME VIII-1 UG-16(b), exclusive of corrosion allowance (see governing-logic reference) |
| t_struct | Minimum thickness required for structural / handling / supplemental loads, where applicable |
| t_req | **Governing required thickness** = max(t_pressure, t_UG16b, t_struct). See `minimum-thickness-governing-logic.md`. |
| t_min | Used interchangeably with t_req in inspection reporting; always the **governing** required thickness, not the pressure value alone |

> **Discipline note:** Older worksheets sometimes set `t_min = t_pressure`. In this
> repository `t_min` always means the **governing** required thickness, which may
> be set by UG-16(b) rather than by pressure on thin, large-diameter, or
> low-pressure components.

---

## 4. Stress, pressure, and efficiency symbols

| Symbol | Definition |
|---|---|
| P | Design or assessment pressure used in the formula (gauge), including static head where applicable |
| P_static | Hydrostatic head contribution to pressure |
| P_op | Operating pressure |
| MAWP | Maximum allowable working pressure (corroded condition unless stated) |
| S | Allowable stress at the temperature of interest (from ASME II Part D for the controlling edition) |
| S_test | Allowable stress at hydrostatic test temperature |
| S_design | Allowable stress at design temperature |
| S_y | Specified minimum yield strength (from code) |
| S_u | Specified minimum ultimate tensile strength (from code) |
| E | Weld joint efficiency (UW-12), consistent with the radiography actually credited |
| LSR | Lowest stress ratio = min over all pressure-boundary materials of (S_test / S_design); governs UG-99(b) test pressure |

---

## 5. Corrosion-rate and life symbols

| Symbol | Definition |
|---|---|
| CR_ST | Short-term corrosion rate (see corrosion-rate reference) |
| CR_LT | Long-term corrosion rate |
| CR_gov | Governing corrosion rate selected for life and interval |
| RL | Remaining life |

Definitions and selection logic are in `corrosion-rate-and-interval-conventions.md`.

---

## 6. FFS (API 579-1/ASME FFS-1) symbols

| Symbol | Definition |
|---|---|
| t_mm | Minimum measured thickness in sound metal within the assessment zone |
| t_rem | Local remaining thickness (e.g., below a pit), as measured |
| RSF | Remaining strength factor (computed) |
| RSF_a | Allowable remaining strength factor (default 0.90 for ASME VIII-1; confirm per controlling edition) |
| MAWP_r | Reduced MAWP when RSF < RSF_a, per the API 579 reduction relation |

> The numeric Level-1 screening constants in Part 6 (e.g., remaining-thickness-ratio
> thresholds and pit dimension/spacing limits) are **edition dependent** and must be
> read from the controlling API 579-1/ASME FFS-1 edition. They are not reproduced
> here as authoritative values.
