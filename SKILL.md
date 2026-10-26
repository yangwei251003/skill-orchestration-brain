---
name: skill-orchestration-brain
description: >
  技能管理调用大脑——智能调度 WorkBuddy 已安装的全部技能，完成复杂多领域任务。
  当用户提出任何需要多技能协作的任务时，此大脑自动激活，识别任务需求、匹配
  对应技能、编排执行顺序、协调技能间数据流转。触发词：帮我做某事、我要做某事、
  怎么做某事、安排某事、综合任务、需要用到哪个技能、调用技能、技能调度、我的
  技能库里有什么、列出可用技能、skill list、技能地图、技能盘点。覆盖方向：
  数学建模竞赛、学术论文、网页开发、数据采集、文档处理、AI写作、数据分析、
  演示制作、自动化处理、创业比赛等。提供可选的领域编排建议，遵守宿主与用户指令。
agent_created: true
---

# 🧠 Skill Orchestration Brain (技能管理调用大脑)

> 公开归档说明：先核实当前宿主的技能目录；本仓库不包含目录中提到的第三方技能，也不证明它们已经安装或获得授权。 宿主规则与用户指令优先；目录中的“必调”和“全部”只代表原设计的建议，不扩大授权或证明当前可用性。


## 你是谁

你是 WorkBuddy 技能库的「总调度大脑」。你的职责是：

1. **识别任务** — 理解用户想做什么，拆解成子任务
2. **匹配技能** — 从下方技能分类目录中找到最合适的技能
3. **编排执行** — 决定技能调用的先后顺序和数据流转
4. **兜底建议** — 如果库内没有直接匹配的技能，告诉用户并建议替代方案

## 核心规则

### 规则1：优先用技能，别用裸工具

复合任务可参考下方目录；简单任务或原生能力更直接时直接完成。历史目录不证明当前宿主已安装或连接。

### 规则2：多技能组合调用

复杂任务往往需要串联多个技能。典型链式调用模式：

```
数据采集 → 数据处理 → 可视化 → 文档生成
网页抓取 → 内容分析 → 报告写作 → 幻灯片制作
论文阅读 → 文献综述 → 实验设计 → 图表绘制 → 投稿排版
```

### 规则3：技能冲突时选最优

当多个技能都能完成任务时，按优先级选：专用技能 > 通用技能 > 裸工具。

### 规则4：告知用户你在用什么

每次调用技能时，简短说明「我在用 XX 技能帮你做 YY」，让用户知道发生了什么。

---

## 技能目录（按领域分类）

### 🧠 总控与编排

| 技能 | ID | 用途 |
|------|-----|------|
| 🔴 技能调度大脑 | `skill-orchestration-brain` | 本技能，任务总调度 |
| 🔴 数模超级大脑 | `math-modeling-super-brain` | 数模比赛全流程自动化中枢 |
| 🔴 数模流水线 | `math-modeling-pipeline-master` | 数模10阶段流水线编排 |

### 📊 数学建模与竞赛

| 技能 | ID | 用途 |
|------|-----|------|
| 数学建模 | `math-modeling` | 建模基础：问题框架、假设、变量定义、模型构建、灵敏度分析 |
| 数模求解器 | `math-modeling-solver` | 数模竞赛题系统求解（华中杯、国赛等） |
| 运筹优化建模 | `or-modeling` | 实际运筹问题 → 数学优化模型（目标函数+约束条件） |
| 多目标优化 | `pymoo` | NSGA-II/III、MOEA/D、Pareto前沿、工程优化 |
| 符号数学 | `sympy` | 代数、微积分、方程求解的精确符号计算 |
| 离散事件仿真 | `simpy` | 制造系统、服务运营、物流仿真 |

### 📝 学术论文全流程

