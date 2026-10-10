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

プラグインはローカルの Node.js サーバーを起動するため、`PATH` に Node.js ≥ 20 が必要です。アプリが標準のフォルダーにない場合は、その変数（例：`DESIGNCRAFT_DIR`）をシステムの環境変数として設定してください。

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
