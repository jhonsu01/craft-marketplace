<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <b>English</b> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.fr.md">Français</a> · <a href="README.de.md">Deutsch</a> · <a href="README.ru.md">Русский</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">Codex plugin marketplace for the Craft MCP connectors: Claude-style bridges to the open-source Craft apps installed on your computer (Windows, macOS, Linux).</p>

---

## Plugins

| Plugin | What it does | Needs |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | Page layout, data merge, InDesign IDML, print-ready PDF/X, PNG, EPUB and HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | Motion graphics, animated titles, effects on videos, templates; MP4, ProRes, WebM, GIF, Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | Raw development: auto tone, 114 sliders, presets, masks, HDR and panoramas; JPEG, TIFF, WebP, AVIF, DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | Photo editing: resize, crop, adjustments, 122 filters, background removal, text and designs; PSD, PNG, JPEG, WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | Vector art: image trace, designs from shapes, text and charts, recolor; SVG, PDF, AI, EPS, DXF, PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF work: merge, split, pages, OCR, forms, signatures, redaction, passwords; to Word, HTML, images, PDF/A | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | Video editing: split, trim, effects, color looks, titles, speed, join with transitions; H.264, ProRes, GIF, OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |

## Install in Codex

1. *Plugins → Add → Add marketplace*.
2. **Source:** `jhonsu01/craft-marketplace` · **Git reference:** `main` · leave *sparse paths* empty.
3. Click **Add marketplace**, open the **Craft Bridges** marketplace and install **DesignCraft Bridge**.

From the command line:

```bash
codex plugin marketplace add jhonsu01/craft-marketplace
```

```bash
codex plugin add designcraft-mcp-server@craft
```

```bash
codex plugin add effectcraft-mcp-server@craft
```

```bash
codex plugin add lightcraft-mcp-server@craft
```

```bash
codex plugin add photocraft-mcp-server@craft
```

```bash
codex plugin add vectorcraft-mcp-server@craft
```

```bash
codex plugin add pdfcraft-mcp-server@craft
```

```bash
codex plugin add filmcraft-mcp-server@craft
```

The plugins start a local Node.js server, so Node.js ≥ 20 must be on `PATH`. If an app is not in its standard folder, set its variable (e.g. `DESIGNCRAFT_DIR`) as a system environment variable.

## Updates

Each new version of a connector is published here. In Codex, refresh the marketplace (or run `codex plugin marketplace upgrade craft`) and the plugin updates.

```bash
codex plugin marketplace upgrade craft
```

## Why a marketplace

Codex can also take a plugin as an uploaded zip, but an uploaded plugin is stored in your account and a newer zip with the same name is refused. A marketplace is a Git repository: Codex reads it, installs the plugins you choose and gets new versions with **Upgrade**.

## Other hosts

Claude Desktop and other `.mcpb` hosts: install the `.mcpb` from each connector's own releases, e.g. [designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest).

## License

Apache-2.0. The Craft apps belong to their authors (Storytold); these plugins are not affiliated with or endorsed by them.
