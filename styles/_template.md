# 风格模板示例

这是创建新风格的模板文件。复制此文件并重命名（如 `my-style.md`），然后修改内容即可添加新风格。

## 文件命名规范

- 使用英文小写 + 短横线
- 示例：`neumorphism.md`, `material-design.md`, `glassmorphism.md`

## 模板结构

```markdown
<role>
你是一位专业的前端工程师和 UI/UX 设计师。你的任务是根据用户需求生成符合特定设计风格的 HTML 页面。

[在这里描述 AI 的角色和职责]
</role>

<design-system>
# Design Style: [风格名称]

## Design Philosophy

### Core Principle
[描述设计的核心理念]

### The Visual Vibe
[描述视觉风格特点]

**Emotional Keywords:**
- *关键词1* — 描述
- *关键词2* — 描述

### The DNA of This Style

#### 1. [特征1名称]
[详细描述]

#### 2. [特征2名称]
[详细描述]

## Design Token System

### Color Strategy

| Token | Value | Usage |
|:------|:------|:------|
| `background` | `#FFFFFF` | 主背景色 |
| `foreground` | `#000000` | 主文字色 |
| `accent` | `#XXXXXX` | 强调色 |
| ... | ... | ... |

### Typography System

**Font Pairing:**
- **Display Font:** `"Font Name", fallback` — 用于标题
- **UI Font:** `"Font Name", fallback` — 用于正文

### Spacing & Layout

[描述间距和布局规则]

### Borders, Surfaces & Shadows

[描述边框、表面和阴影]

## Component Styling

### Buttons

**Primary Button:**
- Background: [颜色]
- Text: [颜色]
- Border-radius: [值]
- Hover: [效果]

### Cards

[卡片样式描述]

### Inputs

[输入框样式描述]

## Effects & Animation

[动画和效果描述]

## Responsive Strategy

[响应式策略描述]

## Accessibility

[可访问性要求]
</design-system>
```

## 关键要素

### 1. Role 部分
定义 AI 的角色和任务，告诉它：
- 你是谁（前端专家、设计师）
- 你要做什么（生成 HTML）
- 你的目标（符合设计风格）

### 2. Design Philosophy
描述设计的哲学和理念：
- 核心理念
- 视觉氛围
- 情感关键词
- 风格 DNA

### 3. Design Tokens
定义设计系统的具体参数：
- 颜色（背景、前景、强调色等）
- 字体（标题字体、正文字体）
- 间距
- 阴影

### 4. Components
定义各个组件的样式：
- 按钮（主要、次要、幽灵按钮）
- 卡片
- 输入框
- 导航

### 5. Effects & Animation
描述动画效果：
- 过渡时间
- 缓动函数
- 悬停效果
- 入场动画

### 6. Responsive
响应式策略：
- 断点设置
- 移动端适配
- 布局变化

## 示例：Minimal SaaS 风格的关键特征

参考 `Saas-style.md` 文件，它包含以下关键特征：

1. **Signature Gradient** - 标志性的蓝色渐变
2. **Inverted Contrast Sections** - 反色区块
3. **Animated Depth** - 动画深度效果
4. **Dual-Font Typography** - 双字体系统
5. **Texture Over Flatness** - 纹理而非平面
6. **Asymmetry** - 不对称布局
7. **Section Labels** - 区块标签系统

## 创建新风格的步骤

1. **复制模板**
   ```bash
   cp _template.md my-style.md
   ```

2. **填写内容**
   - 修改风格名称
   - 定义设计哲学
   - 设置设计 token
   - 描述组件样式
   - 添加动画效果

3. **测试风格**
   - 使用 `/html-style` 命令
   - 选择新风格
   - 检查生成效果

4. **迭代优化**
   - 根据生成结果调整提示词
   - 添加更多细节描述
   - 修正不清晰的部分

## 提示词编写技巧

### 1. 具体而非抽象
❌ 不好："使用现代设计"  
✅ 好："使用 12px 圆角、蓝色渐变背景、白色文字"

### 2. 提供视觉参考
- 描述颜色值（#0052FF）
- 描述间距（16px, 24px）
- 描述字体大小（14px, 16px, 24px）

### 3. 包含交互状态
- 默认状态
- 悬停状态
- 点击状态
- 禁用状态

### 4. 考虑边界情况
- 空状态
- 加载状态
- 错误状态

### 5. 保持简洁
- 每个部分聚焦一个主题
- 使用列表和表格
- 避免冗长的段落

## 常见风格类型

### 1. Neumorphism（新拟态）
- 柔和的阴影
- 凸起和凹陷效果
- 单色调色板

### 2. Glassmorphism（玻璃拟态）
- 半透明背景
- 背景模糊
- 鲜艳的边框

### 3. Material Design
- 纸张隐喻
- 阴影层次
- 波纹效果

### 4. Brutalism（粗野主义）
- 高对比度
- 粗边框
- 系统字体

### 5. Minimal（极简主义）
- 大量留白
- 有限的色彩
- 清晰的排版

## 参考资源

- [Material Design Guidelines](https://material.io/design)
- [Apple Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines/)
- [Refactoring UI](https://refactoringui.com/)
- [Tailwind UI](https://tailwindui.com/)

---

**提示**：创建新风格时，可以先从简单的描述开始，然后根据生成效果逐步完善细节。
