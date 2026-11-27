# Retro Relay Browser — Gaming Edition

**Project status:** Windows Preview 3 is the existing published/development lineage. This folder is the home for Gaming Edition documentation and (after review) project-specific source code. The existing root-level GitHub releases and notes are retained.

## Purpose
Gaming-centric web browsing: Twitch, Kick, game and indie discovery, upcoming releases, customizable gaming themes, browser import and privacy controls.

## Future source layout
```
projects/gaming/
  README.md
  app/                  # gaming edition Python source (not yet uploaded)
  tests/
  packaging/
```

The user's local source currently resides on their Windows machine at `C:\RRBrowser`. Do not assume documentation-only GitHub folders contain runnable source.

## Releases
Use release asset and tag names that clearly identify Gaming Edition. Retain the existing Preview 2 and Preview 3 links/files; do not move or delete them during initial organization.

## Shared foundation
Core browsing/navigation, security patches, bookmark import and non-branded utilities may eventually be shared with Anime Edition through a reviewed common library, while application identifiers and browser profiles remain isolated.
