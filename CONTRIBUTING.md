# Contributing and Document Control

This repository is a controlled engineering workspace. Engineering calculations,
assumptions, inputs, and outputs must be traceable. The following rules govern all
changes.

---

## 1. Technical accuracy (non-negotiable)

- Do not fabricate clause numbers, formulas, material properties, allowable
  stresses, acceptance criteria, or inspection requirements. This applies to every
  template, reference, example, and report.
- Code clause numbers and values are taken from the **controlling edition** of the
  governing code and recorded with the edition. Do not state code chart values
  (e.g., UCS-66 curves, ASME II-D allowables, API 579 screening constants) from
  memory.
- Where a value must come from the code and is not yet confirmed, leave a field and
  mark it as a hold point rather than entering an assumed value.
- Worked examples that use illustrative inputs must label them clearly as
  illustrative and not as code lookups.

See `CLAUDE.md` for the governing engineering approach and `references/` for the
controlled conventions.

---

## 2. Revision and status convention

- Each controlled template, reference, and report carries a document number,
  revision, and status.
- Status values: `draft`, `issued_for_review`, `issued`, `superseded`.
- Increment the revision on any technical change. Record what changed in the
  `CHANGELOG.md`.
- A `superseded` document is retained for traceability and references the document
  that replaces it.

---

## 3. Branch, commit, and pull request workflow

1. Create a feature branch from `main` (e.g., `feature/<short-description>`).
2. Make additive, reviewable changes. Avoid large rewrites of controlled documents
   when a small surgical change suffices.
3. Use a single logical commit per change set where practical.
4. Open a pull request using the PR template. Fill the technical-accuracy
   checklist.
5. At least one independent technical review is required before merge for any
   change that affects a formula, clause reference, acceptance criterion, or
   numeric value.
6. Merge to `main` only after the checklist is satisfied.

---

## 4. Review checklist (summary)

- Formulas match the cited code paragraph for the controlling edition.
- Corroded geometry is used where required.
- Governing required thickness uses `max(t_pressure, t_UG16b, t_struct)`.
- Units are consistent; every value carries a unit.
- No code chart value is entered from memory.
- Assumptions and limitations are stated.
- The change is recorded in `CHANGELOG.md`.

The full checklist is in `.github/pull_request_template.md`.

---

## 5. Cross-references

- `CLAUDE.md`
- `references/symbols-and-conventions.md`
- `references/minimum-thickness-governing-logic.md`
- `references/corrosion-rate-and-interval-conventions.md`
- `references/input-data-schema.md`
