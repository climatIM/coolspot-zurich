# US-03 · Full-page map & layout shell

**Priority:** Must · **Milestone:** M1 · **Depends on:** US-01

## Story
As a **student**, I want a full-screen map of the city of Zurich with all main controls at hand – on my laptop or my phone – so that I can start looking for cool places right away.

## Acceptance criteria
- [ ] Google Map fills the viewport and initially frames the **city of Zurich**.
- [ ] Filters, the marker legend and (if US-17 is built) search are always reachable.
- [ ] **Responsive layout** for desktop and mobile (from 360 px width), without horizontal scrolling:
  - desktop: side panel for results and place details next to the map;
  - mobile: map stays full-screen; results and details open in a bottom sheet or full-screen panel that can be closed to return to the map.
- [ ] Works with mouse and touch: tapping behaves like clicking (markers, map spots, list entries); controls are large enough to tap.
- [ ] The city boundary is available to the app for eligibility checks (used by creation and search stories). The map itself may be panned beyond the city.
- [ ] **No** "Use my location" control and no user-position marker.
- [ ] App name "CoolSpot Zurich"; English UI; currency CHF.
- [ ] Polished style on desktop and mobile: one consistent font throughout (developer's choice), readable controls, cooling and cost info visually prominent.