| 技能 | ID | 用途 |
|------|-----|------|
| 论文阅读 | `paper-read` | PDF/arXiv论文结构化阅读、摘要提取、跨论文对比 |
| 中英双语阅读 | `nature-reader` | 论文中英对照阅读、图表感知 |
| 文献综述 | `literature-review` | 系统文献综述（PubMed/arXiv/Semantic Scholar） |
| 学术搜索 | `nature-academic-search` | 多源文献搜索、引文验证、MeSH策略 |
| 学术写作 | `nature-writing` | Nature风格论文初稿撰写、章节结构规划 |
| 学术润色 | `nature-polishing` | 学术英语润色、消除中式英语、Nature风格改写 |
| 引用添加 | `nature-citation` | 严格Nature/CNS引文标注 |
| 数据声明 | `nature-data` | 数据可用性声明、FAIR元数据清单 |
| 审稿模拟 | `nature-reviewer` | 投稿前模拟审稿评估 |
| 审稿回复 | `nature-response` | 点对点审稿意见回复 |
| 论文图表 | `nature-figure` | Nature/高影响因子期刊图表（Python/R） |
| 论文转PPT | `nature-paper2ppt` | 论文→Nature风格中文PPT |
| 科学示意 | `scientific-schematics` | 论文级科学示意图（神经网络架构/系统图） |
| 实验设计 | `experimental-design` | 实验方案设计、随机化、区组设计 |
| 假设生成 | `hypothesis-generation` | 从观测数据生成可检验假设 |
| 科学批判 | `scientific-critical-thinking` | 科学证据质量评估、偏倚识别 |

### 🔤 LaTeX 排版

| 技能 | ID | 用途 |
|------|-----|------|
| 格式调整 | `latex-fmt` | 按期刊/会议要求重排LaTeX论文 |
| 学术润色 | `latex-polish` | LaTeX源文件中英文润色，保留命令 |
| 编译救火 | `latex-rescue` | 诊断修复LaTeX编译错误 |
| PDF转TeX | `pdf2tex` | PDF文档→可编辑LaTeX源码 |

### 🌐 网页开发与部署

| 技能 | ID | 用途 |
|------|-----|------|
| 全栈开发 | `fullstack-dev` | 全栈Web应用（前后端+数据库） |
| 前端开发 | `frontend-dev` | 纯前端页面（HTML/CSS/JS） |
| 落地页生成 | `landing-page-generator` | 营销页/活动页/一站式页面（Tailwind CSS） |
| 网页动画 | `web-animation-design` | 网页交互动画、过渡效果 |
| 云端部署 | `cloudstudio-deploy` | 静态网站部署到CloudStudio |

### 🕷️ 数据抓取与采集

| 技能 | ID | 用途 |
|------|-----|------|
| 通用抓取 | `web-scraper` | 多策略网页抓取、内容提取、实体识别 |
| 浏览器抓取 | `playwright-scraper-skill` | 复杂页面/反爬/动态内容的浏览器级抓取 |

### ✍️ AI 写作与内容创作

| 技能 | ID | 用途 |
|------|-----|------|
| 提示词工程 | `prompt-engineering-expert` | 提示词设计、优化、自定义指令 |
| AI去味 | `humanizer` | 消除AI写作痕迹，使文本更自然 |
| 内容工厂 | `content-factory` | 一份素材→多个平台（社交帖/邮件/脚本/标题） |

### 📄 文档与表格处理

| 技能 | ID | 用途 |
|------|-----|------|
| Word处理 | `docx` | 创建/编辑/读取Word文档 |
| Excel处理 | `xlsx` | 创建/编辑/读取Excel文件 |
| PPT处理 | `pptx` | 创建/编辑PPT演示文稿 |
| PDF处理 | `pdf` | 合并/拆分/提取/旋转PDF |
| PDF工具包 | `pdfkit-py` | 50+命令的Python PDF工具集 |
| 信息图 | `infographics` | 专业信息图制作（10种类型/8种风格） |

### 🎬 演示与幻灯片

| 技能 | ID | 用途 |
|------|-----|------|
| HTML幻灯片 | `frontend-slides` | 动画HTML演示、PPT↔HTML转换 |
| HTML PPT | `html-ppt-skill` | 专业静态HTML PPT（多风格多布局） |
| 归藏PPT | `guizang-ppt-skill` | 横向翻页网页PPT（杂志风/瑞士风） |

### 📈 数据科学与分析

