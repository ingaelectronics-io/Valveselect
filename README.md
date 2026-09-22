# Inga Electronics — Engineering Tools

A hub of free, browser-based engineering tools from Inga Electronics. Each tool is a
single self-contained HTML file — nothing to install, nothing to build, no server required.

**Live site (once Pages is enabled):** `https://<your-username>.github.io/<repo-name>/`

## What's in this repo

```
/
├── index.html            ← landing page listing all tools
├── valveselect/
│   └── index.html        ← ValveSelect v1.9.26 (preliminary valve selection tool)
└── README.md
```

Each tool lives in its own folder as `index.html`, so it gets a clean URL:
`https://<your-username>.github.io/<repo-name>/valveselect/`

To add a new tool later, create a new folder (e.g. `/pressureconvert/index.html`) and
add a card for it on the root `index.html`.

## How to publish this with GitHub Pages (5 minutes, no coding needed)

1. **Create the repository.**
   On GitHub, click **New repository**. Suggested name: `inga-electronics-tools`
   (or `<your-username>.github.io` if you want it at the root of your GitHub domain
   with no `/repo-name/` in the URL). Set it to **Public**. Don't add a README —
   this package already has one.

2. **Upload these files.**
   On the new repo's page, click **Add file → Upload files**, then drag in
   everything from this package (`index.html`, `README.md`, and the whole
   `valveselect/` folder, keeping the folder structure). Commit the changes.

3. **Turn on GitHub Pages.**
   Go to **Settings → Pages** (left sidebar). Under **Build and deployment**,
   set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
   Save.

4. **Wait ~1 minute**, then refresh the Pages settings page — GitHub will show
   your live URL at the top, e.g.:
   `https://your-username.github.io/inga-electronics-tools/`

   ValveSelect itself will be at:
   `https://your-username.github.io/inga-electronics-tools/valveselect/`

5. **(Optional) Custom domain.** If Inga Electronics has its own domain, you can
   point a subdomain (e.g. `tools.ingaelectronics.com`) at this repo from the
   same Settings → Pages screen — GitHub gives you the DNS record to add.

## Updating a tool

When a new version of a tool is ready, just re-upload its `index.html` to the
matching folder (overwriting the old one) and commit. GitHub Pages redeploys
automatically within a minute or two — no other steps needed.

## Notes

- These are preliminary engineering aids only. Every tool includes its own
  disclaimer; results should be verified against manufacturer data and
  applicable standards before procurement or installation.
- No user data is sent to any server — each tool runs entirely client-side in
  the visitor's browser. Any "saved projects" style features use the browser's
  local storage on that visitor's own device only.
