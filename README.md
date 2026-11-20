# OLFACULATOR · AMBOSS Default & S-tier Video Restore

This release continues from the latest Original Winner build and preserves the existing Supabase configuration, authentication flow, saved records, responsive navigation, icons, manifest and SQL schema.

## Updates
- Changed the default **Original** theme to an AMBOSS-inspired palette: black/dark-charcoal surfaces, cool gray text and restrained teal-blue accents.
- Kept the masthead independent of theme selection and removed the extra inset bordered rectangle. The brand identity and navigation remain inside one clean banner.
- Changed the Note Relationships disclosure chevron from gold to a neutral silver-gray.
- Restored the S-tier Compatibility Score appearance from the supplied reference video: rounded metallic-gold edging, a warm bronze/black reflective surface, a brighter soft golden outer bloom, subtle glints, a breathing glow, and a moving specular sweep.
- Removed all rectangular halo/frame elements from the S-tier treatment.
- Respects the user's reduced-motion system preference.

## Deploy
Replace the repository root `index.html`, `manifest.webmanifest`, and `service-worker.js` with the versions in this project. Keep the `icons/` folder and both Supabase SQL files. Commit and push to deploy. No database migration is required.
