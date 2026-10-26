<div align="center">

# 📝 MD Studio Pro
### *The Zero-Backend, Privacy-First Markdown Publishing Suite*

A fast, lightweight, and modern desktop-grade Markdown editor with live KaTeX mathematical notation, Mermaid flowcharts, executive styling themes, and multi-format publishing to **Vector PDF**, **Microsoft Word (.docx)**, and **Standalone HTML**.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Zero Backend](https://img.shields.io/badge/Architecture-Zero--Backend-00F5D4?style=for-the-badge&logo=shield)](https://github.com/cyb3rdr4g0n17)
[![Pure Vanilla](https://img.shields.io/badge/Stack-HTML5%20%7C%20CSS3%20%7C%20JS-f7df1e?style=for-the-badge&logo=javascript&logoColor=black)](https://github.com/cyb3rdr4g0n17)
[![Deploy on GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-22c55e?style=for-the-badge&logo=github)](https://github.com/cyb3rdr4g0n17/md-studio)

[🚀 Live Demo](https://cyb3rdr4g0n17.github.io/md-studio/) • [✨ Features](#-features) • [⌨️ Keyboard Shortcuts](#-keyboard-shortcuts) • [🚀 Quick Start](#-quick-start) • [📄 Export Matrix](#-export-format-matrix)

---

</div>

## 🛡️ Why MD Studio Pro?

Most modern Markdown editors either lock you into cloud subscriptions, send your sensitive notes to remote servers, or produce blurry, rasterized PDF screenshots that ruin code blocks and formulas.

**MD Studio Pro is built differently:**
* **100% Client-Side:** Everything compiles inside your browser via Web APIs. Zero telemetry, zero external APIs, zero servers.
* **Vector-Grade PDF Output:** Generates razor-sharp, searchable vector PDFs of any length with real text, page break control, and zero canvas memory crashes.
* **Native Word (.docx) Compilation:** Bundles OpenXML `.docx` files complete with running headers, footers, page numbering, and custom A4/Letter margins.
* **Zero Installation:** A single standalone `index.html` file that runs instantly in Chrome, Firefox, Edge, Safari, or offline from a flash drive.

---

## ✨ Features

### 📐 Scientific & Technical Writing
* **LaTeX Formula Typesetting:** Fast, crisp mathematical typesetting powered by KaTeX 0.16 (`$...$` for inline and `$$...$$` for display equations).
* **Flowcharts & Diagrams:** Render Mermaid.js diagrams directly within code blocks (flowcharts, sequence diagrams, class trees, state machines).
* **Code Syntax Highlighting:** Multi-language syntax highlighting with Prism.js (Python, JavaScript, Bash, JSON, etc.).
* **GitHub-Style Callouts:** Automatically converts `> [!NOTE]`, `> [!TIP]`, `> [!IMPORTANT]`, `> [!WARNING]`, and `> [!CAUTION]` into responsive admonition cards.

### 📄 Document Styling & Paper Presets
* **Curated Themes:** Instant toggle between **Modern Sans** (Plus Jakarta Sans), **Classic Serif** (Lora), **Academic Formal** (Merriweather), and **Clean Slate**.
* **Page Formatting:** Support for standard **A4** and **US Letter** page dimensions with real-time approximate page count indicators.
* **Running Headers & Footers:** Customize left, center, and right text with dynamic page numbering macros (`{n}` and `{N}`) and cover page suppression.
* **Custom Color System:** Tweak primary accents, headings, body text, and link colors in real time.

### ⚡ Editorial Workflow & Productive Tooling
* **Clipboard & Drag-and-Drop Image Embedding:** Paste screenshots or drop images straight into the editor. MD Studio automatically compresses and embeds them as clean Base64 data URIs.
* **Smart Typography:** One-click conversion for curly quotes, em-dashes, en-dashes, and ellipses.
* **Automated Table of Contents:** Scans headings and builds an indented, anchor-linked TOC with a single click.
* **Split, Editor-Only & Preview-Only Views:** Toggle effortlessly between writing and full-page reading layouts.
* **Synchronized Dual-Pane Scrolling:** Seamless scroll matching between raw source and styled paper output.

---

## 📄 Export Format Matrix

| Format | Extension | Engine / Method | Best For |
|:---|:---:|:---|:---|
| **Vector PDF** | `.pdf` | Browser Native Vector Engine (`Ctrl + P`) | **Formal publication**, infinite-length documents, crystal-clear searchable text & vector diagrams. |
| **Direct PDF** | `.pdf` | `html2pdf.js` (Canvas + jsPDF) | Quick one-click automated downloads with custom page numbers for short documents. |
| **Word Document** | `.docx` | `html-docx-js` + `JSZip` (OpenXML) | Sharing with colleagues, submitting academic coursework, or further editing in Microsoft Office / LibreOffice. |
| **Standalone HTML** | `.html` | Self-contained HTML with embedded styles | Clean web publishing, email newsletters, or sharing as an interactive standalone report. |
| **Markdown Source** | `.md` | Raw UTF-8 text with local storage auto-save | Archiving, Git version control, Obsidian, Notion, or GitHub wikis. |

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|:---|:---|
| `Ctrl + S` / `Cmd + S` | **Save locally** (updates browser state and notifies status) |
| `Ctrl + P` / `Cmd + P` | **Save as Vector PDF** (launches clean print-to-PDF view) |
| `Ctrl + B` / `Cmd + B` | Bold text (`**text**`) |
| `Ctrl + I` / `Cmd + I` | Italic text (`*text*`) |
| `Ctrl + K` / `Cmd + K` | Insert Markdown link (`[text](url)`) |
| `Ctrl + M` / `Cmd + M` | Insert KaTeX LaTeX math block |
| `Tab` | Indent 2 spaces |
| `Shift + Tab` | Un-indent 2 spaces |

---

## 🚀 Quick Start

### 1. Run Locally (No Build Tools Required)
No `npm install`, no `node_modules`, no setup:
1. Clone this repository:
   ```bash
   git clone https://github.com/cyb3rdr4g0n17/md-studio.git
   cd md-studio
   ```
2. Double-click `index.html` to open it in any modern browser.

Or serve with any static web server:
```bash
# Python 3
python -m http.server 8080

# Or npx
npx serve .
```

### 2. Deploy to GitHub Pages in 30 Seconds
1. Push this repository to GitHub.
2. In your repository, go to **Settings > Pages**.
3. Under **Build and deployment > Branch**, select `main` (or `master`) and folder `/ (root)`.
4. Click **Save**. Your studio will be live at `https://<username>.github.io/<repo-name>/`.

---

## 🧩 Libraries & Dependencies

MD Studio Pro utilizes high-performance open-source libraries via reliable CDN mirrors:

* [Marked.js](https://marked.js.org/) — High-speed GFM Markdown parsing
* [DOMPurify](https://github.com/cure53/DOMPurify) — XSS sanitization
* [KaTeX](https://katex.org/) — Fast LaTeX mathematical typesetting
* [Mermaid.js](https://mermaid.js.org/) — Diagram and flowchart generation
* [Prism.js](https://prismjs.com/) — Syntax highlighting
* [html-docx-js](https://github.com/evidenceprime/html-docx-js) & [JSZip](https://stuk.github.io/jszip/) — Client-side Microsoft Word OpenXML generation
* [html2pdf.js](https://ekoopmans.github.io/html2pdf.js/) — Client-side PDF generation

---

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

---

<div align="center">
  <sub>Crafted with precision by <b><a href="https://github.com/cyb3rdr4g0n17">Rahul Singh (cyb3rdr4g0n17)</a></b></sub>
</div>
