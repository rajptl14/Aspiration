# College Vision Board

A drag-and-drop corkboard for goals, photos, quotes, and checklists — built as a single HTML file, no build step required.

## Run it locally
Just open `index.html` in a browser. That's it.

## Host it on GitHub Pages (free)

1. Create a new repository on GitHub (e.g. `vision-board`).
2. Add `index.html` to the root of the repo (drag-and-drop it in the GitHub web UI, or `git add`/`commit`/`push` from your machine).
3. Go to **Settings → Pages** in your repo.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. Wait about a minute, then refresh the Pages settings page — you'll see a link like:
   `https://yourusername.github.io/vision-board/`

That's your live board. Bookmark it.

## How saving works

The board autosaves to your browser's `localStorage` every time you edit something — no accounts, no backend, nothing to configure. It'll be there next time you visit the same URL **in the same browser on the same device**.

Notes on that:
- It does **not** sync across devices or browsers on its own. Use the **Export** button to download a `vision-board.json` backup, and **Import** to load it somewhere else (a different browser, a friend's laptop, after clearing your browser data, etc.).
- Private/incognito windows may not persist `localStorage` between sessions — export before you close the window if you're using one.
- If you ever want cross-device sync without manual export/import, that would need a small backend or a service like Firebase — happy to help set that up if you want to go there later.

## Customizing

Everything is in `index.html` — the CSS is in the `<style>` block up top, the card/board logic is vanilla JS at the bottom. No dependencies except two Google Fonts (Caveat + Work Sans), loaded via CDN.
