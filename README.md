# Family Feud — Player Onboarding (Static Site)

Single-file static web app to onboard up to 30 participants for a 30‑minute Family Feud session.

## Quick Start
1. Unzip the package.
2. Open `index.html` locally to test.
3. To share online, host the folder on any static host (GitHub Pages, Netlify, Vercel, S3, etc.).

## GitHub Pages (no build step)
- Create a new repo (e.g., `family-feud-lobby`).
- Add `index.html` at the root, commit, and push.
- In repo Settings → Pages → Set Source to **Deploy from a branch**, select `main` and root (`/`). Save.
- Your site will be served at: `https://<username>.github.io/family-feud-lobby/`

## Netlify (drag & drop)
- Go to app.netlify.com → **Add new site** → **Deploy manually**.
- Drag the unzipped folder onto the drop zone.

## Usage
- Share the page URL. It auto-generates a **room** code and appends `?room=ABCDE` to the URL.
- Send that URL or use the **QR** on the page.
- Roster, lock status, and timer persist in the host browser via `localStorage`.
- Export roster as CSV anytime.

## Notes
- This is a lobby/registration tool. To add *buzzers/answers/scorekeeping*, connect this page to a backend (e.g., Firebase/Supabase) and build the game UI.
- If you want a React/TypeScript version or multi-device sync, let me know and I'll provide a project scaffold.
