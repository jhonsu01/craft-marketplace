<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <b>Français</b> · <a href="README.de.md">Deutsch</a> · <a href="README.ru.md">Русский</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">Marketplace de plugins Codex pour les connecteurs MCP Craft : des passerelles vers les applications Craft open source installées sur votre ordinateur (Windows, macOS, Linux).</p>

---

## Plugins

| Plugin | Ce qu'il fait | Prérequis |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | Mise en page, fusion de données, IDML d'InDesign, PDF/X pour l'impression, PNG, EPUB et HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | Motion design, titres animés, effets sur vidéos, modèles ; MP4, ProRes, WebM, GIF, Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | Développement raw : tonalité auto, 114 réglages, préréglages, masques, HDR et panoramas ; JPEG, TIFF, WebP, AVIF, DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | Retouche photo : taille, recadrage, réglages, 122 filtres, détourage, texte et créations ; PSD, PNG, JPEG, WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | Dessin vectoriel : vectorisation, créations avec formes, texte et graphiques, recoloration ; SVG, PDF, AI, EPS, DXF, PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF : fusionner, scinder, pages, OCR, formulaires, signatures, caviardage, mots de passe ; vers Word, HTML, images, PDF/A | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | Montage vidéo : découper, rogner, effets, looks couleur, titres, vitesse, assembler avec transitions ; H.264, ProRes, GIF, OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |

## Installer dans Codex

1. *Plugins → Ajouter → Ajouter un marketplace*.
2. **Source :** `jhonsu01/craft-marketplace` · **Référence Git :** `main` · laissez les *chemins partiels* vides.
3. Cliquez sur **Ajouter le marketplace**, ouvrez le marketplace **Craft Bridges** et installez **DesignCraft Bridge**.

En ligne de commande :

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

Les plugins lancent un serveur Node.js local : Node.js ≥ 20 doit donc être dans le `PATH`. Si une application n'est pas dans son dossier standard, définissez sa variable (par ex. `DESIGNCRAFT_DIR`) comme variable d'environnement système.

## Mises à jour

Chaque nouvelle version d'un connecteur est publiée ici. Dans Codex, actualisez le marketplace (ou lancez `codex plugin marketplace upgrade craft`) et le plugin se met à jour.

```bash
codex plugin marketplace upgrade craft
```

## Pourquoi un marketplace

Codex accepte aussi un plugin envoyé en zip, mais il est enregistré dans votre compte et un zip plus récent portant le même nom est refusé. Un marketplace est un dépôt Git : Codex le lit, installe les plugins choisis et récupère les nouvelles versions avec **Mettre à jour**.

## Autres logiciels

Claude Desktop et autres logiciels `.mcpb` : installez le `.mcpb` depuis les versions de chaque connecteur, par ex. [designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest).

## Licence

Apache-2.0. Les applications Craft appartiennent à leurs auteurs (Storytold) ; ces plugins ne sont ni affiliés ni approuvés par eux.
