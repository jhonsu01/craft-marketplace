<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.fr.md">Français</a> · <b>Deutsch</b> · <a href="README.ru.md">Русский</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">Codex-Plugin-Marketplace für die Craft-MCP-Konnektoren: Brücken zu den quelloffenen Craft-Apps auf Ihrem Computer (Windows, macOS, Linux).</p>

---

## Plugins

| Plugin | Was es tut | Voraussetzung |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | Seitenlayout, Datenzusammenführung, InDesign-IDML, druckfertiges PDF/X, PNG, EPUB und HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | Motion Graphics, animierte Titel, Effekte auf Videos, Vorlagen; MP4, ProRes, WebM, GIF, Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | Raw-Entwicklung: Auto-Tonwert, 114 Regler, Vorgaben, Masken, HDR und Panoramen; JPEG, TIFF, WebP, AVIF, DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | Bildbearbeitung: Größe, Zuschnitt, Korrekturen, 122 Filter, Hintergrund entfernen, Text und Designs; PSD, PNG, JPEG, WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | Vektorgrafik: Bilder nachzeichnen, Designs aus Formen, Text und Diagrammen, umfärben; SVG, PDF, AI, EPS, DXF, PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF: zusammenführen, teilen, Seiten, OCR, Formulare, Signaturen, Schwärzen, Passwörter; nach Word, HTML, Bilder, PDF/A | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | Videoschnitt: teilen, trimmen, Effekte, Farblooks, Titel, Tempo, mit Übergängen verbinden; H.264, ProRes, GIF, OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |
| **WordCraft Bridge** (`wordcraft-mcp-server`) | Textverarbeitung: Dokumente mit Überschriften, Listen, Tabellen und Bildern, Suchen / Ersetzen, Kommentare, Änderungsverfolgung, Serienbriefe; DOCX, PDF, ODT, RTF, Markdown, LaTeX | [WordCraft](https://github.com/storytold/wordcraft) + Node.js ≥ 20 |

## In Codex installieren

1. *Plugins → Hinzufügen → Marketplace hinzufügen*.
2. **Quelle:** `jhonsu01/craft-marketplace` · **Git-Referenz:** `main` · *Sparse-Pfade* leer lassen.
3. Auf **Marketplace hinzufügen** klicken, den Marketplace **Craft Bridges** öffnen und **DesignCraft Bridge** installieren.

Über die Kommandozeile:

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

```bash
codex plugin add wordcraft-mcp-server@craft
```

Die Plugins starten einen lokalen Node.js-Server, daher muss Node.js ≥ 20 im `PATH` liegen. Liegt eine App nicht in ihrem Standardordner, setzen Sie ihre Variable (z. B. `DESIGNCRAFT_DIR`) als Systemumgebungsvariable.

## DeepSeek Harness

Jeder Plugin-Ordner ist auch ein DeepSeek-Harness-Bundle. In *Plugins → Add plugin* die Adresse eines Plugins eingeben, **Install** und **Enable now** klicken:

```text
github:jhonsu01/craft-marketplace#path:/plugins/designcraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/effectcraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/lightcraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/photocraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/vectorcraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/pdfcraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/filmcraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/wordcraft-mcp-server
```

Harness aktualisiert Plugins noch nicht selbst: Zum Aktualisieren deinstallieren und neu installieren.

## Updates

Jede neue Version eines Konnektors wird hier veröffentlicht. Aktualisieren Sie in Codex den Marketplace (oder führen Sie `codex plugin marketplace upgrade craft` aus), dann wird das Plugin aktualisiert.

```bash
codex plugin marketplace upgrade craft
```

## Warum ein Marketplace

Codex nimmt ein Plugin auch als hochgeladenes Zip an, aber es wird in Ihrem Konto gespeichert und ein neueres Zip mit demselben Namen wird abgelehnt. Ein Marketplace ist ein Git-Repository: Codex liest es, installiert die gewählten Plugins und holt neue Versionen mit **Aktualisieren**.

## Andere Programme

Claude Desktop, SunsamCode und andere `.mcpb`-Programme: Die `.mcpb` aus dem neuesten Release des jeweiligen Konnektors herunterladen und doppelklicken:

- **DesignCraft Bridge**: [designcraft-mcp-server.mcpb](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest/download/designcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/designcraft-mcp-server)
- **EffectCraft Bridge**: [effectcraft-mcp-server.mcpb](https://github.com/jhonsu01/effectcraft-mcp-server/releases/latest/download/effectcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/effectcraft-mcp-server)
- **LightCraft Bridge**: [lightcraft-mcp-server.mcpb](https://github.com/jhonsu01/lightcraft-mcp-server/releases/latest/download/lightcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/lightcraft-mcp-server)
- **PhotoCraft Bridge**: [photocraft-mcp-server.mcpb](https://github.com/jhonsu01/photocraft-mcp-server/releases/latest/download/photocraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/photocraft-mcp-server)
- **VectorCraft Bridge**: [vectorcraft-mcp-server.mcpb](https://github.com/jhonsu01/vectorcraft-mcp-server/releases/latest/download/vectorcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/vectorcraft-mcp-server)
- **PdfCraft Bridge**: [pdfcraft-mcp-server.mcpb](https://github.com/jhonsu01/pdfcraft-mcp-server/releases/latest/download/pdfcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/pdfcraft-mcp-server)
- **FilmCraft Bridge**: [filmcraft-mcp-server.mcpb](https://github.com/jhonsu01/filmcraft-mcp-server/releases/latest/download/filmcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/filmcraft-mcp-server)
- **WordCraft Bridge**: [wordcraft-mcp-server.mcpb](https://github.com/jhonsu01/wordcraft-mcp-server/releases/latest/download/wordcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/wordcraft-mcp-server)

## Lizenz

Apache-2.0. Die Craft-Apps gehören ihren Autoren (Storytold); diese Plugins sind weder mit ihnen verbunden noch von ihnen unterstützt.
