# OLFACULATOR · Original Theme & S-tier Winner Polish

This release continues from `OLFACULATOR_FIXED_BANNER_FOOTER` and preserves the existing Supabase configuration, authentication flow, saved records, mobile navigation, icons, manifest, and SQL files.

## Updates
- Rebuilt the S-tier Compatibility Score treatment with a rounded metallic champagne-gold border, contained moving reflective shine, and soft animated glow. Removed the legacy rectangular halo effect.
- Added **Original** as the first theme and the new default. It uses a graphite/charcoal palette and restrained gold accents that match the fixed banner. Existing users are migrated to Original once; later theme choices remain saved.
- Enlarged the bordered inner panel inside the banner while retaining the fixed black/gray masthead background.
- Refined the consistency of workspace cards and dialog surfaces, with normal title casing and no small-caps treatment on dialog headings.
- Renamed the previous **My Library** label to **My Shelf** throughout visible UI copy and changed the navigation icon to a shelf/rack vector.
- Renamed **About Us** to **About**.
- Updated the PWA manifest chrome colors and advanced the service-worker cache to v9.

## Deploy
Replace the repository root `index.html`, `manifest.webmanifest`, and `service-worker.js` with the versions in this project. Keep the `icons/` folder and both Supabase SQL files. Commit and push to deploy. No database migration is required.
