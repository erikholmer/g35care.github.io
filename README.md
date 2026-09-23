# G35 Care — standalone / GitHub Pages export

`index.html` is the complete application. Its styles, JavaScript, fonts, and icon are embedded. No build step, package install, server, API key, or ChatGPT sign-in is required. It works at a domain root or a GitHub Pages project path such as `/g35-care/`.

## Included files

- `index.html` — ready-to-host maintenance tracker.
- `.nojekyll` — tells GitHub Pages to serve the files without Jekyll processing.
- `THIRD_PARTY_LICENSES.txt` — licenses for the embedded DM Sans and Manrope fonts.
- `README.md` — this guide.

## Privacy before publishing

Nothing has been uploaded to GitHub or published as part of this export. The exported HTML does not inherit the original Sites access controls and does not contain a password gate. Maintenance records are not embedded in these files.

A private GitHub repository does **not** automatically make its Pages website private. GitHub documents private Pages access control for eligible organization project sites on GitHub Enterprise Cloud. If the webpage must remain private, keep using the original private Site or arrange appropriate private hosting before enabling Pages. The HTML's `noindex` tag is only an indexing request, not access control.

## GitHub Pages setup — when you choose to publish

1. Extract the ZIP. Keep `index.html` at the top of your chosen publishing folder; include `.nojekyll` and the font licenses.
2. Add those files to your chosen repository. Do not add exported maintenance backups to the repository.
3. Once you have decided the site's visibility, open **Settings → Pages**. For branch publishing, select **Deploy from a branch**, then your branch and **/(root)** (or `/docs` if you placed the files there).
4. Use the Pages URL GitHub provides. Both `.../g35-care/` and `.../g35-care/index.html` use the same saved records.

No GitHub Actions configuration is included, so the package itself does not enable automatic deployment.

## Move your existing maintenance records

1. Open the original tracker in the browser where you recorded services.
2. Select **Export backup** and save its JSON file.
3. Open the new copy and select **Restore backup**. Choose that JSON file and confirm the restore.

Restoring replaces the records and custom intervals in the destination browser. Export its existing records first if needed. The format remains compatible with the original tracker. A different origin, browser, device, or project path uses a separate record store; records do not sync automatically.

## Everyday use and backups

Set your current odometer and body style, then record known completed services. Each record accepts a date, mileage, or both. Unknown history remains unverified. The tracker marks due, overdue, and upcoming work; you can tap a service name to change its interval. Update your odometer regularly.

Records save in browser localStorage. Clearing site data, switching browsers, or ending a private-browsing session may remove access to records. Export backups regularly and keep them privately. Anyone with access to the same browser profile may see its saved records. Keep other content hosted on the same origin trustworthy; separate project paths are not security boundaries.

You can double-click `index.html` to preview it locally in a modern browser. File-URL storage behavior varies by browser; use HTTPS hosting for regular use and export a backup before moving the file. With all assets embedded, the downloaded file needs no network connection for the tracker itself. The owner's-manual and recall links open external websites only when selected.

## Maintenance source

The starter intervals follow the 2003 Infiniti G35 owner's manual, maintenance section 9-3–9-9. Schedule 1 is the default; Schedule 2 and custom intervals are available. Tire rotation depends on body style. Coolant and belt reminders use recurring intervals appropriate after the initial interval. The tracker does not diagnose vehicle faults.

https://cdn.dealereprocess.org/cdn/servicemanuals/infiniti/2003-g35.pdf

## GitHub documentation

- Publishing source: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- Static files and repository/site visibility: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- Private Pages eligibility: https://docs.github.com/en/enterprise-cloud@latest/pages/getting-started-with-github-pages/changing-the-visibility-of-your-github-pages-site
