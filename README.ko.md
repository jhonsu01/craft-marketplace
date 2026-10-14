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
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | 모션 그래픽, 애니메이션 타이틀, 영상 효과, 템플릿; MP4, ProRes, WebM, GIF, Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | RAW 현상: 자동 톤, 114개 슬라이더, 프리셋, 마스크, HDR과 파노라마; JPEG, TIFF, WebP, AVIF, DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | 사진 편집: 크기, 자르기, 보정, 122개 필터, 배경 제거, 텍스트와 디자인; PSD, PNG, JPEG, WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | 벡터 아트: 이미지 추적, 도형·텍스트·차트로 디자인, 색 변경; SVG, PDF, AI, EPS, DXF, PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF: 병합, 분할, 페이지, OCR, 양식, 서명, 가리기, 암호; Word, HTML, 이미지, PDF/A로 변환 | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | 영상 편집: 분할, 트림, 효과, 색 보정, 타이틀, 속도, 전환 효과로 이어 붙이기; H.264, ProRes, GIF, OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |
| **WordCraft Bridge** (`wordcraft-mcp-server`) | 워드 프로세서: 제목, 목록, 표, 이미지로 문서 작성, 찾기 / 바꾸기, 메모, 변경 내용 추적, 편지 병합; DOCX, PDF, ODT, RTF, Markdown, LaTeX | [WordCraft](https://github.com/storytold/wordcraft) + Node.js ≥ 20 |

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

플러그인은 로컬 Node.js 서버를 시작하므로 `PATH`에 Node.js ≥ 20이 있어야 합니다. 앱이 표준 폴더에 없다면 해당 변수(예: `DESIGNCRAFT_DIR`)를 시스템 환경 변수로 설정하세요.

## DeepSeek Harness

각 플러그인 폴더는 DeepSeek Harness 번들이기도 합니다. *Plugins → Add plugin*에서 플러그인 주소를 입력하고 **Install**과 **Enable now**를 누르세요:

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

Harness는 아직 플러그인을 자동 업데이트하지 않습니다. 업데이트하려면 제거 후 다시 설치하세요.

## 업데이트

각 커넥터의 새 버전은 여기에 게시됩니다. Codex에서 마켓플레이스를 새로 고치면(또는 `codex plugin marketplace upgrade craft` 실행) 플러그인이 업데이트됩니다.

```bash
codex plugin marketplace upgrade craft
```

## 마켓플레이스를 쓰는 이유

Codex는 zip으로 업로드한 플러그인도 받지만, 업로드한 플러그인은 계정에 저장되고 같은 이름의 새 zip은 거부됩니다. 마켓플레이스는 Git 저장소입니다. Codex가 이를 읽어 원하는 플러그인을 설치하고, **업데이트**로 새 버전을 받습니다.

## 다른 프로그램

Claude Desktop, SunsamCode 등 `.mcpb`를 지원하는 프로그램: 각 커넥터의 최신 릴리스에서 `.mcpb`를 내려받아 두 번 클릭하세요:

- **DesignCraft Bridge**: [designcraft-mcp-server.mcpb](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest/download/designcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/designcraft-mcp-server)
- **EffectCraft Bridge**: [effectcraft-mcp-server.mcpb](https://github.com/jhonsu01/effectcraft-mcp-server/releases/latest/download/effectcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/effectcraft-mcp-server)
- **LightCraft Bridge**: [lightcraft-mcp-server.mcpb](https://github.com/jhonsu01/lightcraft-mcp-server/releases/latest/download/lightcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/lightcraft-mcp-server)
- **PhotoCraft Bridge**: [photocraft-mcp-server.mcpb](https://github.com/jhonsu01/photocraft-mcp-server/releases/latest/download/photocraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/photocraft-mcp-server)
- **VectorCraft Bridge**: [vectorcraft-mcp-server.mcpb](https://github.com/jhonsu01/vectorcraft-mcp-server/releases/latest/download/vectorcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/vectorcraft-mcp-server)
- **PdfCraft Bridge**: [pdfcraft-mcp-server.mcpb](https://github.com/jhonsu01/pdfcraft-mcp-server/releases/latest/download/pdfcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/pdfcraft-mcp-server)
- **FilmCraft Bridge**: [filmcraft-mcp-server.mcpb](https://github.com/jhonsu01/filmcraft-mcp-server/releases/latest/download/filmcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/filmcraft-mcp-server)
- **WordCraft Bridge**: [wordcraft-mcp-server.mcpb](https://github.com/jhonsu01/wordcraft-mcp-server/releases/latest/download/wordcraft-mcp-server.mcpb) · [repo](https://github.com/jhonsu01/wordcraft-mcp-server)

## 라이선스

Apache-2.0. Craft 앱의 권리는 저작자(Storytold)에게 있으며, 이 플러그인들은 그들과 관련이 없고 보증을 받지 않았습니다.
