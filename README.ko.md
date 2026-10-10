<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.fr.md">Français</a> · <a href="README.de.md">Deutsch</a> · <a href="README.ru.md">Русский</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a> · <b>한국어</b>
</p>

<p align="center">Craft MCP 커넥터용 Codex 플러그인 마켓플레이스: 컴퓨터에 설치된 오픈 소스 Craft 앱과 연결합니다(Windows, macOS, Linux).</p>

---

## 플러그인

| 플러그인 | 기능 | 필요 |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | 페이지 레이아웃, 데이터 병합, InDesign IDML, 인쇄용 PDF/X, PNG, EPUB, HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |

## Codex에 설치

1. *플러그인 → 추가 → 마켓플레이스 추가*를 엽니다.
2. **소스:** `jhonsu01/craft-marketplace` · **Git 참조:** `main` · *스파스 경로*는 비워 둡니다.
3. **마켓플레이스 추가**를 누르고 **Craft Bridges** 마켓플레이스를 열어 **DesignCraft Bridge**를 설치합니다.

명령줄에서:

```bash
codex plugin marketplace add jhonsu01/craft-marketplace
```

```bash
codex plugin add designcraft-mcp-server@craft
```

플러그인은 로컬 Node.js 서버를 시작하므로 `PATH`에 Node.js ≥ 20이 있어야 합니다. 앱이 표준 폴더에 없다면 해당 변수(예: `DESIGNCRAFT_DIR`)를 시스템 환경 변수로 설정하세요.

## 업데이트

각 커넥터의 새 버전은 여기에 게시됩니다. Codex에서 마켓플레이스를 새로 고치면(또는 `codex plugin marketplace upgrade craft` 실행) 플러그인이 업데이트됩니다.

```bash
codex plugin marketplace upgrade craft
```

## 마켓플레이스를 쓰는 이유

Codex는 zip으로 업로드한 플러그인도 받지만, 업로드한 플러그인은 계정에 저장되고 같은 이름의 새 zip은 거부됩니다. 마켓플레이스는 Git 저장소입니다. Codex가 이를 읽어 원하는 플러그인을 설치하고, **업데이트**로 새 버전을 받습니다.

## 다른 프로그램

Claude Desktop 등 `.mcpb`를 지원하는 프로그램: 각 커넥터의 릴리스에서 `.mcpb`를 설치하세요. 예: [designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest).

## 라이선스

Apache-2.0. Craft 앱의 권리는 저작자(Storytold)에게 있으며, 이 플러그인들은 그들과 관련이 없고 보증을 받지 않았습니다.
