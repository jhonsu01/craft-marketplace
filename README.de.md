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

Die Plugins starten einen lokalen Node.js-Server, daher muss Node.js ≥ 20 im `PATH` liegen. Liegt eine App nicht in ihrem Standardordner, setzen Sie ihre Variable (z. B. `DESIGNCRAFT_DIR`) als Systemumgebungsvariable.

## Updates

Jede neue Version eines Konnektors wird hier veröffentlicht. Aktualisieren Sie in Codex den Marketplace (oder führen Sie `codex plugin marketplace upgrade craft` aus), dann wird das Plugin aktualisiert.

```bash
codex plugin marketplace upgrade craft
```

## Warum ein Marketplace

Codex nimmt ein Plugin auch als hochgeladenes Zip an, aber es wird in Ihrem Konto gespeichert und ein neueres Zip mit demselben Namen wird abgelehnt. Ein Marketplace ist ein Git-Repository: Codex liest es, installiert die gewählten Plugins und holt neue Versionen mit **Aktualisieren**.

## Andere Programme

Claude Desktop und andere `.mcpb`-Programme: Installieren Sie die `.mcpb` aus den Releases des jeweiligen Konnektors, z. B. [designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest).

## Lizenz

Apache-2.0. Die Craft-Apps gehören ihren Autoren (Storytold); diese Plugins sind weder mit ihnen verbunden noch von ihnen unterstützt.
