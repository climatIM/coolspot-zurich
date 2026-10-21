# US-04 · Add a Google place with first rating

**Priority:** Must · **Milestone:** M1 · **Depends on:** US-02, US-03

## Story
As a **student**, I want to click a Google place on the map and rate it, so that others learn how cool it is.

## Acceptance criteria
- [ ] Clicking an **unsaved** Google POI (with Place ID) opens a creation form prefilled from Google.
- [ ] Clicking an **existing app POI** opens its details instead (no form).
- [ ] Required: valid Place ID, resolved position, name, ≥ 1 category, cooling, noise. Optional: crowding and visitor info.
- [ ] Google types pre-select suggested categories; the user can change them. Unmapped types → "Other".
- [ ] Place must be inside the city of Zurich, otherwise it cannot be saved.
- [ ] If the Google lookup fails: show error with retry; no partial record is saved.
- [ ] A Place ID that already exists reopens that POI – never a duplicate.
- [ ] Successful save stores POI **and** first assessment, closes the form, opens details. Data persists after refresh, restart of the app and in another browser.
- [ ] A failed save never shows success; input is preserved.
- [ ] Input rules from README apply.
- [ ] Cancel creates nothing.

## Notes
- Rating form content (scales, wording "usual hot-weather conditions") is defined in US-06 and reused here.
