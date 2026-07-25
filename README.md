# Times2

A times-table practice app with two modes: **Grid Mode** (fill the full 1-12 grid, beat your best time) and **Practice Mode** (drill specific tables against a 1-minute clock).

## Put this on GitHub Pages

1. Create a new repository on GitHub (e.g. `times2`).
2. Upload all files in this zip (flat, no folders) to the root of the repository.
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, pick the `main` branch and `/ (root)` folder, then **Save**.
5. GitHub will give you a URL like `https://yourusername.github.io/times2/`.

## How it works

- **Name entry**: type a new name (required), or pick a returning player from the dropdown.
- **Mode select**: choose Grid Mode or Practice Mode each time you play.
- **Grid Mode**: full 1-12 × 1-12 grid (144 squares), shuffled each round. A wrong attempt flashes red immediately, then lets you try again (3 attempts total); after 3 misses the answer is revealed in red. Best time + accuracy tracked per player on a leaderboard.
- **Practice Mode**: pick any combination of tables. One fact at a time, 1-minute timer. Correct answers advance instantly; wrong answers flash red for 2 seconds before moving on. A Restart link resets the round anytime. Leaving the page mid-round stops the timer. Best "correct in 1 minute" tracked per player per number combination.
- **Results screen**: buttons are briefly disabled for 3 seconds after finishing. Includes a New Player button.
- **History**: Grid Mode and Practice Mode quick-jump buttons at the top, a Grid Mode leaderboard, and a player dropdown to see individual stats.

## App icon

Icon files are already linked from `index.html` and `manifest.json` — keep them in the same folder as `index.html`.

**iPhone/iPad (Safari):** Share icon → **Add to Home Screen**. **Android (Chrome):** menu (⋮) → **Add to Home screen**.

## Notes

Player names, sessions, and best stats are saved in the browser's local storage, per device/browser.
