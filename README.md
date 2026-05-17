# BinaryKit

Одностраничный инструментарий для анализа бинарных файлов. Работает полностью в браузере — никакого сервера.

**[Открыть BinaryKit](https://ihowi2.github.io/TestSite/BinaryKit.html)**

## Возможности

- **File Inspector** — определение формата по magic bytes, энтропия Шеннона с графиком, извлечение ASCII-строк
- **Hex Viewer** — виртуальный скролл для файлов любого размера, поиск hex-паттернов
- **Disassembler** — дизассемблер на базе Capstone.js (x86, ARM, ARM64, MIPS)
- **WASM Tools** — декомпиляция WebAssembly через wabt.js (WAT / C-like / метаданные)
- **PE / ELF Analyzer** — парсинг заголовков, секций, импортов и экспортов
- **Converter** — Base64, hex, byte arrays (C/Python/JS/Rust), числовые и строковые конвертеры
- **Hash & Compress** — SHA-1/256/512, MD5, gzip/deflate
- **AI Agent** — интеграция с Fireworks API (DeepSeek V4 Pro) для анализа бинарных файлов

## Запуск локально

```bash
python3 -m http.server 8080
# Открыть http://localhost:8080/BinaryKit.html
```

## Технологии

- Capstone.js (lazy load)
- wabt.js (lazy load)
- pe-exe-parser
- SubtleCrypto + CompressionStream API
- Fireworks AI API (SSE streaming)
