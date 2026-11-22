# OLFACULATOR v21 — Note Relationships & Combination Title Fix

## Updates
- Removed the Note Relationships title/banner so the first visible control is “Minimum matches to show”. The panel keeps its existing bounded, translucent glass surface and layout.
- Fixed duplicate relationship hover details. Hidden in-place source tooltip nodes remain in the note markup for cloning, while only the single pointer-following tooltip clone rendered in `document.body` is visible.
- Centered saved combination names across the full card width, with balanced clearance for the delete control.
- Preserved collection rename, quoted/italic combination names, tier treatments, saved fragrance color swatches, Supabase configuration, mobile navigation, manifest and icon assets.
- Advanced the service-worker cache name to v21.

## Deployment
Replace the repository root `index.html` and `service-worker.js` with the versions in this archive. Keep the `icons/` directory, `manifest.webmanifest`, and both Supabase SQL files. No database migration is required.
