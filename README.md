# CA Final MCQ Trainer

A single-file, offline-capable MCQ practice app for CA Final students — currently loaded with Financial Reporting (FR), with room for the other five subjects (AFM, Audit, DT, IDT, IBS) as their question banks are added.

## Deploy to GitHub Pages (2 minutes)

1. Create a new GitHub repository (public or private, either works with Pages on most plans).
2. Upload `index.html` and `.nojekyll` to the root of the repo (drag-and-drop on GitHub's web UI works fine, or `git add . && git commit -m "deploy" && git push`).
3. Go to **Settings → Pages**.
4. Under "Build and deployment", set **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)**. Save.
5. GitHub will give you a URL like `https://<your-username>.github.io/<repo-name>/` within a minute or two.

That's it — no build step, no dependencies to install, nothing else to configure.

## Notes

- **Progress is saved per device**, in the browser's local storage. Clearing browser data/site data will reset progress. There's no login and no server — everything runs client-side.
- To add more subjects or chapters later, the question data lives in one place inside `index.html` (the `GAME_DATA` object near the top of the script). Send me the next subject's MCQ/Question Bank PDF and I'll regenerate this file with it merged in.
- Works on mobile and desktop browsers. Add-to-homescreen works but this isn't a full PWA (no offline service worker) — let me know if you'd like that added.
