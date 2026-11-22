# OLFACULATOR v24 · Left Scroll & Collection Card Refinement

## Changes
- Restored the desktop Note Relationships panel's own vertical scrollbar while preserving its fixed position, translucent surface and rounded shell. Tablet and mobile keep natural page scrolling.
- Made My Collection fragrance cards and My Combinations cards more compact with consistent spacing and quieter surfaces.
- Kept Fragrance A on the left and Fragrance B on the right in every saved-combination card, including narrow mobile screens.
- Removed all individual border/capsule styling around fragrance names. The single centre divider remains, and saved note-colour swatches are retained beneath each fragrance name.
- Retained combination title ornament, score, tier effects, rename/delete/load actions, Supabase integration and PWA assets.

## Deployment
Replace the repository root `index.html` and `service-worker.js` with these versions. Keep the `icons` folder, `manifest.webmanifest`, `supabase-schema.sql`, and `supabase-permissions-fix.sql`. No database migration is required. The service-worker cache is v24.
