# AAC Document Guideline

| Item | Value |
|------|-------|
| Document | AAC Document Guideline |
| Version | v1.0.0 |
| Status | Released |
| Based on | - |
| Compatibility | All Project Documents |
| Owner | Miles |
| Last Update | 2026-07-05 |
| Next Document | 01_Product_Blueprint.md |

---

# 1. Purpose（目的）

本文件定义 AAC 项目所有文档的统一编写规范。

目的包括：

- 建立统一的文档格式
- 提高文档可读性
- 降低维护成本
- 建立文档之间的关联关系
- 提供统一版本管理方式
- 建立长期可维护的产品文档体系

所有 Markdown 文件均应遵循本规范。

---

# 2. Metadata Header（文件标头）

所有文档第一页均应建立 Metadata Header。

统一格式如下：

| Item | Value |
|------|-------|
| Document | 文档名称 |
| Version | v1.0.0 |
| Status | Draft / Review / Released / Deprecated |
| Based on | 上层关联文档 |
| Compatibility | 兼容版本 |
| Owner | 文档负责人 |
| Last Update | YYYY-MM-DD |
| Next Document | 下一份文档 |

---

# 3. Document Status（文档状态）

所有文档统一采用以下状态：

| Status | Description |
|---------|-------------|
| Draft | 草稿，内容仍持续讨论。 |
| Review | 内容完成，等待确认。 |
| Released | 正式发布版本。 |
| Deprecated | 已停止维护，仅保留历史记录。 |

---

# 4. Version Rule（版本规范）

所有文档统一采用 Semantic Versioning（语义化版本）。

格式：

```
Major.Minor.Patch
```

例如：

```
v1.0.0
v1.0.1
v1.1.0
v2.0.0
```

版本规则：

| Type | Description |
|------|-------------|
| Major | 产品方向、文档结构或设计原则发生重大调整。 |
| Minor | 新增章节、规范、原则或功能说明。 |
| Patch | 修正文字、格式、描述或轻微调整。 |

---

# 5. File Naming Rule（文件命名规范）

所有文档统一采用数字排序。

例如：

```
00_Document_Guideline.md

01_Product_Blueprint.md

02_Design_System.md

03_Component_System.md

04_Flutter_Architecture.md

05_AI_Roadmap.md

06_Development_Log.md
```

命名原则：

- 使用 Pascal Case。
- 单词使用底线（_）连接。
- 文件名称保持简洁明确。
- 不使用空格。
- 不使用特殊符号。

---

# 6. Markdown Rule（Markdown 编写规范）

统一采用 Markdown 原生语法。

标题：

```markdown
# 一级标题

## 二级标题

### 三级标题
```

建议使用：

- Markdown Table
- Markdown Quote
- Markdown List
- Markdown Code Block

避免使用：

- HTML 标签
- 复杂排版
- 颜色标记
- 依赖特定编辑器功能

确保 GitHub、VS Code Preview 等环境均可正常显示。

---

# 7. Writing Style（写作风格）

所有产品文档统一采用正式、客观、简洁的描述方式。

建议：

- 使用陈述句。
- 一段说明一个概念。
- 描述明确、避免歧义。
- 保持逻辑一致。

避免：

- 口语化表达。
- 主观推测。
- 模糊描述。
- 情绪性文字。

例如：

❌

```
应该可以这样。
```

改为：

✅

```
统一采用此设计。
```

---

# 8. Language Rule（语言规范）

为保持整个 AAC 项目文档的一致性，所有文档统一采用以下语言规范。

## 文档语言

产品文档统一使用**简体中文**编写。

英文仅用于：

- 专有名词
- 技术术语
- API 名称
- Flutter 官方名称
- Design System 相关名称

例如：

```
Flutter
Product Blueprint
Design System
Design Token
Focus Card
PageView
AI
OCR
```

---

## 命名规范

所有技术名称统一采用官方英文名称。

正文首次出现建议采用：

```
Design System（设计系统）
```

之后可直接使用：

```
Design System
```

避免同一术语出现多个名称。

例如：

统一：

```
Button
Card
Dialog
Design Token
```

避免：

```
按钮 / Button / Btn

卡片 / Card

设计变量 / Token
```

同一概念应仅保留一种正式名称。

---

## 标点规范

中文内容：

统一使用中文标点。

英文内容：

统一使用英文标点。

中英文混排时保持自然阅读。

例如：

```
AAC Design System 定义了整个 App 的设计规范。
```

---

# 9. File Structure（文档结构）

建议所有产品文档采用统一结构。

```
Metadata Header

↓

Purpose（目的）

↓

Main Content（主要内容）

↓

Notes（可选）

↓

Revision History（版本记录）
```

不同类型文档可根据实际需求调整章节，
但建议整体保持一致。

---

# 10. Revision History（版本记录）

所有文档建议保留版本记录。

格式如下：

| Version | Date | Description |
|----------|------|-------------|
| v1.0.0 | 2026-07-05 | Initial Release |

后续版本持续追加。

---

# Appendix A（Project Glossary｜项目术语）

| Term | Official Name | Description |
|------|---------------|-------------|
| Product Blueprint | Product Blueprint | 产品蓝图 |
| Design System | Design System | 设计系统 |
| Design DNA | Design DNA | 设计 DNA |
| Design Language | Design Language | 设计语言 |
| Design Token | Design Token | 设计变量 |
| Component | Component | 可复用 UI 组件 |
| Theme | Theme | Flutter 全局主题 |
| Focus Card | Focus Card | 焦点卡片 |
| Personal Library | Personal Library | 个人词库 |
| Core Library | Core Library | 核心词库 |
| Flutter Architecture | Flutter Architecture | Flutter 项目架构 |

---

> **Good documentation improves communication.**

> **Clear documentation builds great products.**