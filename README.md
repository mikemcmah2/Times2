# Times2

A times-table practice app — pick your numbers, fill in the grid, beat your best time.

## Put this on GitHub Pages

1. Create a new repository on GitHub (e.g. `times2`).
2. Upload **all files, keeping the folder structure** (`index.html`, `manifest.json`, and the whole `icons/` folder) to the root of the repository.
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, pick the `main` branch and `/ (root)` folder, then **Save**.
5. GitHub will give you a URL like `https://yourusername.github.io/times2/` — that's your live app. It can take a minute or two to go live the first time.

No build step, no dependencies, no server — just static files.

## App icon

The `icons/` folder has your Grid Spark (Plum & Citrine) icon pre-sized for iOS and Android:

- `apple-touch-icon.png` (180×180) — used automatically when you Add to Home Screen on iPhone
- `apple-touch-icon-152.png` / `-167.png` — iPad sizes
- `icon-192.png` / `icon-512.png` — Android / PWA install icon
- `favicon-16.png` / `favicon-32.png` — browser tab icon
- `icon-1024.png` — a high-res master, handy if you ever need to submit to an app store or generate more sizes

`index.html` already links to all of these, and `manifest.json` registers the Android icons — nothing extra to configure.

## Add it to your home screen

**iPhone/iPad (Safari):** open your GitHub Pages link → Share icon → **Add to Home Screen**. It'll use the Times2 icon and open full-screen like a real app.

**Android (Chrome):** open the link → menu (⋮) → **Add to Home screen**.

## Notes

- Player names, session history, and best times are saved in the browser's local storage, per device/browser. Clearing browser data will clear that history.
