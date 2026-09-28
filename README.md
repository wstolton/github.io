# Training Log

Two versions of the app, ready to host on GitHub Pages:

- `index.html` — the **blank** version, no preset exercises. This is the one to share with friends.
- `mine.html` — **your** version, with the 14 exercises, routines, and progression notes already built in.

Both are single self-contained files. No build step, no dependencies — just static HTML.

## Set up GitHub Pages

1. Create a new repository on GitHub (public or private both work for Pages).
2. Add `index.html` and `mine.html` to the repo root (drag-and-drop upload on github.com works fine, or `git add`/`commit`/`push` if you're using the command line).
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", pick the branch (usually `main`) and folder `/ (root)`, then save.
5. GitHub gives you a URL, usually `https://<your-username>.github.io/<repo-name>/` — it can take a minute or two to go live the first time.

## Resulting links

- `https://<your-username>.github.io/<repo-name>/` → the blank version (`index.html`)
- `https://<your-username>.github.io/<repo-name>/mine.html` → your version

Share the first link with friends; keep the second for yourself.

## Notes

- Each person's logged data is stored locally in their own browser (`localStorage`), scoped to this URL. Since it's a real hosted `https://` address rather than a file opened from disk, storage works reliably — no plan restrictions, no login, and no dependency on Claude at all once it's live.
- If you ever update the app again and want to redeploy, just replace the file(s) in the repo — GitHub Pages picks up the change automatically (again, may take a minute or two).
