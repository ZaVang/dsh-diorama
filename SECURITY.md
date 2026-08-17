# Security

## Scope

This plugin is a browser-only client bundle for the DeepSeek Harness Web GUI. It runs entirely in the browser and makes no model requests.

## What it does with your data

- **localStorage**: skin selection (`dsh.skinSwitcher.active`) and per-skin decoration configs (`dsh.skinDeco.*`) are stored in your browser only. Nothing is sent anywhere.
- **Uploads**: images you add in the decoration editor are read as data URLs and stored in localStorage. They never leave your machine.
- **No network**: the plugin performs no network calls. All artwork is inlined in the bundle.

## Trust model

The decoration editor executes no third-party code; it only positions `<img>` elements. Imported diorama packs are parsed as JSON data and applied as image positions — the `src` values are data URLs your browser already trusts, and no scripts are evaluated.

## Reporting

Open an issue at https://github.com/ZaVang/dsh-diorama/issues.
