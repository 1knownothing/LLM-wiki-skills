# 🧠 LLM Wiki Skills

> **为你的 AI 助手赋予持久知识管理能力**

[English](./README.md) | [中文](./README.zh.md) 

---

## 为什么选择这个技能集？

| 特性 | 传统 RAG | **LLM Wiki Skills** |
|------|----------|---------------------|
| 知识持久化 | ❌ 每次重新检索 | ✅ 随时间积累 |
| 交叉引用 | ❌ 无连接 | ✅ 自动关联关系 |
| 矛盾检测 | ❌ 无 | ✅ 自动标记 |
| 多格式输出 | ❌ 仅文本 | ✅ Markdown、表格、幻灯片 |
| 查询综合 | ❌ 简单检索 | ✅ 推理 + 引用 |

> **这些技能将你的 AI 从无状态的查询工具转变为持久学习的伙伴。**

---

## ✨ 核心功能

### 1. **wiki-init** — 一键 Wiki 初始化
- 创建完整的 Wiki 架构
- 生成 CLAUDE.md 供 AI 理解上下文
- 设置 index.md 和 log.md

### 2. **wiki-ingest** — 智能源文件处理
- 读取文章、论文、书籍
- 提取关键要点、实体、概念
- 自动更新交叉引用
- 标记矛盾点

### 3. **wiki-query** — 上下文感知的问答
- 先搜索索引，再深入阅读
- 综合答案并提供 Wiki 引用
- 支持多种输出格式
- 将有价值的答案存回 Wiki

### 4. **wiki-lint** — 自动质量控制
- 检测矛盾的声明
- 查找孤立页面
- 识别缺失的链接
- 建议数据缺口

### 5. **wiki-maintain** — Schema 演进
- 更新约定俗成
- 优化工作流程
- 添加新的页面类型

---

## 🔗 完美组合：Obsidian + Web Clipper + CLI

### 工作流程

```
🌐 网页 → Obsidian Web Clipper → 📝 Obsidian 知识库
                                        ↓
                                    LLM Wiki Skills
                                        ↓
                                    📚 知识库
```

### 1. 使用 Obsidian Web Clipper 捕获
- 直接将文章、研究论文、网页内容保存到 Obsidian
- 使用模板保持结构一致

### 2. 使用 Obsidian CLI 处理
```bash
# 列出知识库中的笔记
obsidian-cli list

# 搜索新来源
obsidian-cli search "source:web"

# 获取笔记内容
obsidian-cli read "My Note"
```

### 3. 使用 LLM Wiki Skills 摄入
```markdown
用户：处理我在 Obsidian 中保存的新文章

AI：（使用 wiki-ingest 提取并整合）
```

### 集成模式

| 工具 | 角色 |
|------|------|
| **Obsidian** | 界面 + 存储 |
| **Web Clipper** | 内容捕获 |
| **Obsidian CLI** | 程序化访问 |
| **LLM Wiki Skills** | AI 驱动的处理 |

---

## 🚀 安装指南

### OpenCode 用户

1. 将 `SKILL.md` 复制到 `~/.config/opencode/skills/wiki-knowledge-base/SKILL.md`
2. 将 `skills/` 子文件夹中的每个技能复制：
   - `skills/wiki-init/SKILL.md`
   - `skills/wiki-ingest/SKILL.md`
   - `skills/wiki-query/SKILL.md`
   - `skills/wiki-lint/SKILL.md`
   - `skills/wiki-maintain/SKILL.md`

### 目录结构
```
~/.config/opencode/skills/
└── wiki-knowledge-base/
    ├── SKILL.md              # 主技能文件
    └── skills/
        ├── wiki-init/SKILL.md
        ├── wiki-ingest/SKILL.md
        ├── wiki-query/SKILL.md
        ├── wiki-lint/SKILL.md
        └── wiki-maintain/SKILL.md
```

### 其他 AI 助手
将 SKILL.md 格式适配到你助手的技能系统。

---

## 📁 项目结构

```
LLM-wiki-skills/
├── SKILL.md                    # 主技能文件
├── README.md                   # 英文版
├── README.zh.md                # 中文版
├── wiki/                       # 示例 Wiki 内容
│   ├── entities/               # 实体页面
│   ├── concepts/               # 概念页面
│   ├── sources/               # 源摘要
│   ├── index.md               # 内容目录
│   └── log.md                 # 操作日志
└── skills/                     # 独立技能
    ├── wiki-init/
    ├── wiki-ingest/
    ├── wiki-query/
    ├── wiki-lint/
    └── wiki-maintain/
```

---

## 🎯 使用场景

- 📚 **研究助手** — 处理论文、提取洞见
- 📖 **阅读笔记** — 捕获和综合书籍
- 💼 **团队知识** — 共享文档
- 🧠 **第二大脑** — 个人知识管理
- 🔬 **技术文档** — API 和代码库知识

*由 AI 构建，由 LLM Wiki Skills 驱动*
