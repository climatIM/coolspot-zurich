# US-13 · Filters

**Priority:** Must · **Milestone:** M2 · **Depends on:** US-11

## Story
As a **student**, I want to filter places (e.g. only free, quiet libraries), so that I only see places that suit me.

## Acceptance criteria
- [ ] Filter groups: **cooling band · noise band · category · price band**.
- [ ] Logic: **AND** between groups, **OR** within a group.
  - e.g. Category = Café OR Library **and** Price = Free → free cafés or libraries.
- [ ] Filters apply to recommendations, browse and (if built) search; list and markers update together.
- [ ] Active filters are visible and removable, plus **"Clear all"**.
- [ ] Filters are applied **before** ranking (ordering of US-11 / US-17 still holds).

## Notes
- Assumption: unrated places have unknown bands, so cooling/noise band filters exclude them.
- Amenity and crowding filters are out of scope for the prototype.
