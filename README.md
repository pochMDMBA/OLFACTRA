# OLFACULATOR · Note Relationships Layout Repair v17

## Changes

- Shifted the large tier letter slightly inward from the right edge in My Combinations while keeping the score on the left.
- Reverted the v16 Note Relationships steel-panel redesign that overrode the rail's positioning and altered its header geometry.
- Applied translucency to the complete Note Relationships window, including the heading and content, while preserving the established rounded layout and theme-derived appearance.
- Updated responsive placement so Note Relationships sits after the main fragrance workspace at tablet and mobile widths. Expanding or collapsing it therefore does not push Fragrance A/B down the page. Desktop retains the fixed left-side panel.
- Preserved account storage, Supabase configuration, fragrance gradients, tier effects, collection, authentication, icons, manifest and SQL files.

## Deploy

1. Replace the repository root `index.html` and `service-worker.js` with these versions.
2. Keep the `icons/` directory, `manifest.webmanifest`, `supabase-schema.sql`, and `supabase-permissions-fix.sql`.
3. Commit and push to GitHub / Vercel.
4. Hard-refresh the site. For an installed PWA, fully close and reopen after the service worker activates.

No Supabase SQL migration is required.
