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

插件会启动本地 Node.js 服务器，因此 `PATH` 中必须有 Node.js ≥ 20。如果某个应用不在标准文件夹中，请把它的变量（例如 `DESIGNCRAFT_DIR`）设为系统环境变量。

## 更新

每个连接器的新版本都会发布到这里。在 Codex 中刷新插件市场（或运行 `codex plugin marketplace upgrade craft`），插件就会更新。

```bash
codex plugin marketplace upgrade craft
```

## 为什么用插件市场

Codex 也可以上传 zip 形式的插件，但上传的插件会保存在你的账户中，同名的新版 zip 会被拒绝。插件市场是一个 Git 仓库：Codex 读取它、安装你选择的插件，并通过 **更新** 获取新版本。

## 其他软件

Claude Desktop 及其他支持 `.mcpb` 的软件：从各连接器的发布页安装 `.mcpb`，例如 [designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest)。

## 许可证

Apache-2.0。Craft 应用归其作者（Storytold）所有；这些插件与他们无关，也未获其认可。
