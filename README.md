<div align="center">

<a href="https://hookline.vante.app"><img alt="Hookline: Catch every webhook. Replay anything." src="https://hookline.vante.app/readme/banner-dark.webp" width="100%"></a>

<br>

**The official [Homebrew](https://brew.sh) tap for the Hookline CLI.**

[![Homebrew](https://img.shields.io/badge/brew-kaanxsrd%2Ftap%2Fhookline-fbb040?style=flat-square&logo=homebrew&logoColor=black)](#install)
[![Version](https://img.shields.io/npm/v/hookline-cli?style=flat-square&label=version&color=8b7cf6)](https://hookline.vante.app/changelog)
[![License: GPL-3.0](https://img.shields.io/badge/license-GPL--3.0-8b7cf6?style=flat-square)](https://www.gnu.org/licenses/gpl-3.0.html)

**[Hookline](https://hookline.vante.app)** ·
**[CLI docs](https://hookline.vante.app/docs/cli)** ·
**[Changelog](https://hookline.vante.app/changelog)**

</div>

<br>

[Hookline](https://hookline.vante.app) gives you a webhook URL that captures every request, shows it live and replays it anywhere. The `hookline` CLI forwards those webhooks to `localhost`, so you can develop against real Stripe, GitHub or Shopify events on your own machine.

## Install

```sh
brew install --cask kaanxsrd/tap/hookline
```

Then sign in and start forwarding:

```sh
hookline login
hookline listen <slug> --forward http://localhost:3000/api/webhooks
```

The cask works on macOS (Apple silicon and Intel) and Linux (x64 and arm64). The binary is not notarized, so the cask clears the macOS quarantine flag during installation.

## Upgrade and uninstall

```sh
brew upgrade hookline
brew uninstall hookline
brew untap kaanxsrd/tap   # optional: remove this tap
```

## Other ways to install

| Platform | Command |
| --- | --- |
| npm (any platform, Node 18+) | `npm install -g hookline-cli` |
| Windows (Scoop) | `scoop bucket add hookline https://github.com/kaanxsrd/scoop-bucket` then `scoop install hookline` |

## About this repository

[`Casks/hookline.rb`](Casks/hookline.rb) is generated and committed by the Hookline release pipeline on every release, with the download URLs and SHA-256 checksums of that release. Please don't edit it by hand. Report problems with the CLI through [hookline.vante.app](https://hookline.vante.app).
