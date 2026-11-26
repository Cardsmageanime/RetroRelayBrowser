# Retro Relay Browser

**Retro Relay Browser** is a free, gaming-focused desktop browser for Windows. Linux support is in development. It offers tabbed browsing, customizable themes, gaming news and discovery, and privacy and resource-management features.

## Windows beta — Preview 3

**Version:** `2.0.0-preview3` — tested locally on Windows 10 (64-bit). The Windows EXE was rebuilt on November 25, 2026, with 79 automated tests passing, and the Preview 3 installer compiled and installed alongside both Preview 2 installations. The installed build's four homepage shortcuts were manually checked.

**Release upload status:** Preview 3 binaries are built locally but **have not yet been uploaded/published as a GitHub Release**. Until the new release is live, the existing Preview 2 release remains the public fallback.

When Preview 3 is published, get the downloads from [GitHub Releases](https://github.com/Cardsmageanime/RetroRelayBrowser/releases):

- **`RetroRelayBrowser-Setup-2.0.0-preview3.exe`** — Windows installer, Start menu shortcut and uninstall support; optional desktop shortcut.
- **`RetroRelayBrowser.exe`** — standalone Windows executable, no installer required.

### What's improved in Preview 3

The four home-page actions now work: **Live Streams**, **Indie Discovery**, **Upcoming Games**, and **Free Themes**. The fix was verified in the rebuilt EXE. The Preview 3 installer uses its own application identity and installation directory so it can coexist with Preview 2.

[Preview 3 release notes](RELEASE_NOTES_PREVIEW3.md)

### Install and upgrade

Download the installer from the release page after Preview 3 is published. Run it and follow the prompts. A separate installation directory does not guarantee separate browser settings or profiles. Keep backups of important user data and test before migrating or uninstalling Preview 2.

This is **beta software**, and further issues may remain. The installer and EXE have not completed independent security or clean-system distribution testing; Windows may show warnings for unsigned executables.

## Previous beta

[Preview 2 (`v2.0.0-preview2`)](https://github.com/Cardsmageanime/RetroRelayBrowser/releases/tag/v2.0.0-preview2) remains available as an archived fallback while Preview 3 is rolled out. It is not the recommended build once Preview 3 is live.

## Future revenue features (planned)

Retro Relay Browser will remain free. We are designing three optional ways to support development: [Indie Developer Spotlight sponsorships](https://github.com/Cardsmageanime/RetroRelayBrowser/issues/2), [Gaming Deals affiliate links](https://github.com/Cardsmageanime/RetroRelayBrowser/issues/3), and [voluntary Support Retro Relay donations](https://github.com/Cardsmageanime/RetroRelayBrowser/issues/4). These features **are not available in Preview 3** and no payments or partnerships are active. See the [monetization roadmap](MONETIZATION_ROADMAP.md).

## Browser import and privacy roadmap

**Current development:** a local-only [bookmark importing feature](https://github.com/Cardsmageanime/RetroRelayBrowser/issues/5) for exported bookmarks from other browsers, plus [configurable privacy-oriented search](https://github.com/Cardsmageanime/RetroRelayBrowser/issues/7). A standalone bookmark-parser component has been tested, but it is **not integrated into the published Preview 3 executable** yet. The Windows application source and UI integration are required.

**2027:** investigate an [optional VPN integration](https://github.com/Cardsmageanime/RetroRelayBrowser/issues/6), subject to provider/security evaluation. No VPN is included today.

## Linux

Linux packaging and CI build scripts are in development. Native Linux compilation and desktop testing are still needed. The Windows EXE is not a Linux release.

## Feedback

Please report bugs and feature requests via [GitHub Issues](https://github.com/Cardsmageanime/RetroRelayBrowser/issues). Include the browser version, Windows version and reproduction steps. Never share passwords or personal browsing data.

## License and third-party software

A project license has not yet been selected. Review and comply with the licenses and notices of all bundled third-party components before redistributing binaries.
