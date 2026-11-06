# TotK Recomp Guide (Unofficial)

An unofficial, plain-English setup and troubleshooting guide to **[TotK Recomp (`valentderah/totk-pc-recomp`)](https://github.com/valentderah/totk-pc-recomp)**, the open-source static recompilation project that builds a user-supplied copy of *The Legend of Zelda: Tears of the Kingdom* into a native Windows or Linux PC executable.

The full updated guide lives at **[totkrecomp.wiki](https://totkrecomp.wiki/)**. This repository summarizes key version notes and links to each topic page.

> Not affiliated with valentderah or Nintendo. No game files, ROMs, `prod.keys`, firmware, or compiled game binaries are hosted here or on the site, and neither explains where to download copyrighted files. Only use dumps from your own Switch cartridge or eShop purchase.

## Quick Facts (v0.3.11 — November 5, 2026)

- **Latest release:** [`v0.3.11`](https://github.com/valentderah/totk-pc-recomp/releases/tag/v0.3.11) (commit `0ae47a5`, published 2026-11-05). Non-16:9 screens (21:9, 32:9, 16:10, 3:2) now get a matching `output_res` by default; fixes for the Hebra blizzard crash with mods (#776), fullscreen=1 not starting fullscreen, the widescreen Recall reticle (#685) and Linux crashes on older x86-64-v2 CPUs; pre-rendered movies keep 16:9 (`movie_aspect`); more mouse and keyboard work (direct mouse camera on 1.2.1, mouse map cursor and wheel zoom on 1.4.3, unified camera speed); optional `frame_queue`; the installer remembers your paths and is sharp on high-DPI screens. Full breakdown on the [changelog page](https://totkrecomp.wiki/changelog/).
- **Supported game updates:** 1.1.0, 1.1.2, 1.2.0, 1.2.1, and 1.4.3 (XCI/NSP/NSZ/XCZ via your own keys). Setup walkthrough in [how to install TotK Recomp](https://totkrecomp.wiki/install/).
- **Steam Deck & Linux:** Native x86_64 AppImage with Steam Deck presets and `v0.3.7+` AMD Depths geometry fixes; v0.3.11 fixes a startup crash on older CPUs. Details in the [Steam Deck & Linux guide](https://totkrecomp.wiki/steam-deck-linux/).
- **Mods & Graphics:** Supports RomFS, TKMM, IPS/pchtxt mods, HDR10, up to 240 fps, and NVIDIA DLSS/DLAA. See [mods & cheats](https://totkrecomp.wiki/mods/) and [totk.ini settings](https://totkrecomp.wiki/settings/).

## v0.3.11 Release Files

Exact sizes and SHA-256 digests as reported by the GitHub Releases API for tag `v0.3.11`. Download only from the [official releases page](https://github.com/valentderah/totk-pc-recomp/releases).

| File | Platform | Bytes | Size | SHA-256 |
| --- | --- | ---: | ---: | --- |
| `TotK-Setup-0.3.11-windows.zip` | Windows x64 | 164,515,808 | 157 MiB | `e77c12f29c3f39c54c0f8c357b87fc89e8ff4c9bb87dababe6fa9c4e686f7427` |
| `TotK-Setup-x86_64-0.3.11-linux.AppImage` | Linux x86_64 / Steam Deck | 229,722,616 | 219 MiB | `5999699362ee7651840a2259a06f1e40eb5e266e33f0c75ff70db35452d18456` |

The same digests in `sha256sum` format are in [`SHA256SUMS-v0.3.11.txt`](SHA256SUMS-v0.3.11.txt). Check a download with `CertUtil -hashfile TotK-Setup-0.3.11-windows.zip SHA256` on Windows or `sha256sum --ignore-missing -c SHA256SUMS-v0.3.11.txt` on Linux. More on telling official files apart on the [GitHub guide page](https://totkrecomp.wiki/github/).

## Guide Pages

| Topic | Page |
| --- | --- |
| Overview & current status | [totkrecomp.wiki](https://totkrecomp.wiki/) |
| Official GitHub repo & release filenames | [/github/](https://totkrecomp.wiki/github/) |
| Step-by-step Windows & Linux setup | [/install/](https://totkrecomp.wiki/install/) |
| Steam Deck & Linux native AppImage guide | [/steam-deck-linux/](https://totkrecomp.wiki/steam-deck-linux/) |
| PC & GPU hardware requirements | [/requirements/](https://totkrecomp.wiki/requirements/) |
| `totk.ini` graphics, FOV, HDR & DLSS settings | [/settings/](https://totkrecomp.wiki/settings/) |
| Controller, mouse camera & keybinds | [/controls/](https://totkrecomp.wiki/controls/) |
| Mods & Atmosphère cheats (`docs/mods.md`) | [/mods/](https://totkrecomp.wiki/mods/) |
| Crash, audio & GPU troubleshooting | [/troubleshooting/](https://totkrecomp.wiki/troubleshooting/) |
| TotK Recomp vs UltraTears vs SkyboundTotk | [/compare/](https://totkrecomp.wiki/compare/) |
| Version history (`0.1.1` → `0.3.11`) | [/changelog/](https://totkrecomp.wiki/changelog/) |
| Legal FAQ | [/is-it-legal/](https://totkrecomp.wiki/is-it-legal/) |

## Official Upstream Project

- Official repository: https://github.com/valentderah/totk-pc-recomp

Spotted an outdated note after a new upstream release? Open an issue here.
