# JUNE AI Corporate Website

This package upgrades the original HUGs website into the JUNE AI corporate website, with HUGs presented as a consumer brand under JUNE AI.

## Structure
- `index.html` — bilingual JUNE AI corporate site
- `styles.css` — responsive corporate visual system
- `script.js` — CN/EN language switch, reveal animations, Netlify form submission
- `assets/` — retained HUGs imagery and product film from the original site

## Bilingual behavior
The site automatically opens in Chinese for Chinese-language browsers and English otherwise. Users can switch language from the top-right language button. The preference is stored in `localStorage`.

## Netlify Forms
The contact form name is `juneai-contact`. On Netlify, enable form detection. The form submits to `/` with URL-encoded POST. When previewed locally via `file://`, form entries are saved to browser `localStorage` under `juneai_contact` for UI testing.

## Recommended deployment
Deploy this folder as a static site to Netlify. If replacing an existing HUGs deployment, keep the existing `assets/` files in the same relative paths.
