# Corrosion Rate and Inspection Interval Conventions

Controlled reference. Defines how corrosion rates, remaining life, and inspection
intervals are calculated and selected across the inspection and FFS templates.
Interval limits are stated per API 510; the controlling API 510 edition governs in
all cases and shall be confirmed before issue.

---

## 1. Corrosion rate definitions

**Long-term corrosion rate** uses the original or earliest reliable baseline
thickness:

```
CR_LT = (t_initial − t_actual) / (time between t_initial and t_actual)
```

- `t_initial` is the nominal/new thickness or the earliest reliable measured
  thickness at the same location.
- The time span is the actual elapsed time in years between the two readings.

**Short-term corrosion rate** uses the most recent previous reading:

```
CR_ST = (t_previous − t_actual) / (time between t_previous and t_actual)
```

- The time span is the actual interval between the previous and current
  inspections, not a nominal value.

Both rates shall be computed at the **same location / CML**. Comparing readings
from different locations does not yield a valid rate.

---

## 2. Selecting the governing corrosion rate

- Compute both CR_LT and CR_ST where data allow.
- The **governing corrosion rate** is selected by engineering judgment. A
  conservative default is the larger of the two:

```
CR_gov = max(CR_LT, CR_ST)
```

- If the short-term rate is significantly higher than the long-term rate, this may
  indicate a change in service, a new or accelerating damage mechanism, or
  measurement scatter; investigate before accepting a rate.
- The basis for the selected rate shall be stated in the report (which rate was
  chosen and why).
- Negative apparent rates (later reading thicker than earlier) usually indicate
  measurement uncertainty or different exact locations; do not report a negative
  corrosion rate as a real value. Treat as measurement scatter and document.

---

## 3. Remaining life

```
RL = (t_actual − t_req) / CR_gov
```

where `t_req` is the **governing** required thickness per
`minimum-thickness-governing-logic.md` (which may be set by UG-16(b), not pressure
alone). Remaining life is the time until the measured thickness reaches the
governing required thickness at the selected corrosion rate.

---

## 4. Inspection interval (API 510 basis)

Per API 510, the maximum period between internal or on-stream inspections is set
to the **lesser of one-half the remaining life or the maximum interval permitted
by the code**. Commonly applied limits (confirm against the controlling edition):

- Internal or on-stream inspection interval: the lesser of one-half the remaining
  life or the code maximum for internal/on-stream inspection.
- External inspection interval: the code maximum for external visual inspection.
- Risk-based inspection (RBI), where established per API 580/581, may set the
  interval in place of the prescriptive limits, subject to the conditions and
  reassessment frequency required by the code.

```
Interval = min( RL / 2 , API 510 prescriptive maximum , RBI-derived interval )
```

> The specific numeric maximum intervals (years) are edition-dependent and are
> not reproduced here as fixed values. Read them from the controlling API 510
> edition and record the figure used, with the clause cited. Do not extend an
> interval beyond the prescriptive maximum without an RBI assessment or
> engineering justification accepted by the Authorized Inspector.

---

## 5. Reporting requirements

Each remaining-life / interval determination shall record:

- the CML(s) and locations used,
- CR_LT, CR_ST, and the governing CR with selection basis,
- the governing required thickness and which criterion set it,
- the remaining life, the half-life, and the prescriptive maximum considered,
- the recommended next inspection date and type,
- the controlling code edition.

---

## 6. Cross-references

- `references/minimum-thickness-governing-logic.md`
- `references/symbols-and-conventions.md`
- `templates/inspection-plan/api-510-pressure-vessel-inspection-report-template.md`
- `templates/inspection-plan/rbi-inspection-planning-template.md`
