# OLFACULATOR — Metallic Polish Release

This release is based on the latest `REFERENCE_MASTHEAD_S_TIER` project. It preserves the existing Supabase account storage, mobile navigation, note database, Original theme, and PWA icons.

## Changes

- Strengthened the S-tier metallic animation with a clearly travelling specular highlight, animated gold rim, warm internal lustre and retained soft winner glow. All layers stay clipped to the rounded score card. Reduced-motion preferences are respected.
- Corrected the desktop Compatibility Score rail so it wraps its content at natural height and no longer stretches down to the fixed Theme selector. Mobile/tablet flow remains unchanged.
- Capitalized the saved-combination action as `Load Pair`.
- Replaced the My Shelf glyph with a clearer inline vector bookshelf showing three upright books on a shelf.
- Applied a restrained finishing pass to window surfaces, controls, buttons and typography for more consistent spacing and styling.
- Advanced the service-worker cache to `olfaculator-shell-v12`.

## Deploy

1. Extract this ZIP.
2. Replace the repository root `index.html` and `service-worker.js` with the included versions.
3. Keep `manifest.webmanifest`, the full `icons/` folder and both Supabase SQL files.
4. Commit and push to trigger your Vercel deployment.
5. If the installed mobile app still shows an older version, close and reopen it or reinstall the home-screen shortcut.

No Supabase schema migration or database reset is required.