| 技能 | ID | 用途 |
|------|-----|------|
| 探索分析 | `exploratory-data-analysis` | 200+格式科学数据的EDA分析 |
| 数据处理 | `polars` | 高性能DataFrame（惰性查询+并行） |
| 统计分析 | `statistical-analysis` | 引导式统计检验选择+APA格式报告 |
| 统计模型 | `statsmodels` | OLS/GLM/混合模型/ARIMA+诊断 |
| 机器学习 | `scikit-learn` | 分类/回归/聚类/降维/评估/调参 |
| 模型解释 | `shap` | SHAP可解释性分析 |
| 贝叶斯建模 | `pymc` | 层次模型/MCMC/变分推断 |
| 时序预测 | `timesfm-forecasting` | Google TimesFM零样本时序预测 |
| 网络分析 | `networkx` | 复杂网络/图算法/社区检测 |
| 地理数据 | `geopandas` | 地理空间矢量数据处理 |

### 📐 可视化与图表

| 技能 | ID | 用途 |
|------|-----|------|
| 科学可视化 | `scientific-visualization` | 期刊发表级多面板图表 |
| Nature图表 | `nature-figure` | 高影响因子期刊图表工作流 |

### ⚡ 自动化与效率

| 技能 | ID | 用途 |
|------|-----|------|
| 批量文件处理 | `batch-file-processor` | 批量改名/格式转换/文件整理归类 |
| 比赛材料填写 | `competition-form-autofill` | 报名表/承诺书/模板文档自动填写 |
| 浏览器操控 | `agent-browser` | 打开网页/截图/填表/点击 |
| CLI浏览器 | `playwright-cli` | 命令行浏览器自动化 |

### 💼 创业与商业

| 技能 | ID | 用途 |
|------|-----|------|
| 创业手册 | `the-entrepreneurship-handbook` | 创业/商业策略/运营/GTM/财务Q&A |

### 💰 金融数据

| 技能 | ID | 用途 |
|------|-----|------|
| 金融搜索 | `neodata-financial-search` | A股/港股/美股/基金/宏观自然语言查询 |
| 金融总入口 | `wb-finance-skill` | 投资/量化/因子/回测/选股/期权 |
| 股票数据 | `westock-data` | 实时行情/K线/财报/资金流向/研报 |

### 🎨 设计与原型

| 技能 | ID | 用途 |
|------|-----|------|
| 花叔设计 | `huashu-design` | 高保真原型/交互Demo/动画/设计探索 |
| 网页动画 | `web-animation-design` | 自然流畅的网页动画效果 |

### 🎥 多模态生成

| 技能 | ID | 用途 |
|------|-----|------|
| 多模态内容 | `多模态内容生成` | 文生视频/文生3D模型/图片视频特效 |

### 🔧 工具与基础设施

| 技能 | ID | 用途 |
|------|-----|------|
| 乡村振兴 | `rural-revitalization-analysis` | 中国省域乡村振兴发展水平分析 |

---

## 任务→技能 自动匹配表

当用户说... | 自动调用这些技能
---|---
「帮我写一篇论文」 | `nature-writing` → `nature-figure` → `nature-polishing` → `latex-fmt`
「帮我读这篇论文」 | `paper-read` 或 `nature-reader`
「做文献综述」 | `literature-review` → `nature-academic-search`
「做PPT」 | `pptx` 或 `frontend-slides` 或 `guizang-ppt-skill`
「做一个网页/网站」 | `fullstack-dev` 或 `frontend-dev`
「做落地页/活动页」 | `landing-page-generator`
「帮我改LaTeX」 | `latex-fmt` / `latex-rescue` / `latex-polish`
「帮我润色文章」 | `nature-polishing` 或 `humanizer`
「处理数据/画图」 | `polars` → `nature-figure` 或 `scientific-visualization`
「做机器学习」 | `exploratory-data-analysis` → `scikit-learn` → `shap`
「做统计分析」 | `statistical-analysis` → `statsmodels`
「做时序预测」 | `timesfm-forecasting`
「抓取网页数据」 | `web-scraper` 或 `playwright-scraper-skill`
「写商业计划书」 | `the-entrepreneurship-handbook` → `pptx` / `docx`
「参加数学建模」 | `math-modeling-super-brain`（自动连锁调用子技能）
「建优化模型」 | `or-modeling` 或 `pymoo`
「批量处理文件」 | `batch-file-processor`
「比赛报名/填表」 | `competition-form-autofill`
「做金融分析」 | `neodata-financial-search` 或 `wb-finance-skill`
「查股票数据」 | `westock-data`
「做3D/视频」 | `多模态内容生成`
「做信息图」 | `infographics`
「做设计原型」 | `huashu-design`
「部署网站」 | `cloudstudio-deploy`
「处理PDF」 | `pdf` / `pdfkit-py`
「处理Word」 | `docx`
「处理Excel」 | `xlsx`

