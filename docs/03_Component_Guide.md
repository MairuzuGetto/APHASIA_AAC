# AAC Component Guide

| Item | Value |
|------|-------|
| Document | AAC Component Guide |
| Version | v1.0.0 |
| Status | Draft |
| Based on | Design System v1.0.0 |
| Compatibility | Design System v1.x |
| Owner | Miles |
| Last Update | 2026-07-06 |
| Next Document | 04_Flutter_Architecture.md |

---

# 1. Purpose（目的）

本文件定义 AAC App 所使用的所有 UI Component。

每个 Component 均应：

- 可重复使用（Reusable）
- 保持一致性（Consistent）
- 遵循 Design Tokens
- 遵循 Component Principles
- 对应 Flutter Widget

本文件不负责定义设计原则，
设计原则请参考：

02_Design_System.md

---

# 2. Component Hierarchy（组件架构）

    AAC App

    │

    ├── Communication（沟通）

    │     ├── Phrase Card（短语卡）

    │     ├── Focus Card（焦点卡）

    │     ├── Category Chip（分类标签）

    │     └── Sentence Builder（句子构建器）

    │

    ├── Navigation（导航）

    │     ├── Bottom Navigation（底部导航）

    │     ├── Page Indicator（分页指示器）

    │     └── Navigation Button（导航按钮）

    │

    ├── Feedback（反馈）

    │     ├── Dialog（对话框）

    │     ├── Snackbar（提示栏）

    │     └── Loading（加载中）

    │

    ├── Input（输入）

    │     ├── Search Bar（搜索栏）

    │     ├── Text Field（文本输入）

    │     └── Voice Button（语音按钮）

    │

    ├── Settings（设置）

    │     ├── Setting Tile（设置项）

    │     ├── Switch Tile（开关项）

    │     └── Slider Tile（滑块项）

    │

    └── Foundation（基础组件）

        ├── Icon（图标）

        ├── Avatar（头像）

        ├── Divider（分隔线）

        └── Badge（徽章）

---

# 3. Component Naming Rule（组件命名规范）

所有 Component 统一采用以下命名规则。

Flutter Widget：

AacPhraseCard

AacFocusCard

AacBottomNavigation

AacDialog

设计文件：

Phrase Card

Focus Card

Bottom Navigation

Dialog

统一命名原则：

- Flutter Widget 使用 PascalCase。
- Component 名称保持英文。
- 同一 Component 不允许出现多个名称。
- 一个 Component 对应一个 Flutter Widget。

---

# 4. Component Lifecycle（组件生命周期）

所有 Component 均应具有明确生命周期。

| Status | Description |
|---------|-------------|
| Draft | 已规划，尚未设计 |
| Design | 完成组件设计 |
| Prototype | Flutter Prototype 已完成 |
| Verified | 真机验证完成 |
| Released | 正式投入使用 |
| Deprecated | 已停止维护 |

---

# 5. Component Template（组件模板）

以下模板适用于所有 Component。

---

## Component Name

### Purpose（用途）

说明此 Component 存在目的。

---

### Usage（使用场景）

列出可使用页面。

例如：

- Home
- Favorites
- History

---

### Structure（组成）

说明组件视觉组成。

例如：

┌────────────────────┐

🖼️

今天感觉很好

└────────────────────┘

---

### Interaction（交互）

说明所有互动行为。

例如：

- Single Tap
- Long Press
- Double Tap

---

### States（状态）

说明所有状态。

例如：

- Normal
- Pressed
- Selected
- Disabled

---

### Accessibility（无障碍）

说明：

- Touch Target
- Text Scale
- Voice Feedback
- Contrast

---

### Related Design Rules

Design DNA：

Design Language：

Component Principles：

例如：

DNA-01

LANG-02

COMP-03

---

### Related Tokens

Color

Typography

Spacing

Radius

Motion

Touch Target

---

### Flutter Widget

对应 Flutter Widget 名称。

例如：

AacPhraseCard

---

### Notes

记录特殊说明。

例如：

- 是否允许长按
- 是否允许编辑
- 是否属于核心组件

---

# 6. Component Status（组件开发状态）

| Component | Category | Status |
|-----------|----------|--------|
| Phrase Card | Communication | Draft |
| Focus Card | Communication | Draft |
| Category Chip | Communication | Draft |
| Bottom Navigation | Navigation | Draft |
| Page Indicator | Navigation | Draft |
| Dialog | Feedback | Draft |
| Snackbar | Feedback | Draft |
| Search Bar | Input | Draft |
| Setting Tile | Settings | Draft |

---

# 7. Component Library

Component Library 定义 AAC App 所使用的所有 UI Component。

所有 Component 均应遵循：

- Component Principles
- Component Template
- Design Tokens
- Design Language

所有 Component 皆依功能进行分类。

## 7.1 Communication Components（沟通组件）

沟通组件为 AAC App 最核心的组件。

所有沟通体验皆围绕 Communication Components 展开。

### 7.1.1 Phrase Card（短语卡）

**Status：Draft**

> 用于快速表达一个词汇、短句或常用语。

### 7.1.2 Focus Card（焦点卡）

**Status：Draft**

> 点击 Phrase Card 后开启的大型沟通卡片。

### 7.1.3 Category Chip（分类标签）

**Status：Draft**

> 用于切换沟通分类。

### 7.1.4 Sentence Builder（句子构建器）

**Status：Planned**

> 用于组合多个词汇形成完整句子。

## 7.2 Navigation Components（导航组件）

负责 App 内部页面切换与导览。

### 7.2.1 Bottom Navigation（底部导航）

**Status：Draft**

> App 主要功能入口。

### 7.2.2 Page Indicator（分页指示器）

**Status：Draft**

> 显示目前分页位置。

### 7.2.3 Navigation Button（导航按钮）

**Status：Draft**

> 页面切换按钮。

## 7.3 Feedback Components（反馈组件）

负责回应使用者操作结果。

### 7.3.1 Dialog（对话框）

**Status：Draft**

> 显示重要确认讯息。

### 7.3.2 Snackbar（提示栏）

**Status：Draft**

> 显示短暂提示讯息。

### 7.3.3 Loading（加载状态）

**Status：Draft**

> 显示处理中状态。

## 7.4 Input Components（输入组件）

负责资料输入。

### 7.4.1 Search Bar（搜索栏）

**Status：Draft**

> 搜索词汇。

### 7.4.2 Text Field（文本输入）

**Status：Draft**

> 输入文字。

### 7.4.3 Voice Button（语音按钮）

**Status：Draft**

> 启动语音相关功能。

## 7.5 Settings Components（设置组件）

负责 App 设置与个人化功能。

### 7.5.1 Setting Tile（设置项）

**Status：Draft**

> 设置页面基本项目。

### 7.5.2 Switch Tile（开关项）

**Status：Draft**

> 开启或关闭功能。

### 7.5.3 Slider Tile（滑块项）

**Status：Draft**

> 调整连续数值。

## 7.6 Foundation Components（基础组件）

Foundation Components 为所有 Component 的基础组成元素。

通常不会单独出现在页面中，而是由其他 Component 重复使用。

### 7.6.1 Icon（图标）

**Status：Draft**

> 图示资源。

### 7.6.2 Avatar（头像）

**Status：Draft**

> 人物头像。

### 7.6.3 Divider（分隔线）

**Status：Draft**

> 区块分隔。

### 7.6.4 Badge（徽章）

**Status：Draft**

> 状态标记。

# 8. Communication Components

## 8.1 Phrase Card

## 8.2 Focus Card

## 8.3 Category Chip

……

所有 Component 均应遵循本 Guide 所定义之模板。
