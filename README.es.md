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

Los complementos arrancan un servidor local de Node.js, así que Node.js ≥ 20 debe estar en el `PATH`. Si una app no está en su carpeta estándar, define su variable (p. ej. `DESIGNCRAFT_DIR`) como variable de entorno del sistema.

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
