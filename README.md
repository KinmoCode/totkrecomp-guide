# TotK Recomp Guide (Unofficial)

An unofficial, plain-English setup and troubleshooting guide to **[TotK Recomp (`valentderah/totk-pc-recomp`)](https://github.com/valentderah/totk-pc-recomp)**, the open-source static recompilation project that builds a user-supplied copy of *The Legend of Zelda: Tears of the Kingdom* into a native Windows or Linux PC executable.

The full updated guide lives at **[totkrecomp.wiki](https://totkrecomp.wiki/)**. This repository summarizes key version notes and links to each topic page.

> Not affiliated with valentderah or Nintendo. No game files, ROMs, `prod.keys`, firmware, or compiled game binaries are hosted here or on the site, and neither explains where to download copyrighted files. Only use dumps from your own Switch cartridge or eShop purchase.

## Quick Facts (v0.3.12 — November 6, 2026)

- **Latest release:** [`v0.3.12`](https://github.com/valentderah/totk-pc-recomp/releases/tag/v0.3.12) (commit `eda417f`, published 2026-11-06). HD texture packs load automatically via their `HeapDef` file (#673), including above content mods such as *The Second Quest* (#858; `tex_heap_extra_mb` under `[mods]` covers packs without one); ExeFS patches that edit game data in `main` now work (#835); permanent FPS drops after the Purah Pad scope on low-VRAM GPUs are fixed (#754); fewer crashes from GPU-written memory (#788, #802); resolutions missing a HUD layout draw a 16:9 picture with black bars instead of stretching the HUD (#809, #814); faster render-pass uniforms (#743), fight command copies, vertex-buffer binding (`perfdraw`) and GPU command recording; play time across runs in F1 > Game (#720); and AMD GPU owners can test `[performance] vk_recorder = 1` in `totk.ini` for higher FPS (set back to `0` on black screen or `VK_ERROR_DEVICE_LOST`). Full breakdown on the [changelog page](https://totkrecomp.wiki/changelog/).
- **Supported game updates:** 1.1.0, 1.2.1, and 1.4.3 (XCI/NSP/NSZ/XCZ via your own keys). Setup walkthrough in [how to install TotK Recomp](https://totkrecomp.wiki/install/).
- **Steam Deck & Linux:** Native x86_64 AppImage with Steam Deck presets, `v0.3.7+` AMD Depths geometry fixes, `v0.3.11` older x86-64-v2 CPU startup fix, and `v0.3.12` VRAM cleanup and HD texture pack support. Details in the [Steam Deck & Linux guide](https://totkrecomp.wiki/steam-deck-linux/).
- **Mods & Graphics:** Supports RomFS, HD texture packs (`v0.3.12`), TKMM, IPS/pchtxt code and data mods, HDR10, up to 240 fps, and NVIDIA DLSS/DLAA. See [mods & cheats](https://totkrecomp.wiki/mods/) and [totk.ini settings](https://totkrecomp.wiki/settings/).

## v0.3.12 Release Files

Exact sizes and SHA-256 digests as reported by the GitHub Releases API for tag `v0.3.12`. Download only from the [official releases page](https://github.com/valentderah/totk-pc-recomp/releases).

| File | Platform | Bytes | Size | SHA-256 |
| --- | --- | ---: | ---: | --- |
| `TotK-Setup-0.3.12-windows.zip` | Windows x64 | 164,322,471 | 157 MiB | `85ad24cd0c658bc6dfa39d5439e917a7a15eb99f0b17a9861febd62a608ef7be` |
| `TotK-Setup-x86_64-0.3.12-linux.AppImage` | Linux x86_64 / Steam Deck | 229,870,072 | 219 MiB | `7b75e66b407067b78b9fcae8ea90d995144ef1e170ea6be1bca02c60eebee9a6` |

The same digests in `sha256sum` format are in [`SHA256SUMS-v0.3.12.txt`](SHA256SUMS-v0.3.12.txt). Check a download with `CertUtil -hashfile TotK-Setup-0.3.12-windows.zip SHA256` on Windows or `sha256sum --ignore-missing -c SHA256SUMS-v0.3.12.txt` on Linux. More on telling official files apart on the [GitHub guide page](https://totkrecomp.wiki/github/).

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
| Mods, HD texture packs & Atmosphère cheats (`docs/mods.md`) | [/mods/](https://totkrecomp.wiki/mods/) |
| Crash, audio & GPU troubleshooting | [/troubleshooting/](https://totkrecomp.wiki/troubleshooting/) |
| TotK Recomp vs UltraTears vs SkyboundTotk | [/compare/](https://totkrecomp.wiki/compare/) |
| Version history (`0.1.1` → `0.3.12`) | [/changelog/](https://totkrecomp.wiki/changelog/) |
| Legal FAQ | [/is-it-legal/](https://totkrecomp.wiki/is-it-legal/) |

## Official Upstream Project

- Official repository: https://github.com/valentderah/totk-pc-recomp

Spotted an outdated note after a new upstream release? Open an issue here.
