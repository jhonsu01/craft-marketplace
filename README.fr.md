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
| **WordCraft Bridge** (`wordcraft-mcp-server`) | Traitement de texte : documents avec titres, listes, tableaux et images, rechercher / remplacer, commentaires, suivi des modifications, publipostage ; DOCX, PDF, ODT, RTF, Markdown, LaTeX | [WordCraft](https://github.com/storytold/wordcraft) + Node.js ≥ 20 |

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

```bash
codex plugin add wordcraft-mcp-server@craft
```

Les plugins lancent un serveur Node.js local : Node.js ≥ 20 doit donc être dans le `PATH`. Si une application n'est pas dans son dossier standard, définissez sa variable (par ex. `DESIGNCRAFT_DIR`) comme variable d'environnement système.

## DeepSeek Harness

Chaque dossier de plugin est aussi un bundle DeepSeek Harness. Dans *Plugins → Add plugin*, saisissez l'adresse d'un plugin, puis cliquez sur **Install** et **Enable now** :

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

Harness ne met pas encore les plugins à jour tout seul : pour mettre à jour, désinstallez puis réinstallez.

## Mises à jour

Chaque nouvelle version d'un connecteur est publiée ici. Dans Codex, actualisez le marketplace (ou lancez `codex plugin marketplace upgrade craft`) et le plugin se met à jour.

```bash
codex plugin marketplace upgrade craft
```

## Pourquoi un marketplace

Codex accepte aussi un plugin envoyé en zip, mais il est enregistré dans votre compte et un zip plus récent portant le même nom est refusé. Un marketplace est un dépôt Git : Codex le lit, installe les plugins choisis et récupère les nouvelles versions avec **Mettre à jour**.

## Autres logiciels

Claude Desktop, SunsamCode et autres logiciels `.mcpb` : téléchargez le `.mcpb` de la dernière version de chaque connecteur et double-cliquez dessus :

- **DesignCraft Bridge**: [designcraft-mcp-server.mcpb](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest/download/designcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/designcraft-mcp-server)
- **EffectCraft Bridge**: [effectcraft-mcp-server.mcpb](https://github.com/jhonsu01/effectcraft-mcp-server/releases/latest/download/effectcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/effectcraft-mcp-server)
- **LightCraft Bridge**: [lightcraft-mcp-server.mcpb](https://github.com/jhonsu01/lightcraft-mcp-server/releases/latest/download/lightcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/lightcraft-mcp-server)
- **PhotoCraft Bridge**: [photocraft-mcp-server.mcpb](https://github.com/jhonsu01/photocraft-mcp-server/releases/latest/download/photocraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/photocraft-mcp-server)
- **VectorCraft Bridge**: [vectorcraft-mcp-server.mcpb](https://github.com/jhonsu01/vectorcraft-mcp-server/releases/latest/download/vectorcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/vectorcraft-mcp-server)
- **PdfCraft Bridge**: [pdfcraft-mcp-server.mcpb](https://github.com/jhonsu01/pdfcraft-mcp-server/releases/latest/download/pdfcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/pdfcraft-mcp-server)
- **FilmCraft Bridge**: [filmcraft-mcp-server.mcpb](https://github.com/jhonsu01/filmcraft-mcp-server/releases/latest/download/filmcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/filmcraft-mcp-server)
- **WordCraft Bridge**: [wordcraft-mcp-server.mcpb](https://github.com/jhonsu01/wordcraft-mcp-server/releases/latest/download/wordcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/wordcraft-mcp-server)

## Licence

Apache-2.0. Les applications Craft appartiennent à leurs auteurs (Storytold) ; ces plugins ne sont ni affiliés ni approuvés par eux.
