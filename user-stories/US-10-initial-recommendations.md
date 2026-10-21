# US-10 · Initial recommendations

**Priority:** Must · **Milestone:** M1 · **Depends on:** US-09

## Story
As a **student**, I want to see the coolest places per category when I open the app, so that I get useful suggestions without searching.

## Acceptance criteria
- [ ] On load, select per category the **top 2 rated places** (coolness order) across the city of Zurich.
- [ ] Only places with ≥ 1 real cooling assessment qualify. Categories with 0–1 rated places contribute 0–1. No filling with Google ratings, unrated or invented places.
- [ ] Merge all selections, deduplicate by POI ID (a multi-category place appears once; no backfill of the freed slot), sort by coolness order.
- [ ] List shows 10 entries, "Load more" adds 10 at a time; the map shows the **whole** selection.
- [ ] A **"Recommendations"** control restores this view from browse/search.

## Example
Cafés: A (3.8), B (3.6), C (3.1) → A, B. Parks: B (3.6), D (2.9) → B, D. Result: A, B, D (B only once).
