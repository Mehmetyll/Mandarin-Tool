**🇺🇸 EN - JAR Analyzer** · [🇹🇷 TR - JAR Analizi](TR-JAR-Analizi)

# 🔬 JAR Analyzer


Inspects the contents of a JAR or ZIP file. Includes a built-in **CFR decompiler** to read `.class` files as Java source code.

---

## How to Open a JAR

- Click **Select JAR** and browse to a file
- **Drag & drop** a `.jar` file onto the tab
- **Right-click** a mod in Mod Analyze → "Analyze in JAR Analyzer"

---

## What You See

**Left side** — Table listing every entry in the archive (name, type, size).

**Right side** — Preview of the selected entry:
- `.class` files → decompiled Java source code
- Text files (`.json`, `.yml`, `.xml`, `.properties`, etc.) → raw content
- Binary files → not displayed

**Bottom bar** — Summary info: file size, hidden, extension changed, obfuscation level, total entries, class count, main class.

---

## Key Features

- **Obfuscation detection** — Uses entropy analysis on class names. High entropy = likely obfuscated.
- **Hidden entry detection** — Flags entries with zero-width Unicode chars, dot-prefixed paths, or RTL override tricks.
- **Extension check** — Detects if the file is disguised (e.g. a JAR renamed to `.png`).
- **Search** — Filter entries by name or type.
- **Right-click** — Copy entry name or preview content.
