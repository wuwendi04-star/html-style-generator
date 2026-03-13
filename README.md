# HTML Prototype Style Generator

**为产品经理打造的快速原型生成工具** — 输入产品需求，10 分钟输出多风格 Web 端高保真原型

## 核心价值

帮助产品经理快速搭建不同风格的 Web 端产品雏形，无需设计资源，无需编码能力，从需求文档直接生成可交互的高保真 HTML 原型。

### 典型使用场景

- **需求评审前**：快速生成原型，让开发和设计直观理解产品意图
- **A/B 方案对比**：同一功能用不同风格生成，直观对比效果
- **客户演示**：现场生成可点击原型，提升提案通过率
- **跨部门沟通**：用视觉化原型替代抽象 PRD，减少沟通成本
- **MVP 验证**：快速搭建多个版本进行用户测试

## 功能特性

- 📋 **智能页面规划**：分析需求文档，自动生成完整页面结构
- 🎨 **10 种设计风格**：从极简 SaaS 到现代暗黑、扁平化、新拟物等风格一键切换
- ✨ **空间构成优化**：自动应用不对称布局、元素叠压、对角线流向等专业设计手法
- 🎭 **动画与微交互**：每个风格独有的动画系统（悬停态、按压态、环境光效）
- ✅ **质量自检验**：生成前自动检查编码、结构、可访问性、响应式适配
- 📁 **智能文件管理**：自动检测文件名冲突，智能递增命名
- 🔧 **渐进式学习**：测试中发现问题自动沉淀到避坑清单，持续优化

## 安装

### 方式 1：Claude Code 项目级安装

将本目录复制到你的项目 `.skills/` 目录下：

```bash
# 在项目根目录执行
mkdir -p .skills
cp -r html-style-generator .skills/
```

### 方式 2：Claude Code 全局安装

将本目录复制到 Claude Code 的 skills 目录：

```bash
# 复制到用户目录
mkdir -p ~/claude-code-skills
cp -r html-style-generator ~/claude-code-skills/
```

## 快速开始

### 1. 触发技能

在 Claude Code 对话中输入：

```
/html-style 我想做一个鼠标电商 SaaS 平台，有首页、功能特色、价格方案、客户评价
```

或使用需求文档：

```
/html-style @product-requirements.md
```

### 2. 六阶段工作流

#### 阶段 1：需求分析与页面规划

AI 分析需求并输出页面结构：

```
📋 理解你的需求！建议生成以下页面：

【页面规划】
1. 首页 (index.html) - 产品展示、核心功能、数据指标、客户证言
2. 功能详情 (features.html) - 完整功能列表、技术规格
3. 价格方案 (pricing.html) - 套餐对比、FAQ
4. 客户案例 (customers.html) - 成功案例、行业解决方案

✅ 请确认：
- 这些页面够吗？需要增减吗？
- 回复"确认"继续，或告诉我调整内容
```

#### 阶段 2：选择设计风格（10 种可选）

```
🎨 请选择设计风格：

1. Minimal SaaS（极简 SaaS）— 蓝色渐变、现代科技感
2. Modern Dark（现代暗黑）— 深色背景、环境光效、Bento 网格
3. Hand-Drawn Sketch（手绘草图）— 手绘线条、纸张纹理
4. Corporate Trust（企业信赖）— 等距 3D、彩色阴影
5. Flat Design（扁平化）— 零阴影、大胆色块、几何装饰
6. Industrial（工业粗犷）— 金属质感、机械动画
7. Material Design（材料设计）— 涟漪扩散、pill 按钮
8. Neumorphism（新拟物）— 软性凸起/凹陷、物理按压
9. Newsprint（报纸印刷）— 油墨扩散、印刷错位
10. Tencent Cloud（腾讯云）— 腾讯蓝、科技感光效

请回复编号：
```

#### 阶段 3：选择输出目录

```
📂 请选择输出目录：
1. 使用当前项目目录
2. 指定其他路径
```

自动检测文件名冲突，智能递增命名（如 `index-5.html`）。

#### 阶段 4：选择生成策略

```
⚙️ 请选择生成策略：
1. 一次性全部生成 — 快速出完整原型
2. 逐个生成 — 逐步确认每个模块
3. 选择性生成 — 只生成指定页面
```

#### 阶段 5：批量生成

