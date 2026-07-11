# Commission Ops

A single-file studio hub for running creative commissions — pipeline, clients, retainers, finances, contracts, invoices and client messages. **All data stays in your browser** (IndexedDB, optional AES-256 encryption); this site is just the tool, and the server never sees anything you enter.

v2.0.0 · no build step · no dependencies · one HTML file.

## Deploy on GitHub Pages

1. Create a new repository on GitHub (e.g. `commission-ops`). Public is fine — the file contains no personal data.
2. Upload `index.html` (and this README) to the repository root — *Add file → Upload files* works, no git needed.
3. In the repo: **Settings → Pages → Build and deployment** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
4. Wait ~1 minute. Your app is live at `https://<your-username>.github.io/commission-ops/`.

## First open

- The app starts as a blank canvas. Fill in **Settings** and **Documents → Provider details** (name, email, Discord, bank/PayPal, rate card), or click **Reset to sample** to explore with fictional demo data first (**Clear all data** removes it).
- Migrating from a local copy? **Settings → Data → Import backup** with your JSON — browser storage is per-site, so data doesn't follow the file automatically.
- **Work straight off a USB stick (Chrome/Edge):** Settings → Data → **Link a backup file…** and pick the backup JSON on your stick. The app then loads from it on open and writes every save back to it — the stick becomes the single source of truth across machines, and unplugging it means the next machine holds only what you choose to leave. Encrypted backups stay encrypted; if the stick's unplugged, saves fall back to the browser and re-sync on the next save after it returns.
- Optionally enable encryption in **Settings → Security**. There is **no passphrase recovery** — keep it in a password manager.

## Things worth knowing

- **Backups are your safety net.** Data lives only in the browser that entered it; export a backup (Settings → Data) after meaningful changes. The app reminds you after 4 days.
- **Each device is its own store.** Your phone and laptop don't sync; move data with backup files.
- **Updating the app:** replace `index.html` with a newer version and push — your data is untouched (it's in the browser, not the file). The version in the footer and in every backup (`appv`) tells you what you're running.
- Being on HTTPS, the live FX rate, clipboard copy and the backup file-picker all work — and you can install it from the browser menu (Add to Dock / Add to Home Screen) for an app-like window.

## Licence & disclaimer

Contract and invoice templates are starting points, not legal advice — have a qualified solicitor review them before relying on them. Tax figures are estimates, not tax advice.
