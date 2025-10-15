# 📝 Notetab

**Notetab** is a lightweight, self-contained Markdown editor and viewer built entirely in a single HTML file.
It combines the **Monaco Editor** (used by VS Code) with **Marked**, **Highlight.js**, and **DOMPurify** to provide a fast, secure, and elegant note-taking environment — all running locally in your browser.

---

## 🚀 Features

- ✍️ **Rich Markdown editing** with syntax highlighting (Monaco)
- 🪄 **Markdown preview** with code highlighting (Marked + Highlight.js)
- 💾 **Auto-save to localStorage** — your notes persist automatically
  - Each note is stored in your browser's localStorage under a key based on the URL query
    - For example: `notetab.html?project-ideas` will store the note under the key `project-ideas`
  - If no query string is given, the default key is `notetab`
- ⌨️ **Keyboard shortcuts**:
  - `Ctrl/Cmd + Shift + E` — Toggle between **edit** and **preview** modes
  - `Ctrl/Cmd + S` — Save current note as a `.md` file
  - `Ctrl/Cmd + K` then `Ctrl/Cmd + K` — Wrap selection in Markdown link syntax
- 🖱️ **Click to toggle** via floating pencil icon
- 🔒 **Secure rendering** using DOMPurify (prevents XSS)
- 🧩 **Standalone file** — no build step, no server required
