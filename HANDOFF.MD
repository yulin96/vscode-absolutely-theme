# 项目交接

## Proof 主题

- Proof 的编辑区、侧栏、标签栏及其他主要工作区统一使用 `#F5F3ED`，文字为 `#2F312D`、强调色为 `#3D755D`；活动标签使用轻微加深的中性色，以便区分状态。Modern UI 的连接式标签需要在 `package.json` 的 `[Proof]` 配置默认值中同步活动及悬停背景。
- 主按钮使用绿色强调色，悬浮时使用较深的绿色；普通徽标、列表悬浮和选中态使用灰黑色。绿色也用于焦点、光标、搜索匹配和新增等需要辨认的状态；源代码语义高亮及 Git 增删颜色保持区分。
- Vue 3.3.14 的语义标记不一定包含组件标签。Proof 同时匹配 Vue 组件的 TextMate 范围：PascalCase 起始标签、未识别的结束标签和短横线组件；后两者需匹配具体的 `entity.name.tag.html`，避免被原生 HTML 标签规则覆盖。
- Proof 的函数使用绿色，普通字符串及引号统一使用蓝色 `#315F86`。HTML 和 Vue 模板以深绿标签、赭红属性名和蓝色静态属性值区分语法；字符串插值和动态绑定表达式仍按自身语法高亮。
- Git 历史的当前引用使用深绿、远程引用使用蓝色、基准引用使用赭金，其他分支使用蓝、紫、赭金、青、赭红。VS Code 1.144.1 将引用颜色同时用于图线和标签底色；`scmGraph.historyItemHoverLabelForeground` 实际也控制列表中的彩色标签文字，需同步使用白色以保证对比度，不能仅按名称当作悬浮颜色处理。
- 用 VS Code 1.144 的 `2026-light.json` 核对过工作台颜色键，并在隔离的扩展开发主机检查 Vue 模板、脚本和样式高亮。主题尚未打包或发布。

## 自动发布

- `.github/workflows/publish.yml` 监听 `v*` tag，仅接受与 `package.json` 一致的正式版本 tag；校验四个主题 JSON 后生成 VSIX，上传 Actions artifact，再通过 `vsce publish --oidc --packagePath` 发布同一安装包到 Marketplace。没有配置 GitHub Release。
- 2026-11-03 已在 Chrome 确认 Marketplace 的 `deploy-vscode-absolutely-theme` 策略为 Active，owner 为 `yulin96`、仓库为 `vscode-absolutely-theme`、工作流为 `publish.yml`，未指定 environment；工作流需保留 `id-token: write`，不需要 PAT。
- npm 官方仓库未找到前期示例中的 `@vscode/vsce@4.0.2`；当前工作流固定为已核实存在的 `4.1.0`，要求 Node.js >=22。`.vscodeignore` 排除工作流、编辑器配置、Codex/技能目录、交接记录和旧 VSIX。
- 本地已使用 `vsce@4.1.0` 实际打包，检查包内清单和四个主题 JSON，确认无开发文件或旧 VSIX；工作流 YAML 解析、匹配 tag 放行、版本不匹配及预发布 tag 拒绝均通过。发布配置已随 `31aedec` 提交并同步至远程；`0.2.11` 为首次通过 tag 验证自动发布链路的版本。
- 发布成功需同时核对对应 tag 的 Actions 运行结果和 Marketplace 返回的版本，不能以 tag 推送成功或 VSIX 打包成功替代发布确认。发布后的修复使用递增版本；不移动已发布的版本 tag。
