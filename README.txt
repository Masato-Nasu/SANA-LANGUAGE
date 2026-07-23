SANA Language v1.4.0-alpha.4 — PWA package

Files at the deployment root:
  index.html
  manifest.webmanifest
  sw.js
  icons/

Cloudflare Pages deployment (existing project):
  npx wrangler pages deploy . --project-name=sana-language

PWA notes:
- HTTPS (or localhost) is required for Service Worker / installability.
- The app shell is cached for offline use after the first successful online load.
- A new sw.js version triggers the in-app update UI.
- Deploy the CONTENTS of this folder as the project root; do not add an extra parent folder level.
