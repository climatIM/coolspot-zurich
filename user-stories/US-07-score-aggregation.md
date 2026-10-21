# US-07 · Coolness score & aggregated levels

**Priority:** Must · **Milestone:** M1 · **Depends on:** US-06

## Story
As a **student**, I want a clear coolness score per place, so that I can compare places at a glance.

## Acceptance criteria
- [ ] Coolness = arithmetic mean of all cooling values, shown with **1 decimal** (1–4 scale).
- [ ] Noise and crowding are averaged separately; missing crowding answers are excluded. Neither affects coolness.
- [ ] Bands use the **unrounded** mean (`<1.5`, `1.5–<2.5`, `2.5–<3.5`, `≥3.5`) and the labels from the README table.
  - e.g. mean 3.46 → shown "3.5" but band 3 "Slightly cooler".
- [ ] No assessments → "Unknown"/"Not yet rated", never 0.
- [ ] Show assessment count (not unique contributors) and date of the latest assessment.
- [ ] Assessments never expire. Comments and Google ratings never change aggregates.
- [ ] Values are recalculated on open/refresh (no live push needed).
- [ ] Unit tests cover mean, band boundaries (1.5, 2.5, 3.5) and empty case.
