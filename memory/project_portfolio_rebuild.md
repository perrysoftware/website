---
name: Portfolio site rebuild
description: Complete Hugo-to-static rebuild of perrysoftware.com as a minimal app portfolio
type: project
---

Rebuilt perrysoftware.com from Hugo + PaperMod to a plain HTML/CSS static site.

**Why:** User no longer does freelance; site should showcase solo apps as a dev portfolio, not a services business.

**How to apply:** Don't suggest Hugo, themes, or CMS tooling — the site is intentionally bare static HTML. Keep the aesthetic minimal: system fonts, off-white bg, white cards, muted text.

**Current state (Nov 2026):**
- Two apps featured: Sproutings (iOS + Android) and Sporadic (iOS only)
- Sproutings uses hero-devices.webp (single phone mockup, white bg)
- Sporadic only has an app icon (sporadic.png) — no real screenshots yet; displayed on lavender gradient background
- Profile photo placeholder — user has a new one coming
- Deploy via GitHub Actions → GitHub Pages (deploy.yml, no build step, serves root dir)

**Sporadic App Store URL:** `https://apps.apple.com/us/app/sporadic-fitness-challenges` — user provided without numeric ID, may need `/id{number}` appended if it breaks
**Sproutings App Store:** `https://apps.apple.com/us/app/sproutings-outings-with-kids/id6760201596`
**Sproutings Google Play:** `https://play.google.com/store/apps/details?id=com.perrysoftware.sproutings&pli=1`
