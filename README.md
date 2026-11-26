# Nexus Downloader Ultimate (NDU)

A userscript that turns Nexus Mods into a **download cart**: queue the exact mod files you want into your own collections, then download them in one controlled batch, in your browser or through Vortex.

**[Install from Greasy Fork](https://greasyfork.org/en/scripts/595739-nexus-downloader-ultimate)**

![Nexus Downloader Ultimate](screenshots/latestNDU.png)

---

## Features

### Mod Vault
- Create, rename, merge and manage your own collections of individual mod files
- Search, select and remove stored files
- Import and export collections as JSON
- Collections are saved locally and persist across sessions

### Add to Collection
- Add specific files straight from Nexus mod pages
- Pick the exact file versions you want and mix files from different mods in one collection

### Official Nexus Collections
- Load published collection revisions and review required and optional files
- Select single files or whole selections, with dependency and install info
- Save selections into your own collection
- External resources and bundled assets are flagged, not downloaded automatically

![File selector](screenshots/modSelector.png)

### Download review and ordering
- See filenames, sizes and categories; search and organize by mod or by file
- Select all, clear, or reselect previously failed files
- Choose the download order: original collection order, largest or smallest first, A–Z or Z–A
- How you sort the view is separate from the order files download in

### Download protection and recovery
- Adaptive concurrent downloads with duplicate-dispatch protection
- Progress and speed tracking where the userscript manager supports it
- Backoff for rate limits (HTTP 429), temporary server errors and server cooldown timers
- Cancellation-aware, and recovers from interrupted runs

### History and diagnostics
- Review completed, failed and interrupted runs down to individual files
- Export run reports and diagnostics as JSON

### Themes
Four visual themes: **Cyberpunk Grid**, **Steampunk Enginéworks**, **Arcane Runeforge** and **Wasteland Salvage**.

![Mods grid](screenshots/modsGrid.png)

---

## Download modes

| Mode | How it works |
|---|---|
| **Browser** | NDU resolves your authorized Nexus download links and hands files to your userscript manager's downloader. Adaptive concurrency and progress where supported. Files save to your browser's download folder. |
| **Vortex** | NDU sends NXM links to Vortex in a controlled order and Vortex does the downloading. NDU can't confirm when Vortex finishes a file. |

---

## Installation

1. Install a userscript manager:

   | Browser | Userscript manager |
   |---|---|
   | Chrome | Tampermonkey or Violentmonkey |
   | Firefox | Tampermonkey, Violentmonkey or Greasemonkey |
   | Edge | Tampermonkey |
   | Opera | Tampermonkey or Violentmonkey |
   | Safari | Tampermonkey or Userscripts |

2. Open the [Greasy Fork page](https://greasyfork.org/en/scripts/595739-nexus-downloader-ultimate) and click **Install this script**.
3. Visit any Nexus Mods page. NDU appears there.

**Tips**
- For Browser mode, set a dedicated default download folder in your browser first. NDU doesn't create folders or change where your browser saves files.
- For Vortex mode, Vortex must be installed and set to handle NXM links.

---

## Limitations

- Nexus may rate-limit frequent requests, so non-stop downloads and specific speeds aren't guaranteed.
- NDU doesn't bypass account permissions, Premium restrictions or server limits.
- Changes to the Nexus Mods site can break things. Please [open an issue](../../issues) if something stops working.
- Please follow the Nexus Mods Terms of Service.

---

## Bugs and feature requests

Found a bug or want a feature? **[Open an issue](../../issues)**. If you can, attach the diagnostics JSON export from NDU's History panel, because it makes problems much faster to fix.

## Support the project

If NDU saved you time, you can support its development. *(Sponsor link coming soon.)*

---

## Disclaimer and license

NDU is an unofficial project and is **not affiliated with, endorsed by, or supported by Nexus Mods**. It is provided "as is", without warranty of any kind.

© 2026 REDR41N. All rights reserved. See [LICENSE](LICENSE).
