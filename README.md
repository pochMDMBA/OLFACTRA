# OLFACULATOR · Note Family Polish

This update refines the Browse Notes By Family disclosure and the Other / Modern Materials group.

## Changes

- Made the Browse Notes By Family panel and note-list body translucent, with a blurred glass-like surface. The summary/header banner remains solid and retains its existing theme styling for contrast.
- Expanded the full Other / Modern Materials list directly beneath its family heading. Its notes are no longer hidden inside a nested “Others” disclosure. Other fragrance families retain their existing “Others” grouping.
- Preserved the existing note selection limit, ranking, search/filter behaviour, live scoring, saved colour gradients, tier effects, Supabase authentication and persistence, themes, mobile navigation, and PWA assets.
- Advanced the service-worker cache to `olfaculator-shell-v15`.

## Deploy

1. Replace the repository root `index.html` and `service-worker.js` with these files.
2. Keep `manifest.webmanifest`, the complete `icons/` directory, `supabase-schema.sql`, and `supabase-permissions-fix.sql`.
3. Commit and push to GitHub / Vercel.
4. Hard-refresh the website. For an installed PWA, close and reopen the app after the new service worker activates.

No Supabase SQL migration is required.
