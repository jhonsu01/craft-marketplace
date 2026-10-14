<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <b>Português</b> · <a href="README.fr.md">Français</a> · <a href="README.de.md">Deutsch</a> · <a href="README.ru.md">Русский</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">Marketplace de plugins do Codex para os conectores MCP Craft: pontes para os apps Craft de código aberto instalados no seu computador (Windows, macOS, Linux).</p>

---

## Plugins

| Plugin | O que faz | Requer |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | Diagramação, mala direta, IDML do InDesign, PDF/X para gráfica, PNG, EPUB e HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | Motion graphics, títulos animados, efeitos em vídeos, modelos; MP4, ProRes, WebM, GIF, Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | Revelação raw: tom automático, 114 controles, predefinições, máscaras, HDR e panoramas; JPEG, TIFF, WebP, AVIF, DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | Edição de fotos: tamanho, recorte, ajustes, 122 filtros, remoção de fundo, texto e designs; PSD, PNG, JPEG, WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | Arte vetorial: vetorizar imagens, designs com formas, texto e gráficos, recolorir; SVG, PDF, AI, EPS, DXF, PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF: juntar, dividir, páginas, OCR, formulários, assinaturas, tarjas, senhas; para Word, HTML, imagens, PDF/A | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | Edição de vídeo: dividir, cortar, efeitos, looks de cor, títulos, velocidade, juntar com transições; H.264, ProRes, GIF, OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |

## Instalar no Codex

1. *Plugins → Adicionar → Adicionar marketplace*.
2. **Origem:** `jhonsu01/craft-marketplace` · **Referência Git:** `main` · deixe *caminhos esparsos* vazio.
3. Clique em **Adicionar marketplace**, abra o marketplace **Craft Bridges** e instale o **DesignCraft Bridge**.

Pela linha de comando:

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

Os plugins iniciam um servidor local Node.js, então o Node.js ≥ 20 precisa estar no `PATH`. Se um app não estiver na pasta padrão, defina a variável dele (ex.: `DESIGNCRAFT_DIR`) como variável de ambiente do sistema.

## DeepSeek Harness

Cada pasta de plugin também é um bundle do DeepSeek Harness. Em *Plugins → Add plugin* digite o endereço de um plugin e clique em **Install** e **Enable now**:

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

O Harness ainda não atualiza plugins sozinho: para atualizar, desinstale e instale de novo.

## Atualizações

Cada nova versão de um conector é publicada aqui. No Codex, atualize o marketplace (ou execute `codex plugin marketplace upgrade craft`) e o plugin é atualizado.

```bash
codex plugin marketplace upgrade craft
```

## Por que um marketplace

O Codex também aceita um plugin enviado como zip, mas ele fica salvo na sua conta e um zip mais novo com o mesmo nome é recusado. Um marketplace é um repositório Git: o Codex o lê, instala os plugins que você escolher e obtém as novas versões com **Atualizar**.

## Outros programas

Claude Desktop, SunsamCode e outros programas `.mcpb`: baixe o `.mcpb` da versão mais recente de cada conector e dê um clique duplo:

- **DesignCraft Bridge**: [designcraft-mcp-server.mcpb](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest/download/designcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/designcraft-mcp-server)
- **EffectCraft Bridge**: [effectcraft-mcp-server.mcpb](https://github.com/jhonsu01/effectcraft-mcp-server/releases/latest/download/effectcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/effectcraft-mcp-server)
- **LightCraft Bridge**: [lightcraft-mcp-server.mcpb](https://github.com/jhonsu01/lightcraft-mcp-server/releases/latest/download/lightcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/lightcraft-mcp-server)
- **PhotoCraft Bridge**: [photocraft-mcp-server.mcpb](https://github.com/jhonsu01/photocraft-mcp-server/releases/latest/download/photocraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/photocraft-mcp-server)
- **VectorCraft Bridge**: [vectorcraft-mcp-server.mcpb](https://github.com/jhonsu01/vectorcraft-mcp-server/releases/latest/download/vectorcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/vectorcraft-mcp-server)
- **PdfCraft Bridge**: [pdfcraft-mcp-server.mcpb](https://github.com/jhonsu01/pdfcraft-mcp-server/releases/latest/download/pdfcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/pdfcraft-mcp-server)
- **FilmCraft Bridge**: [filmcraft-mcp-server.mcpb](https://github.com/jhonsu01/filmcraft-mcp-server/releases/latest/download/filmcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/filmcraft-mcp-server)

## Licença

Apache-2.0. Os apps Craft pertencem aos seus autores (Storytold); estes plugins não são afiliados nem endossados por eles.
