# OLFACULATOR · Score Panel & Glass Scrollbar Repair v18

## Updates

- Fixed S/B saved-combination letter clipping by widening the tier glyph box and adding a safe inset.
- Kept Compatibility Score within the desktop viewport above the floating Theme control. The header, score, metrics and Save action stay visible; long score details scroll inside their own panel.
- Added slim, rounded, theme-aware scrollbars to Note Relationships, score details and dialog content.
- Made the full Note Relationships panel translucent, including the header, using a low-opacity glass surface and backdrop blur. Panel geometry and disclosure behavior are unchanged.
- Preserved fragrance atmosphere gradients, all tier effects, My Collection, Supabase configuration, authentication, PWA icons, manifest and SQL files.

## Deploy

1. Replace repository root `index.html` and `service-worker.js` with these versions.
2. Keep the `icons/` directory, `manifest.webmanifest`, `supabase-schema.sql`, and `supabase-permissions-fix.sql`.
3. Commit and push to GitHub / Vercel.
4. Hard-refresh the website. For an installed PWA, close and reopen after the v18 service worker activates.

No Supabase SQL migration is required.
