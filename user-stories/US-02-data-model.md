# US-02 · Data model & persistence

**Priority:** Must · **Milestone:** M1 · **Depends on:** US-01

## Story
As the **developer**, I want a persistent data model for places, assessments and comments, so that community data survives refreshes and is shared across browsers.

## Acceptance criteria
- [ ] A **local database** is sufficient (e.g. SQLite file); no remote DB required. It is created automatically on first start.
- [ ] Entities exist (physical schema is free):

| Entity | Minimum fields |
|---|---|
| POI | internal ID · optional **unique** Google Place ID · name · coordinates · custom fields · derived categories · optional visitor info · source provenance · created/updated timestamps |
| Assessment | ID · POI ID · cooling · noise · optional crowding · ≥ 1 category · timestamp |
| Comment | ID · POI ID · text · timestamp |

- [ ] A POI is only visible if it has a name and coordinates.
- [ ] Provenance is stored per field: Google-sourced vs. community-contributed. Confirming a prefilled Google value does **not** make it community data.
- [ ] Only Place IDs and community data are stored permanently; Google content is cached only as allowed by Google's terms.
- [ ] No contributor identity, accounts, admin or moderation records.

## Notes
- Visitor info fields: price band, exact CHF cost + explanation, opening hours, shade, air conditioning, drinking water, toilets, seating, access restrictions (see US-08).
