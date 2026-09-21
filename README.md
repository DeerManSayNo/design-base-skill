# Design System Skill

面向编码代理的设计系统调度 Skill。它从用户任务与项目既有依据出发，按需建立设计规则、实施界面与组件改动，并验证最终效果。

## 安装

下载 Release 中的 `design-system-v1.0.0.zip`，解压到代理的 Skills 目录。安装后的目录入口应为：

```text
design-system/
├── SKILL.md
├── VERSION
├── agents/
├── modules/
├── references/
└── templates/
```

代理只需注册 `SKILL.md`；其余模块和参考资料由入口按任务需要加载。

## 内容

- `modules/foundation`：建立或治理设计规则与项目设计资产。
- `modules/compose`：将既有设计依据落实为页面、样式和组件改动。
- `modules/verify`：验证实现、交互、响应式表现与设计一致性。
- `references`：提供设计推导、架构、规范和审查依据。
- `templates`：提供项目内模块化设计资产模板。

## 版本

项目使用[语义化版本](https://semver.org/lang/zh-CN/)，当前版本记录在 [`VERSION`](VERSION)，变更记录见 [`CHANGELOG.md`](CHANGELOG.md)。Git 标签与 GitHub Release 使用 `v<版本号>` 格式。
