# GOD SMACK!

**An original anime universe** — interactive pitch site and slide deck for investors and partners.

A [Thiink Media Graphics](https://thiinkmediagraphics.com) property · Draft 1.0 · May 2026

## View Site

[View Pitch](https://jrlordmoose.github.io/god-smack-show-idea/)

---

## Live site

After you enable GitHub Pages, the site will be available at:

| Format | URL |
|--------|-----|
| **Scrollable pitch site** (primary) | https://jrlordmoose.github.io/god-smack-show-idea/ |
| **Slide deck** (16:9 presentation) | https://jrlordmoose.github.io/god-smack-show-idea/deck.html |

Repository: [github.com/JrLordMoose/god-smack-show-idea](https://github.com/JrLordMoose/god-smack-show-idea)

---

## Logline

Every 100,000 years, the gods are summoned to compete for the throne of creation. This time — a boy with no clan, no class, and no name shows up.

**Format:** 12 episodes · Season One · 30 min · animated · streaming-first, with a built-in multi-season tournament structure.

**Tone:** Mythic tournament shōnen for an audience that has aged into prestige horror, ritual violence, and meta-religious worldbuilding — inspired by the art of *Berserk*, *Devilman Crybaby*, *Fullmetal Alchemist*, and *Devil May Cry*.

---

## What’s in this repo

Static HTML/CSS/JS — no build step, no npm. Open locally or deploy as-is to GitHub Pages.

| File / folder | Purpose |
|---------------|---------|
| [`index.html`](index.html) | **Main pitch site** — scrollable long-form deck (15 sections) |
| [`deck.html`](deck.html) | Short URL redirect to the slide deck |
| [`God SMACK Pitch Deck.html`](God%20SMACK%20Pitch%20Deck.html) | **Slide deck** — keyboard-navigable presentation |
| [`page.css`](page.css) | Styles for the scrollable site |
| [`deck.css`](deck.css) | Styles for the slide deck |
| [`deck-stage.js`](deck-stage.js) | Slide navigation and stage logic |
| [`image-slot.js`](image-slot.js) | Image placeholder components (slide deck) |
| [`assets/img/`](assets/img/) | Key art and tone-reel imagery |
| [`Image Prompts for Gemini.md`](Image%20Prompts%20for%20Gemini.md) | Internal prompts used to generate concept art |
| [`uploads/GodSMACK_Pitch_Deck.pdf`](uploads/GodSMACK_Pitch_Deck.pdf) | Optional PDF export for offline sharing |

### Site sections (`index.html`)

1. Hero · 2. Premise · 3. World (Centuria) · 4. Tone reel · 5. Society · 6. Competition · 7. Core mechanic (bead walk) · 8. Factions · 9. Power system · 10. Cast · 11. Pilot · 12. Series arc · 13. Market · 14. Franchise · 15. Credits

Character modals on the cast section: Kairu, Vorath, Sevryn, Omi.

---

## Run locally

Any static file server works. Examples:

```bash
# Python
python -m http.server 8080

# Node (npx, no install)
npx --yes serve .
```

Then open [http://localhost:8080](http://localhost:8080) for the site and [http://localhost:8080/deck.html](http://localhost:8080/deck.html) for slides.

Or open `index.html` directly in a browser (relative asset paths are written for that).

---

## Deploy to GitHub Pages

### 1. Create the repository

```bash
git init
git add .
git commit -m "Initial commit: GOD SMACK! pitch site"
git branch -M main
git remote add origin https://github.com/<username>/<repo>.git
git push -u origin main
```

Suggested repo name: `god-smack` or `god-smack-pitch`.

### 2. Enable Pages

1. On GitHub: **Settings → Pages**
2. **Build and deployment → Source:** Deploy from a branch
3. Branch: `main` · Folder: `/ (root)`
4. Save — GitHub publishes the repo root (`index.html`) as the site

`.nojekyll` is included so Jekyll does not process the site.

### 3. Private vs public

- **Public repo:** Pages URL is world-readable — suitable only if you are comfortable sharing the pitch publicly.
- **Private repo:** GitHub Pages on private repos requires a paid GitHub plan; otherwise keep the repo private and share via local server or PDF.

---

## Repository hygiene

Excluded via [`.gitignore`](.gitignore) (not required for the live site):

- `debug/` … `debug5/` — screenshot QA folders  
- `uploads/pasted-*.png` — duplicate working copies of `assets/img/`  
- `assets/img/04-tone-reel-contactsheet.png` — large dev contact sheet (not used in HTML)

**Repo size:** Key art PNGs are ~1–2 MB each (~25 MB total). Under GitHub’s file limits, but consider compressing or WebP if the repo grows.

---

## Credits & rights

© 2026 **Thiink Media Graphics, LLC.** All rights reserved.

Created by **Mustapha C. A. Jr** · [hello@thiinkmediagraphics.com](mailto:Team@thiinkmediagraphics.com)

Visual references in the pitch are placeholders for licensed or original art. Fill the credit table in section 15 before external distribution. See the site footer for confidentiality notice.

---

## Contact

**Thiink Media Graphics** · [thiinkmediagraphics.com](https://thiinkmediagraphics.com) · [Team@thiinkmediagraphics.com](mailto:Team@thiinkmediagraphics.com)
