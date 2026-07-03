# Compliance Catchers — GitHub Pages bundle

Everything in this folder is ready to host on **GitHub Pages** (free). Once live, your UK and
Australia teams open one URL, pick their region, and play — on any laptop or phone.

```
index.html      ← landing page (players pick Australia or UK)
au.html         ← Australian edition (AML/CTF Tranche 2)
uk.html         ← UK edition (Money Laundering Regs 2017)
images/         ← APLYiD logo + house-catcher graphic
.nojekyll       ← tells GitHub Pages to serve files as-is (leave it there)
README.md       ← this file
```

---

## Deploy in 5 steps (no coding)

1. **Create a repo.** Go to https://github.com/new. Give it a name (e.g. `compliance-catchers`),
   set it to **Public**, and click **Create repository**.
   *(Free GitHub Pages needs a public repo. The captured player details never go into the repo —
   they only go to your device or your Google Sheet — so public code is fine.)*

2. **Upload these files.** On the repo page click **Add file ▸ Upload files**. Drag in the
   **contents of this folder** — `index.html`, `au.html`, `uk.html`, the `images` folder,
   and `.nojekyll`. Click **Commit changes**.

3. **Turn on Pages.** Go to **Settings ▸ Pages**. Under "Build and deployment":
   - **Source:** Deploy from a branch
   - **Branch:** `main` and `/ (root)` → **Save**

4. **Wait ~1 minute**, then refresh the Settings ▸ Pages screen. It shows your live URL, like:
   `https://YOUR-NAME.github.io/compliance-catchers/`

5. **Share it.** That link opens the region picker. Direct links also work:
   - Australia: `https://YOUR-NAME.github.io/compliance-catchers/au.html`
   - UK: `https://YOUR-NAME.github.io/compliance-catchers/uk.html`

To update anything later, edit the file in GitHub (or re-upload) and commit — Pages redeploys
automatically in a minute or so.

---

## Before your event

- **Central scoreboard (optional).** To collect every score into one Google Sheet, follow
  `Google-Sheet-Setup-Guide.md` and paste your Web-App URL into the `SHEET_ENDPOINT = ""` line
  in **both** `au.html` and `uk.html` *before* uploading. Without it, the game still works and
  each device keeps its own scoreboard + admin export.
- **Change the admin passcode.** In `au.html` and `uk.html` find `const ADMIN_PASS = "aplyid";`
  and set your own.
- **Offline backup.** Venue wifi can be flaky. Also keep the single-file builds
  (`Compliance-Catchers.html` / `Compliance-Catchers-UK.html`) downloaded on each event device —
  they run with no internet at all.

## Running it at the kiosk

- Open the link, then go **fullscreen** (F11 on Windows, `Ctrl/Cmd+Shift+F` on Mac browsers;
  Guided Access on iPad).
- Turn off the device's auto-sleep/screensaver.
- On a tablet, use the browser's **"Add to Home Screen"** so it launches like an app.
- Host controls (top 3 winners + Excel/CSV export) are behind the faint **⚙ admin** button,
  bottom-right — passcode is whatever you set above.

---

*Educational game. Not legal advice. Powered by APLYiD.*
