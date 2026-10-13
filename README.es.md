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

Los complementos arrancan un servidor local de Node.js, así que Node.js ≥ 20 debe estar en el `PATH`. Si una app no está en su carpeta estándar, define su variable (p. ej. `DESIGNCRAFT_DIR`) como variable de entorno del sistema.

## DeepSeek Harness

Cada carpeta de plugin es también un bundle de DeepSeek Harness. En *Plugins → Add plugin* escribe la dirección de un plugin, pulsa **Install** y **Enable now**:

- `github:jhonsu01/craft-marketplace#path:/plugins/designcraft-mcp-server`
- `github:jhonsu01/craft-marketplace#path:/plugins/effectcraft-mcp-server`
- `github:jhonsu01/craft-marketplace#path:/plugins/lightcraft-mcp-server`
- `github:jhonsu01/craft-marketplace#path:/plugins/photocraft-mcp-server`
- `github:jhonsu01/craft-marketplace#path:/plugins/vectorcraft-mcp-server`
- `github:jhonsu01/craft-marketplace#path:/plugins/pdfcraft-mcp-server`
- `github:jhonsu01/craft-marketplace#path:/plugins/filmcraft-mcp-server`

Harness aún no actualiza los plugins por sí solo: para actualizar, desinstala y vuelve a instalar.

## Actualizaciones

Cada versión nueva de un conector se publica aquí. En Codex, actualiza el marketplace (o ejecuta `codex plugin marketplace upgrade craft`) y el complemento se actualiza.

```bash
codex plugin marketplace upgrade craft
```

## Por qué un marketplace

Codex también acepta un complemento subido como zip, pero queda guardado en tu cuenta y un zip más nuevo con el mismo nombre se rechaza. Un marketplace es un repositorio Git: Codex lo lee, instala los complementos que elijas y obtiene las versiones nuevas con **Actualizar**.

## Otros programas

Claude Desktop y otros programas `.mcpb`: instala el `.mcpb` desde las versiones de cada conector, p. ej. [designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest).

## Licencia

Apache-2.0. Las apps Craft pertenecen a sus autores (Storytold); estos complementos no están afiliados ni respaldados por ellos.
