# Retro Relay Anime Browser — Anime Edition

**Project status:** New separate product in the same GitHub repository. Planned initial version: **0.1 Alpha**. **No Anime Edition binary is published or tested as a standalone application yet.**

## Goal
Reuse the reliable browsing engine from Retro Relay Browser, but create an **anime-only interface** instead of a gaming dashboard. Remove Twitch, Kick, game discovery and gaming-specific branding from this edition.

## Planned Anime Edition features
- Seasonal anime calendars, including the Spring 2027 view with dates identified as tentative when unconfirmed
- Authorized streaming destinations, original source announcements, and optional watchlists
- Manga/light novels, anime news, anime DVDs and Blu-rays
- Official Japanese figure/action-figure manufacturers, import shops, clothing and licensed merchandise
- Local-first bookmarks import and configurable privacy-oriented search
- No unlicensed anime video hosting; avoid scraping or redistributing protected artwork without permission

## Separation requirements
- Local Windows workspace: `C:\RRAnimeBrowser` (separate copy or branch, not editing `C:\RRBrowser` in place)
- Separate app name, executable, installer AppId, install path and Start menu/desktop shortcuts
- **Separate profile directory**, bookmarks, history, cookies, sessions and cache from Gaming Edition
- Clearly distinguish both editions' release assets and tags, while retaining one repository and one GitHub account
- First audit/reuse the previously developed anime discovery modules from the user's local source only after confirming they were preserved in a backup

## Future source layout
```
projects/anime/
  README.md
  app/                  # anime edition Python source (to be added after local development)
  tests/
  packaging/
```

## Release naming example
`anime-v0.1.0-alpha` tag and `RetroRelayAnimeBrowser-Setup-0.1.0-alpha.exe` asset. Do not publish a release until the complete packaged app has passed testing.

## Shared core
Reuse the web engine, tabs, navigation, bookmark import and carefully reviewed privacy/security improvements. Do not share user profiles or payment/affiliate settings between editions by default.
