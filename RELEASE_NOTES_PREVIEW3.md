# Retro Relay Browser 2.0 — Preview 3 Windows Beta

**Tag:** `v2.0.0-preview3`  
**Release type:** Pre-release  
**Platform:** Windows 10 (64-bit); other versions not yet independently verified.

## Downloads for this release

Upload these two distinct Windows artifacts to GitHub Releases:

- **`RetroRelayBrowser-Setup-2.0.0-preview3.exe`** — Inno Setup installer, built locally at `C:\RRBrowser\setup_output\RetroRelayBrowser-Setup-2.0.0-preview3.exe`.
- **`RetroRelayBrowser.exe`** — standalone executable, rebuilt locally at `C:\RRBrowser\dist\RetroRelayBrowser.exe`.

**Important:** These paths are on the developer's computer. They are not public download URLs until the binaries are uploaded as release assets.

## Changes from Preview 2

- Fixed the four homepage shortcut actions: **Live Streams**, **Indie Discovery**, **Upcoming Games**, and **Free Themes**.
- Rebuilt the Windows executable and packaged a new Preview 3 installer.
- Assigned Preview 3 a distinct Inno Setup application identity and installation directory, allowing side-by-side installation with Preview 2.

## Verification so far

- **79/79 automated tests passed** in the November 25, 2026 local rebuild.
- PyInstaller generated the new standalone EXE successfully.
- Inno Setup 7 compiled the Preview 3 Windows installer successfully.
- Preview 3 installed with a separate Windows uninstall registration while preserving two previously installed Preview 2 variants.
- Homepage actions were manually tested. Further minor issues may remain.

This does not establish successful testing on a clean Windows device or independent security auditing. The binaries may be unsigned.

## Known limitations

- Linux binaries are not included in this release.
- Preview 3 and Preview 2 may still share profile/settings locations; separate installers do not automatically isolate user data.
- This is an early beta, not a stable production release.

## Publish checklist

- [ ] Upload **both** Windows EXEs as assets of release tag `v2.0.0-preview3`.
- [ ] Mark the release **Pre-release**.
- [ ] Download and test the published installer and standalone EXE, preferably on a clean Windows test machine.
- [ ] Confirm uninstall and shortcuts, and do not delete shared browsing profiles inadvertently.
- [ ] Confirm third-party license obligations before broader distribution.
- [ ] Retain Preview 2 as an archived fallback until Preview 3 downloads are confirmed.

Report issues through [GitHub Issues](https://github.com/Cardsmageanime/RetroRelayBrowser/issues). Do not attach browsing profiles, passwords, or private information.
