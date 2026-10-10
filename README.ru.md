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
