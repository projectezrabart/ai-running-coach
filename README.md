# AI Running Coach

A collection of self-contained, browser-based interval-running workouts. Each workout is a single HTML file with a built-in timer, audio cues, and on-screen prompts — no app, no account, no internet connection required once the page has loaded. A dashboard (`index.html`) lets you browse, search, and filter all of them.

Built to run as a static site on **GitHub Pages**, so it can be opened from any browser — including an iPhone.

## What's inside

```
ai-running-coach/
├── index.html        # Dashboard / hub — search and filter all workouts
├── workouts/         # 45 self-contained workout timer pages
├── README.md
└── .gitignore
```

The dashboard reads a built-in list of workouts and links to each file in `workouts/`. Every workout page is standalone, so you can also open any file in `workouts/` directly.

## Use it

Once published (see below), open the site's URL in any browser. From the dashboard:

- **Search** by name, or **filter** by duration / intensity / long runs.
- Tap a workout to open its timer page.
- Press start and follow the on-screen and audio cues.

### On iPhone

1. Open the published URL in Safari (e.g. `https://<your-username>.github.io/ai-running-coach/`).
2. Tap the **Share** button, then **Add to Home Screen** — this gives you an app-style icon that opens the dashboard full-screen.
3. Open a workout, then leave the screen on (or adjust Auto-Lock in Settings) so the timer keeps running during your session. Make sure your phone isn't on silent if you want the audio cues.

## Publish on GitHub Pages

This repo is set up to serve directly from the repository root — `index.html` is the landing page.

1. Create a GitHub repo named `ai-running-coach` and push this folder to the `main` branch.
2. In the repo on GitHub: **Settings → Pages → Build and deployment**.
3. Set **Source** to *Deploy from a branch*, **Branch** to `main`, folder `/ (root)`, then **Save**.
4. After a minute, the site is live at `https://<your-username>.github.io/ai-running-coach/`.

> **Note:** GitHub Pages on the free plan only works for **public** repositories. To keep the repo private and still use Pages, you need GitHub Pro (or another paid plan).

## Growing this into a toolkit

This is the first of a planned set of personal web tools. Two clean ways to grow it:

- **More tools, more repos** — give each tool its own repo (each gets its own Pages URL), and optionally create a `<your-username>.github.io` repo as a master hub that links to all of them. Recommended; keeps each tool simple.
- **One repo, many tools** — keep this repo's `index.html` as the hub and add each new tool in its own subfolder (e.g. `workouts/`, `another-tool/`), linking to them from the hub.

## Notes

- Everything is plain HTML/CSS/JavaScript — no build step, no dependencies.
- Workout pages are fully self-contained and work offline once loaded.
