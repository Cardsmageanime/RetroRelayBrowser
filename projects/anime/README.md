# Retro Relay Anime Browser — Anime Edition

**Status (November 27, 2026): 0.1 Alpha source starter prepared; Windows EXE and installer still require build and GUI testing.** Gaming Edition remains unchanged.

This is a **separate anime-only QtWebEngine application** under the same repository, not another feature embedded in Gaming Edition.

## 0.1 Alpha starter — implemented locally

- Independent application name, Qt Settings namespace, WebEngine profile, cache and bookmarks from Gaming Edition
- Dedicated anime homepage, tabs, navigation, search, anime sidebar and Anime Calendar action
- On-demand seasonal AniList metadata with Spring 2027 selected; official streaming, Japanese figures/clothing, and Blu-ray retailer directories
- Local-only bookmarks import from user-selected HTML and compatible Chromium JSON, with confirmation and duplicate checks
- No Twitch, Kick, indie-gaming dashboard, or gaming edition installation changes
- Python syntax check passed; **5/5 alpha unit tests passed locally** (not a Windows GUI test)
- Download the generated `RetroRelayAnimeBrowser_0_1_Alpha_Starter.zip` from the development conversation to build on Windows. The source is not yet published in this repo as runnable code.

## Windows development procedure

1. Extract the provided ZIP into `C:\RRAnimeBrowser`.
2. Run `powershell -NoProfile -ExecutionPolicy Bypass -File "C:\RRAnimeBrowser\Build_Anime_Alpha.ps1"`.
3. If the tests and PyInstaller succeed, launch `C:\RRAnimeBrowser\dist\RetroRelayAnimeBrowser.exe`.
4. Verify the window, tabs, all sidebar links, Spring 2027 refresh (including error handling), and bookmarks import.
5. Build a distinct Anime Edition installer **only after** Windows testing. Do not replace the Gaming Edition installer.

## Feature boundaries

Anime 0.1 is a proof-of-concept browser edition. Streaming links and shops are third-party destinations, not affiliated or guaranteed inventory feeds. Anime dates can be tentative. Manga, notifications, watchlists, richer privacy settings, and DVD/merchandise announcement feeds remain future development.

VPN remains a 2027 evaluation. Security review, browser-engine updates and clean Windows testing are needed before broad distribution.

## Repository release naming

Use `anime-v0.1.0-alpha` (future release tag), `RetroRelayAnimeBrowser.exe` and `RetroRelayAnimeBrowser-Setup-0.1.0-alpha.exe`, without renaming or removing existing Gaming Edition releases.
