# SkillfulMeans Client Demo

A single-page, click-through demo used on prospect calls. It runs the 15-slide deck,
then walks through working versions of the platform screens — check-in and assessment,
HR portal, challenge day, and the referral partner portal — that you can scroll and click
live on the call.

**Keyboard:** `→ / ←` move · `N` presenter notes · `L` open the real platform in a second tab ·
`F` full screen · `S` links and setup.

## Deploying to Railway (no terminal needed)

1. Put this folder in a GitHub repository (drag-and-drop upload at github.com works fine).
2. Go to railway.app → **New Project** → **Deploy from GitHub repo** → pick the repo.
3. Railway detects Node automatically and runs `npm start`. No environment variables needed.
4. Under **Settings → Networking**, click **Generate Domain** to get the public URL.

Every push to `main` redeploys automatically.

## Running it locally

```
npm start
```

Then open http://localhost:3000

## What's in here

| Path | What it is |
|---|---|
| `public/index.html` | The whole demo — one self-contained file, images embedded |
| `server.js` | Tiny static file server, no dependencies |
| `package.json` | Tells Railway how to start it |
| `railway.json` | Build and start configuration |

## Updating the demo

`public/index.html` is one self-contained file. The presenter script lives in the
`STEPS` array near the top of the `<script>` block; the four working demo screens live in
the `SITES` object just above it.

## Notes for whoever presents

- Sample data only — Lakeside Manufacturing (HR) and Horizon Benefits Group / Alex Morgan
  (broker). No real client data is in this file.
- Press `S` once on a new computer to set the client's name and check the live links.
- Sign in to app.skillfulmeans.life and courses.skillfulmeans.life before the call so the
  "Open live" buttons land on the screen rather than a login page.
