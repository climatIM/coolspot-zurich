# US-18 · Handover & documentation

**Priority:** Must · **Milestone:** M2 · **Depends on:** all Must stories

## Story
As the **client**, I want the source code and clear instructions, so that I can run the app locally with my own API keys without help from the developer.

## Acceptance criteria
- [ ] Delivered: frontend + backend source code and database schema (or migrations).
- [ ] README describes: prerequisites (e.g. Node.js version), install, configuration, start command (e.g. `npm run start`).
- [ ] All environment variables are documented (`.env.example`).
- [ ] Google API guide: which APIs to enable, which keys are needed, recommended key restrictions (origin/API), and a note on quotas and billing alerts.
- [ ] Local database is created automatically on first start (or with one documented command); optional seed/test data script.
- [ ] No API keys or other secrets in the repository.
- [ ] A fresh clone + own keys + documented steps = working app (verified once on a clean machine/checkout).

## Notes
Deployment and hosting are not required. No admin interface or moderation guide needed.
