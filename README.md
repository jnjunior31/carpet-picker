# CRC Carpet Walkthrough

A small static site for comparing Bentley Mills carpet options (Lucky Break, Victory Lap, Windfall)
across the actual rooms in the Hillcrest Community Resource Center.

## Publish it on GitHub Pages

1. Create a new repo (public or private — Pages works either way on paid plans, public repos get it free) and push these files as-is:
   ```
   git init
   git add .
   git commit -m "CRC carpet walkthrough"
   git branch -M main
   git remote add origin <your-repo-url>
   git push -u origin main
   ```
2. In the repo's **Settings → Pages**, set "Deploy from a branch", branch `main`, folder `/ (root)`, then Save.
3. GitHub will publish it at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

No build step — it's a single `index.html` plus an `images/` folder.

## Adding or fixing a room/color photo later

Images live at `images/<style-slug>/<color-slug>/<room-slug>.jpg`, e.g. `images/windfall/aced-it/hk-class.jpg`.
Slugs in use:

- Styles: `lucky-break`, `victory-lap`, `windfall`
- Colorways: `favored-to-win`, `game-set-match`, `aced-it`
- Rooms: `bxa-admin`, `bxa-work`, `gathering`, `gathering-north`, `hk-class`, `corridor`

Drop a same-named `.jpg` into the right folder and it shows up automatically — no code changes needed.
