# AAC Design System

| Item | Value |
|------|-------|
| Document | AAC Design System |
| Version | v1.0.0 |
| Status | Draft |
| Based on | Product Blueprint v1.3.1 |
| Compatibility | Blueprint v1.3.1 |
| Owner | Miles |
| Last Update | 2026-07-05 |
| Next Document | 03_Component_System.md |

---

# 1. Design Manifesto（设计宣言）

AAC 不只是一套表达工具，
更是一位陪伴使用者日常生活的伙伴。

因此，本产品不追求华丽的视觉效果，
也不刻意展现科技感。

我们相信，
好的设计应该让介面逐渐消失，
让使用者把注意力放在「想表达什么」，
而不是「如何操作」。

所有视觉设计、互动设计与功能设计，
皆遵循本 Design System 所定义之设计原则。

> **好的设计，不需要被注意。**  
> **好的沟通，才值得被看见。**

---

# 2. Design DNA（设计 DNA）

Design DNA 定义的是本产品最核心的设计价值。

它回答的是：

> **「我们相信什么？」**

所有 Design Language、Design Tokens、Component 与 Flutter 实作，
皆应建立于这些价值之上。

---

## DNA-01 Communication First（沟通优先）

沟通永远是产品的核心。

所有设计都应帮助使用者更快速、更自然地完成表达，
而非增加额外操作流程。

---

## DNA-02 Respect（尊重）

每位使用者皆拥有完整的思考能力。

设计不应幼化、医疗化，
也不应刻意凸显其障碍身份。

尊重，是所有设计的起点。

---

## DNA-03 Stable（稳定）

固定位置比聪明的位置更重要。

AAC 属于长期使用工具。

稳定的介面能够建立空间记忆与肌肉记忆，
降低认知负担，提升沟通效率。

---

## DNA-04 Personal（个人化）

每位使用者都拥有不同的生活方式。

产品应围绕使用者建立个人化沟通体验，
而不是要求使用者适应固定模板。

---

## DNA-05 Invisible Technology（科技退居幕后）

AI、OCR、语音合成与资料分析，
皆只是辅助工具。

真正的主角，
始终都是沟通。

---

# 3. Design Language（设计语言）

Design Language 定义了本产品希望带给使用者的整体体验。

它并不规定颜色、字体或元件样式，
而是定义所有设计应呈现出的共同语言。

后续所有 Design Tokens、Component、Theme 与 Flutter 实作，
皆应遵循以下设计语言。

## LANG-01 Clear（清晰）

> 让重要资讯一眼即可辨识。

介面应以资讯传达为优先，减少装饰元素，
避免使用者将注意力放在 UI 本身。

## LANG-02 Focused（专注）

> 每个画面只专注于一件事情。

介面仅呈现当下需要的内容，
减少视觉干扰，避免同时出现过多资讯。

让沟通成为唯一焦点。

## LANG-03 Predictable（可预期）

> 所有操作都应符合使用者的预期。

位置一致、互动一致、动画一致。

让使用者清楚知道下一步会发生什么。

## LANG-04 Gentle（柔和）

> 降低焦虑，而非制造刺激。

所有互动皆应自然、柔和、稳定。

设计应给予陪伴感，
而不是压迫感。

## LANG-05 Familiar（熟悉）

> 所有设计都应贴近日常生活经验。

降低学习成本，让使用者能够凭直觉理解内容。

不追求科技感，也不过度强调医疗感。

## LANG-06 Efficient（高效率）

> 每一次操作，都应缩短表达时间。

设计追求沟通效率，而非视觉炫技。

任何新增功能，都应帮助使用者更快完成表达。

# 4. Component Principles（组件原则）

Component 是 AAC App 的基本组成单位。

所有 UI 都应由可重复使用的 Component 组成，
而非针对单一页面独立开发。

每个 Component 都应遵循以下原则。

## COMP-01 Reusable（可复用）

每个 Component 应可在多个页面重复使用。

避免为单一页面建立专属 Widget。

## COMP-02 Consistent（一致性）

相同功能应使用相同 Component。

例如：

Phrase Card 在首页、收藏、历史纪录，
皆应保持一致的视觉与互动方式。

## COMP-03 Token Driven（由 Design Token 驱动）

所有 Component 应引用 Design Tokens。

不得直接使用：

- Color
- Font Size
- Radius
- Padding

等硬编码数值。

## COMP-04 Modular（模块化）

每个 Component 应保持单一职责。

复杂画面应由多个 Component 组合，
而非建立大型 Widget。

## COMP-05 Accessible（可存取）

所有 Component 应符合 Accessibility 规范。

包括：

