<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.fr.md">Français</a> · <a href="README.de.md">Deutsch</a> · <a href="README.ru.md">Русский</a> · <b>简体中文</b> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">Craft MCP 连接器的 Codex 插件市场：连接你电脑上安装的开源 Craft 应用（Windows、macOS、Linux）。</p>

---

## 插件

| 插件 | 功能 | 需要 |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | 排版、数据合并、InDesign IDML、印刷用 PDF/X、PNG、EPUB 和 HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | 动态图形、动画标题、视频特效、模板；MP4、ProRes、WebM、GIF、Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | RAW 冲洗：自动色调、114 个滑块、预设、蒙版、HDR 与全景；JPEG、TIFF、WebP、AVIF、DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | 照片编辑：尺寸、裁剪、调整、122 种滤镜、去除背景、文字与设计；PSD、PNG、JPEG、WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | 矢量图形：图像描摹、用形状、文字和图表设计、重新着色；SVG、PDF、AI、EPS、DXF、PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF：合并、拆分、页面、OCR、表单、签名、涂黑、密码；转 Word、HTML、图片、PDF/A | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | 视频剪辑：分割、修剪、特效、调色、标题、变速、带转场拼接；H.264、ProRes、GIF、OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |
| **WordCraft Bridge** (`wordcraft-mcp-server`) | 文字处理：由标题、列表、表格和图片组成的文档，查找 / 替换、批注、修订、邮件合并；DOCX、PDF、ODT、RTF、Markdown、LaTeX | [WordCraft](https://github.com/storytold/wordcraft) + Node.js ≥ 20 |
| **SoundCraft Bridge** (`soundcraft-mcp-server`) | 音乐与音频：用音频文件和合成器或鼓的音符制作多轨歌曲，效果、总线，带 LUFS 的混音、分轨、MIDI、音频处理；WAV、AIFF、FLAC | [SoundCraft](https://github.com/storytold/soundcraft) + Node.js ≥ 20 |
| **DeckCraft Bridge** (`deckcraft-mcp-server`) | 演示文稿：带项目符号、图片、图表、表格和备注的幻灯片，主题、切换、查找替换；PowerPoint pptx、pdf、图片 | [DeckCraft](https://github.com/storytold/deckcraft) + Node.js ≥ 20 |
| **GridCraft Bridge** (`gridcraft-mcp-server`) | 电子表格：带实时公式的工作表、表格、格式、条件格式、图表和数据透视表，计算结果；xlsx、csv、json、html、pdf | [GridCraft](https://github.com/storytold/gridcraft) + Node.js ≥ 20 |

## 在 Codex 中安装

1. *插件 → 添加 → 添加插件市场*。
2. **来源：** `jhonsu01/craft-marketplace` · **Git 引用：** `main` · *稀疏路径* 留空。
3. 点击 **添加插件市场**，打开 **Craft Bridges** 插件市场并安装 **DesignCraft Bridge**。

命令行方式：

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

```bash
codex plugin add soundcraft-mcp-server@craft
```

```bash
codex plugin add deckcraft-mcp-server@craft
```

```bash
codex plugin add gridcraft-mcp-server@craft
```

插件会启动本地 Node.js 服务器，因此 `PATH` 中必须有 Node.js ≥ 20。如果某个应用不在标准文件夹中，请把它的变量（例如 `DESIGNCRAFT_DIR`）设为系统环境变量。

## DeepSeek Harness

每个插件文件夹同时也是 DeepSeek Harness 的 bundle。在 *Plugins → Add plugin* 中输入某个插件的地址，点击 **Install** 和 **Enable now**：

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

```text
github:jhonsu01/craft-marketplace#path:/plugins/soundcraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/deckcraft-mcp-server
```

```text
github:jhonsu01/craft-marketplace#path:/plugins/gridcraft-mcp-server
```

Harness 目前不会自动更新插件：要更新，请卸载后重新安装。

## 更新

每个连接器的新版本都会发布到这里。在 Codex 中刷新插件市场（或运行 `codex plugin marketplace upgrade craft`），插件就会更新。

```bash
codex plugin marketplace upgrade craft
```

## 为什么用插件市场

Codex 也可以上传 zip 形式的插件，但上传的插件会保存在你的账户中，同名的新版 zip 会被拒绝。插件市场是一个 Git 仓库：Codex 读取它、安装你选择的插件，并通过 **更新** 获取新版本。

## 其他软件

Claude Desktop、SunsamCode 及其他支持 `.mcpb` 的软件：从各连接器的最新发布下载 `.mcpb` 并双击安装：

- **DesignCraft Bridge**: [designcraft-mcp-server.mcpb](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest/download/designcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/designcraft-mcp-server)
- **EffectCraft Bridge**: [effectcraft-mcp-server.mcpb](https://github.com/jhonsu01/effectcraft-mcp-server/releases/latest/download/effectcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/effectcraft-mcp-server)
- **LightCraft Bridge**: [lightcraft-mcp-server.mcpb](https://github.com/jhonsu01/lightcraft-mcp-server/releases/latest/download/lightcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/lightcraft-mcp-server)
- **PhotoCraft Bridge**: [photocraft-mcp-server.mcpb](https://github.com/jhonsu01/photocraft-mcp-server/releases/latest/download/photocraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/photocraft-mcp-server)
- **VectorCraft Bridge**: [vectorcraft-mcp-server.mcpb](https://github.com/jhonsu01/vectorcraft-mcp-server/releases/latest/download/vectorcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/vectorcraft-mcp-server)
- **PdfCraft Bridge**: [pdfcraft-mcp-server.mcpb](https://github.com/jhonsu01/pdfcraft-mcp-server/releases/latest/download/pdfcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/pdfcraft-mcp-server)
- **FilmCraft Bridge**: [filmcraft-mcp-server.mcpb](https://github.com/jhonsu01/filmcraft-mcp-server/releases/latest/download/filmcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/filmcraft-mcp-server)
- **WordCraft Bridge**: [wordcraft-mcp-server.mcpb](https://github.com/jhonsu01/wordcraft-mcp-server/releases/latest/download/wordcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/wordcraft-mcp-server)
- **SoundCraft Bridge**: [soundcraft-mcp-server.mcpb](https://github.com/jhonsu01/soundcraft-mcp-server/releases/latest/download/soundcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/soundcraft-mcp-server)
- **DeckCraft Bridge**: [deckcraft-mcp-server.mcpb](https://github.com/jhonsu01/deckcraft-mcp-server/releases/latest/download/deckcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/deckcraft-mcp-server)
- **GridCraft Bridge**: [gridcraft-mcp-server.mcpb](https://github.com/jhonsu01/gridcraft-mcp-server/releases/latest/download/gridcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/gridcraft-mcp-server)

## 许可证

Apache-2.0。Craft 应用归其作者（Storytold）所有；这些插件与他们无关，也未获其认可。
