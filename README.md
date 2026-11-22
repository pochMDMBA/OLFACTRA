# OLFACULATOR v20 — Collection Rename, Note Tooltip & Panel Repair

## Updates
- Combination names are quoted and italicized after saving.
- Added a Rename action to each saved combination, using the existing themed action dialog and updating Supabase `saved_combinations` safely for the signed-in user.
- Saved fragrance-name labels in each combination use a translucent glass treatment.
- Fixed relationship hover details by cloning tooltip nodes before portaling them to `document.body`. The original tooltip remains in the note chip, so it continues to work after repeated hover in/out cycles.
- Added a collapsed “Other notes · no recorded relationship” group to selected-note breakdowns. Notes without a defined high/conditional/penalty pairing (including notes such as Chestnut and Tonka bean when applicable) remain discoverable and explain their no-record status on hover.
- Reworked the Note Relationships window sizing and header/body surfaces so the summary uses exactly the panel width and cannot protrude past its rounded right edge.
- Preserved the existing visual themes and applied high-contrast ivory lettering with a subtle dark edge to Load Pair, Save This Combination, Load A, Load B and related primary collection actions.
- Advanced the PWA cache name to v20.

## Deployment
Replace the repository's root `index.html` and `service-worker.js` with these files. Keep the `icons/` directory, `manifest.webmanifest`, and both Supabase SQL files. No database migration is required.
