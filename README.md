# 🧠 LLM Wiki Skills

> **Supercharge your AI agent with persistent knowledge management**

[English](./README.md) | [中文](./README.zh.md) | [🔄 Switch Language](./README.zh.md)

---

## Why This Skill Set?

| Feature | Traditional RAG | **LLM Wiki Skills** |
|---------|-----------------|---------------------|
| Knowledge Persistence | ❌ Retrieve each time | ✅ Accumulates over time |
| Cross-Reference | ❌ No connections | ✅ Auto-linked relationships |
| Contradiction Detection | ❌ None | ✅ Automatic flagging |
| Multi-Format Output | ❌ Text only | ✅ Markdown, Tables, Slides |
| Query Synthesis | ❌ Simple retrieval | ✅ Reasoning + citations |

> **These skills transform your AI from a stateless query tool into a persistent learning companion.**

---

## ✨ Core Features

### 1. **wiki-init** — One-command wiki setup
- Creates complete wiki architecture
- Generates CLAUDE.md schema for AI context
- Sets up index.md and log.md

### 2. **wiki-ingest** — Intelligent source processing
- Reads articles, papers, books
- Extracts key takeaways, entities, concepts
- Auto-updates cross-references
- Flags contradictions

### 3. **wiki-query** — Context-aware Q&A
- Searches index first, then deep-dives
- Synthesizes answers with wiki citations
- Supports multiple output formats
- Files valuable answers back to wiki

### 4. **wiki-lint** — Automatic quality control
- Detects contradictory claims
- Finds orphan pages
- Identifies missing links
- Suggests data gaps

### 5. **wiki-maintain** — Schema evolution
- Updates conventions
- Refines workflows
- Adds new page types

---

## 🔗 Perfect Combo: Obsidian + Web Clipper + CLI

### Workflow

```
🌐 Web → Obsidian Web Clipper → 📝 Obsidian Vault
                                        ↓
                                    LLM Wiki Skills
                                        ↓
                                    📚 Knowledge Base
```

### 1. Capture with Obsidian Web Clipper
- Save articles, research papers, web content directly to Obsidian
- Use templates for consistent structure

### 2. Process with Obsidian CLI
```bash
# List notes in vault
obsidian-cli list

# Search for new sources
obsidian-cli search "source:web"

# Get note content
obsidian-cli read "My Note"
```

### 3. Ingest with LLM Wiki Skills
```markdown
User: Process the new article I saved in Obsidian

AI: (uses wiki-ingest to extract and integrate)
```

### Integration Pattern

| Tool | Role |
|------|------|
| **Obsidian** | UI + Storage |
| **Web Clipper** | Content capture |
| **Obsidian CLI** | Programmatic access |
| **LLM Wiki Skills** | AI-powered processing |

---

## 🚀 Installation

### For OpenCode Users

1. Copy `SKILL.md` to `~/.config/opencode/skills/wiki-knowledge-base/SKILL.md`
2. Copy each skill in `skills/` subfolder:
   - `skills/wiki-init/SKILL.md`
   - `skills/wiki-ingest/SKILL.md`
   - `skills/wiki-query/SKILL.md`
   - `skills/wiki-lint/SKILL.md`
   - `skills/wiki-maintain/SKILL.md`

### Directory Structure
```
~/.config/opencode/skills/
└── wiki-knowledge-base/
    ├── SKILL.md              # Master skill
    └── skills/
        ├── wiki-init/SKILL.md
        ├── wiki-ingest/SKILL.md
        ├── wiki-query/SKILL.md
        ├── wiki-lint/SKILL.md
        └── wiki-maintain/SKILL.md
```

### For Other AI Assistants
Adapt the SKILL.md format to your agent's skill system.

---

## 📁 Project Structure

```
LLM-wiki-skills/
├── SKILL.md                    # Master skill file
├── README.md                   # English version
├── README.zh.md                # 中文版
├── wiki/                       # Example wiki content
│   ├── entities/               # Entity pages
│   ├── concepts/               # Concept pages
│   ├── sources/               # Source summaries
│   ├── index.md               # Content catalog
│   └── log.md                 # Operation log
└── skills/                     # Individual skills
    ├── wiki-init/
    ├── wiki-ingest/
    ├── wiki-query/
    ├── wiki-lint/
    └── wiki-maintain/
```

---

## 🎯 Use Cases

- 📚 **Research Assistant** — Process papers, extract insights
- 📖 **Reading Notes** — Capture and synthesize books
- 💼 **Team Knowledge** — Shared documentation
- 🧠 **Second Brain** — Personal knowledge management
- 🔬 **Technical Docs** — API and codebase knowledge

---

## 📖 Further Reading

- [LLM Wiki Pattern](https://github.com/karpathy/llm-wiki) — Andrej Karpathy
- [Transformer Circuits](https://transformer-circuits.pub/) — Anthropic
- [Obsidian CLI](https://github.com/yoursunny/obsidian-cli)

---

## 🤝 Contributing

PRs welcome! Please ensure:
- Skills follow the SKILL.md format
- Documentation is bilingual
- Examples work as described

---

## 📜 License

MIT License — Free to use, modify, and distribute.

---

*Built with by AI, powered by LLM Wiki Skills*