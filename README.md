# OLFACULATOR v23 · Combination Layout Refinement

## Changes
- Saved combinations now show Fragrance A and Fragrance B side by side in equal left/right columns on desktop and mobile.
- Removed separate borders and capsule outlines from individual fragrance names.
- Kept one subtle vertical separator between the two fragrance columns.
- Preserved each fragrance's colour swatches and saved colour data.
- Extended the ornamental rule beneath the centered combination title across the full balanced title width.
- Preserved the existing tier effects, collection actions, account configuration, PWA assets and database files.
- Advanced the service-worker cache to v23.

## Deployment
Replace the repository root `index.html` and `service-worker.js` with the versions in this project. Keep the `icons` folder, `manifest.webmanifest`, and Supabase SQL files. No database migration is required.
