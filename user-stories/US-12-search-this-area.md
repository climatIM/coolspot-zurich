# US-12 · "Search this area"

**Priority:** Must · **Milestone:** M2 · **Depends on:** US-11

## Story
As a **student**, I want to move the map and search only the visible area, so that I find cool places where I'm going.

## Acceptance criteria
- [ ] A **"Search this area"** button reruns the current browse (or search, if US-17 is built) for the viewport **intersected with the city of Zurich**.
- [ ] The map center at submit time is the origin for radius-based requests.
- [ ] Moving or zooming the map alone triggers **no** API request.
- [ ] No browser geolocation, no IP-based location, no user position shown.
- [ ] Results ordered and paginated as in US-11 (or US-17 for searches).
