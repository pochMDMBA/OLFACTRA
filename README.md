# OLFACULATOR · Tooltip, Collection & Note Panel Polish v19

## Updates

- Unified the translucent Note Relationships panel tint so ambient page gradients no longer create a brighter blue edge on one side. The panel remains glass-like and theme-aware.
- Portaled relationship breakdown tooltips to the document layer and positioned them adjacent to the pointer. This avoids fixed-position tooltips being displaced by the scrolling/backdrop-filter panel. Tooltips reposition within the viewport and dismiss on panel scroll or pointer exit.
- Improved My Combinations cards with larger combination names and two clearly separated fragrance rows. Each fragrance displays up to three stored note-colour swatches, with a backwards-compatible note-colour fallback for earlier records.
- Shifted the score and tier letter slightly right/inward together while preserving each tier's metallic/neutral/distressed display.
- Preserved Supabase account storage, saved profiles, PWA icons, manifest, existing scoring and mobile layout.

## Deploy

1. Replace repository root `index.html` and `service-worker.js` with these versions.
2. Keep the `icons/` directory, `manifest.webmanifest`, `supabase-schema.sql`, and `supabase-permissions-fix.sql`.
3. Commit and push to GitHub / Vercel.
4. Hard-refresh the site. For an installed PWA, close and reopen after the v19 service worker activates.

No Supabase SQL migration is required.