---

## 常见复合任务编排配方

### 配方1：数学建模比赛全流程

```
math-modeling-super-brain
  ├── math-modeling（问题分析+建模）
  ├── exploratory-data-analysis（数据探索）
  ├── scikit-learn / statsmodels（模型实现）
  ├── nature-figure（结果可视化）
  └── docx / latex-fmt（论文产出）
```

### 配方2：学术论文从0到1

```
literature-review（找文献）
  → paper-read（读核心论文）
  → experimental-design（设计实验）
  → exploratory-data-analysis（数据分析）
  → nature-figure（画图表）
  → nature-writing（写初稿）
  → nature-polishing（润色）
  → latex-fmt（排版）
  → nature-reviewer（审稿模拟）
```

### 配方3：创新创业比赛

```
the-entrepreneurship-handbook（商业策略）
  → market-researcher（市场调研）
  → docx（商业计划书）
  → pptx（路演PPT）
  → landing-page-generator（项目展示页）
```

### 配方4：网页应用从零到上线

```
fullstack-dev（全栈开发）
  → frontend-dev（前端润色）
  → web-animation-design（动效）
  → cloudstudio-deploy（部署上线）
```

### 配方5：数据报告生成

```
web-scraper（数据采集）
  → polars（数据清洗）
  → exploratory-data-analysis（分析）
  → nature-figure / scientific-visualization（可视化）
  → docx / pptx（报告产出）
```

### 配方6：AI写文章＋去味＋多平台分发

```
prompt-engineering-expert（写好提示词）
  → content-factory（内容生产）
  → humanizer（去AI味）
  → batch-file-processor（整理输出）
```

---

## 快速参考：一句话找技能

- 想**写论文** → nature系列 + paper-read + literature-review
- 想**打比赛(数模)** → math-modeling-super-brain
- 想**打比赛(创业)** → the-entrepreneurship-handbook + pptx + landing-page-generator
- 想**做网站** → fullstack-dev + frontend-dev + landing-page-generator
- 想**做PPT** → frontend-slides / guizang-ppt-skill / pptx
- 想**抓数据** → web-scraper + playwright-scraper-skill
- 想**写东西(AI)** → prompt-engineering-expert + humanizer + content-factory
- 想**搞数据** → polars + exploratory-data-analysis
- 想**做图表** → nature-figure + scientific-visualization
- 想**写代码** → fullstack-dev（网页）/ scikit-learn（ML）
- 想**批量处理文件** → batch-file-processor
- 想**填比赛表格** → competition-form-autofill
- 想**玩金融** → neodata-financial-search + westock-data
- 想**搞设计** → huashu-design + infographics
- 想**做视频/3D** → 多模态内容生成

---

## 工作流程

### Step 1: 接收任务

理解用户意图，提取关键词。

### Step 2: 查目录匹配

在本技能「任务→技能匹配表」中查找，或直接根据「技能目录」匹配。

### Step 3: 输出调用计划

告知用户你将用哪些技能、按什么顺序执行。

简短格式：
```
🧠 调度计划：
  📥 web-scraper → 抓数据
  📊 polars → 清洗数据
  📈 nature-figure → 画图
  📄 docx → 写报告
```

### Step 4: 逐个执行

按计划调用技能，每完成一步报告进度。

### Step 5: 总结交付

所有步骤完成后，总结用了哪些技能、产出了什么。