**全部生成模式**：
```
🚀 开始生成 Modern Dark 风格原型...

[1/4] 生成首页 (index-5.html)...
✅ 已保存：D:\test\index-5.html
   ✓ 多层背景系统 + 环境光团
   ✓ 不对称 Bento 网格布局
   ✓ 鼠标追踪聚光灯效果
   ✓ 滚动视差动画

[2/4] 生成价格方案 (pricing-2.html)...
✅ 已保存：D:\test\pricing-2.html
   ✓ 非对称提升卡片
   ✓ 渐变文字 + 光泽扫过
   ✓ hover 态阴影递进

...

✨ 全部完成！共生成 4 个页面
📂 D:\test\
├── index-5.html      (首页)
├── features-2.html   (功能详情)
├── pricing-2.html    (价格方案)
└── customers-2.html  (客户案例)
```

**逐个生成模式**：
```
🚀 开始生成...

[1/4] 生成首页 (index-5.html)...
✅ 已保存：D:\test\index-5.html

💡 请查看效果，回复"继续"生成下一个，或提出调整意见
   （例如："Hero 区域再大一些"、"按钮颜色换成紫色"）
```

#### 阶段 6：质量自检报告

每个文件生成后自动输出质量检查报告：

```
## 质量自检报告

### 基础结构
- ✅ DOCTYPE / charset / viewport
- ✅ 语义化标签（nav/section/footer）
- ✅ 简体中文内容

### 风格符合度（Modern Dark）
- ✅ 背景 #050506（非纯黑）
- ✅ 多层环境光背景系统
- ✅ 动态光团（float 动画 8-11s）
- ✅ 鼠标追踪聚光灯效果
- ✅ 渐变文字 + shimmer 动画
- ✅ 不对称 Bento 网格（英雄卡 4×2）
- ✅ 精准缓动 cubic-bezier(0.16,1,0.3,1)

### 空间构成
- ✅ 不对称布局（Hero 7:5 比例）
- ✅ 元素叠压（浮动徽章超出父容器）
- ✅ 对角线流向（clip-path 斜切）
- ✅ 留白与密度对比

### 响应式
- ✅ ≤1024px 双列布局
- ✅ ≤640px 单列 + 导航折叠
```

## 技术架构

### 底层设计要求（所有风格必须遵守）

1. **语言要求**：简体中文输出（代码注释、页面文本、按钮文字）
2. **设计视角**：设计师思维，追求美感而非程序员思维
3. **字体排版**：禁用 Inter/Roboto/Arial，使用展示性字体 + 精致正文字体
4. **色彩系统**：CSS 变量构建统一美学，主色调 + 点缀色
5. **图片资源**：Unsplash CDN（`https://images.unsplash.com/photo-{ID}?w={宽度}&q=80`）
6. **技术栈**：
   - HTML5 语义化标签
   - 原生 CSS（变量、Flexbox、Grid、@keyframes）
   - Font Awesome CDN（图标）
   - ECharts（数据可视化图表）
7. **空间构成**（新增）：
   - 不对称布局（避免镜像对称）
   - 元素叠压（浮动徽章超出边界）
   - 对角线流向（clip-path 斜切引导视线）
   - 留白与密度刻意对比
8. **动画强制执行**：
   - 必须实现风格模板所有动画效果
   - 完整三态（default/hover/active）
   - 精确参数（duration/easing/delay）

### 项目结构

```
html-style-generator/
├── skill.md                    # 核心工作流定义（6 阶段 + 8 项底层要求）
├── README.md                   # 使用说明
├── config/
│   └── pitfalls.yaml          # 避坑清单（持续积累）
└── styles/
    ├── Saas-style.md          # Minimal SaaS 风格
    ├── Modern-Dark.md         # Modern Dark 风格（Bento 网格 + 环境光）
    ├── Flat-Design.md         # Flat Design 风格（零阴影 + 色块）
    ├── Neumorphism.md         # Neumorphism 风格（双向软阴影）
    ├── Corporate.Trust.md     # Corporate Trust 风格（等距 3D）
    ├── Hand-Drawn-Sketch.md   # Hand-Drawn Sketch 风格（抖动线条）
    ├── Industrial.md          # Industrial 风格（金属光泽）
    ├── Material.md            # Material Design 风格（涟漪扩散）
    ├── Newsprint.md           # Newsprint 风格（油墨扩散）
    ├── Tencent-Cloud.md       # Tencent Cloud 风格（腾讯蓝光效）
    └── _template.md           # 新风格模板
```

## 扩展能力

### 添加新风格

1. 在 `styles/` 目录创建 `.md` 文件（如 `Cyberpunk.md`）
2. 参考 `_template.md` 编写设计 Token 系统、组件规范、动画要求
3. 在 skill.md 的风格列表中注册新风格
4. 重启 Claude Code 即可使用

### 自定义避坑规则

测试中发现问题时，AI 会自动记录到 `config/pitfalls.yaml`：

