# OLFACULATOR · Modal & Collection Polish

## Changes

- Made collection, combinations, save, About, authentication and themed confirmation popups translucent so the underlying workspace remains visible for orientation. The dialog surfaces use a smoked-glass treatment with blur and retain readable contrast.
- Reworked the My Combinations score strip: the numerical score (for example, `93/100`) is on the left and the large tier letter is on the right. Removed the redundant `S-TIER` label. Existing S/A/B/C/F tier materials, colours and animation classes are retained.
- Restyled Note Relationships as a cool graphite / steel smoked-glass panel with a distinct header banner, refined disclosure control and softer content surfaces.
- Preserved account/authentication, saved data, score logic, fragrance gradients, themes, mobile navigation and PWA assets.

## Deploy

1. Replace the repository root `index.html` and `service-worker.js` with these versions.
2. Keep the `icons/` directory, `manifest.webmanifest`, `supabase-schema.sql`, and `supabase-permissions-fix.sql`.
3. Commit and push to GitHub / Vercel.
4. Hard-refresh the site. For an installed PWA, close and reopen after the service worker activates.

No Supabase SQL migration is required.
