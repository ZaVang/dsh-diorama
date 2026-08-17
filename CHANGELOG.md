# Changelog

## 0.1.0 — 2026-08-17

Initial release.

### Features

- **Two character skins** for DeepSeek Harness:
  - 雪乃 · 暖阳日常 (Yukino warm daily): dual character sprites (school chibi + magazine) plus three sticker sheets
  - 隐秘年代志 (Occult editorial): dual character sprites plus two sticker sheets
- **Skin switcher**: bottom-right dropdown to pick a skin or restore the official default; each skin row carries an inline ✎ edit button.
- **Decoration editor**: drag to move, corner handle to resize, rotate / opacity sliders, numeric X / Y / width fine-tune, bottom/top + left/right anchor switching, and custom asset upload.
- **Shareable diorama packs**: export bundles assets (data URLs) with the layout as a single JSON; import restores the pack, switches to its skin, and opens the editor for further tweaks.
- **Persistence**: skin selection and decoration config live in localStorage and survive reloads.

### Notes

- All artwork is inlined (webp / jpeg data URLs), so the plugin carries no static assets.
- Artwork for the bundled characters originates from the Codex-Dream-Skin preset collection; check asset rights before redistributing commercially.
