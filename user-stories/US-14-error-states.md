# US-14 · Basic loading & error states

**Priority:** Must · **Milestone:** M2 · **Depends on:** M1 stories

## Story
As a **student**, I want basic feedback when something loads or fails, so that I'm never stuck or misled.

## Acceptance criteria
- [ ] Loading indicator while results load and while a form is saving.
- [ ] No results → short hint plus a **"Clear filters"** action.
- [ ] Failed save → error message, input preserved; never a false success.
- [ ] Map or Google API fails to load → readable message with **Retry**.

## Notes
Build these alongside each feature; this story is the final check. Detailed handling of partial Google failures is out of scope.
