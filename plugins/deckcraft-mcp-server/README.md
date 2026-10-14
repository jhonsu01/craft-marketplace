<p align="center"><img src="icon.png" width="120" alt="DeckCraft Bridge icon"></p>

<h1 align="center">DeckCraft MCP Server</h1>

<p align="center">
  <b>English</b> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.fr.md">Français</a> · <a href="README.de.md">Deutsch</a> · <a href="README.ru.md">Русский</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">
  Let Claude make slide decks with the <b>DeckCraft</b> installed on your computer — <b>Windows, macOS and Linux</b>:<br>
  slides with bullets, pictures, charts, tables and notes, themes and transitions, PowerPoint pptx, pdf, slide images and outlines.
</p>

---

## Why

[DeckCraft](https://github.com/storytold/deckcraft) is an open-source, PowerPoint-class presentation app with a headless CLI (`deckcraft-cli`), 226 commands, eight themes, PowerPoint `.pptx` import and export and an MCP mode. This [Model Context Protocol](https://modelcontextprotocol.io) server turns that engine into **file-in / file-out tools** for Claude, so you can ask things like:

> *"Make a 6-slide pitch deck with a chart of our sales and a table by region, as PPTX and PDF."*
> *"Turn this outline into slides with the Harbor theme, slide numbers and speaker notes."*
> *"In every deck in `D:\Decks`, replace 'ACME Ltd.' with 'ACME Inc.' and add a footer."*
> *"Export this presentation as notes pages and as one PNG per slide."*
> *"Read this pptx and summarize what each slide says."*

Sibling of [designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server), [effectcraft-mcp-server](https://github.com/jhonsu01/effectcraft-mcp-server), [lightcraft-mcp-server](https://github.com/jhonsu01/lightcraft-mcp-server), [photocraft-mcp-server](https://github.com/jhonsu01/photocraft-mcp-server), [vectorcraft-mcp-server](https://github.com/jhonsu01/vectorcraft-mcp-server), [filmcraft-mcp-server](https://github.com/jhonsu01/filmcraft-mcp-server), [pdfcraft-mcp-server](https://github.com/jhonsu01/pdfcraft-mcp-server), [wordcraft-mcp-server](https://github.com/jhonsu01/wordcraft-mcp-server), [soundcraft-mcp-server](https://github.com/jhonsu01/soundcraft-mcp-server), [gridcraft-mcp-server](https://github.com/jhonsu01/gridcraft-mcp-server) and [audacity-mcp-server](https://github.com/jhonsu01/audacity-mcp-server).

## Platforms

| OS | DeckCraft package to install | Where the server finds it (no setup needed) | Status |
| --- | --- | --- | --- |
| **Windows** 10/11 (x64, x86, arm64) | MSI or portable zip | `C:\Program Files\DeckCraft`, `%LOCALAPPDATA%\Programs\DeckCraft`, `PATH` | ✅ Verified (Windows 11) |
| **Linux** (x86_64, aarch64, riscv64) | `.deb`, `.rpm` or `.tar.gz` | `/usr/bin`, `/usr/local/bin`, `/opt/deckcraft/bin`, `~/.local/bin`, `PATH` | ✅ Verified (Debian 12, headless) |
| **macOS** 11+ (Apple silicon and Intel) | `.dmg` (the app) **plus** `deckcraft-cli-<version>-macos-universal.zip` | `/Applications/DeckCraft.app`, `/usr/local/bin`, `/opt/homebrew/bin`, `~/.local/bin`, `~/bin`, `PATH` | 🟡 Supported, not yet tested on a Mac |

All downloads: [DeckCraft releases](https://github.com/storytold/deckcraft/releases) (there is also a FreeBSD tar.gz; set `DECKCRAFT_DIR` to it). Anywhere else: set `DECKCRAFT_DIR` (folder, `.tar.gz` root or `DeckCraft.app`) or `DECKCRAFT_CLI`.

- **macOS:** the DMG contains only the app. Unzip the separate `deckcraft-cli` zip and move `deckcraft-cli` to `/usr/local/bin` (or point `DECKCRAFT_CLI` at it). The first run checks Apple's notarization online.
- **Linux:** the AppImage and Flatpak contain only the app, not `deckcraft-cli`; use the deb, rpm or tar.gz. For an AppImage app, set `DECKCRAFT_APP` so `open_in_deckcraft` can start it. On a server without a GPU, the verified setup used `libxkbcommon0 libvulkan1 libegl1 mesa-vulkan-drivers libasound2 fontconfig`.

## How it works

| Part | What it is |
| --- | --- |
| **DeckCraft engine** (`deckcraft-cli mcp`) | DeckCraft's own engine: layouts, placeholders, text, shapes, pictures, charts, tables, themes, transitions, animations and the PPTX / PDF / PNG / outline writers. Started fresh and **headless** for each job, so it never touches the DeckCraft app or an open deck. |
| **MCP server** (Node.js) | 9 high-level tools. Builds decks from a list of slides: picks the layout, fills the placeholders, sets bullet levels, puts a picture, chart or table in the free content area (pictures kept in proportion), removes empty placeholders, turns text white on dark backgrounds, checks every output first and returns **pictures of the slides** to check them. |
| **Live app** (optional) | `open_in_deckcraft control=true` starts the app with its loopback-only control channel (port 7990) and `run_deckcraft_commands live=true` drives it. Close the app when you are done. |

## Tools

| Tool | What it does |
| --- | --- |
| `create_presentation` | A new deck from slides (title, subtitle, bullets with levels in one or two columns, picture, chart, table, shapes, text boxes, notes, background, transition, bullet animation) or from an outline; theme, colour and font schemes, 16:9 or 4:3, slide numbers, footer, properties |
| `edit_presentation` | One deck, a list or a folder: find and replace (titles, text, shapes, table cells, footers), theme, colour and font schemes, slides added at any position or deleted, notes, transitions, slide numbers and footer; written as a new copy |
| `convert_presentation` | One deck, a list or a folder → pptx, pdf (slides, notes pages, handouts 1-9 per page), deckcraft, png / jpeg per slide, outline |
| `get_presentation_info` | Slides with layouts, every shape (id, kind, box, text), tables, charts, notes, transitions and animations; theme, fonts, size; optional spelling and accessibility review |
| `render_slides` | Slides shown to Claude and optionally saved as PNG |
| `list_deckcraft_catalog` | 226 commands with parameters, themes and colour / font schemes, layouts, shape presets, transitions, animations, formats |
| `run_deckcraft_commands` | Any engine commands plus `add_slide`, `add_shape`, `insert_chart`, `inspect_slide`... in one session (`$steps[N].field` references), headless or live, then save |
| `open_in_deckcraft` | Open decks in the DeckCraft app, optionally with the control channel |
| `get_deckcraft_status` | Platform, installation, version, commands, themes, app / control port |

| | |
| --- | --- |
| **Opens** | PowerPoint .pptx (also .pptm, .potx), .deckcraft; places PNG, JPEG, GIF, BMP, WebP and SVG |
| **Saves** | pptx, pdf (slides, notes pages, handouts), deckcraft, png / jpeg per slide, text outline |

Coordinates are **points** on the slide (a 16:9 slide is 960 × 540 pt); a picture, chart or table without a box fills the free content area. Themes: DeckCraft, Harbor, Ember, Meadow, Nocturne, Paper, Coral Reef, Slate.

## Example

```json
{
  "name": "Q4 plan",
  "theme": "Ember",
  "slide_numbers": true,
  "footer": "ACME Inc.",
  "transition": "fade",
  "slides": [
    { "title": "Q4 plan", "subtitle": "Sales team · October" },
    { "title": "Goals", "bullets": ["Grow 12 %", { "text": "Colombia and Peru", "level": 1 }, "Cut costs 5 %"],
      "notes": "One minute per goal.", "animate_bullets": "fade" },
    { "title": "Sales by quarter", "bullets": ["Q3 was the best quarter"],
      "chart": { "type": "column", "categories": ["Q1", "Q2", "Q3"],
                 "series": [{ "name": "2025", "values": [9, 10, 11] }, { "name": "2026", "values": [10, 12, 15] }], "legend": "bottom" } },
    { "title": "Results by region", "table": { "rows": [["Region", "Sales", "Change"], ["North", "1,200", "+8 %"], ["South", "950", "+15 %"]] } },
    { "title": "Our team", "bullets": ["Design", "Engineering"], "image": { "path": "C:\\Pictures\\team.jpg" } },
    { "title": "Thank you", "layout": "sectionHeader", "subtitle": "Questions?", "background": "#1E2B3C" }
  ],
  "formats": ["pptx", "pdf"],
  "output_dir": "C:\\Decks"
}
```

## Requirements

- **DeckCraft** with `deckcraft-cli` (tested with **0.6.1**); see [Platforms](#platforms)
- Node.js ≥ 20 (bundled with Claude Desktop for `.mcpb` installs)

## Installation

### Claude Desktop (recommended, all platforms)

1. Download `deckcraft-mcp-server.mcpb` from the [latest release](https://github.com/jhonsu01/deckcraft-mcp-server/releases/latest).
2. Double-click it (or drag it into Claude Desktop → *Settings → Extensions*) and click **Install**.
3. Optional: if DeckCraft is not in a standard location, fill in its folder or the `deckcraft-cli` path in the extension settings.

### Sunsam Code

Install **DeckCraft Bridge** from the [Sunsam Code marketplace](https://github.com/jhonsu01/marketplace-SunsamCode), or drop the `.mcpb` into *MCP → Install extension*.

### Codex (OpenAI)

**Recommended — the marketplace (gets updates):** *Plugins → Add → Add marketplace*, source `jhonsu01/craft-marketplace`, reference `main`, then install **DeckCraft Bridge** from **Craft Bridges** ([craft-marketplace](https://github.com/jhonsu01/craft-marketplace)). New versions arrive by refreshing the marketplace. Or upload the zip (Codex then keeps it in your account and refuses a newer zip with the same name):

1. Download `deckcraft-mcp-server-<version>-codex.zip` from the [latest release](https://github.com/jhonsu01/deckcraft-mcp-server/releases/latest).
2. In Codex: *Plugins → Add → New plugin*, choose the zip and click **Add plugin**.
3. Codex starts the server with `node`, so Node.js ≥ 20 must be on `PATH`. If DeckCraft is not in a standard location, set `DECKCRAFT_DIR` or `DECKCRAFT_CLI` as system environment variables (Codex has no settings form for local plugins).

### DeepSeek Harness

1. *Plugins → Add plugin*, enter `github:jhonsu01/craft-marketplace#path:/plugins/deckcraft-mcp-server` and click **Install**, then **Enable now**.
2. Harness runs the server with its own MCP client and `node` (Node.js ≥ 20 on `PATH`); the tools appear as `mcp__deckcraft__<tool>` and the output files as cards that open in Harness.
3. Harness does not update plugins by itself yet: to upgrade, uninstall the plugin and install it again with the same address.

### Claude Code / other MCP clients

```bash
git clone https://github.com/jhonsu01/deckcraft-mcp-server.git
cd deckcraft-mcp-server
npm install
npm run build
```

Windows:

```bash
claude mcp add deckcraft -- node "%CD%\dist\bundle.cjs"
```

macOS / Linux:

```bash
claude mcp add deckcraft -- node "$PWD/dist/bundle.cjs"
```

## Configuration

| Variable | Meaning |
| --- | --- |
| `DECKCRAFT_DIR` | DeckCraft folder, one of its executables, a `.tar.gz` root (with `bin/`) or `DeckCraft.app`. Default: auto-detect |
| `DECKCRAFT_CLI` | Path of `deckcraft-cli` / `deckcraft-cli.exe` (wins over `DECKCRAFT_DIR`) |
| `DECKCRAFT_APP` | Path of the desktop app when it lives elsewhere (e.g. a Linux AppImage) |
| `DECKCRAFT_CONTROL_PORT` | Control port of the desktop app (default 7990) |
| `DECKCRAFT_MCP_TIMEOUT` | Maximum seconds per engine call (default 3600) |

## Safety

- Files are **never overwritten** unless `overwrite: true`: a free name (`_2`) is used in folders and an existing `output_path` is an error. Inputs are only read; an edited file is saved only as a new copy (`_edited`).
- All paths must be absolute. The engine runs headless and never touches the DeckCraft app unless `live: true`.
- Everything runs locally with no network access. Each job uses a private engine in a temporary folder that is deleted at the end.

## Development

```bash
npm run build       # TypeScript + single-file bundle (dist/bundle.cjs)
npm test            # unit tests (Windows, macOS and Linux path logic)
npm run test:e2e    # 28 end-to-end checks (30 with `E2E_LIVE=1`) over real MCP stdio (synthetic picture)
npm run pack:mcpb   # deckcraft-mcp-server.mcpb
npm run pack:codex  # Codex / DeepSeek Harness plugin zip
```

Linux test in Docker (unpack `deckcraft-<version>-linux-x86_64.tar.gz` first):

```bash
docker run --rm -v "$PWD:/work:ro" -v "/path/to/deckcraft-0.6.1-linux-x86_64:/opt/deckcraft:ro" -e DECKCRAFT_DIR=/opt/deckcraft -w /work node:22-bookworm bash -c "apt-get update && apt-get install -y libxkbcommon0 libvulkan1 libegl1 mesa-vulkan-drivers libasound2 fontconfig && node scripts/e2e.mjs"
```

## License

Apache-2.0. DeckCraft is © its authors (Storytold), MIT or Apache-2.0.
This project is not affiliated with or endorsed by DeckCraft or Storytold. PowerPoint is a trademark of Microsoft.
