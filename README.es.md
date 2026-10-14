<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <a href="README.md">English</a> · <b>Español</b> · <a href="README.pt-BR.md">Português</a> · <a href="README.fr.md">Français</a> · <a href="README.de.md">Deutsch</a> · <a href="README.ru.md">Русский</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">Marketplace de complementos de Codex para los conectores MCP Craft: puentes hacia las apps Craft de código abierto instaladas en tu equipo (Windows, macOS, Linux).</p>

---

## Complementos

| Complemento | Qué hace | Necesita |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | Maquetación, combinación de datos, IDML de InDesign, PDF/X para imprenta, PNG, EPUB y HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | Motion graphics, títulos animados, efectos en videos, plantillas; MP4, ProRes, WebM, GIF, Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | Revelado raw: tono automático, 114 controles, ajustes preestablecidos, máscaras, HDR y panorámicas; JPEG, TIFF, WebP, AVIF, DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | Edición de fotos: tamaño, recorte, ajustes, 122 filtros, quitar fondos, texto y diseños; PSD, PNG, JPEG, WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | Arte vectorial: vectorizar imágenes, diseños con formas, texto y gráficos, recolorear; SVG, PDF, AI, EPS, DXF, PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF: unir, dividir, páginas, OCR, formularios, firmas, redacción, contraseñas; a Word, HTML, imágenes, PDF/A | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | Edición de video: dividir, recortar, efectos, looks de color, títulos, velocidad, unir con transiciones; H.264, ProRes, GIF, OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |
| **WordCraft Bridge** (`wordcraft-mcp-server`) | Procesador de textos: documentos con títulos, listas, tablas e imágenes, buscar / reemplazar, comentarios, control de cambios, combinación de correspondencia; DOCX, PDF, ODT, RTF, Markdown, LaTeX | [WordCraft](https://github.com/storytold/wordcraft) + Node.js ≥ 20 |

## Instalar en Codex

1. *Complementos → Añadir → Añadir marketplace*.
2. **Origen:** `jhonsu01/craft-marketplace` · **Referencia de Git:** `main` · deja *Rutas dispersas* vacío.
3. Pulsa **Añadir marketplace**, abre el marketplace **Craft Bridges** e instala **DesignCraft Bridge**.

Desde la línea de comandos:

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

Los complementos arrancan un servidor local de Node.js, así que Node.js ≥ 20 debe estar en el `PATH`. Si una app no está en su carpeta estándar, define su variable (p. ej. `DESIGNCRAFT_DIR`) como variable de entorno del sistema.

## DeepSeek Harness

Cada carpeta de plugin es también un bundle de DeepSeek Harness. En *Plugins → Add plugin* escribe la dirección de un plugin, pulsa **Install** y **Enable now**:

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

Harness aún no actualiza los plugins por sí solo: para actualizar, desinstala y vuelve a instalar.

## Actualizaciones

Cada versión nueva de un conector se publica aquí. En Codex, actualiza el marketplace (o ejecuta `codex plugin marketplace upgrade craft`) y el complemento se actualiza.

```bash
codex plugin marketplace upgrade craft
```

## Por qué un marketplace

Codex también acepta un complemento subido como zip, pero queda guardado en tu cuenta y un zip más nuevo con el mismo nombre se rechaza. Un marketplace es un repositorio Git: Codex lo lee, instala los complementos que elijas y obtiene las versiones nuevas con **Actualizar**.

## Otros programas

Claude Desktop, SunsamCode y otros programas `.mcpb`: descarga el `.mcpb` de la última versión de cada conector y haz doble clic:

- **DesignCraft Bridge**: [designcraft-mcp-server.mcpb](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest/download/designcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/designcraft-mcp-server)
- **EffectCraft Bridge**: [effectcraft-mcp-server.mcpb](https://github.com/jhonsu01/effectcraft-mcp-server/releases/latest/download/effectcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/effectcraft-mcp-server)
- **LightCraft Bridge**: [lightcraft-mcp-server.mcpb](https://github.com/jhonsu01/lightcraft-mcp-server/releases/latest/download/lightcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/lightcraft-mcp-server)
- **PhotoCraft Bridge**: [photocraft-mcp-server.mcpb](https://github.com/jhonsu01/photocraft-mcp-server/releases/latest/download/photocraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/photocraft-mcp-server)
- **VectorCraft Bridge**: [vectorcraft-mcp-server.mcpb](https://github.com/jhonsu01/vectorcraft-mcp-server/releases/latest/download/vectorcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/vectorcraft-mcp-server)
- **PdfCraft Bridge**: [pdfcraft-mcp-server.mcpb](https://github.com/jhonsu01/pdfcraft-mcp-server/releases/latest/download/pdfcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/pdfcraft-mcp-server)
- **FilmCraft Bridge**: [filmcraft-mcp-server.mcpb](https://github.com/jhonsu01/filmcraft-mcp-server/releases/latest/download/filmcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/filmcraft-mcp-server)
- **WordCraft Bridge**: [wordcraft-mcp-server.mcpb](https://github.com/jhonsu01/wordcraft-mcp-server/releases/latest/download/wordcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/wordcraft-mcp-server)

## Licencia

Apache-2.0. Las apps Craft pertenecen a sus autores (Storytold); estos complementos no están afiliados ni respaldados por ellos.
