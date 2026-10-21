# Milestones

Two milestones. Each ends with a **local demo** (app started via e.g. `npm run start`) and client sign-off. No fixed dates – the whole project is expected to take roughly 1–3 weeks.

```
M1 Setup & core functionality ─► M2 Additional features & delivery
```

## M1 · Setup & core functionality
**Goal:** The app runs locally with the client's own API key. Students can add and rate places, see scores and details, and discover places via recommendations and browsing.

| Story | Priority |
|---|---|
| US-01 Project setup & own API keys | Must |
| US-02 Data model & persistence | Must |
| US-03 Full-page map & layout shell | Must |
| US-04 Add a Google place with first rating | Must |
| US-05 Add a custom place | Must |
| US-06 Rate an existing place | Must |
| US-07 Coolness score & aggregated levels | Must |
| US-08 Place details panel | Must |
| US-09 Markers, legend & list sync | Must |
| US-10 Initial recommendations | Must |
| US-11 Browse all places | Must |

**Done when:**
- after adding an API key to `.env`, one start command shows the map framed on the city of Zurich (usable on desktop and mobile width) and creates the local database;
- a place added and rated in one browser shows the correct score, band and marker in another browser after refresh;
- recommendations and browse ordering match US-10 and US-11.

## M2 · Additional features & delivery
**Goal:** Extra discovery and community features, basic error handling, and a complete handover so the client can run the app with their own keys.

| Story | Priority |
|---|---|
| US-12 "Search this area" | Must |
| US-13 Filters | Must |
| US-14 Basic loading & error states | Must |
| US-15 Edit place information | Should |
| US-16 Comments | Should |
| US-17 Search by name or address | Could (optional) |
| US-18 Handover & documentation | Must |

**Done when:** acceptance test passes in current Chrome on desktop and on a mobile device (or Chrome mobile emulation) on a fresh local setup with the client's own keys, and source, schema and docs are handed over. Optional stories only count if they were built.

## If time gets tight
1. Skip the optional search story (US-17) first, then defer **Should** stories (US-15, US-16) – only after agreement with the client.
2. **Must** stories are never dropped; US-14 states should be built alongside each feature, not only at the end.
