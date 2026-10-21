# US-01 · Project setup & own API keys

**Priority:** Must · **Milestone:** M1 · **Depends on:** –

## Story
As the **client**, I want a project that runs locally with one command and uses Google API keys I provide myself, so that I can run the app as soon as I receive the code.

## Acceptance criteria
- [ ] Repository with frontend and backend; after installing dependencies, `npm run start` (or a similarly simple command) starts the whole app locally.
- [ ] Google API keys are read from configuration (e.g. a `.env` file) – **no keys are included in the code or delivered**.
- [ ] `.env.example` lists every required variable with a short description.
- [ ] Missing or invalid key → clear message in the app/console explaining what to configure (no silent failure).
- [ ] Any server-side key stays on the server and is never sent to the browser.

## Notes
- Stack choice is the developer's.
- Which Google APIs to enable and how to restrict keys is documented in US-18.
- Deployment to a server or hosting is **not** required.
