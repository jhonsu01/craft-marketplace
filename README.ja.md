<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.fr.md">Français</a> · <a href="README.de.md">Deutsch</a> · <a href="README.ru.md">Русский</a> · <a href="README.zh-CN.md">简体中文</a> · <b>日本語</b> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">Craft MCP コネクター用の Codex プラグインマーケットプレイス。お使いのコンピューターにインストールされたオープンソースの Craft アプリにつなぎます（Windows、macOS、Linux）。</p>

---

## プラグイン

| プラグイン | 機能 | 必要なもの |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | ページレイアウト、データ結合、InDesign の IDML、入稿用 PDF/X、PNG、EPUB、HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | モーショングラフィックス、アニメーションタイトル、動画エフェクト、テンプレート。MP4、ProRes、WebM、GIF、Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | RAW 現像：自動トーン、114 のスライダー、プリセット、マスク、HDR とパノラマ。JPEG、TIFF、WebP、AVIF、DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | 写真編集：サイズ変更、切り抜き、補正、122 種のフィルター、背景除去、テキストとデザイン。PSD、PNG、JPEG、WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | ベクターアート：画像トレース、図形・テキスト・グラフでのデザイン、再配色。SVG、PDF、AI、EPS、DXF、PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF：結合、分割、ページ操作、OCR、フォーム、署名、墨消し、パスワード。Word、HTML、画像、PDF/A へ変換 | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | 動画編集：分割、トリム、エフェクト、カラールック、タイトル、速度、トランジション付き結合。H.264、ProRes、GIF、OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |

## Codex へのインストール

1. *プラグイン → 追加 → マーケットプレイスを追加* を開きます。
2. **ソース：** `jhonsu01/craft-marketplace` · **Git 参照：** `main` · *スパースパス* は空のままにします。
3. **マーケットプレイスを追加** をクリックし、**Craft Bridges** マーケットプレイスを開いて **DesignCraft Bridge** をインストールします。

コマンドラインから：

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

プラグインはローカルの Node.js サーバーを起動するため、`PATH` に Node.js ≥ 20 が必要です。アプリが標準のフォルダーにない場合は、その変数（例：`DESIGNCRAFT_DIR`）をシステムの環境変数として設定してください。

## DeepSeek Harness

各プラグインのフォルダーは DeepSeek Harness のバンドルでもあります。*Plugins → Add plugin* でプラグインのアドレスを入力し、**Install** と **Enable now** をクリックします：

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

Harness はまだプラグインを自動更新しません。更新するにはアンインストールして再インストールしてください。

## 更新

各コネクターの新しいバージョンはここで公開されます。Codex でマーケットプレイスを更新する（または `codex plugin marketplace upgrade craft` を実行する）と、プラグインが更新されます。

```bash
codex plugin marketplace upgrade craft
```

## マーケットプレイスを使う理由

Codex は zip をアップロードしてプラグインを追加することもできますが、アップロードしたプラグインはアカウントに保存され、同じ名前の新しい zip は拒否されます。マーケットプレイスは Git リポジトリです。Codex はそれを読み込み、選んだプラグインをインストールし、**更新** で新しいバージョンを取得します。

## その他のアプリ

Claude Desktop など `.mcpb` に対応したアプリ：各コネクターのリリースから `.mcpb` をインストールしてください。例：[designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest)。

## ライセンス

Apache-2.0。Craft アプリの権利はその作者（Storytold）にあります。これらのプラグインは作者とは無関係であり、承認も受けていません。
