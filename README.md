# doto

Two small task apps set like the pages of a book.

- **Tasks** (`/tasks`): today's list. Tick everything off, then fold the corner of the page to finish the day. Unfinished tasks can wait in Later.
- **Projects** (`/projects`): long-running projects with sections. Each task fills in a quarter at a time. Fold a finished project away to the Finished shelf.

Press and hold a task, project or section to rename it. Enter saves, Escape cancels.

Plain HTML, CSS and JavaScript. No build step, no dependencies besides the Literata font from Google Fonts.

## Your data

Everything is stored in your browser (`localStorage`), on each device separately. Nothing is sent anywhere.

Use **Save a backup** on the main menu now and then. It downloads one JSON file with both apps. **Restore a backup** loads it back, on the same device or a new one.

On iPhone, add doto to your Home Screen (Share → Add to Home Screen). Safari can clear storage for websites you haven't visited in a while; an app on the Home Screen keeps its data.

## Run it

Locally, serve the folder with any static server:

```
npx serve .
```

On GitHub Pages: push this repo, then Settings → Pages → Deploy from a branch → `main` / root. It will be at `https://<your-username>.github.io/doto/`.

## Updating

After changing files, bump `CACHE` in `sw.js` (`doto-v1` → `doto-v2`) so installed copies pick up the new version.
