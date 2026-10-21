# US-08 · Place details panel

**Priority:** Must · **Milestone:** M1 · **Depends on:** US-07

## Story
As a **student**, I want to see everything known about a place, so that I can decide whether to go there.

## Acceptance criteria
- [ ] Side panel shows:

| Section | Content |
|---|---|
| Name & categories | Google or custom name; all community categories (Google-mapped categories as fallback for unrated places) |
| Location | Address if available, otherwise coordinates |
| Cooling | Score, band label, assessment count, last contribution date |
| Noise & crowding | Aggregated levels + counts |
| Google rating | Stars and review count, shown **separately** (display only) |
| Price band | Free · CHF 1–20 · 21–40 · 41–80 · 81+ · Unknown |
| Cost details | Optional exact CHF cost + what it covers |
| Opening hours | Google hours or custom hours; may be Unknown |
| Shade | None · Partial · Mostly shaded · Unknown |
| AC, drinking water, toilets, seating | Yes · No · Unknown each |
| Access restrictions | Optional text (e.g. "student ID required") |
| Comments | See US-16 |

- [ ] Missing values show "Unknown" / "Not yet rated" – unknown never implies "No".
- [ ] Google vs. community information is **visually distinguished**.
- [ ] Google price level (if shown) keeps its original meaning – no CHF conversion.
- [ ] Google open-now status is labelled as coming from Google; no open-now calculation for custom hours.
- [ ] Actions: **"Directions in Google Maps"** (opens Google Maps by Place ID, else coordinates, in a new tab), **"Edit place information"** (US-15), **"Add rating"** (US-06), **"Add comment"** (US-16).
- [ ] Optional sections may be collapsible.

## Notes
- Prices are informational only, no booking.
- Custom opening hours are stored and shown as text; no open-now calculation for them.
