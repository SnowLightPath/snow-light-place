# ✨ snow-light-place

> A plugin marketplace for [Claude Cowork](https://claude.com/product/cowork) and [Claude Code](https://code.claude.com/).

---

## 🎯 What is this?

A curated collection of plugins that extend Claude with specialized workflows. Install plugins from this marketplace to add new capabilities to your Claude sessions.

---

## 📦 Available Plugins

| Plugin | Description |
|--------|-------------|
| 📄 **[scribe](./scribe/)** | Document writing workflow: draft outlines, write in parallel, export to any format |

### Scribe — Supported Formats

| Format | Extension | Tool Chain |
|--------|-----------|------------|
| Markdown | `.md` | Direct write |
| PDF | `.pdf` | pandoc + xelatex |
| Word | `.docx` | pandoc |
| HTML | `.html` | pandoc |
| Excel | `.xlsx` | Python + openpyxl |
| PowerPoint | `.pptx` | Python + python-pptx |
| Pencil Design | `.pen` | Pencil MCP |
| Confluence | `--confluence` | Atlassian MCP |

---

## 🚀 Installation

### Claude Code (CLI)

```bash
# Add marketplace
claude plugin marketplace add SnowLightPath/snow-light-place

# Install plugin
claude plugin install scribe@snow-light-place
```

### Claude Cowork (Web)

Install directly from `claude.com/plugins/` or search for **scribe** in the plugin browser.

---

## 🔄 The Scribe Loop

```
  /scribe:draft          Design the outline
       ↓
  scribe.md         ←→   Document structure
       ↓
  /scribe:realize        Write & export
       ↓
  report.pdf             Output file
       ↓
  /scribe:reflect        Review & improve
       ↓
  (iterate)
```

| Command | Action |
|---------|--------|
| 📝 `/scribe:draft` | Design document outline, audience, format |
| ⚡ `/scribe:realize` | Write and export the document |
| 🪞 `/scribe:reflect` | Review quality and improve |

> Parallel section writing with [Agent Teams](https://code.claude.com/docs/en/agent-teams). Documents with 2+ sections are written concurrently.

---

## 🏗️ Origin

This marketplace distributes plugins from the [DDL (Design-Doc Loop)](https://github.com/SnowLightPath/DDL) project. The canonical source for the Scribe plugin is [`DDL/examples/scribe-plugin/`](https://github.com/SnowLightPath/DDL/tree/main/examples/scribe-plugin).

---

## 📄 License

[Apache-2.0](./LICENSE)
