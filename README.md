# OLFACULATOR v22 · Combination Symmetry

This release updates the saved-combination card layout.

## Changes
- Fragrance A appears on the left and Fragrance B on the right, including on mobile.
- Removed individual coloured borders around fragrance names.
- Added one restrained vertical divider between the two fragrance columns.
- Centered the combination name and added a small ornamental rule beneath it.
- Preserved existing note-colour swatches, saved combination data, tier effects, authentication and Supabase configuration.
- Advanced the service-worker cache to v22.

## Deployment
Replace the repository root `index.html` and `service-worker.js` with the versions in this project. Keep the `icons` folder, `manifest.webmanifest`, and Supabase SQL files. No database migration is required.
