# Pull Request

## Summary

<!-- What does this change do and why? -->

## Type of change

- [ ] New controlled template
- [ ] New reference / convention document
- [ ] Worked example
- [ ] Technical correction to an existing template (formula / clause / criterion)
- [ ] Editorial / structural (no technical content change)
- [ ] Governance / tooling

## Technical accuracy checklist (required)

- [ ] No clause numbers, formulas, allowable stresses, material properties, or
      acceptance criteria were fabricated or entered from memory.
- [ ] All code references identify the controlling edition / addenda.
- [ ] Code chart values (e.g., ASME II-D allowables, UCS-66 curves, API 579
      screening constants) are read from the code or left as hold points, not
      assumed.
- [ ] Pressure-thickness and MAWP calculations use corroded geometry where required.
- [ ] Governing required thickness uses `max(t_pressure, t_UG16b, t_struct)`.
- [ ] Units are consistent within every equation; every reported value carries a unit.
- [ ] Any worked-example inputs that are illustrative are labeled as illustrative,
      not as code lookups.
- [ ] Assumptions and limitations are stated.

## Review

- [ ] Independent technical reviewer assigned.
- [ ] `CHANGELOG.md` updated.
- [ ] Affected `references/` cross-links updated.

## Notes for the reviewer

<!-- Anything specific to check, known limitations, or follow-up items. -->