- Touch Target
- 字体缩放
- 语音辅助
- 对比度

## COMP-06 Predictable（可预期）

Component 的互动行为必须保持一致。

例如：

点击、

长按、

动画、

状态变化，

皆应符合使用者预期。

## Component Relationship

Design Language

↓

Component Principles

↓

Component Guide

↓

Flutter Widget

---

# 5. Design Tokens（设计变量）
> Token 数值将在 Flutter Prototype 与真机测试完成后逐步回填，
> Design Tokens 属于 Living Specification。

Design Tokens 定义了整个 AAC Design System 所使用的基础设计变量。

所有 Component、Theme 与 Flutter Widget，
皆应引用 Design Tokens，不得直接使用硬编码（Hard Code）。

Design Tokens 的目的：

- 保持设计一致性
- 提高维护性
- 降低重复开发
- 支援主题切换
- 支援无障碍设定

### TOKEN-01 Color
| Token | Value | Status | Description |
|--------|-------|--------|-------------|
| Primary | TBD | Draft | 品牌主色 |
| Secondary | TBD | Draft | 辅助色 |
| Background | TBD | Draft | 页面背景 |
| Surface | TBD | Draft | 内容背景 |
| Card | TBD | Draft | 卡片背景 |
| Border | TBD | Draft | 边框颜色 |
| Text Primary | TBD | Draft | 主要文字 |
| Text Secondary | TBD | Draft | 次要文字 |
| Success | TBD | Draft | 成功状态 |
| Warning | TBD | Draft | 警告状态 |
| Error | TBD | Draft | 错误状态 |

### TOKEN-02 Typography
| Token | Size | Weight | Status | Description |
|--------|------|--------|--------|-------------|
| Display | TBD | TBD | Draft | 首页大标题 |
| Headline | TBD | TBD | Draft | 页面标题 |
| Title | TBD | TBD | Draft | 卡片标题 |
| Subtitle | TBD | TBD | Draft | 次标题 |
| Body | TBD | TBD | Draft | 一般内容 |
| Caption | TBD | TBD | Draft | 提示说明 |
| Button | TBD | TBD | Draft | 按钮文字 |

### TOKEN-03 Spacing
| Token | Value | Status | Description |
|--------|-------|--------|-------------|
| XS | TBD | Draft | 最小间距 |
| S | TBD | Draft | 小间距 |
| M | TBD | Draft | 一般间距 |
| L | TBD | Draft | 区块间距 |
| XL | TBD | Draft | 页面边距 |
| XXL | TBD | Draft | 大留白 |

### TOKEN-04 Radius
| Token | Value | Status | Description |
|--------|-------|--------|-------------|
| Small | TBD | Draft | 小圆角 |
| Medium | TBD | Draft | Button |
| Large | TBD | Draft | Card |
| Dialog | TBD | Draft | Focus Card |
| Circle | TBD | Draft | Avatar |

### TOKEN-05 Elevation
| Token | Value | Status | Description |
|--------|-------|--------|-------------|
| Level 0 | TBD | Draft | 无阴影 |
| Level 1 | TBD | Draft | Card |
| Level 2 | TBD | Draft | Dialog |
| Level 3 | TBD | Draft | Floating |

### TOKEN-06 Motion
| Token | Duration | Curve | Status | Description |
|--------|----------|-------|--------|-------------|
| Fast | TBD | TBD | Draft | 快速反馈 |
| Normal | TBD | TBD | Draft | 一般动画 |
| Slow | TBD | TBD | Draft | 慢速动画 |
| Page | TBD | TBD | Draft | 页面切换 |
| Dialog | TBD | TBD | Draft | Focus Card |
| Card | TBD | TBD | Draft | 卡片动画 |

### TOKEN-07 Icon Size
| Token | Size | Status | Description |
|--------|------|--------|-------------|
| XS | TBD | Draft | 极小图标 |
| S | TBD | Draft | 小图标 |
| M | TBD | Draft | 标准图标 |
| L | TBD | Draft | 大图标 |
| XL | TBD | Draft | 特大图标 |

### TOKEN-08 Touch Target
| Token | Value | Description |
|--------|-------|-------------|
| Minimum | 48dp | 最小可点击区域 |
| Recommended | 56dp | 建议点击区域 |
| Large | 64dp | 大尺寸按钮 |

---

# 6. Icon & Illustration（图标与插画）

> Coming Soon

---

# 7. Motion System（动画系统）

> Coming Soon

---

# 8. Accessibility（无障碍设计）

> Coming Soon

---

# 9. Theme System（主题系统）

> Coming Soon

---

# 10. Flutter Architecture（Flutter 架构）

> Coming Soon