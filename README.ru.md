<p align="center"><img src="plugins/designcraft-mcp-server/assets/icon.png" width="96" alt="Craft Bridges"></p>

<h1 align="center">Craft Bridges</h1>

<p align="center">
  <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.fr.md">Français</a> · <a href="README.de.md">Deutsch</a> · <b>Русский</b> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a>
</p>

<p align="center">Маркетплейс плагинов Codex для MCP-коннекторов Craft: мосты к установленным на вашем компьютере приложениям Craft с открытым исходным кодом (Windows, macOS, Linux).</p>

---

## Плагины

| Плагин | Что делает | Требуется |
| --- | --- | --- |
| **DesignCraft Bridge** (`designcraft-mcp-server`) | Вёрстка, слияние данных, IDML из InDesign, PDF/X для печати, PNG, EPUB и HTML | [DesignCraft](https://github.com/storytold/designcraft) + Node.js ≥ 20 |
| **EffectCraft Bridge** (`effectcraft-mcp-server`) | Моушн-графика, анимированные титры, эффекты для видео, шаблоны; MP4, ProRes, WebM, GIF, Lottie | [EffectCraft](https://github.com/storytold/effectcraft) + Node.js ≥ 20 |
| **LightCraft Bridge** (`lightcraft-mcp-server`) | Проявка raw: автотон, 114 ползунков, пресеты, маски, HDR и панорамы; JPEG, TIFF, WebP, AVIF, DNG | [LightCraft](https://github.com/storytold/lightcraft) + Node.js ≥ 20 |
| **PhotoCraft Bridge** (`photocraft-mcp-server`) | Обработка фото: размер, кадрирование, коррекция, 122 фильтра, удаление фона, текст и макеты; PSD, PNG, JPEG, WebP | [PhotoCraft](https://github.com/storytold/photocraft) + Node.js ≥ 20 |
| **VectorCraft Bridge** (`vectorcraft-mcp-server`) | Векторная графика: трассировка, макеты из фигур, текста и диаграмм, перекраска; SVG, PDF, AI, EPS, DXF, PNG | [VectorCraft](https://github.com/storytold/vectorcraft) + Node.js ≥ 20 |
| **PdfCraft Bridge** (`pdfcraft-mcp-server`) | PDF: объединение, разделение, страницы, OCR, формы, подписи, скрытие, пароли; в Word, HTML, изображения, PDF/A | [PdfCraft](https://github.com/storytold/pdfcraft) + Node.js ≥ 20 |
| **FilmCraft Bridge** (`filmcraft-mcp-server`) | Видеомонтаж: нарезка, обрезка, эффекты, цветокоррекция, титры, скорость, склейка с переходами; H.264, ProRes, GIF, OTIO | [FilmCraft](https://github.com/storytold/filmcraft) + Node.js ≥ 20 |

## Установка в Codex

1. *Плагины → Добавить → Добавить маркетплейс*.
2. **Источник:** `jhonsu01/craft-marketplace` · **Ссылка Git:** `main` · *разреженные пути* оставьте пустыми.
3. Нажмите **Добавить маркетплейс**, откройте маркетплейс **Craft Bridges** и установите **DesignCraft Bridge**.

Из командной строки:

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

Плагины запускают локальный сервер Node.js, поэтому Node.js ≥ 20 должен быть в `PATH`. Если приложение установлено не в стандартную папку, задайте его переменную (например, `DESIGNCRAFT_DIR`) как системную переменную окружения.

## Обновления

Каждая новая версия коннектора публикуется здесь. В Codex обновите маркетплейс (или выполните `codex plugin marketplace upgrade craft`), и плагин обновится.

```bash
codex plugin marketplace upgrade craft
```

## Зачем маркетплейс

Codex принимает плагин и в виде загруженного zip, но такой плагин сохраняется в вашей учётной записи, и более новый zip с тем же именем отклоняется. Маркетплейс — это Git-репозиторий: Codex читает его, устанавливает выбранные плагины и получает новые версии по кнопке **Обновить**.

## Другие программы

Claude Desktop и другие программы с поддержкой `.mcpb`: установите `.mcpb` из релизов нужного коннектора, например [designcraft-mcp-server](https://github.com/jhonsu01/designcraft-mcp-server/releases/latest).

## Лицензия

Apache-2.0. Приложения Craft принадлежат их авторам (Storytold); эти плагины не связаны с ними и не одобрены ими.
