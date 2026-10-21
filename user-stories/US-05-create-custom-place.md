# US-05 · Add a custom place

**Priority:** Must · **Milestone:** M1 · **Depends on:** US-04

## Story
As a **student**, I want to add a place Google doesn't know (e.g. a shaded bench), so that hidden cool spots appear on the map.

## Acceptance criteria
- [ ] Clicking a map spot without a Google Place ID opens a coordinate-based creation form.
- [ ] The selected position is shown on the map before saving.
- [ ] Required: name, position inside the city of Zurich, ≥ 1 category ("Other" allowed), cooling, noise. Optional: crowding and visitor info.
- [ ] Position outside the city is rejected inline.
- [ ] If an existing POI lies **within 30 m**, show a duplicate warning but still allow saving.
- [ ] Save, failure and cancel behave as in US-04 (persisted, opens details, no false success, cancel creates nothing).
- [ ] Input rules from README apply.

## Out of scope
Separate "Add place" button – adding via map click is enough. Fuzzy duplicate matching, automatic merging.
