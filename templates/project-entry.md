# {{项目名}} 设计系统

{{简述产品用途、设计方向和采用的组件体系。}}

先读取本入口与相关系统规则，再审查现有组件，决定复用、改造或构建。

## 设计依据

{{链接到 design-system/design-basis.md 或已有等价独立文件；具体设计依据在该文件维护。}}

## 公共入口

- Token：{{使用说明与权威源路径}}
- 组件：{{源码与导出入口}}
- 示例：{{已有页面或工作台入口及运行方式；没有则省略}}
- 页面与任务模式：{{已有适用规则及代表性页面；尚无稳定复用模式时省略}}
- 验证：{{已有命令或检查方式}}

## 系统索引

状态只用“可用、待补齐、不适用”。可用表示已有明确规则及可引用资产，不代表所有场景均已验证。每项链接对应独立规则文件；待补齐项在该文件写缺口，不适用写原因。间距、尺寸和布局须有基础契约。下列路径相对于项目设计入口；已有等价目录时替换为实际路径。此表用于基础覆盖，业务所需模式与组件按需补充。

| 系统 | 规范路径 | 状态 |
| --- | --- | --- |
| 颜色 | `design-system/systems/color.md` | {{状态}} |
| 按钮 | `design-system/systems/button.md` | {{状态}} |
| 滑动条 | `design-system/systems/slider.md` | {{状态}} |
| 圆角 | `design-system/systems/radius.md` | {{状态}} |
| 字体 | `design-system/systems/typography.md` | {{状态}} |
| 图标 | `design-system/systems/icons.md` | {{状态}} |
| 阴影 | `design-system/systems/elevation.md` | {{状态}} |
| 动效 | `design-system/systems/motion.md` | {{状态}} |
| 过渡与骨架屏 | `design-system/systems/transition-loading.md` | {{状态}} |
| 交互行为 | `design-system/systems/interaction.md` | {{状态}} |
| 间距 | `design-system/systems/spacing.md` | {{状态}} |
| 尺寸 | `design-system/systems/sizing.md` | {{状态}} |
| 布局 | `design-system/systems/layout.md` | {{状态}} |

## 当前事项

{{只记未决假设和选择、必要验证限制；分批迁移时补充目标规则、本次及剩余范围、保留例外与退出条件。没有则删除本节，测试历史不在此堆积。}}
