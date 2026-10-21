# US-06 · Rate an existing place

**Priority:** Must · **Milestone:** M1 · **Depends on:** US-04

## Story
As a **student**, I want to add my own assessment to a saved place, so that its rating reflects more experiences.

## Acceptance criteria
- [ ] "Add rating" on a place opens the assessment form; the question refers to **usual hot-weather conditions**.
- [ ] Fields (scales see README):
  - Cooling – required (4 = A lot cooler … 1 = Hotter)
  - Noise – required (1 = Silent … 4 = Noisy)
  - Typical crowding – optional (1 = Usually quiet … 4 = Usually crowded)
  - Categories – required, ≥ 1, multi-select from the fixed list
- [ ] Each submission creates a **new** assessment immediately – no sign-in, no approval.
- [ ] Repeated submissions from the same browser all count; nothing is replaced or deduplicated.
- [ ] Place categories = **union** of categories over all its assessments (no majority vote, no primary category).
- [ ] Details refresh and show the updated values after saving.

## Out of scope
Editing or retracting past assessments; per-person limits.
