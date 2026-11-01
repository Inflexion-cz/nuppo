# Nuppo for macOS

Nuppo lives in your menu bar and the notch. Hover the notch (or the fake one on a Mac without it) and a panel slides out with your latest screenshots, downloads, a shelf for files and quick notes. Built for dropping a screenshot straight into a terminal or an AI chat, no Finder in between. Free.

This repository only hosts downloads and update info. More at **https://nuppo.inflexion.cz**.

Requires macOS 14 or later (Apple silicon and Intel).

## Install

One line in Terminal:

```sh
curl -fsSL https://nuppo.inflexion.cz/install.sh | sh
```

It downloads the latest release, checks its SHA-256, and puts Nuppo.app into /Applications (or ~/Applications).

### Manual install

1. Download [Nuppo.zip](https://github.com/Inflexion-cz/nuppo/releases/latest/download/Nuppo.zip) and unzip it.
2. Drag Nuppo.app to your Applications folder.
3. Open it (see below).

### Opening an app from an unidentified developer

Nuppo is not notarized by Apple, so macOS asks for confirmation the first time:

- **macOS 15 and later:** try to open Nuppo once, then go to System Settings › Privacy & Security, scroll down and click **Open Anyway**.
- **macOS 14:** right-click Nuppo.app › **Open** › Open.

You only need to do this once. The installer above skips this step. Later updates arrive automatically inside the app.

## Verify

Each release includes `Nuppo.zip.sha256`:

```sh
shasum -a 256 -c Nuppo.zip.sha256
```
