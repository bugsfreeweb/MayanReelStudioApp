# Mayan Reel Studio — App, Releases & Website

This is the **public ship repo** for **Mayan Reel Studio** — an all-in-one, offline, GPU-first video
studio for Windows (edit, generate, caption, mix and export). MIT licensed.

It hosts three things:

| What | Where |
| --- | --- |
| **Product website** (this site) | `index.html` at the repo root — serve via GitHub Pages |
| **Release builds** (installer + portable) | the [Releases](../../releases) tab |
| **The app's update feed** | `latest*.yml` attached to each Release — `electron-updater` reads this repo |

> Source code lives in the private development repo
> **[`bugsfreeweb/MayanReelStudio`](https://github.com/bugsfreeweb/MayanReelStudio)**.
> This repo only holds the shipped site and the signed release artifacts, so app updates always
> resolve against finished builds — never against work in progress.

## Download

- **Installer:** `MayanReelStudio-<version>-x64.exe` (per-user, no admin prompt)
- **Portable:** `MayanReelStudio-<version>-portable.exe` (single file, shares the same app data)

Grab the latest from **[Releases](../../releases/latest)**.

## Why a separate repo

Publishing releases from the churning dev repo breaks the in-app "Check for updates". Keeping releases
here means the feed is stable and public while the source stays private during development.

## Website

A single self-contained `index.html` (no build step, no external CDNs, works offline). Enable **GitHub
Pages → Deploy from branch → `main` / root** to publish it.

---

MIT licensed · 2026 — Organise by: **Bugsfree Studio**. No watermark, no subscription, no telemetry.
