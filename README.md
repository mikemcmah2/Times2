# Times2

A times-table practice app with two modes: **Grid Mode** (fill the full 1-12 grid, beat your best time) and **Practice Mode** (drill specific tables against a 1-minute clock).

## Put this on GitHub Pages

1. Create a new repository on GitHub (e.g. `times2`).
2. Upload all files in this zip (they're all flat, no folders) to the root of the repository.
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, pick the `main` branch and `/ (root)` folder, then **Save**.
5. GitHub will give you a URL like `https://yourusername.github.io/times2/` — that's your live app.

No build step, no dependencies, no server — just static files.

## How it works

- **Name entry**: type a new name, or pick a returning player from the dropdown.
- **Mode select**: choose Grid Mode or Practice Mode each time you play.
- **Grid Mode**: always the full 1-12 × 1-12 grid (144 squares), row/column order shuffled each round. 3 attempts per square, then the answer is revealed. Best time + accuracy tracked per player on a leaderboard.
- **Practice Mode**: pick any combination of tables (2s-12s). One fact at a time, no grid, 1-minute timer. Correct answers advance instantly; wrong answers flash the right answer in red for a second before moving on. Best "correct in 1 minute" is tracked per player *per combination* of numbers chosen.
- **History**: a Grid Mode leaderboard, plus each player's best results broken out by mode and number combination.

## App icon

The icon files (`apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `favicon-16.png`, `favicon-32.png`, `icon-1024.png`) are already linked from `index.html` and `manifest.json` — nothing to configure, just keep them in the same folder as `index.html`.

**iPhone/iPad (Safari):** open your GitHub Pages link → Share icon → **Add to Home Screen**.
**Android (Chrome):** open the link → menu (⋮) → **Add to Home screen**.

## Notes

- All player names, sessions, and best stats are saved in the browser's local storage, per device/browser. Clearing browser data clears that history.