```yaml
# 示例规则
- category: "布局问题"
  description: "标签云必须使用 flex-wrap: wrap，防止标签重叠"
  trigger_condition: "当页面包含标签云功能时"
  solution: "确保容器设置 display: flex; flex-wrap: wrap; gap: 8px"
```

可直接编辑 YAML 文件增删规则。

## 质量保障机制

### 生成前自检清单

每个文件生成前，AI 必须逐项检查：

**基础结构**
- [ ] DOCTYPE / charset=UTF-8 / viewport
- [ ] 语义化标签（nav/section/article/footer）
- [ ] 简体中文内容（包括注释）

**风格符合度**
- [ ] 颜色 Token 与风格模板一致
- [ ] 字体栈符合要求（禁用 Inter/Roboto）
- [ ] 圆角系统匹配风格（如 Material 24px+，Flat Design 6-8px）
- [ ] 阴影策略正确（Neumorphism 双向软阴影 / Flat Design 零阴影）

**动画系统**
- [ ] 实现风格模板所有独特动画
- [ ] 完整三态（default/hover/active）
- [ ] 精确参数（duration/easing/delay）
- [ ] 装饰元素到位（光斑/浮动/渐变）

**空间构成**
- [ ] 不对称布局（避免镜像对称）
- [ ] 元素叠压（至少一处超出父容器边界）
- [ ] 对角线流向（clip-path 或 skew 斜切）
- [ ] 留白与密度对比

**响应式**
- [ ] ≤1024px 断点（双列 → 单列）
- [ ] ≤640px 断点（导航折叠/CTA 垂直）
- [ ] 无横向滚动条

**可访问性**
- [ ] Focus ring 可见
- [ ] 对比度通过 WCAG AA
- [ ] 图标 aria-hidden 处理

### 生成后验证报告

每个文件生成后自动输出详细报告（参考阶段 6 示例）。

## 常见问题

**Q: 生成的 HTML 有乱码怎么办？**  
A: 立即反馈，AI 会修复并自动将问题记录到避坑清单，下次生成时自动避免。

**Q: 如何切换不同风格对比效果？**  
A: 使用相同需求重新运行 `/html-style`，选择不同风格编号即可。建议保存多个版本进行 A/B 测试。

**Q: 生成的文件保存在哪里？**  
A: 默认保存在用户指定的目录（如 `D:\test\`），首次使用会询问确认。

**Q: 可以修改已生成的文件吗？**  
A: 可以。告知 AI 修改意见（如"Hero 标题字号加大"、"按钮换成圆角"），AI 会重新生成该文件。

**Q: 如何让某个风格永久生效特定要求？**  
A: 修改对应风格文档（如 `styles/Modern-Dark.md`），或在对话中提出后让 AI 更新 skill.md 底层要求。

**Q: 支持生成移动端原型吗？**  
A: 当前聚焦 Web 端响应式布局（桌面/平板/手机三档适配），如需纯移动端 H5 原型可单独提出需求。

**Q: 能导出为 React/Vue 组件吗？**  
A: 当前输出纯 HTML/CSS/JS，如需转换为组件需手动迁移或提出需求让 AI 协助。

## 版本历史

### v2.0.0 (2026-03-13)
- ✨ **新增 9 种设计风格**：Modern Dark、Flat Design、Neumorphism、Corporate Trust 等
- 🎨 **空间构成要求**：强制不对称布局、元素叠压、对角线流向、留白对比
- 🎭 **动画强制执行**：每个风格独特动画系统 + 完整三态 + 精确参数
- 🔍 **质量自检升级**：生成前 8 项检查清单 + 生成后详细验证报告
- 📐 **技术栈扩展**：集成 Font Awesome、ECharts、Unsplash CDN
- 🚀 **性能优化**：纯 CSS 动画优先、will-change 提示、避免 layout thrashing
- 🌐 **响应式增强**：三档断点（1024px/640px）+ 移动端导航优化

### v1.0.0 (2026-03-13)
- 初始版本
- 六阶段工作流程
- 三种生成策略
- Minimal SaaS 单风格支持
- 避坑清单机制

## 贡献

欢迎提交 Issue 和 PR！

## 成果展示

### 示例原型

以下是使用本工具生成的真实原型示例：

#### Minimal SaaS 风格
![Minimal SaaS 风格示例](examples/example_1.png)

#### Modern Dark 风格
![Modern Dark 风格示例](examples/example_2.png)

#### Hand-Drawn Sketch 风格
![Hand-Drawn Sketch 风格示例](examples/example_3.png)

> 💡 **提示**：更多示例可在 `examples/` 目录查看，每个风格都支持完整的交互动画和响应式布局。

## License

MIT
