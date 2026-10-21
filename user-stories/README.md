# CoolSpot Zurich – User Stories

Backlog for a **prototype/MVP** of **CoolSpot Zurich** (repository: `coolspot-zurich`). The stories are self-contained and are the reference for development (see "Out of scope" for what is intentionally left out).

- **Timeline & milestones:** see [MILESTONES.md](MILESTONES.md)
- **Priority (MoSCoW):** all stories are MVP scope. Priority sets the build order and what could be deferred (by agreement) if time runs short.
  - **Must** – app is not usable/acceptable without it
  - **Should** – important, but the core flow works without it
  - **Could** – nice to have, first to defer

## Backlog

| ID | Story | Priority | Milestone |
|---|---|---|---|
| [US-01](US-01-project-setup.md) | Project setup & own API keys | Must | M1 |
| [US-02](US-02-data-model.md) | Data model & persistence | Must | M1 |
| [US-03](US-03-map-shell.md) | Full-page map & layout shell | Must | M1 |
| [US-04](US-04-create-google-place.md) | Add a Google place with first rating | Must | M1 |
| [US-05](US-05-create-custom-place.md) | Add a custom place | Must | M1 |
| [US-06](US-06-submit-assessment.md) | Rate an existing place | Must | M1 |
| [US-07](US-07-score-aggregation.md) | Coolness score & aggregated levels | Must | M1 |
| [US-08](US-08-place-details.md) | Place details panel | Must | M1 |
| [US-09](US-09-markers-and-list.md) | Markers, legend & list sync | Must | M1 |
| [US-10](US-10-initial-recommendations.md) | Initial recommendations | Must | M1 |
| [US-11](US-11-browse-all.md) | Browse all places | Must | M1 |
| [US-12](US-12-search-this-area.md) | "Search this area" | Must | M2 |
| [US-13](US-13-filters.md) | Filters | Must | M2 |
| [US-14](US-14-error-states.md) | Basic loading & error states | Must | M2 |
| [US-15](US-15-edit-place-info.md) | Edit place information | Should | M2 |
| [US-16](US-16-comments.md) | Comments | Should | M2 |
| [US-17](US-17-search-name-address.md) | Search by name or address | Could (optional) | M2 (optional) |
| [US-18](US-18-handover.md) | Handover & documentation | Must | M2 |

## Shared definitions (used across stories)

- **Eligible:** location lies inside the **city of Zurich** (municipal boundary). Only eligible places can be created or appear in results.
- **POI / saved place:** a place stored in the app. Not every Google business is a POI.
- **Rated / unrated:** rated = at least one cooling assessment.
- **Coolness score:** mean of all cooling values (1–4), shown with 1 decimal.
- **Band:** unrounded mean `< 1.5` → 1, `1.5–<2.5` → 2, `2.5–<3.5` → 3, `≥ 3.5` → 4.

| Level | Cooling | Noise | Typical crowding |
|---|---|---|---|
| 4 | A lot cooler | Noisy | Usually crowded |
| 3 | Slightly cooler | Normal | Busy |
| 2 | Same as outside | Relatively quiet | Moderately busy |
| 1 | Hotter | Silent | Usually quiet |

- **Coolness order:** unrounded score desc → assessment count desc → name A–Z → stable ID.
- **Categories:** Parks and gardens · Libraries and study spaces · Public buildings · Cafés · Restaurants · Swimming and waterside locations · Other. No free-text categories.
- **Price band:** Free · CHF 1–20 · CHF 21–40 · CHF 41–80 · CHF 81+ · Unknown. Price = minimum spend for one person to use the place for cooling.
- **Input rules**, apply to all forms: name 2–100 chars · comment 1–500 chars (trimmed) · access/cost notes ≤ 500 chars · CHF cost ≥ 0. Inline errors, input preserved on error, submitted HTML/scripts never executed.
- **Anonymous:** no sign-in, no browser identity, no per-person limits anywhere.

## Out of scope (whole project)

**Removed for the prototype:** "Add place" button (custom places are added via map click) · category search (use the category filter instead) · radius filter · "Mark as irrelevant" votes · formal performance benchmark · keyboard/accessibility and viewport requirements · marker clustering · amenity filters (shade, AC, water, toilets, seating, accessible entrance, crowding) · advanced error handling for partial Google failures.

**Also excluded:** Deployment / hosting (the app only needs to run locally) · remote database (local DB such as SQLite is fine) · provided Google API keys (client brings own keys) · user accounts / contributor identity / repeat-vote controls · admin users, moderation, deletion of POIs, assessments or comments · changing POI coordinates or Google Place IDs · mobile/tablet/touch layouts, offline maps, other languages · browser geolocation · in-app routing · live push updates · custom spelling correction, autocomplete, natural-language search.
