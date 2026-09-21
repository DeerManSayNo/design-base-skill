<h1 align="center">DESIGN BASE SKILL</h1>

<p align="center">
  <strong>GIVE YOUR CODING AGENT A DESIGN SYSTEM, NOT A BAG OF UI TRICKS.</strong>
</p>

<p align="center">
  <a href="https://github.com/DeerManSayNo/design-base-skill/releases/latest"><img alt="Release" src="https://img.shields.io/github/v/release/DeerManSayNo/design-base-skill?style=for-the-badge&color=22c55e" /></a>
  <a href="https://github.com/DeerManSayNo/design-base-skill/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/DeerManSayNo/design-base-skill/total?style=for-the-badge&color=f59e0b" /></a>
  <img alt="Skill" src="https://img.shields.io/badge/AGENT-SKILL-111827?style=for-the-badge" />
  <img alt="Language" src="https://img.shields.io/badge/LANG-中文-ef4444?style=for-the-badge" />
</p>

<p align="center">
  <strong>从设计意图到规则，从规则到实现，从实现到验证。</strong><br />
  一套为编码代理打造的模块化设计系统调度 Skill。
</p>

<p align="center">
  <a href="https://www.pexels.com/photo/apple-monitors-326518/">
    <img src="assets/design-workspace.jpg" alt="双屏网页设计工作台，展示真实的界面设计过程" width="100%" />
  </a>
</p>

---

**Design Base Skill** 试图解决一个越来越明显的问题：AI 可以在几秒钟内写出界面，却常常只是在重复熟悉的卡片、渐变、圆角和营销模板。

它为编码代理增加一层完整的**设计判断能力**。面对新项目、存量产品、组件改造或设计系统治理任务，代理会先识别真实目标、信息关系和既有依据，再决定规则、组件与视觉表达，最后用运行结果验证改动。

这不只是一份“让页面更好看”的提示词。它是一套可以进入真实项目、持续演进、约束实现并接受验证的设计工作流。

> **让每一个界面决定都有依据，让每一次实现都能被检查。**

## Why Design Base

编码代理缺少的通常不是 CSS 能力，而是稳定的设计决策过程。

- **拒绝无依据的模板拼装**：先理解产品任务、信息优先级与主操作，再选择布局和组件。
- **尊重现有产品语言**：读取项目主题、Token、组件和设计资料，避免局部改动破坏整体一致性。
- **从页面升级到系统**：把有效决定沉淀为可复用规则，同时控制共享规则的准入范围。
- **主动对抗 AI 平均化**：识别多个默认选择叠加形成的模板感，而非机械禁用某种颜色、圆角或渐变。
- **用结果结束争论**：检查真实渲染、关键状态、响应式表现、交互反馈和视觉一致性。
- **按需加载上下文**：只读取当前任务需要的模块与参考资料，避免把整套规范一次性塞进上下文。

## The Design Engine

Design Base 将复杂的界面工作压缩成三个连续阶段：

| 阶段 | 模块 | 作用 |
| --- | --- | --- |
| **01 · FOUNDATION** | `modules/foundation` | 建立设计依据、Token 契约、共享规则和项目设计资产 |
| **02 · COMPOSE** | `modules/compose` | 把任务、内容与规则落实为页面、组件、样式和交互 |
| **03 · VERIFY** | `modules/verify` | 验证实现质量、关键状态、响应式表现与设计一致性 |

```text
USER INTENT
    ↓
PRODUCT CONTEXT
    ↓
FOUNDATION → COMPOSE → VERIFY
    ↓             ↑        │
DESIGN RULES      └────────┘
    ↓
A COHERENT, TESTABLE INTERFACE
```

<p align="center">
  <a href="https://www.pexels.com/photo/white-printer-paper-196645/">
    <img src="assets/wireframe-process.jpg" alt="纸面上的 UX 线框稿与界面结构推导" width="49%" />
  </a>
  <a href="https://www.pexels.com/photo/a-person-holding-black-smartphone-11780441/">
    <img src="assets/mobile-validation.jpg" alt="在应用流程草图上验证移动端界面" width="49%" />
  </a>
