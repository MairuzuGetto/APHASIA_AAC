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

本文件定义 AAC 专案所有文件的统一编写规范。

目的包括：

- 建立一致的文件格式
- 提高文件可读性
- 降低维护成本
- 建立文件之间的关联关系
- 提供统一版本管理方式
- 建立长期可维护的产品文档体系

所有 Markdown 文件皆应遵循本规范。

---

# 2. Metadata Header（文件标头）

每份文件皆应于第一页建立 Metadata Header。

统一格式如下：

| Item | Value |
|------|-------|
| Document | 文件名称 |
| Version | v1.0.0 |
| Status | Draft / Review / Released / Deprecated |
| Based on | 关联文件 |
| Compatibility | 相容版本 |
| Owner | 文件负责人 |
| Last Update | YYYY-MM-DD |
| Next Document | 下一份文件 |

---

# 3. Document Status（文件状态）

所有文件统一采用以下状态。

| Status | Description |
|---------|-------------|
| Draft | 草稿，内容仍持续讨论。 |
| Review | 内容完成，等待确认。 |
| Released | 正式发布版本。 |
| Deprecated | 已停止维护，仅保留历史纪录。 |

---

# 4. Version Rule（版本规范）

所有文件统一采用 Semantic Versioning。

格式：

Major.Minor.Patch

例如：

v1.0.0

版本规则：

| Type | Description |
|------|-------------|
| Major | 产品方向或文件结构发生重大调整。 |
| Minor | 新增章节、原则、功能说明。 |
| Patch | 修正文字、格式、描述或轻微调整。 |

例如：

```
v1.0.0
v1.0.1
v1.1.0
v2.0.0
```

---

# 5. File Naming Rule（文件命名规范）

所有文件统一采用数字排序。

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

原则：

- 使用 Pascal Case。
- 单字使用底线（_）分隔。
- 文件名称简洁明确。
- 避免空格与特殊符号。

---

# 6. Markdown Rule（Markdown 编写规范）

统一采用 Markdown 原生语法。

标题：

```
# Heading

## Heading

### Heading
```

建议使用：

- Markdown Table
- Markdown Quote
- Markdown List
- Markdown Code Block

避免：

- HTML 标签
- 复杂排版
- 过度颜色标记

保持 GitHub、VS Code Preview 良好兼容性。

---

# 7. Writing Style（写作风格）

所有产品文件统一采用正式描述。

建议：

✔ 使用陈述句。

✔ 使用客观描述。

✔ 保持简洁。

✔ 一段说明一个概念。

避免：

✘ 口语化。

✘ 主观推测。

✘ 含糊不清。

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

统一语言格式。

中文：

- 使用繁体中文。
- 使用全形中文标点。

英文：

- 保持原文。
- 使用半形标点。

技术名称：

保持官方命名。

例如：

```
Flutter

Material Design

Design System

Focus Card

PageView

AI

OCR
```

避免同一词汇出现多个写法。

例如：

```
Button

按钮

Btn
```

统一择一使用。

---

# 9. File Structure（文件结构）

建议所有文件采用统一结构。

```
Metadata Header

↓

Purpose（目的）

↓

Main Content（主要内容）

↓

Notes（可选）

↓

Revision History（版本纪录）
```

不同类型文件可依需求调整章节，
但建议维持整体一致性。

---

# 10. Revision History（版本纪录）

每份文件建议保留版本纪录。

格式：

| Version | Date | Description |
|----------|------|-------------|
| v1.0.0 | 2026-07-05 | Initial Release |

后续更新持续追加。

---

# Appendix A（术语定义）

| Term | Description |
|------|-------------|
| Blueprint | 产品蓝图，定义产品方向。 |
| Design System | 定义产品视觉与互动规范。 |
| Component | 可重复使用的 UI 元件。 |
| Design Token | 设计变量，例如颜色、字体、间距。 |
| Theme | Flutter 全域主题。 |
| Flutter Architecture | Flutter 专案程式架构。 |

---

> **Good documentation improves communication.**

> **Clear documentation builds great products.**