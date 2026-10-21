# US-17 · Search by name or address

**Priority:** Could (optional) · **Milestone:** M2 (optional) · **Depends on:** US-04, US-09

## Story
As a **student**, I want to search for a place by name or address – even with typos – so that I can find out how cool it is.

## Acceptance criteria
- [ ] Query is sent to Google **and** matched against saved places (incl. custom places without Place ID).
- [ ] Partial/misspelled queries rely on Google's matches (no own spell-checker).
- [ ] Results: eligible places only (city of Zurich), active filters applied, deduplicated by Place ID; Google and community data of the same POI are combined.
- [ ] **Exact search** = query equals an eligible result's full name or address (case-insensitive, trimmed). Order:
  1. Google's first eligible result (even if unrated)
  2. remaining rated matches – coolness order
  3. remaining unrated Google results – Google relevance
- [ ] **Non-exact search** order:
  1. up to 5 rated matches – coolness order (fewer if fewer exist)
  2. best-matching unrated Google result, labelled "Add rating" (skip if none)
  3. remaining rated matches – coolness order
  4. remaining unrated Google results – Google relevance
- [ ] Ordering is applied to the **combined** list first, then paginated in batches of 10; "Load more" continues without repeats (the "first 5" rule applies once per search, not per page).
- [ ] Unrated Google results are labelled **"Add rating"**; Google stars/review counts are display-only and never affect ranking.
- [ ] Selecting an unrated Google result (or an address result) opens the creation form directly (US-04, or US-05 without Place ID); searching alone never creates a place.
- [ ] No results → "No matching place found" with a way to retry.

## Notes
Optional for the prototype: build only if time allows, after the other M2 stories. Without it, places are found via recommendations, browse, "Search this area" and filters.

## Out of scope
Separate preview of unrated Google results, autocomplete, natural-language search, exhaustive Google coverage.