</p>
<p align="center"><sub>从低保真结构推导，到真实设备上的界面验证。</sub></p>

代理只注册一个入口：`SKILL.md`。入口会根据任务类型调度模块，并在确有需要时加载设计推导、架构、规范、审查依据或项目模板。

## What It Can Handle

- 从零开始建立项目界面与设计基础
- 在已有设计体系中增加页面或调整流程
- 修改局部组件、样式、布局和交互
- 审查响应式、状态覆盖与设计一致性
- 治理 Token、共享规则和组件契约
- 识别模板感、通用生成痕迹与无产品依据的视觉选择
- 为项目建立可维护的模块化设计资产

## Built Against "AI Look"

Design Base 不用简单的风格黑名单判断设计。紫色、渐变、卡片、圆角和大标题本身都不是问题；真正的问题是它们是否服务于产品、内容与用户任务。

Skill 会要求代理检查：

- 视觉方向是否来自产品语义，而非模型最熟悉的页面公式
- 信息层级是否支持扫描、比较和行动
- 组件选择是否符合任务密度和使用频率
- 品牌表达是否真实进入首屏与核心体验
- 装饰是否有明确作用，还是只在填充空间
- 页面是否在真实尺寸和关键状态下仍然成立

目标很直接：**让 AI 生成的界面看起来属于这个产品，而不是属于某个提示词模板。**

## Install

从 [Latest Release](https://github.com/DeerManSayNo/design-base-skill/releases/latest) 下载 `design-system-v1.0.0.zip`，解压到编码代理的 Skills 目录：

```text
design-system/
├── SKILL.md
├── VERSION
├── agents/
├── modules/
├── references/
└── templates/
```

安装后注册 `design-system/SKILL.md`。内部模块无需单独注册，代理会按任务读取。

## Inside The Skill

```text
design-system/
├── SKILL.md                         # 唯一调度入口
├── VERSION                          # 当前语义化版本
├── agents/
│   └── openai.yaml                  # Agent 展示元数据
├── modules/
│   ├── foundation/instructions.md   # 规则与设计资产治理
│   ├── compose/instructions.md      # 页面和组件实施
│   └── verify/instructions.md       # 运行与设计验证
├── references/
│   ├── design-reasoning.md          # 从任务推导设计方向
│   ├── anti-ai-aesthetic.md         # AI 平均化与模板感审查
│   ├── design-spec.md               # 视觉和交互规则参考
│   ├── architecture.md              # 设计资产架构
│   └── shared-rule-review.md        # 共享规则准入检查
└── templates/                       # 项目设计资产模板
```

## Design Principles

1. **任务先于版式**：先确定用户要完成什么，再决定页面长什么样。
2. **依据先于偏好**：品牌、内容、场景和既有系统共同决定视觉表达。
3. **规则必须有边界**：局部决定不会自动升级为全局规范。
4. **实现必须可验证**：截图、交互、状态和响应式表现都属于设计结果。
5. **系统必须可演进**：新决定明确适用范围，旧规则与例外保持可追踪。
6. **上下文保持克制**：资料足以支持决定时停止扩展读取。

## Versioning

项目遵循[语义化版本](https://semver.org/lang/zh-CN/)。当前版本记录在 [`VERSION`](VERSION)，完整变化见 [`CHANGELOG.md`](CHANGELOG.md)，Git 标签与 GitHub Release 使用 `v<版本号>` 格式。

<sub>Images used under the [Pexels License](https://www.pexels.com/license/): [Tranmautritam](https://www.pexels.com/@tranmautritam/), [picjumbo.com](https://www.pexels.com/@picjumbo-com-55570/), and [Akshar Dave](https://www.pexels.com/@akshar-dave/).</sub>

<p align="center">
  <strong>STOP GENERATING PAGES. START BUILDING DESIGN SYSTEMS.</strong>
</p>
